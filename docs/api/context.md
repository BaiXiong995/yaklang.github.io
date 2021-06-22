# context


|成员函数|函数描述/介绍|
|:------|:--------|
 | [context.Background](#contextbackground) |  |
 | [context.New](#contextnew) |  |
 | [context.Seconds](#contextseconds) |  |
 | [context.TODO](#contexttodo) |  |
 | [context.TimeoutContextSecond](#contexttimeoutcontextsecond) |  |
 | [context.WithCancel](#contextwithcancel) |  |
 | [context.WithDeadline](#contextwithdeadline) |  |
 | [context.WithTimeout](#contextwithtimeout) |  |
 | [context.WithValue](#contextwithvalue) |  |




## 变量定义

|变量调用名|变量类型|变量解释/帮助信息|
|:-----------|:---------- |:-----------|
|`context.Canceled`|`*errors.errorString`| //|
|`context.DeadlineExceeded`|`context.deadlineExceededError`| //|





## 函数定义

### context.Background



#### 定义：

`func () return(context.Context) `

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |


### context.New



#### 定义：

`func () return(context.Context) `

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |


### context.Seconds



#### 定义：

`func (v1: int) return(context.Context) `


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | int |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |


### context.TODO



#### 定义：

`func () return(context.Context) `

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |


### context.TimeoutContextSecond



#### 定义：

`func (v1: int) return(context.Context) `


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | int |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |


### context.WithCancel



#### 定义：

`func (v1: context.Context) return(context.Context, func CancelFunc() ) `


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | context.Context |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |
| r1 | func CancelFunc()  |   |


### context.WithDeadline



#### 定义：

`func (v1: context.Context, v2: time.Time) return(context.Context, func CancelFunc() ) `


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | context.Context |   |
| v2 | time.Time |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |
| r1 | func CancelFunc()  |   |


### context.WithTimeout



#### 定义：

`func (v1: context.Context, v2: time.Duration) return(context.Context, func CancelFunc() ) `


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | context.Context |   |
| v2 | time.Duration |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |
| r1 | func CancelFunc()  |   |


### context.WithValue



#### 定义：

`func (v1: context.Context, v2: interface {}, v3: interface {}) return(context.Context) `


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | context.Context |   |
| v2 | interface {} |   |
| v3 | interface {} |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | context.Context |   |




