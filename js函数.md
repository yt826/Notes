# js函数

## 函数的声明

```js
function 函数名(){}
let f1 = x => x*x			//传入参数x,返回x*x
let f1 = (x,y) => x+y    		//传入x和y 返回x+y
let f1 = (x,y) => ({name:x,name:y})		//返回对象时需要加括号，不然会出错。

```

## this和arguments

代码

```js
function fn (){
    console.log(arguments)
    console.log(this)  
}
```





