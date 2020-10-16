# JS对象笔记

## 定义

无序的数据集合

键值对的组合

## 创建方法

```js
let obj = {"name" : }
let obj = new object {"name" :}
console.log ({"name":})
```



### 如何使用变量做属性名

eg :

```js
let p1 = 'name'
let obj = {p1:"frank"}//属性名为p1
let obj = {[p1]:"frank"}//属性名为'name'
```

## 删除属性

```js
delete obj.name
delete obj['name']
'name' in obj	检查name是否在obj里面
```

## 增加属性

批量增加

```js
obj.assign(obj,(p1:1,p2:2,p3:3))
```

## 查属性

```js
Object.key(obj)
console.dir(obj)
obj['name']
obj.name//这里的name是字符串
obj[name]//这里的name是变量

```

## 改属性

```js
object['name'] = 'xxx'		//改自身
Object.assign(obj,{age:18,name:'xxx'})	//批量改自身
obj.__proto__['toString'] = 'xxx'  //改共有属性
Object.prototype['toString'] = 'xxx'  //改共有属性
obj.__proto__ = common //改原型
let obj = Object.creat(common) //改原型（推荐）


```

### 补充

'name' in obj 和obj.hasOwnProperty('name')的区别：

前者检查name是否为obj的属性（包括共有属性），后者则检查name是否为自身的属性。

eg

```js
var obj = {name:'frank'}
'name' in obj   				//true
obj.hasOwnProperty('toString')	//true
'toString' in obj  //  true
obj.hasOwnProperty('toString') //false
```

这里的toString是obj的共有属性，但不是他自身的属性，所以前者返回的是true,后者返回的是false

