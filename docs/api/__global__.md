# __global__


|成员函数|函数描述/介绍|
|:------|:--------|
 | [append](#append) |  |
 | [assert](#assert) |  |
 | [assertEmpty](#assertempty) |  |
 | [assertTrue](#asserttrue) |  |
 | [assertf](#assertf) |  |
 | [atoi](#atoi) |  |
 | [cap](#cap) |  |
 | [chr](#chr) |  |
 | [close](#close) |  |
 | [copy](#copy) |  |
 | [date](#date) |  |
 | [datetime](#datetime) |  |
 | [datetimeToTimestamp](#datetimetotimestamp) |  |
 | [delete](#delete) |  |
 | [desc](#desc) |  |
 | [descStr](#descstr) |  |
 | [die](#die) |  |
 | [dump](#dump) |  |
 | [eval](#eval) |  |
 | [fail](#fail) |  |
 | [fprintln](#fprintln) |  |
 | [get](#get) |  |
 | [import](#import) |  |
 | [isEmpty](#isempty) |  |
 | [len](#len) |  |
 | [logdiscard](#logdiscard) |  |
 | [loglevel](#loglevel) |  |
 | [logquiet](#logquiet) |  |
 | [logrecover](#logrecover) |  |
 | [make](#make) |  |
 | [mapFrom](#mapfrom) |  |
 | [mapOf](#mapof) |  |
 | [max](#max) |  |
 | [min](#min) |  |
 | [mkmap](#mkmap) |  |
 | [mkslice](#mkslice) |  |
 | [nanotimestamp](#nanotimestamp) |  |
 | [now](#now) |  |
 | [ord](#ord) |  |
 | [panic](#panic) |  |
 | [panicf](#panicf) |  |
 | [parseBool](#parsebool) |  |
 | [parseBoolean](#parseboolean) |  |
 | [parseFloat](#parsefloat) |  |
 | [parseInt](#parseint) |  |
 | [parseStr](#parsestr) |  |
 | [parseString](#parsestring) |  |
 | [parseTime](#parsetime) |  |
 | [print](#print) |  |
 | [printf](#printf) |  |
 | [println](#println) |  |
 | [randn](#randn) |  |
 | [randstr](#randstr) |  |
 | [sdump](#sdump) |  |
 | [set](#set) |  |
 | [sleep](#sleep) |  |
 | [slice](#slice) |  |
 | [sliceOf](#sliceof) |  |
 | [sprint](#sprint) |  |
 | [sprintf](#sprintf) |  |
 | [sprintln](#sprintln) |  |
 | [sub](#sub) |  |
 | [tick1s](#tick1s) |  |
 | [timestamp](#timestamp) |  |
 | [timestampToDatetime](#timestamptodatetime) |  |
 | [timestampToTime](#timestamptotime) |  |
 | [uuid](#uuid) |  |
 | [wait](#wait) |  |




## 变量定义

|变量调用名|变量类型|变量解释/帮助信息|
|:-----------|:---------- |:-----------|
|`bool`|`builtin.tyBool`| //|
|`byte`|`builtin.tyUint8`| //|
|`false`|`bool`| //|
|`float`|`builtin.tyFloat64`| //|
|`float32`|`builtin.tyFloat32`| //|
|`float64`|`builtin.tyFloat64`| //|
|`int`|`builtin.tyInt`| //|
|`int16`|`builtin.tyInt16`| //|
|`int32`|`builtin.tyInt32`| //|
|`int64`|`builtin.tyInt64`| //|
|`int8`|`builtin.tyInt8`| //|
|`sliceFrom`|`builtin.goSliceFrom`| //|
|`string`|`builtin.tyString`| //|
|`true`|`bool`| //|
|`type`|`builtin.goTypeOf`| //|
|`uint`|`builtin.tyUint`| //|
|`uint16`|`builtin.tyUint16`| //|
|`uint32`|`builtin.tyUint32`| //|
|`uint64`|`builtin.tyUint64`| //|
|`uint8`|`builtin.tyUint8`| //|
|`undefined`|`*spec.undefinedType`| //|
|`var`|`builtin.tyVar`| //|





## 函数定义

### append



#### 详细描述



#### 定义：

`func append(v1: any, v2 ...any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### assert



#### 详细描述



#### 定义：

``func assert(v1: bool, v2 ...any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `bool` |   |
| v2 | `...any` |   |




 

 
### assertEmpty



#### 详细描述



#### 定义：

``func assertEmpty(v1: any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |




 

 
### assertTrue



#### 详细描述



#### 定义：

``func assertTrue(v1: bool, v2 ...any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `bool` |   |
| v2 | `...any` |   |




 

 
### assertf



#### 详细描述



#### 定义：

``func assertf(v1: bool, v2: string, v3 ...any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `bool` |   |
| v2 | `string` |   |
| v3 | `...any` |   |




 

 
### atoi



#### 详细描述



#### 定义：

`func atoi(v1: string) return (r0: int, r1: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |
| r1 | `error` |   |


 
### cap



#### 详细描述



#### 定义：

`func cap(v1: any) return (r0: int)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |


 
### chr



#### 详细描述



#### 定义：

`func chr(v1: any) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### close



#### 详细描述



#### 定义：

``func close(v1: any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |




 

 
### copy



#### 详细描述



#### 定义：

`func copy(v1: any, v2: any) return (r0: int)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |


 
### date



#### 详细描述



#### 定义：

`func date() return (r0: string)`

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### datetime



#### 详细描述



#### 定义：

`func datetime() return (r0: string)`

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### datetimeToTimestamp



#### 详细描述



#### 定义：

`func datetimeToTimestamp(v1: string) return (r0: int64, r1: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int64` |   |
| r1 | `error` |   |


 
### delete



#### 详细描述



#### 定义：

``func delete(v1: any, v2: any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |




 

 
### desc



#### 详细描述



#### 定义：

``func desc(v1: any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |




 

 
### descStr



#### 详细描述



#### 定义：

`func descStr(v1: any) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### die



#### 详细描述



#### 定义：

``func die(v1: any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |




 

 
### dump



#### 详细描述



#### 定义：

``func dump(v1 ...any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |




 

 
### eval



#### 详细描述



#### 定义：

`func eval(v1: any) return (r0: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `error` |   |


 
### fail



#### 详细描述



#### 定义：

``func fail(v1 ...any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |




 

 
### fprintln



#### 详细描述



#### 定义：

`func fprintln(v1: io.Writer, v2 ...any) return (r0: int, r1: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `io.Writer` |   |
| v2 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |
| r1 | `error` |   |


 
### get



#### 详细描述



#### 定义：

`func get(v1: any, v2: any, v3 ...any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |
| v3 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### import



#### 详细描述



#### 定义：

`func import(v1: string, v2: string) return (r0: *yak.yakVariable, r1: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |
| v2 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `*yak.yakVariable` |   |
| r1 | `error` |   |


 
### isEmpty



#### 详细描述



#### 定义：

`func isEmpty(v1: any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### len



#### 详细描述



#### 定义：

`func len(v1: any) return (r0: int)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |


 
### logdiscard



#### 详细描述



#### 定义：

``func logdiscard()``

 

 

 
### loglevel



#### 详细描述



#### 定义：

``func loglevel(v1: any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |




 

 
### logquiet



#### 详细描述



#### 定义：

``func logquiet()``

 

 

 
### logrecover



#### 详细描述



#### 定义：

``func logrecover()``

 

 

 
### make



#### 详细描述



#### 定义：

`func make(v1: spec.GoTyper, v2 ...int) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `spec.GoTyper` |   |
| v2 | `...int` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### mapFrom



#### 详细描述



#### 定义：

`func mapFrom(v1 ...any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### mapOf



#### 详细描述



#### 定义：

`func mapOf(v1: any, v2: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### max



#### 详细描述



#### 定义：

`func max(v1 ...any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### min



#### 详细描述



#### 定义：

`func min(v1 ...any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### mkmap



#### 详细描述



#### 定义：

`func mkmap(v1: any, v2 ...int) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `...int` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### mkslice



#### 详细描述



#### 定义：

`func mkslice(v1: any, v2 ...any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### nanotimestamp



#### 详细描述



#### 定义：

`func nanotimestamp() return (r0: int64)`

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int64` |   |


 
### now



#### 详细描述



#### 定义：

`func now() return (r0: time.Time)`

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `time.Time` |   |


 
### ord



#### 详细描述



#### 定义：

`func ord(v1: any) return (r0: int)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |


 
### panic



#### 详细描述



#### 定义：

``func panic(v1: any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |




 

 
### panicf



#### 详细描述



#### 定义：

``func panicf(v1: string, v2 ...any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |
| v2 | `...any` |   |




 

 
### parseBool



#### 详细描述



#### 定义：

`func parseBool(v1: any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### parseBoolean



#### 详细描述



#### 定义：

`func parseBoolean(v1: any) return (r0: bool)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### parseFloat



#### 详细描述



#### 定义：

`func parseFloat(v1: string) return (r0: float64)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `float64` |   |


 
### parseInt



#### 详细描述



#### 定义：

`func parseInt(v1: string) return (r0: int)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |


 
### parseStr



#### 详细描述



#### 定义：

`func parseStr(v1: any) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### parseString



#### 详细描述



#### 定义：

`func parseString(v1: any) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### parseTime



#### 详细描述



#### 定义：

`func parseTime(v1: string, v2: string) return (r0: time.Time, r1: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |
| v2 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `time.Time` |   |
| r1 | `error` |   |


 
### print



#### 详细描述



#### 定义：

`func print(v1 ...any) return (r0: int, r1: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |
| r1 | `error` |   |


 
### printf



#### 详细描述



#### 定义：

`func printf(v1: string, v2 ...any) return (r0: int, r1: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |
| v2 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |
| r1 | `error` |   |


 
### println



#### 详细描述



#### 定义：

`func println(v1 ...any) return (r0: int, r1: error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |
| r1 | `error` |   |


 
### randn



#### 详细描述



#### 定义：

`func randn(v1: int, v2: int) return (r0: int)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `int` |   |
| v2 | `int` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int` |   |


 
### randstr



#### 详细描述



#### 定义：

`func randstr(v1: int) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `int` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### sdump



#### 详细描述



#### 定义：

`func sdump(v1 ...any) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### set



#### 详细描述



#### 定义：

``func set(v1: any, v2 ...any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `...any` |   |




 

 
### sleep



#### 详细描述



#### 定义：

``func sleep(v1: float64)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `float64` |   |




 

 
### slice



#### 详细描述



#### 定义：

`func slice(v1: any, v2 ...any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### sliceOf



#### 详细描述



#### 定义：

`func sliceOf(v1: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### sprint



#### 详细描述



#### 定义：

`func sprint(v1 ...any) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### sprintf



#### 详细描述



#### 定义：

`func sprintf(v1: string, v2 ...any) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |
| v2 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### sprintln



#### 详细描述



#### 定义：

`func sprintln(v1 ...any) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `...any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### sub



#### 详细描述



#### 定义：

`func sub(v1: any, v2: any, v3: any) return (r0: any)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `any` |   |
| v3 | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `any` |   |


 
### tick1s



#### 详细描述



#### 定义：

``func tick1s(v1: func () return(bool) )``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `func () return(bool) ` |   |




 

 
### timestamp



#### 详细描述



#### 定义：

`func timestamp() return (r0: int64)`

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `int64` |   |


 
### timestampToDatetime



#### 详细描述



#### 定义：

`func timestampToDatetime(v1: int64) return (r0: string)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `int64` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### timestampToTime



#### 详细描述



#### 定义：

`func timestampToTime(v1: int64) return (r0: time.Time)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `int64` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `time.Time` |   |


 
### uuid



#### 详细描述



#### 定义：

`func uuid() return (r0: string)`

 


#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### wait



#### 详细描述



#### 定义：

``func wait(v1: any)``


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |




 

 


