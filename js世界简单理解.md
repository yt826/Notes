# js世界简单理解

在学习JS的过程中，我们会遇到三座大山，

- 原型

- this

- AJAX

  

接下来，我会简单的谈一谈我对于我对于原型的理解

## 三个重要的知识

### 1. js公式

对象.__proto__ === 其构造函数.prototype

也就是任何对象的原型都是其构造函数的prototype对象

eg:

```js
let obj = new Object()
obj__proto__ === Object.prototype//true
let arr = new Array()
arr.__proto__ === Array.prototype//true
```

### 2.根公理

Object.prototype是所有对象的（直接或间接）原型

### 3. 函数公理

所有的函数都是由Function构造的

```js
任何函数.__proto__ === Function.prototype
任意函数有Object/Array/Function
```

在这里我们得先明确几个概念

“的原型”等价于“.__proto__”

eg：

Object的原型是Object.__proto__ 而不是Object.prototype

原型分为两种：直接原型和间接原型

对于普通对象来说，Object.prototype是直接原型

对于数组、函数对象来说，Object.prototype是间接对象



### JS世界的构造顺序

接下来我们来简单的介绍一下JS世界的构造顺序

1. 创建根对象#101(toString)，根对象没有名字

2. 创建函数的原型#208（call/apply）,原型__p为#101

3. 创建数组的原型#404（push/pop）,原型__p为#101

4. 创建Function#342，原型__p为#208

5. 用Function.prototype存储函数的原型，等于#208

6. 这里我们发现Function的__proto__和prototype都是#208

7. 用Function创建Object

8. Object.prototype存储对象的原型，等于#101

9. 用Function创建Array

10. 用Array.prototype存储数组的原型，等于#404

11. 创建window对象

12. 用window的'Object' 'Array'属性将7和9中的函数命名

13. 记住一点，js创建一个对象时，不会给这个对象名字的。

    

续：

- 用new Object创建obj1
- new 会将obj1的原型__p设置为Object.prototype,也就是#101
- 用new Array()创建arr1
- new  会将arr1的原型__p设置为Array.protoype，也就是#404
- 用new Function创建f1
- new 会将f1的原型__p设置为Function.prototype，也就是#208