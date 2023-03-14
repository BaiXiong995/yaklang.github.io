---
sidebar_position: 13
---

# 会话标识伪造

**漏洞描述：**

通过检测会话标识的生成方式，确认每个会话标识是否具有规律性，是否可以被伪造。进而利用预测、遍历等方式来
伪造出系统中存在的、有效的会话标识符，并通过该会话标识劫持其他用户身份。

**漏洞案例：**

暂无案例


:::note

漏洞修复方案

会话标识不应该存在某种规律或关联性（如 SessionID=sfdsfljsldfwe-fsdfsd-0002 和 SessionID=sfdsfljsldfwe-fsdfsd-0001）且不应该含有可理解的身份信息和登录信息（如username，userid，role等），同时会话标识应采用不易被猜解的强算法进行加密。

:::


 