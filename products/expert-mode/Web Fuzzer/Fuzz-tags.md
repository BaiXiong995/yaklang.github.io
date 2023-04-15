---
sidebar_position: 19
---

# 使用Web Fuzzer进行模糊测试

手工测试场景中需要渗透人员对报文进行反复的发送畸形或者特定的payload进行查看服务器的反馈并以此来进行下一步的判断。

Fuzz标签便是来配合渗透人员应对不同测试场景，可以到达免配置适配大量测试场景。

通过Fuzz标签，自然且完美整合了Host碰撞、Intruder、目录爆破等等功能。

我们如果想要使用 fuzz 标签，需要明确两个概念，标签的格式是自定义的，目前支持{{和}}作为标签的标记。

### 使用 Web Fuzzer 进行爆破

使用 Burp 的 Intruder 爆破其实是任何一个渗透测试同学的必修课，在原数据流程，我们需要做的事情是：
1. 把需要爆破的数据包发送到 Intruder
2. 为爆破的位置打标记
3. 设置字典
4. 开始爆破
5. 等待结果，查看爆破过程

然而在 Yakit 中，这个过程变得更加简单并且符合人的逻辑。
1. 把需要爆破的数据包发送到 Intruder
2. 选中需要打标记的位置
3. 右键选择字典
4. 发包！

当然，这类场景非常多，很多时候我们想要的遍历订单类，遍历手机号，甚至遍历 Path 都可以通过这个方式做到.

实际 Yakit 在进行标记的时候，和 Burp 略微不同，并不是用序号进行标记，而是通过一个特殊的 Fuzz 标签，标签可以支持非常多的种类。

比如说，如果要进行一个参数遍历 1-10，在 Yakit 中只需要 {{int(1-10)}} 即可把这个位置用数字 1-10 依次替换。如果需要用到字典，通过 {{x(your-dict)}} 即可把字典内容依次替换标签位置内容，从而达到 Fuzz / 爆破的目的。

更让人高兴的是，实际上我们的爆破有时候并不完全依赖字典，如果单纯只是想测试少数的几个路径，我们费力去传一个字典，其实有点浪费了，在 Yakit 中我们可以通过 {{list(element1|element2|...)}} 来测试几个特定的值。


接下来，我们以实际的操作为例给大家讲解爆破的操作：

左边靶场登录框输入任意账号密码登录，右边MITM交互坚持点击详情即可看见详情数据包内容。

![](/img/products/yakit/fuzz-1.png)

点击数据包右键，可以发送到web fuzzer，或者在History里面找到该条数据，查看详情直接参数名进行模糊测试。

![](/img/products/yakit/fuzz-2.png)

选择想要爆破的参数，然后点击右键，这里有三种方式来使用字典。

![](/img/products/yakit/fuzz-3.png)

**① 插入临时字典：通过手工方式添加一个临时的字典,添加的文本可以直接读取文件内容或者按行读取**

![](/img/products/yakit/fuzz-4.png)

**② 插入模糊测试字典标签：payload模块里面，选择需求的字典，复制Fuzz标签，粘贴到你所需要fuzz的参数处，payload模块的字典可以自行上传保存等操作，payload模块可以理解为一个字典库。**

![](/img/products/yakit/fuzz-5.png)

**③ 插入文件标签：从本地导入字典文件，对文件内容可以按行读取，或直接读取文本内容**

![](/img/products/yakit/fuzz-6.png)

插入字典之后可以看到原来的参数已经被替换为fuzz标签，点击发送请求，右侧可以看见请求结果。

点开高级配置，还可以设置爆破的并发线程数、代理、随机延迟，对于爆破结果的筛选，可以通过正则、状态码、关键词匹配对响应包进行过滤，并且支持正则提取响应数据。

![](/img/products/yakit/fuzz-7.png)

### 常用 fuzz 标签

通过上面的案例，想必大家对fuzz标签有了初步的认识。除了账号密码的爆破之外，fuzz标签还有很多使用的场景，如:

1. 短信验证码类型Fuzz：
  * 4位数验证码：{{int(0000-9999|4)}}
  * 随机4位数验证码最小0000最大9999 枚举200次 有效4位：{{randint(0000,9999,200|4)}}
  * 6位数验证码：{{int(000000-999999|6)}}
  * 随机6位数验证码最小000000最大999999 枚举200次 有效6位：{{randint(000000,999999,200|6)}}
2. 学号/工号/手机号类型Fuzz:
* 手机号Fuzz：手机号组成结构（3位网号+4位HLR号+4位的个人代码）
  1. 网号固定，HLR和个人代码随机枚举：{{int(133,153,180)}}{{randint(0000,9999,100|4)}}{{randint(0000,9999,100|4)}}
  2. 网号固定，HLR和个人代码递归枚举：{{int(133,153,180)}}{{int(0000-9999|4)}}{{int(0000-9999|4)}}
* 学号/工号Fuzz：学号/工号组成结构（入学年份+三位系别代码+两位专业代码+三位学生编号):{{int(2015-2023)}}{{int(000-999|3)}}{{int(00-99|2)}}{{int(000-999|3)}}同理也可也用{{rangint()}}随机生成几位数值组成相关代码
3. MD5 Fuzz:{md5({{int(000-999|3)}})}}  
  * 000-999的3位数MD5加密枚举Fuzz：{{md5({{int(000-999|3)}})}}
  * 嵌套字典MD5加密枚举Fuzz：{{md5({{x(user_top10)}})}}
4. Base64 Fuzz
  * 000-999的3位数base64加密枚举Fuzz：{{base64enc({{int(000-999|3)}})}}
  * 嵌套字典base64加密枚举Fuzz：{{base64enc({{x(user_top10)}})}}
5. 重定向并发 Fuzz
  * 渗透测试需求中可能会对某些需求重复发包，或重复生成数据。repeat重复产生空字符串，例如：{{repeat(3)}}，结果为：["", "", ""] 一般用来重复发包，或重复生成数据
    重复发送100次数据包：{{repeat(100)}}
6. host碰撞 Fuzz
  * Web Fuzzer 默认请求的是 Request 请求包中的 Host ，除此外也可以在 “高级配置” 中设置 “请求 Host”。
   Host 碰撞时请求 Host 与请求包的 Host 不一致，可以在 “高级配置” 中指定目标 Host。
    ![](/img/products/yakit/fuzz-8.png)
  * 比如我们发现某一漏洞POC 需要批量测试多个目标是否存在漏洞则可以在Host处设置Fuzz标签。
    {{host(192.168.3.14/24)}}:{{port(3000)}}

更多Fuzz标签的使用和详解可以参考以下几篇文章：

_[Web Fuzz 基础](/docs/newforyak/fuzz_tutorial)_

_[Web Fuzz 高级教程](/docs/newforyak/fuzz_for_more)_

_[Fuzz Tag Playbook](/docs/newforyak/fuzztag)_

   
