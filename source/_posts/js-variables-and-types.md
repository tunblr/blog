---
title: JavaScript基础 - 变量和类型
date: 2019-10-18 11:23:52
tags:
---

### 变量和类型

##### `JavaScript`规定了几种语言类型？

###### 原生类型包括6种：

- Number（数字）

- String（字符串）

- Boolean（布尔值）

- Symbol（符号）

- Null（空）

- Undefined（未定义）

###### 其余都是对象类型，例如：

- Function（函数）
- Array（数组）
- Date（日期）
- RegExp（正则表达式）

##### typeof运算符

```javascript
typeof 123 // "number"
typeof '123' // "string"
typeof false // "boolean"
function f() {}
typeof f // "function"
typeof undefined // "undefined"
typeof window // "object"
typeof {} // "object"
typeof [] // "object"
typeof null // "object" 由于历史原因，typeof null 返回 "object"
```

##### null和undefined的区别

```javascript
Number(null) // 0
5 + null // 5
Number(undefined) // NaN
5 + undefined // NaN
```


##### `JavaScript`对象的底层数据结构是什么

##### `Symbol`类型在实际开发中的应用、可手动实现一个简单的`Symbol`

##### `JavaScript`中的变量在内存中的具体存储形式

##### 基本类型对应的内置对象，以及他们之间的装箱拆箱操作

##### 理解值类型和引用类型

##### `null`和`undefined`的区别

##### 至少可以说出三种判断`JavaScript`数据类型的方式，以及他们的优缺点，如何准确的判断数组类型

##### 可能发生隐式类型转换的场景以及转换原则，应如何避免或巧妙应用

##### 出现小数精度丢失的原因，`JavaScript`可以存储的最大数字、最大安全数字，`JavaScript`处理大数字的方法、避免精度丢失的方法

