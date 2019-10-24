---
title: JavaScript的语言类型
date: 2019-10-18 11:23:52
tags:
---

### `JavaScript`规定了几种语言类型？

###### [原始](https://developer.mozilla.org/en-US/docs/Glossary/Primitive)类型包括7种：

- [Boolean](https://developer.mozilla.org/en-US/docs/Glossary/Boolean)（布尔值）
- [Null](https://developer.mozilla.org/en-US/docs/Glossary/Null)（空）
- [Undefined](https://developer.mozilla.org/en-US/docs/Glossary/Undefined)（未定义）
- [Number](https://developer.mozilla.org/en-US/docs/Glossary/Number)（数字）
- [BigInt](https://developer.mozilla.org/en-US/docs/Glossary/BigInt)
- [String](https://developer.mozilla.org/en-US/docs/Glossary/String)（字符串）
- [Symbol](https://developer.mozilla.org/en-US/docs/Glossary/Symbol)（符号）

###### 其余都是[对象](https://developer.mozilla.org/en-US/docs/Glossary/Object)类型，例如：

- [Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function)（函数）
- [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)（数组）
- [String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)（字符串）
- [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)（日期）
- [RegExp](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp)（正则表达式）

##### `typeof`运算符

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

##### `null`和`undefined`的区别

`null`表示一个“空”的对象，`undefined`表示一个“未定义”的原始值

```javascript
Number(null) // 0
5 + null // 5
Number(undefined) // NaN
5 + undefined // NaN
```

返回`undefined`的典型场景

```javascript
// 变量声明了，但没有赋值
var i;
i // undefined

// 调用函数时，应该提供的参数没有提供，该参数等于 undefined
function f(x) {
  return x;
}
f() // undefined

// 对象没有赋值的属性
var  o = new Object();
o.p // undefined

// 函数没有返回值时，默认返回 undefined
function f() {}
f() // undefined
```

[细说 JavaScript 七种数据类型](https://www.cnblogs.com/onepixel/p/5140944.html)