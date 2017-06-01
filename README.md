# From Node To Go
If you are familiar with Node.js and want to learn Go, so this is right for you. And same to Goher

* 运行代码
* 声明变量
* 循环
* 遍历
* if/else
* 方法
* 类型转换
* array常用操作
* string常用操作
* 发送http请求
* 创建web server
* 导入, 包管理
* 获取当前路径
* 读取文件
* 工具


#### Run

```shell
# node
$ node main.js
# go
$ go run main.go   # in production env you need build and then run
```


#### Hello world

```js
console.log("Hello world")
```

```go
package main

func main() {
    println("Hello world!")
}
```

#### data type

```js
Number, String, Boolean, null, undefined, Array, Object, Function
```

```go
int, float32, byte, string, bool, nil, array, slice, map, struct, interface, chan, func, complex64, uintptr
```

#### declare variable

```js
var a;
var b = 1;
var c = 'string';
var d = true;
let e = [1, 2, 3];
const F = {hello: 1};
```

```go
// var 变量名字 类型 = 表达式
var a int = 1
// 其中“类型”或“= 表达式”两个部分可以省略其中的一个。如果省略的是类型信息，那么将根据初始化表达式来推导变量的类型信息。如果初始化表达式被省略，那么将用零值初始化该变量
var a int
var b = 2
// 声明多个变量
var i, b, k int
// 声明并赋值
var b, f, s = true, 2.3, "four"
// 常量
const freezingF, boilingF = 32.0, 212.0
// 简短声明方式
b := 1
// 声明多个
const (
    a1 = 1
    a2 = 2
    a3 = 3
)
// 使用 _ 表示定义, 而不使用
a, _ = os.Open("./file")
```

#### 内建函数或变量

```js
__dirname, setTimeout, setInterval
```

```go
make len cap new append copy close delete complex real imag panic recover
```

#### install package

```shell
$ npm install package-name  # node
$ go get module-url  # go
```

#### import & export

```js
var a = require('fs')
module.exports = function hello() {}
```

```go
import "os"

// 首字母大写, 自动导出
func Hello() {
}
```




