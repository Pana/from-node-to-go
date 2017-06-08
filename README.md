# From Node To Go
If you are familiar with Node.js and want to learn Go, so this is right for you. And same to Goher.

* Run code
* Hello world
* Declare variable
* For loop
* Interate
* if/else
* function
* type convert
* array common operates
* string common operates
* send http requests
* create web server
* package management
* get current dir
* file common operates
* tools


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
Number, String, Boolean, Array, Object, Function, null, undefined
```

```go
int, float32, byte, string, bool, rune, nil, array, slice, map, struct, interface, chan, func, complex64, uintptr
```

#### Declaring variables

```js
var a;
var b = 1;
var c = 'string';
var d = true;
let e = [1, 2, 3];
const F = {hello: 1};
```

```go
// 直接声明一个变量
var a int
a = 1
// 声明变量并赋初始值
var a int = 1
// 省略类型, 自动推到
var b = 2
// 声明多个变量
var i, b, k int
// 声明多个变量
var width, height = 100, 50
var b, f, s = true, 2.3, "four"
var (
    name   = "naveen"
    age    = 29
    height int
)
// 常量
const freezingF, boilingF = 32.0, 212.0
// 简短声明方式
b := 1
// 使用 _ 表示定义, 而不使用
a, _ = os.Open("./file")
// var 变量名字 类型 = 表达式
// 其中“类型”或“= 表达式”两个部分可以省略其中的一个。如果省略的是类型信息，那么将根据初始化表达式来推导变量的类型信息。如果初始化表达式被省略，那么将用零值初始化该变量
```

#### builtin functions

```js
__dirname, setTimeout, setInterval, console, global, process, module, exports
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

#### Current dir

```js
__dirname
```

```go
os.Getwd()
```

#### function

```js
function add (a, b) {
    return a + b;
}

let add = (a, b) => {return a + b;}
```

```go
func add(a, b int) int {
    return a + b
}
// multiple return value
func openfile (path string) (string, error) {
    return "hello", nil
}
// rest params
func params (a, b int, ...string) int {

}
```

#### array

```js
var a = [1, 2, 3];
```

```go
// array has an specific length
var a [3]int = {1, 2, 3}
// slice's length can change dynamic
var a []int = {1, 2, 3}
```

#### object

```js
var a = {key1: 1, key2: 'hello', key3: true, key4: [], key5: {}}
```

```go
// map's value has same data type
var b map[string]int = {"k1": 1, "k2": 2, "k3": 3}
// struct
type A struct{
    k1 int
    k2 string
    k3 bool
    k4 []int
    k5 struct{}
}
var b A = {1, "hello", false, {}, {}}
```

#### if/else

```js
if (condition) {

} else {

}
```

```go
if condition {

} else if condition {

}
```

#### loops

```js
for (initialisation; condition; post) {
}
for (var i = 0; i < 10; i++) {

}
```

```go
for initialisation; condition; post {
}
for var i = 0; i < 10; i++ {

}
// infinite loop
for {
}
```


#### iterate

```js
for (var i in array) {
    console.log(i, array[i]);
}
// ES6
for (var t of iterator) {
    console.log(t)
}
```


```go
//
for key, val := range mapObject {

}
```





