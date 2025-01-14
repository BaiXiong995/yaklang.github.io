# x


|成员函数|函数描述/介绍|
|:------|:--------|
 | [x.All](#xall) | 所有元素都存在且为 true |
 | [x.Any](#xany) | 元素中至少有一个为 true |
 | [x.Chunk](#xchunk) | 把集合按数量分组 |
 | [x.Contains](#xcontains) | 集合中是否包含某一个元素 |
 | [x.ConvertToMap](#xconverttomap) | 把一个对象尽可能转换为 map[string][]string |
 | [x.Difference](#xdifference) | 计算两个元素的差分 |
 | [x.Drop](#xdrop) | 丢弃数组 |
 | [x.Equal](#xequal) | 判断两个元素是否相等 |
 | [x.Every](#xevery) |  |
 | [x.Filter](#xfilter) | 使用一个函数 func(i): bool 过滤某数组 |
 | [x.Find](#xfind) | 寻找符合要求的某个元素 |
 | [x.Foreach](#xforeach) | For 循环的函数式编程支持 |
 | [x.ForeachRight](#xforeachright) | 反向 For 循环 |
 | [x.Head](#xhead) | 取第一个元素 |
 | [x.If](#xif) | 类似 SQL 中的 IF 函数 |
 | [x.IndexOf](#xindexof) | 判断元素在数组中的位置 |
 | [x.Intersect](#xintersect) | 计算交集 |
 | [x.IsSubset](#xissubset) | 判断子集关系 |
 | [x.Keys](#xkeys) | 取 Map 的所有 Key |
 | [x.Map](#xmap) | 批处理 |
 | [x.Max](#xmax) | 取最大值 |
 | [x.Min](#xmin) | 取最小值 |
 | [x.Range](#xrange) | 生成一个范围数组/Slice |
 | [x.Reduce](#xreduce) | 函数式编程 Reducer 支持 |
 | [x.RemoveRepeat](#xremoverepeat) | 移除数组/Slice中重复元素 |
 | [x.Reverse](#xreverse) | 数组反向 |
 | [x.Shift](#xshift) | 取出第一个数组元素 |
 | [x.Shuffle](#xshuffle) | 打乱集合顺序 |
 | [x.Some](#xsome) |  |
 | [x.Sort](#xsort) |  |
 | [x.Subtract](#xsubtract) | 集合相减 |
 | [x.Sum](#xsum) | 取和 |
 | [x.Tail](#xtail) | 出去第一个元素之外的所有数组 |
 | [x.ToFloat64](#xtofloat64) | 解析成数字（double/float64） |
 | [x.ToMap](#xtomap) | 数字根据某一个字段生成 Map |
 | [x.Values](#xvalues) | 取 Map 中的 Value |
 | [x.WaitConnect](#xwaitconnect) | 等待一个链接具体多少秒钟 |
 | [x.Zip](#xzip) |  |




 



## 函数定义

### x.All

所有元素都存在且为 true

#### 详细描述



#### 定义：

`func x.All(v1 ...any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### x.Any

元素中至少有一个为 true

#### 详细描述



#### 定义：

`func x.Any(v1 ...any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### x.Chunk

把集合按数量分组

#### 详细描述



#### 定义：

`func x.Chunk(sliceOrigin: any, groupSize: int) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| sliceOrigin | `any` |   |
| groupSize | `int` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Contains

集合中是否包含某一个元素

#### 详细描述



#### 定义：

`func x.Contains(slice: any, element: any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| slice | `any` |   |
| element | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### x.ConvertToMap

把一个对象尽可能转换为 map[string][]string

#### 详细描述



#### 定义：

`func x.ConvertToMap(v1: any) return (r0: map[string][]string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `map[string][]string` |   |


 
### x.Difference

计算两个元素的差分

#### 详细描述



#### 定义：

`func x.Difference(v1: any, v2: any) return (r0: any, r1: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |
| r1 | `any` |   |


 
### x.Drop

丢弃数组

#### 详细描述



#### 定义：

`func x.Drop(slice: any, size: int) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| slice | `any` |   |
| size | `int` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Equal

判断两个元素是否相等

#### 详细描述



#### 定义：

`func x.Equal(v1: any, v2: any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### x.Every



#### 详细描述



#### 定义：

`func x.Every(v1: any, v2 ...any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### x.Filter

使用一个函数 func(i): bool 过滤某数组

#### 详细描述



#### 定义：

`func x.Filter(slice: any, v2: func (v1: any) return(bool) ) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| slice | `any` |   |
| v2 | `func (v1: any) return(bool) ` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Find

寻找符合要求的某个元素

#### 详细描述



#### 定义：

`func x.Find(v1: any, v2: func (v1: any) return(bool) ) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `func (v1: any) return(bool) ` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Foreach

For 循环的函数式编程支持

#### 详细描述



#### 定义：

``func x.Foreach(v1: any, v2: func (v1: any) )``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `func (v1: any) ` |   |




 

 
### x.ForeachRight

反向 For 循环

#### 详细描述



#### 定义：

``func x.ForeachRight(v1: any, v2: func (v1: any) )``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `func (v1: any) ` |   |




 

 
### x.Head

取第一个元素

#### 详细描述



#### 定义：

`func x.Head(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.If

类似 SQL 中的 IF 函数

#### 详细描述



#### 定义：

`func x.If(condition: bool, obj1: any, obj2: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| condition | `bool` |   |
| obj1 | `any` |   |
| obj2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.IndexOf

判断元素在数组中的位置

#### 详细描述



#### 定义：

`func x.IndexOf(v1: any, v2: any) return (r0: int)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |


 
### x.Intersect

计算交集

#### 详细描述



#### 定义：

`func x.Intersect(v1: any, v2: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.IsSubset

判断子集关系

#### 详细描述



#### 定义：

`func x.IsSubset(v1: any, v2: any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### x.Keys

取 Map 的所有 Key

#### 详细描述



#### 定义：

`func x.Keys(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Map

批处理

#### 详细描述



#### 定义：

`func x.Map(v1: any, v2: func funkGeneralFuncType(v1: any) return(any) ) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `func funkGeneralFuncType(v1: any) return(any) ` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Max

取最大值

#### 详细描述



#### 定义：

`func x.Max(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Min

取最小值

#### 详细描述



#### 定义：

`func x.Min(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Range

生成一个范围数组/Slice

#### 详细描述



#### 定义：

`func x.Range(v1: int) return (r0: []any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `int` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `[]any` |   |


 
### x.Reduce

函数式编程 Reducer 支持

#### 详细描述



#### 定义：

`func x.Reduce(v1: any, v2: func funkGeneralReduceFuncType(v1: any, v2: any) return(any) , initValue: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `func funkGeneralReduceFuncType(v1: any, v2: any) return(any) ` |   |
| initValue | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.RemoveRepeat

移除数组/Slice中重复元素

#### 详细描述



#### 定义：

`func x.RemoveRepeat(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Reverse

数组反向

#### 详细描述



#### 定义：

`func x.Reverse(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Shift

取出第一个数组元素

#### 详细描述



#### 定义：

`func x.Shift(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Shuffle

打乱集合顺序

#### 详细描述



#### 定义：

`func x.Shuffle(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Some



#### 详细描述



#### 定义：

`func x.Some(v1: any, v2 ...any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### x.Sort



#### 详细描述



#### 定义：

``func x.Sort(v1: any, v2: func (v1: int, v2: int) return(bool) )``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `func (v1: int, v2: int) return(bool) ` |   |




 

 
### x.Subtract

集合相减

#### 详细描述



#### 定义：

`func x.Subtract(v1: any, v2: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Sum

取和

#### 详细描述



#### 定义：

`func x.Sum(v1: any) return (r0: float64)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `float64` |   |


 
### x.Tail

出去第一个元素之外的所有数组

#### 详细描述



#### 定义：

`func x.Tail(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.ToFloat64

解析成数字（double/float64）

#### 详细描述



#### 定义：

`func x.ToFloat64(v1: any) return (r0: float64, r1: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `float64` |   |
| r1 | `bool` |   |


 
### x.ToMap

数字根据某一个字段生成 Map

#### 详细描述



#### 定义：

`func x.ToMap(slice: any, fieldName: string) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| slice | `any` |   |
| fieldName | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.Values

取 Map 中的 Value

#### 详细描述



#### 定义：

`func x.Values(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### x.WaitConnect

等待一个链接具体多少秒钟

#### 详细描述



#### 定义：

`func x.WaitConnect(addr: string, timeoutSeconds: float64) return (r0: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| addr | `string` |   |
| timeoutSeconds | `float64` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `error` |   |


 
### x.Zip



#### 详细描述



#### 定义：

`func x.Zip(v1: any, v2: any) return (r0: []funk.Tuple)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `[]funk.Tuple` |   |


 


