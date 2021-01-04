---
title: JavaScript
---

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [JavaScript](#javascript)
  - [一. 类型](#一-类型)
    - [1.1 数据类型](#11-数据类型)
      - [1.1.1 Undefined](#111-undefined)
      - [1.1.2 Null](#112-null)
      - [1.1.3 String](#113-string)
      - [1.1.4 Number](#114-number)
      - [1.1.5 Symbol](#115-symbol)
      - [1.1.6 Object](#116-object)
    - [1.2 类型转换](#12-类型转换)
    - [1.3 其他常用规范类型](#13-其他常用规范类型)
  - [二. 面向对象](#二-面向对象)
    - [2.1 JS对象的特征](#21-js对象的特征)
    - [2.2 JS对象的两类属性](#22-js对象的两类属性)
      - [2.2.1 数据属性](#221-数据属性)
      - [2.2.2 访问器属性（getter/setter）](#222-访问器属性gettersetter)
    - [2.3 JS的原形](#23-js的原形)
      - [2.3.1 概述](#231-概述)
      - [2.3.2 JS的原形](#232-js的原形)
      - [2.3.3 早期版本中的类与原型](#233-早期版本中的类与原型)
      - [2.3.4 ES6中的类](#234-es6中的类)
    - [2.4 JS的对象](#24-js的对象)
      - [2.4.1 对象的分类](#241-对象的分类)
        - [2.4.1.1 宿主对象（host Object）](#2411-宿主对象host-object)
        - [2.4.1.2 内置对象·固有对象（intrinsic Object）](#2412-内置对象固有对象intrinsic-object)
        - [2.4.1.3 内置对象·原生对象（Native Object）](#2413-内置对象原生对象native-object)
      - [2.4.2 用对象来模拟函数和构造器：函数对象和构造器对象](#242-用对象来模拟函数和构造器函数对象和构造器对象)
      - [2.4.3 特殊行为的对象](#243-特殊行为的对象)
  - [三. JS的执行](#三-js的执行)
    - [3.1 Promise、async/await](#31-promise-asyncawait)
      - [3.1.1. 宏观和微观任务](#311-宏观和微观任务)
      - [3.1.2 Promise](#312-promise)
      - [3.1.3 async/await](#313-asyncawait)
    - [3.2 闭包](#32-闭包)
    - [3.3 执行上下文：执行的基础设施](#33-执行上下文执行的基础设施)
    - [3.4 var的声明与赋值](#34-var的声明与赋值)
    - [3.5 let](#35-let)
    - [3.6 Realm](#36-realm)
    - [3.7 函数的种类](#37-函数的种类)
    - [3.8 this 关键字](#38-this-关键字)
      - [3.8.1 行为](#381-行为)
      - [3.8.2 机制](#382-机制)
      - [3.8.3 操作this的内置函数](#383-操作this的内置函数)
    - [3.9 语句](#39-语句)
      - [3.9.1 Completion 类型](#391-completion-类型)
  - [四. 文法](#四-文法)
    - [4.1. 词法](#41-词法)
      - [4.1.1 空白符号 WhiteSpace](#411-空白符号-whitespace)
      - [4.1.2 换行符 LineTerminator](#412-换行符-lineterminator)
      - [4.1.3 注释 Comment](#413-注释-comment)
      - [4.1.4 标识符名称 IdentifierName](#414-标识符名称-identifiername)
      - [4.1.5 符号 Punctuator](#415-符号-punctuator)
      - [4.1.6 数字直接量 NumericLiteral](#416-数字直接量-numericliteral)
      - [4.1.7 字符串直接量 StringLiteral](#417-字符串直接量-stringliteral)
      - [4.1.8 正则表达式直接量 RegularExpressionLiteral](#418-正则表达式直接量-regularexpressionliteral)
      - [4.1.10 字符串模板 Template](#4110-字符串模板-template)
    - [4.2 语法](#42-语法)
      - [4.2.1 自动插入分号](#421-自动插入分号)
      - [4.2.2 no LineTerminator here 规则](#422-no-lineterminator-here-规则)
      - [4.2.3 语法](#423-语法)
        - [4.2.3.1 import声明](#4231-import声明)
        - [4.2.3.2 export声明](#4232-export声明)
        - [4.2.3.3 函数体](#4233-函数体)
        - [4.2.3.4 预处理](#4234-预处理)
          - [4.2.3.4.1 var声明](#42341-var声明)
          - [4.2.3.4.2 function声明](#42342-function声明)
          - [4.2.3.4.3 class声明](#42343-class声明)
        - [4.2.3.5 指令序言机制](#4235-指令序言机制)
      - [4.2.4 语句](#424-语句)
        - [4.2.4.1 语句块](#4241-语句块)
        - [4.2.4.2 空语句](#4242-空语句)
        - [4.2.4.3 if语句](#4243-if语句)
        - [4.2.4.4 switch语句](#4244-switch语句)
        - [4.2.4.5 循环语句](#4245-循环语句)
          - [4.2.4.5.1 while循环 和 do while循环](#42451-while循环-和-do-while循环)
          - [4.2.4.5.2 普通for循环](#42452-普通for循环)
          - [4.2.4.5.3 for in 循环](#42453-for-in-循环)
          - [4.2.4.5.4 for of 循环和 for await of 循环](#42454-for-of-循环和-for-await-of-循环)
        - [4.2.4.6 return](#4246-return)
        - [4.2.4.7 break 和 continue](#4247-break-和-continue)
        - [4.2.4.8 try 语句和 throw语句](#4248-try-语句和-throw语句)
        - [4.2.4.9 debugger语句](#4249-debugger语句)
        - [4.2.4.10 var](#42410-var)
        - [4.2.4.11 let和const](#42411-let和const)
        - [4.2.4.12 class声明](#42412-class声明)
        - [4.2.4.13 函数声明](#42413-函数声明)
      - [4.2.5 表达式语句](#425-表达式语句)
        - [4.2.5.1 PrimaryExpression 主要表达式](#4251-primaryexpression-主要表达式)
        - [4.2.5.2 Member Expression 成员表达式](#4252-member-expression-成员表达式)
        - [4.2.5.3 New Expression New表达式](#4253-new-expression-new表达式)
        - [4.2.5.4 call Expression 函数调用表达式](#4254-call-expression-函数调用表达式)
        - [4.2.5.5 LeftHandSideExpression 左值表达式](#4255-lefthandsideexpression-左值表达式)
        - [4.2.5.6 AssignmentExpression 赋值表达式](#4256-assignmentexpression-赋值表达式)
        - [4.2.5.7 Expression 表达式](#4257-expression-表达式)
        - [4.2.5.8 ConditionalExpression 条件表达式](#4258-conditionalexpression-条件表达式)
        - [4.2.5.9 UpdateExpression 更新表达式](#4259-updateexpression-更新表达式)
        - [4.2.5.10 UnaryExpression 一元运算表达式](#42510-unaryexpression-一元运算表达式)
        - [4.2.5.11 ExponentiationExpression 乘方表达式](#42511-exponentiationexpression-乘方表达式)
        - [4.2.5.12 MultiplicativeExpression 乘法表达式](#42512-multiplicativeexpression-乘法表达式)
        - [4.2.5.13 AdditiveExpression 加法表达式](#42513-additiveexpression-加法表达式)
        - [4.2.5.14 ShiftExpression 移位表达式](#42514-shiftexpression-移位表达式)
        - [4.2.5.15 关系表达式 RelationalException](#42515-关系表达式-relationalexception)
        - [4.2.5.16 相等表达式 EqualityExpression](#42516-相等表达式-equalityexpression)
        - [4.2.5.17 位运算表达式](#42517-位运算表达式)
        - [4.2.5.18 逻辑与表达式和逻辑或表达式](#42518-逻辑与表达式和逻辑或表达式)
      - [4.2.5.19 TernaryOperatorExpression 三目运算符](#42519-ternaryoperatorexpression-三目运算符)

<!-- /code_chunk_output -->

# JavaScript

----

![JavaScript知识架构](./image/JavaScript知识架构.png)

## 一. 类型

### 1.1 数据类型

JS 语言的每一个值都属于某一种数据类型。JS 语言规定了 **7** 种语言类型。
语言类型广泛用于变量、函数参数、表达式、函数返回值等场合，运行时类型是代码实际执行过程中用到的类型。
所有的类型数据都会属于 7 个类型之一。从变量、参数、返回值到表达式中间结果，任何 JS 代码运行过程中产生的数据，都具有运行时类型。

1. Undefined
2. Null
3. Boolean
4. String
5. Number
6. Symbol
7. Object

#### 1.1.1 Undefined

Undefined表示未定义，它的类型只有一个值，就是 undefined。任何变量在赋值前都是 Undefined 类型，值为 undefined，一般情况下可以用undefined（就是名为undefined的这个全局变量）来表达这个值，或者void运算来把任意一个表达式变成undefined值。

> 建议使用 `void 0` 或 `void(0)` 来获取 undefined 值。在实际编程时，一般不会把变量赋值为 undefined，这样可以保证所有值为 undefined 的变量，都是从未赋值的自然状态。

#### 1.1.2 Null

Null表示的是："定义了但是为空"。Null的类型也只有一个值，就是null，与undefined 不同 `null` 是JS关键字，在任何程序中，都可以使用null 关键字来获取 null 值。

#### 1.1.3 String

**字符串是否有最大长度？**
String 用于表示文本数据，String 有最大长度是 **2^53 - 1**，String的意义并非字符串，而是字符串的UTF16编码，字符串的操作 `charAt`、`charCodeAt`、`length` 等方法针对的都是UTF16编码。所以字符串最大长度，是受字符串的编码长度影响。

JS 中的字符串是永远无法变更的，所以字符串具有值类型的特征

> 注意 : JS 字符串把每个UTF16单元当作一个字符来处理，所以处理非 BMP（超出 U+0000 - U+FFFF 范围）的字符时，应该格外小心。

#### 1.1.4 Number

JS 中的 Number 类型有 **18437736874454810627(即 2^64-2^53+3)** 个值。

JS 中的 Number 类型基本符合 IEEE 754-2008 规定的双精度浮点数规则，但是 JS 为了表达几个额外的语言场景（比如，不让除以 0 出错，而引入了无穷大的概念），规定了几个例外情况：

- **NaN** : NaN规定和参考双精度浮点数的表达方式，1位符号位+52位尾数位共53位，指数固定为 2^e–1 并去掉 ±∞ 两个值，NaN其实是 2^53-2 个特殊数字的合集（2^53-2 = 9007199254740990 ）所以，为什么NaN !== NaN，因为它不是一个值，而是一群值
- **Infinity** : 无穷大
- **-Infinity** : 负无穷大

注意:

1. JS中有 +0 和 -0，在加法类运算中没有区别，但是在除法的场合需要特别留意，除以 -0 会得到 负无穷大,除以 +0 会得到 正无穷大，而区分 +0 或 -0 的方式是 `1/x` 是 Infinity 还是 -Infinity

2. 根据双精度浮点数的定义，Number 类型中有效的整数范围是 -0x1fffffffffffff 至 0x1fffffffffffff，所以 Number 无法精确表示此范围外的整数。同样根据浮点数的定义，非整数的 Number 类型无法用 ==（=== 也不行） 来比较，也就是 console.log(0.1 + 0.2 == 0.3)，这里输出的是 false，说明两边不相等，这是浮点运算的特点（number类型运算都要将其转化为二进制，将二进制运算，运算的结果再转化为十进制，因为number是64位双精度，小数部分只有52位，但0.1转化成为二进制是无限循环的，所以四舍五入了这里就发生了精度丢失，0.1的二进制和0.2的二进制相加需要保留有效数字，所以又发生了精度丢失，所以结果为0.30000000000000004）。浮点数运算的精度问题导致等式左右的结果并不是严格相等，而是相差了个微小的值。
正确的比较方法是使用JS提供的最小精度值：`console.log(Math.abs(0.1 + 0.2 - 0.3) <= Number.EPSILON)` 检查等式两侧的绝对值是否小于绝对精度，才是正确比较浮点数的方法。

**Number.EPSILON**
: ES6 在Number对象上面，新增一个极小的常量 `Number.EPSILON`。Number.EPSILON = 2.220446049250313e-16。根据规范，它表示 1 与大于 1 的最小浮点数之间的差。对于 64 位浮点数来说，大于 1 的最小浮点数相当于二进制的1.00..001，小数点后面有连续 51 个零。这个值减去 1 之后，就等于 2 的 -52 次方。Number.EPSILON实际上是 JS 能够表示的最小精度。误差如果小于这个值，就可以认为已经没有意义了，即不存在误差了。引入一个这么小的量的目的，在于为浮点数计算，Number.EPSILON可以用来设置"能够接受的误差范围"。

#### 1.1.5 Symbol

`Symbol` 是 ES6 中引入的新类型，它是一切非字符串的对象 `key` 的集合，在ES6规范中，整个对象系统被用 `Symbol` 重塑。
Symbol可以具有字符串类型的描述，但是即使描述相同，Symbol也不相等。
创建Symbol的方式是使用全局的Symbol函数。

```js
var symbol = Symbol("my symbol")
```

可以使用 `Symbol.iterator` 来自定义 `for…of` 在对象上的行为。当需要对一个对象进行迭代时（比如开始用于一个for..of循环中），它的 `Symbol.iterator` 方法都会在不传参情况下被调用，返回的迭代器用于获取要迭代的值。

[Symbol.iterator为对象定义默认迭代器](./HTML演示文件/Symbol.iterator为对象定义默认迭代器.html)

#### 1.1.6 Object

Object 是JS中最复杂的类型，也是JS的 **核心机制之一**，Object表示对象的意思，它是一切有形和无形物体的总称。
在JS中对象的定义是 "属性的集合"。属性分为 **数据属性** 和 **访问器属性** ，两者都是 `key-value` 结构，`key`可以是字符串或Symbol类型。

提到对象，必须提到一个概念：类，JS中的类仅仅是运行时对象的一个私有属性，JS中无法自定义类型。

JS中的几个基本类型，都在对象中有一个"亲戚"：

- String
- Boolean
- Number
- Symbol

在JS中，`3` 和 `new Number(3)` 是两个完全不同的值，`3` 是 Number 类型，`new Number(3)` 是对象类型。

Number、Boolean、String，三个构造器是两用的，当跟 `new` 搭配时，它们产生对象，当单独使用时，表示强制类型转换。
Symbol比较特殊，直接用 `Symbol` 调用它会抛出错误，但它依然是Symbol对象的构造器。

JS在语言设计上试图模糊基本类型与对象之间的关系，在日常代码中可以把对象的方法放在基本类型上使用

```js
console.log("ab".charAt(0));
```

甚至在原型上添加方法都可以应用于基本类型， `.` 运算符提供了装箱操作，它会根据基础类型构造一个临时对象，使能在基础类型上调用对应对象的方法。

### 1.2 类型转换

JS是弱类型语言，所以类型转换发生的非常频繁，大部分常用的运算都会先进行类型转换。

![JS类型转换规则](./image/JS类型转换规则.jpg)

**StringToNumber**
: 字符串到数字的类型转换，存在一个语法结构，类型转换支持二进制，八进制，十进制，十六进制，此外，JS支持的字符串语法还包括，正负号科学计数法，可以使用大写或小写的 `e` 来表示

```js
Number("1e3") = 1 * 10^3 = 1000
Number(-1e-2) = -1 * 10^-2 = -0.01
```

> 注意:
> `parseInt` 和 `parseFloat` 并不使用这个转换，所以支持的语法跟 Number 不同。
> `parseInt`，在不传入第二个参数时，如果第一个参数是Number类型，会自动识别进制（不可靠），而且会遇到非数字直接返回非数字前面的数字，如果第一个参数是字符串，只能识别十六进制，也不支持科学计数法，所以需要传入第二个参数。
> `parseFloat` 直接把原字符串作为十进制解析，它不会引入任何其他进制。多数情况下，Number 是比 parseInt 和 parseFloat 更好的选择。

**NumberToString**
: 在较小的范围内，数字到字符串的转换是完全符合直觉的十进制表示。当 Number 绝对值较大或者较小时，字符串则是使用科学计数法表示的。是为了保证产生的字符串不会过长。具体算法，看JS语言标准。

**装箱转换**
: 每一种基本类型Number、String、Boolean、Symbol在对象中都有对应的类，所谓装箱转换就是把基本类型转换为对应的对象，它是类型转换中一种相当重要的种类。

全局的Symbol函数无法使用 new 来调用，但可以使用装箱机制来得到一个 Symbol 对象，可以利用函数的 `.call()` 方法来强迫产生装箱。

```js
var symbolObject = (function(){ return this; }).call(Symbol("a"));
console.log(typeof symbolObject); //object
console.log(symbolObject instanceof Symbol); //true
console.log(symbolObject.constructor == Symbol); //true
```

> 装箱机制会频繁产生临时对象，在对性能要求较高的场景下，应该尽量避免对基本类型做装箱转换。

使用内置的Object函数，可以JS代码中显式的调用装箱能力

```js
var symbolObject = Object(Symbol("a"));
console.log(typeof symbolObject); //object
console.log(symbolObject instanceof Symbol); //true
// 原型链 symbolObject.__proto__  =>  Symbol.__proto__ => Object
console.log(symbolObject.constructor == Symbol); //true
```

每一类装箱对象都有私有的Class属性，这些属性可以用 `Object.prototype.toString` 获取

```js
var symbolObject = Object(Symbol("0"));
var symbolT      = Symbol("b");
console.log(Object.prototype.toString.call(symbolObject)); // [Object Symbol]
console.log(Object.prototype.toString.call(symbolT)); // [Object Symbol]
console.log(typeof symbolObject); // Object
console.log(typeof symbolT); // Symbol
```

> 1. 在JS中没有任何方法可以改变私有的Class属性，所以，`Object.prototype.toString` 是可以准确识别对象对应的基本类型的方法，它比 `instanceof` 更准确，需要注意 `.call()` 会产生装箱操作，所以需要配合 `typeof` 来区分基本类型还是对象类型
> 2. `instanceof` 运算符用来判断一个构造函数的 prototype属性(或对象的__proto__) 所指向的对象是否存在另外一个要检测对象的原型链上。

**拆箱转换**
: 在JS标准中，规定了 `toPrimitive` 函数，它是对象类型到基本类型的转换（即拆箱转换）。
对象到 String 和 Number 的转换都遵循 "先拆箱再转换" 的规则，通过拆箱转换，把对象先转为基本类型，再从基本类型转为对应的String或Number。
所以，拆箱转换会先尝试调用 `valueOf` 和 `toString` 来获取拆箱后的基本类型，如果 `typeOf` 和 `toString` 都不存在或没有返回基本类型，则会报类型错误TypeError。

```js
// 拆箱转换会先尝试调用 valueOf 和 toString 来获得拆箱后的基本类型，如果 valueOf 和 toString 都不存在或没有返回基本类型，则会产生类型错误TypeError
var o = {
  // 箭头函数表达式适用于需要匿名函数的地方,并且它不能用作构造函数。
  valueOf  : () => { console.log("valueOf"); return {}},
  toString : () => { console.log("toString"); return {}}
};

o * 2;
// valueOf
// toString
// TypeError: Cannot convert object to primitive value
```

```js
// 到String的拆箱转换会优先调用toString，调用顺序变化
var o = {
  valueOf : () => {console.log("valueOf"); return{}},
  toString: () => {console.log("toString"); return{}}
}

String(o);
// toString
// valueOf
// TypeError: Cannot convert object to primitive value
```

```js
// 在ES6之后，还允许对象通过显式指定 @@toPrimitive Symbol 来覆盖原有的行为
var o = {
  valueOf : () => { console.log("valueOf"); return {}},
  toString : () => { console.log("toString"); return {}}
}
o[Symbol.toPrimitive] = () => { console.log("toPrimitive"); return "hello"}

console.log(o + " World");
// toPrimitive
// hello World
```

“类型”在 JS 中是一个有争议的概念。一方面，标准中规定了运行时数据类型；另一方面，JS 语言中提供了 `typeof` 这样的运算，用来返回操作数的类型，但 `typeof` 的运算结果，与运行时类型的规定有很多不一致的地方。

![JS类型对照表](./image/JS类型对照表.png)

> **注意** : object——Null 和 function——Object 是特例，理解类型的时候需要特别注意这个区别。

### 1.3 其他常用规范类型

1. List 和 Record：用于描述函数传参过程。
2. Set：主要用于解释字符集等。
3. Completion Record：用于描述异常、跳出等语句执行过程。
4. Reference：用于描述对象属性访问、delete 等。
5. Property Descriptor：用于描述对象的属性。
6. Lexical Environment 和 Environment Record：用于描述变量和作用域。
7. Data Block：用于描述二进制数据。

## 二. 面向对象

JS标准对 基于对象 的定义
: 语言和宿主的基础设施由对象来提供，并且JS程序即是一系列互相通讯的对象的集合。

### 2.1 JS对象的特征

1. **对象具有唯一标识性** : 即使两个完全相同的对象，也并非同一个对象。一般而言，对象的唯一标识性，是用内存地址来体现的，对象具有唯一标识的内存地址，所以具有唯一的标识。
2. **对象有状态** : 对象具有状态，同一个对象可能处于不同状态下
3. **对象有行为** : 即对象的状态可能因为它的行为产生变迁

在JS中将状态和行为统一抽象为属性，JS中将函数设计成一种特殊对象，所以，JS中的状态和行为都能用属性来抽象。

JS对象独有的特色：对象具有高度的动态性，因为JS赋予了使用者在运行时为对象添改状态和行为的能力。

为了提高抽象能力，JS的属性被设计成比其他语言更复杂的形式，它提供了 **数据属性** 和 **访问器属性（getter/setter）** 两类。

### 2.2 JS对象的两类属性

对于JS，属性并非简单的名称和值，JS用一组特征（attribute）来描述属性（property）

#### 2.2.1 数据属性

特征

1. value：就是属性的值
2. writable：决定属性能否被赋值
3. enumerable：决定 for in 能否枚举该属性
4. configurable：决定该属性能否被删除或改变特征值

通常用于定义属性的代码会产生数据属性，其中的 writable、enumerable、configurable都默认为true。可以使用内置函数 `Object.getOwnPropertyDescriptor` 来查看。

```js
// 数据属性具有4个特征
var o = { a : 1 };
o.b = 2;
// 可以使用内置函数 Object.getOwnPropertyDescriptor 来查看
console.log(Object.getOwnPropertyDescriptor(o,"a")); // {value: 1, writable: true, enumerable: true, configurable: true}
console.log(Object.getOwnPropertyDescriptor(o,"b")); // {value: 2, writable: true, enumerable: true, configurable: true}
```

#### 2.2.2 访问器属性（getter/setter）

特征

1. getter：描述获取该属性值时调用的函数，并返回函数的结果，默认值为undefined
2. setter：描述该属性被赋值时调用的函数，默认值为undefined
3. enumerable：决定 for in 能否枚举该属性
4. configurable：决定该属性能否被删除或者改变特征值

访问器属性使得属性在读和写时执行代码，它允许使用者在写和读时得到完全不同的值，它可以视为函数的一种语法糖。

使用 `Object.defineProperty`，可以 **改变特征值** 或 **定义访问器属性**，但是不能同时指定 访问器属性和值或可写属性 writable。

```js
var o = { a : 1 };
// Object.defineProperty 可以改变特征值
Object.defineProperty(o, "a", {writable:false});
Object.defineProperty(o, "b", {value: 2, writable:false, enumerable:false, configurable:true});
console.log(Object.getOwnPropertyDescriptor(o, "a")); // {value: 1, writable: false, enumerable: true, configurable: true}
console.log(Object.getOwnPropertyDescriptor(o, "b")); // {value: 2, writable: false, enumerable: false, configurable: true}
o.b = 3;
console.log(o.b); // 2  writable: false o对象的b属性不能被赋值
```

在创建对象时，也可以使用 `get` 和 `set` 关键字来创建访问器属性，访问器属性跟数据属性不同，每次访问属性都会执行 `getter` 或者 `setter` 函数。

```js
// object.defineProperty 使用 get 和 set 关键字来创建访问器属性
var o = { a : 1 };
// 不能同时指定访问器属性和 值或可写属性writable
Object.defineProperty(o, "b", { enumerable : false, get: () => { return o.a + "get";}, set : (value) => { o.a = value; } });
console.log(o.b); // 1get
o.b = 3;
console.log(o.b); // 3get
console.log(o.a); // 3
```

**总结**：
实际上JS对象的运行时是一个 "具有高度动态性的属性集合"，属性以 **字符串** 或 **Symbol** 为 `key`，以 **数据属性特征值** 和 **访问器属性特征值** 为 `value`。
对象是一个属性的索引结构（索引结构是一种常见的数据结构，可以把它理解为一个能够以较快速度用key来查找value的字典），能够以Symbol为属性名是JS对象的一个特色。

### 2.3 JS的原形

#### 2.3.1 概述

原型是顺应人类自然思维的产物。是用来描述对象的一种方法。

“基于原型”的编程更为提倡去关注一系列对象实例的行为，而后才去关心如何将这些对象，划分到最近的使用方式相似的原型对象，而不是将它们分成类。

基于原型的面向对象系统通过“复制”的方式来创建新对象。一些语言的实现中，还允许复制一个空对象。这实际上就是创建一个全新的对象。

原型系统的“复制操作”有两种实现思路：

- 并不真的去复制一个原型对象，而是使得新对象持有一个原型的引用。
- 切实地复制对象，从此两个对象再无关联。

**JS使用的是第一种实现思路。**

#### 2.3.2 JS的原形

如果抛开JS用于模拟Java的复杂语法设施（如 new、Function Object、函数的prototype属性等），可以用两条概括：

1. 如果所有对象都有私有字段 [`[[prototype]]`](#__proto__)（即__proto__），就是对象的原形

2. 读一个属性，如果对象没有，则会继续访问对象的原形，直到原形为空或找到为止

ES6以来，JS提供了一系列的内置函数，以便更为直接的访问操纵原形

- `Object.create` : 根据指定的原形创建新对象，原形可以是null
- `Object.getPrototypeOf` : 获得一个对象的原形
- `Object.setPrototypeOf` : 设置一个对象的原形

利用这三个方法，可以完全抛开类的思维，利用原型来实现抽象和复用。

```js
// 创建一个对象cat
var cat = {
  say() {
    console.log("meow~");
  },
  jump() {
    console.log("jump");
  }
}

/*
*  使用 Object.create 根据cat对象做了一些修改创建了一个tiger对象
*/
var tiger = Object.create(cat, {
  say: {
    writable: true,
    configurable: true,
    enumerable: true,
    value: () => {
      console.log("roar!");
    }
  }
})

// 使用Object.create 创建其他cat对象，可以通过控制原始cat对象来控制所有cat对象的行为
var anotherCat = Object.create(cat);
anotherCat.say();   // meow~
anotherCat.jump();  // jump

// 使用Object.getPrototypeOf 来获得一个对象的原形
console.log(Object.getPrototypeOf(anotherCat)); // {say: ƒ, jump: ƒ}

var anotherTiger = Object.create(tiger);
anotherTiger.say();   // roar!
anotherTiger.jump();  // jump
console.log(Object.getPrototypeOf(anotherTiger)); // {say: ƒ}

var blueTiger = new Object();
blueTiger.name = "小明";
blueTiger.eat  = () => { console.log("eat meat"); }
console.log(blueTiger.name); // 小明
blueTiger.eat(); // eat meat
// 使用 Object.setPrototypeOf(a, b) 来设置对象的原形  a 是 要设置的对象，b是原形
Object.setPrototypeOf(blueTiger, tiger);
blueTiger.say(); // roar!
blueTiger.jump(); // jump
```

#### 2.3.3 早期版本中的类与原型

在早期版本的JS中，"类"的定义是一个私有属性 `[[class]]`，语言标准为内置类型如：Number、String、Date 等指定了 `[[class]]` 属性，以表示它们的类。唯一可以访问 `[[class]]` 属性的方式是 `Object.prototype.toString` 。

从ES5开始，`[[class]]` 私有属性被 `Symbol.toStringTag` 替代，`Object.prototype.toString` 的意义从命名上不再跟class相关，甚至可以自定义。

```js
// 使用 Symbol.toStringTag 来自定义 Object.prototype.toString
var o = { [Symbol.toStringTag] : "MY"} // 创建一个对象，给它唯一的属性 Symbol.toStringTag
console.log(o + "") // [object MY]     使用 + 来触发 Object.prototype.toString 的调用，发现这个属性最终对 Object.prototype.toSting 的结果产生了影响
```

new 运算接受一个构造器和一组调用参数，实际上做了3件事

1. 以构造器的prototype属性为原形，创建新对象
2. 将 this 和 调用参数 传给构造器，执行
3. 如果构造器返回的是对象，则返回，否则返回第一步创建的对象

new 这样的行为，试图让函数对象在语法上跟类变得相似，但是，new 客观上提供了两种添加属性的方式:

1. 在构造器中添加属性
2. 在构造器的 prototype 上添加属性

```js
// 直接在构造器中修改 this，给 this 添加属性。
function c1(){
    this.p1 = 1;
    this.p2 = function(){
        console.log(this.p1);
    }
}
var o1 = new c1;
o1.p2(); // 1

// 修改构造器的 prototype 属性指向的对象，它是从这个构造器构造出来的所有对象的原型。
function c2(){
}
c2.prototype.p1 = 2;
c2.prototype.p2 = function(){
    console.log(this.p1);
}

var o2 = new c2;
o2.p2(); // 2
```

#### 2.3.4 ES6中的类

ES6 中引入了 `class` 关键字，并且在标准中删除了所有 `[[class]]` 相关的私有属性描述，类的概念正式从属性升级成语言的基础设施，从此，基于类的编程方式成为了 JS 的官方编程范式。

> 在任何场景下都优先使用ES6的语法来定义类，令 function 回归原本的函数定义。

  ```js
  class Rectangle {
    constructor(height, width) {
      this.height = height;
      this.width = width;
    }
    // 通过get关键字来创建 getter
    get area() {
      return this.calcArea();
    }
    // Method
    calcArea() {
      return this.height * this.width;
    }
    let r = new Rectangle(2, 6);
    console.log(r.area); // 4
    console.log(r.calcArea()); // 12
  }
  ```

在现有的类语法中，`getter/setter` 和 `method` 是兼容性最好的。

通过 `get/set` 关键字来创建 `getter/setter`，通过括号和大括号来创建方法，数据型成员最好写在构造器里面。

类的写法实际上也是由原型运行时来承载的，逻辑上 JS 认为每个类是有共同原型的一组对象，类中定义的方法和属性则会被写在原型对象之上。

类通过 `extends` 关键字提供了继承能力，使用 `extends` 关键字会自动设置了 `constructor`，并且会自动调用父类的构造函数。使用类的思想来设计代码时，应该尽量使用 `class` 来声明类，而不是用函数来模拟对象。

  ```js
  class Animal {
    constructor(name, sex) {
      this.name = name;
      this.sex = sex;
    }

    get h() {
      console.log(this.name + " is " + this.sex);
    }

    set sex(sex) {
      // 创建一个新的数据型成员_sex 和 sex 不是同一个值
      // 不可以写 this.sex = sex，因为定义了sex的读写器，给 this.sex 赋值的时候会调用 set sex ，这样会导致无限递归直到栈溢出
      this._sex = sex;
      console.log(this.name + " is " + this._sex);
    }

    set setName(name) {
      this.name = name;
      console.log("My name is " + this.name);
    }

    speak() {
      console.log(this.name + " makes a noise!");
    }

    setNameAndSex(name) {
      this.name = name;
      console.log("Set name " + this.name);
    }
  }

  // Dog类 通过 extends 关键字继承了 Animal类
  // 使用 extends 关键字自动设置了 constructor，并且会自动调用父类的构造函数
  class Dog extends Animal {
    constructor(name) {
      super(name); // 调用super()类构造函数并传递name参数
    }

    speak() {
      console.log(this.name + " barks!");
    }

    // 使用 static 关键字定义静态方法
    static formatName(name) {
      return name[2].toUpperCase();
    }
  }

  let d = new Dog("HanHan");
  d.speak(); // HanHan barks!
  d.h; // HanHan is undefined
  d.sex = "男"; // HanHan is 男
  d.setName = "Tom"; // My name is Tom
  console.log(Dog.formatName("HanKe")); // N
  d.setNameAndSex("刘禅"); // Set name 刘禅
  ```

### 2.4 JS的对象

#### 2.4.1 对象的分类

- 宿主对象（host Object）: 由 JS 宿主环境提供的对象，它们的行为完全由宿主环境决定
- 内置对象（Built-in Object）: 由 JS 语言提供的对象
  - 固有对象（intrinsic Object）：由标准规定，随着JS运行时创建而自动创建的对象实例。
  - 原生对象（Native Object）：可以由用户通过 Array、RegExp 等内置构造器或特殊语法创建的对象。
  - 普通对象（Ordinary Object）：由 `{}` 语法、`Object`构造器 或 `class` 关键字定义类创建的对象，它能够被原形继承。

##### 2.4.1.1 宿主对象（host Object）

在浏览器环境中，全局对象是 window，window上又有很多属性，如：document。
window上的属性，一部分来自JS语言，另一部分来自浏览器环境。
JS标准中规定了全局对象属性，W3C的各种标准中规定了Window对象的其他属性。
宿主对象也分 固有 和 用户可创建，比如：`document.createElement` 就可以创建一些DOM对象。
宿主也会提供一些构造器，比如可以使用 `new Image` 来创建 img 元素。

##### 2.4.1.2 内置对象·固有对象（intrinsic Object）

固有对象是由标准规定，随着 JS 运行时创建而自动创建的对象实例。

固有对象在任何 JS 代码执行前就已经被创建出来了，它们通常扮演者类似基础库的角色

ECMA 标准为提供了一份固有对象表，里面含有 150+ 个固有对象，可以通过 [这个链接](https://www.ecma-international.org/ecma-262/9.0/index.html#sec-well-known-intrinsic-objects) 。

##### 2.4.1.3 内置对象·原生对象（Native Object）

JS中能够通过语言本身的构造器创建的对象称为原生对象。

![内置对象·原生对象分类](./image/内置对象·原生对象分类.png)

JS标准中提供了39个构造器。通过这些构造器，可以用 `new` 运算创建新的对象，所以把这些对象称为原生对象。

这些构造器几乎所有的能力都无法用纯JS代码来实现，也无法用 `class/extends` 语法来继承。因为这些构造器创建的对象多数使用了私有字段。例如:

- Error: `[[ErrorData]]`
- Boolean: `[[BooleanData]]`
- Number: `[[NumberData]]`
- Date: `[[DateValue]]`
- RegExp: `[[RegExpMatcher]]`
- Symbol: `[[SymbolData]]`
- Map: `[[MapData]]`

这些字段使得原型继承方法无法正常工作，所以，这些原生对象都是为了特定能力或性能，而设计出来的特权对象。

#### 2.4.2 用对象来模拟函数和构造器：函数对象和构造器对象

在JS中，还有一个看待对象的不同视角，就是用对象来模拟函数和构造器。
JS为这一类对象预留了私有字段机制，并规定了抽象的函数对象和构造器对象的概念。

- 函数对象：具有私有字段 `[[call]]` 的对象。
- 构造器函数：具有私有字段 `[[construct]]` 的对象。

JS 用对象模拟函数的设计代替了一般编程语言中的函数，它们可以像其他语言的函数一样被调用、传参。任何宿主只要提供了"具有私有字段 `[[call]]` 的对象"，就可以被 JS 函数调用语法支持。

> `[[call]]` 私有字段必须是一个引擎中定义的函数，需要接受 this 值和 调用参数，并且会产生域的切换。

任何对象只要实现了 `[[call]]`，它就是一个函数对象，可以作为函数去调用。如果它实现了 `[[construct]]`，它就是一个构造器对象，可以作为构造器被调用。

用 `function` 关键字创建的函数必定同时是函数和构造器。不过，它们表现出的效果并不相同。对于宿主和内置对象来说，它们实现[[call]](作为函数被调用) 和 [[construct]](作为构造函数被调用)不总是一致的。例如：内置函数 Date 在作为构造器被调用时产生新的对象，作为函数时，则产生字符串。

```js
console.log(typeof new Date()); // object
console.log(typeof Date()); //
```

而在宿主环境中，提供的 `Image` 构造器，则根本不允许作为函数被调用。

```js
console.log(new Image); // <img>
console.log(Image());  //抛出错误
```

基本函数 (String，Boolean，Number)，它们的构造器被当做函数调用时，则产生类型转换的效果。

> 在 ES6 之后 `=>` 语法创建的函数仅仅是函数，它们无法被当做构造器使用。

使用 `function` 语法或者 `Function` 构造器创建的对象来说，`[[call]]` 和 `[[construct]]` 行为总是类似的。

```js
function f(){
    return 1;
}
var v = f(); //把f作为函数调用
var o = new f(); //把f作为构造器调用
```

大致可以认为，它们 `[[construct]]` 的执行过程如下：

1. 以 `Object.prototype` 作为原形创建一个新对象
2. 以新对象为 this，执行函数的 `[[call]]`
3. 如果 `[[call]]` 的返回值是对象，那么返回这个对象，否则，返回第一步创建的新对象

这样的规则造成了个现象，如果构造器返回了一个新的对象，那么 `new` 创建的新对象就变成了一个构造函数之外完全无法访问的对象，这一定程度可以实现"私有"。

```js

function cls(){
  this.a = 100;
  return {
    getValue:() => this.a
  }
}
var o = new cls;
o.getValue(); //100
//a在外面永远无法访问到
```

#### 2.4.3 特殊行为的对象

在固有对象和原生对象中，有一些对象的行为跟正常行为的对象有很大的区别。

它们常见的下标运算（就是使用中括号或者点来做属性访问）或者设置原型跟普通对象不同

- Array：Array 的 length 属性根据最大的下标自动发生变化。
- Object.prototype：作为所有正常对象的默认原型，不能再给它设置原型了。
- String：为了支持下标运算，String 的正整数属性访问会去字符串里查找。
- Arguments：arguments 的非负整数型下标属性跟对应的变量联动。
- 模块的 namespace 对象：特殊的地方非常多，跟一般对象完全不一样，尽量只用于 import。
- 类型数组和数组缓冲区：跟内存块相关联，下标运算比较特殊。
- bind 后的 function：跟原来的函数相关联。

## 三. JS的执行

### 3.1 Promise、async/await

在 ES5 之后，JavaScript 引入了 Promise，这样，不需要浏览器的安排，JavaScript 引擎本身也可以发起任务了。

#### 3.1.1. 宏观和微观任务

使用 JSC引擎 的术语，把宿主发起的任务称为宏观任务，把JS引擎发起的任务称为微观任务。

JS引擎等待宿主环境分配宏观任务，在操作系统中，通常等待的行为都是一个事件循环，所以在 Node 术语中，也会把这个部分称为 **事件循环**。

事件的循环原理，在底层的C/C++代码中，这个事件循环是一个跑在独立事件中的循环，用伪代码来表示：

```js
while(TRUE) {
  r = wait();
  execute(r);
}
```

整个循环都是反复的 "等待 - 执行"，每次的执行过程，都是一个宏观任务。在宏观任务中，JS的 `Promise` 还会产生异步代码，JS必须保证这些异步任务在同一个宏观任务中完成，因此，每个宏观任务中又包含了一个微观任务队列。

![宏观任务与微观任务队列](./image/宏观任务与微观任务队列.jpg)

有了宏观任务和微观任务机制，就可以实现 JS 引擎级和宿主级的任务了，例如：Promise 永远在队列尾部添加微观任务。setTimeout 等 宿主API，则会添加宏观任务。

#### 3.1.2 Promise

Promise 是JS语言提供的一种标准化的异步管理方式，它的总体思想是，需要进行io、等待或者其他异步操作的函数，不返回真实结果，而是返回一个"承诺"，函数的调用方可以选择在合适的时机，选择等待这个承诺实现(通过Promise的 then 方法的回调)。

```js
// 等候传入参数指定的时长
function sleep(duration) {
  return new Promise(function(resolve, reject) {
    setTimeout(resolve,duration);
  })
}
sleep(1000).then( () => console.log("finished"));
```

Promise有三个状态：

1. pending[待定] 初始状态
2. fulfilled[实现] 操作成功
3. rejected[失败] 操作失败

当Promise状态发生改变，就会触发 `then()` 里的响应函数处理后续步骤，Promise状态一旦改变，不会再变。

```js
new Promise(function (resolve, reject) {
  resolve("成功");
}).then(
  (res) => {
    console.log(res);
  },
  (err) => {
    console.log(err);
  }
);
```

**resolve的作用**
: 将 Promise 对象的状态从"未完成"变为"成功"（即从pending变为fulfilled），在异步操作成功时调用，并将异步操作的结果，作为参数传递出去

**reject的作用**
: 将 Promise 对象的状态从"未完成"变为"失败"（即从pending变为rejected），在异步操作失败时调用，并将异步操作报出的错误，作为参数传递出去

Promise的then回调是一个异步的执行过程。

```js
var r = new Promise(function(resolve, reject){
    console.log("a");
    resolve()
});
r.then(() => console.log("c"));
console.log("b") // a b c
```

[Promise和async/await的使用](./HTML演示文件/Promise和async、await的使用.html)

**分析异步执行的顺序**：

1. 首先分析有多少个宏任务
2. 在每个宏任务中，分析有多少个微任务
3. 根据调用顺序确定宏任务中微任务的执行顺序
4. 根据宏任务的触发规则和调用次序，确定宏任务的执行顺序
5. 确定整个顺序

#### 3.1.3 async/await

`async/await` 是ES6新加入的特性，它提供了for、if等代码结构来编写异步的方式。它的运行基础是 Promise。
`async` 函数必定返回 `Promise`，所有返回 `Promise` 的函数都可以认为是异步函数。
`async` 函数是一种特殊语法，特征是在 `function` 关键字前加上 `async` 关键字，就定义了一个 async 函数，可以在其中使用 await 来等待一个 Promise。

```js
function sleep(duration) {
  return new Promise(function(resolve, reject) {
    setTimeout(resolve,duration);
  })
}

async function foo(){
  console.log("a")
  await sleep(2000)
  console.log("b")
}
```

async 函数强大之处在于，它是可以嵌套的。

```js
function sleep(duration) {
  return new Promise(function(resolve, reject) {
    setTimeout(resolve,duration);
  })
}
async function foo(name){
  await sleep(2000)
  console.log(name)
}
async function foo2(){
  await foo("a");
  await foo("b");
}
```

### 3.2 闭包

实际上 JS 中跟闭包对应的概念就是“函数”。

![函数执行过程](./image/函数执行过程.png)

闭包翻译自英文单词 closure，在计算机领域有三个完全不同的意义：

- 编译原理：它是处理语法产生式的一个步骤
- 计算几何：它表示包裹片面点集的凸多边形（翻译作凸包）
- 编程语言：它表示一种函数

闭包是一个绑定了执行环境的函数，闭包与普通函数的区别是，它携带了执行的环境。

**JS中对应的闭包组成部分**:

- 环境部分
  - 环境 : 函数的词法环境（执行上下文的一部分）
  - 标识符列表 : 函数中用到的未声明的变量
- 表达式部分 : 函数体

JS 中的函数完全符合闭包的定义，它的环境部分是函数词法环境部分组成，它的标识符列表是函数中用到的未声明变量，他的表达式部分就是函数体。

### 3.3 执行上下文：执行的基础设施

JS函数的复杂性主要来自于它携带的"环境部分"。
JS中与闭包"环境部分"相对应的术语是"词法环境"，但是JS中需要处理this、变量声明、with 等等一系列复杂的语法，所以，在JS的设计中，词法环境只是 JS 执行上下文 的一部分。

JS 标准把一段代码（包括函数），执行所需的所有信息定义为："执行上下文"

执行上下文 在ES2018中的定义：

- lexical environment：词法环境，当获取变量或者 this 值时使用。
- variable environment：变量环境，当声明变量时使用。
- code evaluation state：用于恢复代码执行位置。
- Function：执行的任务是函数时使用，表示正在被执行的函数。
- ScriptOrModule：执行的任务是脚本或模块时使用，表示正在被执行的代码。
- Realm：使用的基础库和内置对象实例。
- Generator：仅生成器上下文有这个属性，表示当前生成器

```js
var b = {}
let c = 1
this.a = 2;
```

想要正确的执行上面的代码，需要知道以下信息：

1. var 把 b 声明到哪里
2. b 表示哪个变量
3. b 的原型是哪个对象
4. let 把 c 声明到哪里
5. this 指向哪个对象

这些信息需要执行上下文来给出，这段代码出现在不同的位置，关联到不同的上下文，同样的代码会产生不一样的行为。

### 3.4 var的声明与赋值

var 声明作用域函数执行的作用域，也就是，var 会穿透 for、if 等语句。

**立即执行的函数表达式(IIFE)**
在只有 var，没有 let 的旧 JS 时代，诞生了一个技巧，叫做：立即执行的函数表达式（IIFE），通过创建一个函数，并且立即执行，来构造一个新的域，从而控制 var 的作用范围。

由于语法规定了 `function` 开头的是函数声明，所以想要让函数变成函数表达式，必须加点东西，推荐使用 `void` 关键字。

```js
void function(){
  var a;
  //code
}();
```

这有效的避免了语法问题，同时语义上 `void` 运算表示忽略后面表达式的值，变成undefined，IIFE不关心函数的返回值，所以语义也比较合理。

void是运算符，其后跟一个表达式，无论 void 后的表达式是什么都会执行，void 操作符都会返回 undefined。

void在JS中一般有3种作用：

1. 返回 undefined
  undefined 在JS中不是保留字，可以定义undefined这个变量，使用全局的undefined可能会被局部变量覆盖，所以使用 void 0来代替undefined。
2. 执行无用操作
  如果有 a 链接，不希望点击的时候跳转，不写又会刷新，通常使用：`<a href="javascript:void(0)">` 来执行空操作
3. void 执行后面的表达式，例如：var a = 1; void a++; // a = 2;

### 3.5 let

let是 ES6 开始引入的新的变量声明模式，比起 var 的诸多弊病，let 做了非常明确地梳理和规定。
为了实现let，JS 在运行时引入了块级作用域。

以下语句会使 let 使用产生作用域：

- for
- if
- switch
- try/catch/finally

### 3.6 Realm

在最新的标准（9.0）中，JavaScript 引入了一个新概念 Realm。
在 ES2016 之前的版本中，标准中甚少提及{}的原型问题。但在实际的前端开发中，通过 iframe 等方式创建多 window 环境并非罕见的操作，所以，这才促成了新概念 Realm 的引入。
Realm 中包含一组完整的内置对象，而且是复制关系。
对不同 Realm 中的对象操作，会有一些需要格外注意的问题，比如 `instanceOf` 几乎是失效的。

```js
// 展示了在浏览器环境中获取来自两个 Realm 的对象，它们跟本土的 Object 做 instanceOf 时会产生差异
var iframe = document.createElement('iframe')
document.documentElement.appendChild(iframe)
iframe.src="javascript:var b = {};"

var b1 = iframe.contentWindow.b;
var b2 = {};

// 由于 b1、 b2 由同样的代码“ {} ”在不同的 Realm 中执行，所以表现出了不同的行为。
console.log(typeof b1, typeof b2); //object object
console.log(b1 instanceof Object, b2 instanceof Object); //false true
```

### 3.7 函数的种类

1. 普通函数：用 `function` 关键字定义的函数

    ```js
    function foo(){
      // code
    }
    ```

2. 箭头函数：用 `=>` 运算符定义的函数

    ```js
    const foo = () => {
      // code
    }
    ```

3. 方法：在 `class` 中定义的函数

    ```js
    class C {
      foo(){
        //code
      }
    }
    ```

4. 生成器函数：使用 `function*` 定义的函数

    ```js
    function* foo(){
      // code
    }
    ```

5. 类：用 `class` 定义的类，也是函数

    ```js
    class Foo {
      constructor(){
        //code
      }
    }
    ```

6. 异步函数：普通函数、箭头函数和生成器函数前加上 `async` 关键字

    ```js
    async function foo(){
      // code
    }
    const foo = async () => {
      // code
    }
    async function foo*(){
      // code
    }
    ```

### 3.8 this 关键字

#### 3.8.1 行为

this 是执行上下文中很重要的一个组成部分。同一个函数调用方式不同，得到的 `this` 值也不同。

普通函数的this值由"调用它所使用的引用"决定，原因在于：获取函数的表达式时，它实际上返回的不是函数本身，而是一个 `Reference` 类型。

Reference类型由两部分组成：一个对象和一个属性值

当做一些算术运算（或其他运算时），Reference类型会被解引用，即获取真正的值（被引用的内容）来参与运算，而类似函数调用、delete等操作，都需要用到Reference类型中的对象。

**行为**:

1. 调用函数时使用的引用，决定了函数执行时刻的 this 值。
2. 而箭头函数，不论什么引用来调用它，都不影响它的this值，它会继承外层函数调用的 this 绑定(无论 this 绑定到什么)
3. 生成器函数、异步生成器函数 和 异步普通函数跟普通函数 行为是一致的，异步箭头函数与箭头函数 行为是一致的。

#### 3.8.2 机制

函数能够引用定义时的变量，函数也能记忆定义时的this，因此，函数内部必定有一个机制来保存这些信息。

在 JS 标准中，为函数规定了用来保存定义时上下文的私有属性 `[[Environment]]` 。

当一个函数执行时，会创建一条新的执行环境记录，记录外层词法环境（outer lexical environment）会被设置成函数的 `[[Environment]]`，这就是 **切换上下文**。

JS 用一个栈来管理执行上下文，这个栈中的每一项又包含一个链表。当函数调用时，会入栈一个新的执行上下文，调用结束后，执行上下文被出栈。

![管理执行上下文的栈](./image/管理执行上下文的栈.jpg)

而 this 是一个更为复杂的机制，JS标准定义了 `[[thisMode]]` 私有属性，`[[thisMode]]` 私有属性有三个取值

- lexical：表示从上下文中找this，这对应了箭头函数
- global： 表示当this为undefined时，取全局对象，这对应了普通函数
- strict： 当严格模式时使用，this严格按照调用时传入的值，可能为 null 或 undefined

> 方法的行为跟普通函数有差异，就是因为 class 设计成了默认按 `strict` 模式执行

函数创建新的执行上下文中的词法环境记录时，会根据 `[[thisMode]]` 来记录新纪录的 `[[ThisBindingStatus]]` 私有属性
代码执行遇到 this 时，会逐层检查当前词法环境记录中的 `[[ThisBindingStatus]]`，当找到有 this 的执行环境记录时获取 this 的值

这样的规则的实际效果是，嵌套的箭头函数中的代码都指向外层 this

```js
var o = {}
o.foo = function foo(){
  console.log(this);
  return () => {
    console.log(this);
    return () => console.log(this);
  }
}

o.foo()()(); // o, o, o
```

#### 3.8.3 操作this的内置函数

`Function.prototype.call` 和 `Function.prototype.apply` 可以指定函数调用时传入的 this 值。

```js

function foo(a, b, c){
  console.log(this);
  console.log(a, b, c);
}
// call 和 apply 作用是一样的，只是传参方式有区别
foo.call({}, 1, 2, 3);
foo.apply({}, [1, 2, 3]);
```

`Function.prototype.bind` 可以生成一个绑定过的新函数，这个新函数的 this 值被指定为 `bind()` 的第一个参数

```js
function foo(a, b, c){
    console.log(this);
    console.log(a, b, c);
}
foo.bind({}, 1, 2, 3)();
```

> call、apply、bind 用于不接受 this 的函数类型，如：箭头函数、class 都不会报错，这时，它们无法实现改变 this 的能力，但可以实现传参。

### 3.9 语句

语句是任何编程语言的基础结构，与JS对象一样 JS语句 有"看起来很像其他语言，但其实一点都不一样"的特点。

JS语句存在嵌套关系，所以执行过程主要在树形结构上进行，树形结构的每一个节点执行后产生 Completion Record 类型，根据语句结构和Completion Record，JS实现了各种分支和跳出逻辑。

#### 3.9.1 Completion 类型

JS语句执行的完成状态，可以用一个标准类型来表示：Completion Record 类型(用于描述异常、跳出等语句执行过程)

Completion Record 表示一个语句执行完之后的结果，它有三个字段:

- `[[type]]` : 表示完成的类型，有 break continue return throw 和 normal 几种类型
- `[[value]]` : 表示语句的返回值，如果语句没有，则是 empty
- `[[target]]` : 表示语句的目标，通常是一个JS标签

JS 正是依靠语句的 Completion Record 类型，方才可以在语句的复杂嵌套结构中，实现各种控制。

```js
function foo() {
  try {
    return 0;
  } catch (err) {} finally {
    console.log("a");
  }
}
// return 执行完毕后，但函数并没有立即返回，又执行了finally
// 因为finally中的语句必须执行，所以，try\catch执行完毕，即使得到的结果是非normal型的完成记录，也必须执行finally
console.log(foo()); // a 0
```

```js
function foo() {
  try {
    return 0;
  } catch (err) {} finally {
    return 1;
  }
}
// finally中的return“覆盖”了try中的return
// 当finally执行也得到非normal记录，则会使finally中的记录作为整个try结构的结果
console.log(foo()); // 1
```

![语句的分类](./image/语句的分类.jpg)

**普通语句**
在JS中，不带控制能力的语句称为 普通语句。有下面几种：

- 声明类语句
  - var声明
  - const声明
  - let声明
  - 函数声明
  - 类声明
- 表达式语句
- 空语句
- debugger语句

这些语句在执行时，从前到后顺序执行（先忽略var和函数声明的预处理机制），没有任何分支或重复执行逻辑。

普通语句执行后，会得到 `[[type]]` 为 normal 的 Completion Record，JS引擎遇到这样的Completion Record，会继续执行下一条语句。

这些语句中只有表达式语句会产生 `[[value]]` 。

> Chrome 控制台输入语句下方显示的正是语句的 Completion Record 的 `[[value]]`。

**语句块**
语句块就是一组用大括号括起来的语句，它是一种语句的复合结构，可以嵌套。
语句块内部语句的Completion Record的 `[[type]]` 如果不为 normal，会打断语句块后续的语句执行。
在语句块中插入一条return语句，产生了一个非normal记录，那么整个语句块会成为非normal。这个结构就保证了非normal的完成类型可以穿透复杂的语句嵌套结构，产生控制效果。

**控制型语句**
控制型语句带 if、switch 关键字，它们会对不同类型的Completion Record产生反应。
控制语句分为两部分：

1. 对其内部造成影响，如：if、switch、while/for、try
2. 对外部造成影响，如：return、break、continue、throw

这两类的配合，会产生控制代码执行顺序和执行逻辑的效果。

![控制语句和控制类型组合产生的效果](./image/控制语句和控制类型组合产生的效果.png)

**带标签的语句**
任何JS语句都是可以加标签的，在语句前加冒号即可：

```js
firstStatement: var a = 1;
```

大部分时候，这个东西相当于注释，没有任何用处。唯一有作用的时候是：与完成记录类型中的target相配合，用于跳出多层循环。

```js
// 与完成记录类型中的target配合，用于跳出多重循环
outer: while (true) {
  inner: while (true) {
    // break/continue 语句如果后面跟了关键字，会产生带 target 的完成记录。一旦完成记录带了 target，那么只有拥有对应 label 的循环语句会消费它。
    break outer;
  }
}
console.log("finished");
```

## 四. 文法

文法是编译原理中对语言的写法的一种规定，一般来说，文法分为 **词法** 和 **语法** 两种。
词法规定了语言的最小语义单位：token，可以翻译为"标记"或"词"。
从字符到词是没有结构的，只要符合词的规则，就构成词，一般来说，词法设计不会包含冲突。词法分析技术上可以使用状态机或正则表达式来进行。

### 4.1. 词法

JS源代码中的输入分类：

- WhiteSpace     空白字符
- LineTerminator 换行符
- Comment        注释
- Token          词
  - IdentifierName  标识符名称，例如：变量名、关键字
  - Punctuator      符号，使用的运算符和大括号等符号
  - NumericLiteral  数字直接量，就是写的数字
  - StringLiteral   字符串直接量，就是用单引号或双引号引起来的直接量
  - Template        字符串模板，用反引号 ` 括起来的直接量

这个设计比较符合通用的编程语言设计方式，但JS有一些特殊的地方：

1. 除法与正则表达式冲突问题。JS不但支持除法运算符"/"和"/="，还支持用斜杠括起来的正则表达式"/abc/"。
  这时候，对于词法分析来说，其实是没有办法处理的，所以，JS的处理方案是定义两组词法，然后靠词法分析传一个标志给词法分析器，让它来决定使用哪一套词法。

2. 字符串模板

    ```js
    `hello，${name}`
    ```

    理论上，`${}` 内部可以放任何JS表达式代码，而这些代码是以 `}` 结尾的，也就是说，这部分词法不允许出现 `}` 运算符。
    是否允许 `}` 的两种情况，与除法和正则表达式的两种情况相乘就是四种词法定义

      - InputElementDiv;
      - InputElementRegExp;
      - InputElementRegExpOrTemplateTail;
      - InputElementTemplateTail

    为了解决这两个问题，标准中不得不把除法、正则表达式直接量 和 `}` 从token中单独抽出来，用词上，也从Token改为CommonToken。
    对于一般语言的词法分析过程来说，都会丢弃除了Token之外的输入，但是对于JS来说，不太一样，换行符和注释还会影响词法分析过程，所以要实现JS的解释器，词法分析和语法分析非常麻烦，需要来回传递信息。

#### 4.1.1 空白符号 WhiteSpace

JS可以支持 18 种空白符号，但在ASCII编码内，只有五种可用：

- `<HT>`（或称`<TAB>`）是U+0009，是缩进TAB符，也就是字符串中写的 `\t`
- `<VT>` 是U+000B，也就是垂直方向的TAB符 `\v`，这个字符很少用
- `<FF>` 是U+000C，Form Feed分页符，字符串直接量中写作 `\f`，现在很少有打印源程序的事情发生了，所以这个字符在JS源代码中很少用到
- `<SP>` 是U+0020，就是普通的空格
- `<NBSP>` 是U+00A0，非断行空格，它是SP的一个变体，在文字排版中，可以避免因为空格，在此处发生断行，其他方面与空格完全一样。HTML中，&nbsp; 生成的就是它
- `<ZWNBSP>`（旧称`<BOM>`）是U+FEFF，这是ES5新加入的空白符，是Unicode中的零宽非断行空格，在以UTF编码格式的文件中，常常在文件首插入一个额外的U+FEFF，解析UTF文件的程序可以根据U+FEFF的表示方式猜测文件采用哪种UTF编码方式。这个字符也叫做"bit order mark"

![JS支持的所有的Unicode的空格分类](./image/JS支持的所有的Unicode的空格分类.png)

#### 4.1.2 换行符 LineTerminator

JS中提供了4种换行符：

- `<LF>` 是U+000A，就是正常的换行符，是字符串中的 `\n`
- `<CR>` 是U+000D，就是"回车"，在字符串中是 `\r`，在一部分Windows风格的编辑器中，换行是两个字符`\r\n`
- `<LS>` 是U+2028，是Unicode中的行分隔符
- `<PS>` 是U+2029，是Unicode中的段落分隔符

> 大部分的换行符在被词法分析器扫描出之后，会被语法分析器丢弃，但是换行符会影响JS的两个重要语法特征：**自动插入分号** 和 **"no line terminator"规则**

#### 4.1.3 注释 Comment

JS的注释分为单行注释和多行注释：

```js
/* MultiLineCommentChars */
// SingleLineCommentChars
```

多行注释中允许出现除了 `*` 之外的所有字符，而每一个 `*` 之后，不能出现正斜杠符 `/`
除了四种LineTerminator之外，任何字符都可以作为单行注释

> 注意：多行注释是否包含换行符，会对 JS 语法产生影响，对于"no line terminator"规则来说，带换行符的多行注释和换行符是等效的

#### 4.1.4 标识符名称 IdentifierName

IdentifierName可以以美元符"$"、下划线"_"、或者Unicode字母开始，除了开始字符以外，IdentifierName中还可以使用Unicode连接标记，字符以及连接符号。

IdentifierName的任意字符可以使用JS的Unicode转义写法，在使用Unicode的转义写法时，没有任何字符限制。

IdentifierName可以是Identifier、NullLiteral、BooleanLiteral或者keyword，在ObjectLiteral中，IdentifierName还可以被直接当做属性名称使用。

仅当不是保留字的时候，IdentifierName会被解析为Identifier

> 注意 `<ZWNJ>`和 `<ZWJ>` 是ES5新加的两个格式控制字符，它们都是0宽

在JS中，有33个关键字：

```txt
await break try catch class const continue debugger default delete else export extends finally for function if import instanceof new return super switch case this throw typeof var void do while with yield
```

除了上面的内容外，还有一个为未来使用而保留的关键字：

```js
enum
```

在严格模式下，有一些额外的为未来使用而保留的关键字：

```js
implements package protected interface private public
```

> 除了这些，NullLiteral（null）和BooleanLiteral（true false）也是保留字，不能用于Identifier

#### 4.1.5 符号 Punctuator

因为除法和正则问题，`/` 和 `/=` 两个运算符被拆分为DivPunctuator，因为字符串模板问题，`}` 也被独立拆分，所有符号为：

```js
{ ( ) [ ] . ... ; , < > <= >= == != === !== + - * % ** ++ -- << >> >>> & | ^ ! ~ && || ? : = += -= *= %= **= <<= >>= >>>= &= |= ^= => / /= }
```

#### 4.1.6 数字直接量 NumericLiteral

JS规范中规定的数字直接量可以支持四种写法：十进制数、二进制整数、八进制整数、十六进制整数

十进制的Number可以带小数，小数点前后都可以忽略，但不能同时忽略

```js
.01  12.  2.1
```

数字直接量还支持科学计数法

```js
10.24E+2  10.24e-2  10.24e2
```

```js
// 0x开头为十六进制
oxFB
// 0o开头为八进制
0o79
// 0b开头为二进制
0b1000
// 上面这几种进制都不支持小数，也不支持科学计数法。
```

#### 4.1.7 字符串直接量 StringLiteral

JS中的 StringLiteral 支持单引号和双引号两种写法。

单双引号的区别仅仅在于写法，在双引号字符串直接量中，双引号必须转义，在单引号字符串直接量中，单引号必须转义。字符串中其他必须转义的字符是 `\` 和 所有换行符。

JS中支持四种转义形式，还有一种虽然标准没有定义，但是大部分实现都支持的八进制转义。

1. 单字符转义，即一个反斜杠\后面跟一个字符这种形式。

有特别意义的字符包括有SingleEscapeCharacter所定义的 9 种，见下表

![有特别意义的转义字符](./image/有特别意义的转义字符.png)

> 除了这 9 种字符、数字、x 和 u 以及所有的换行符之外，其它字符经过 `\` 转义后都是自身

#### 4.1.8 正则表达式直接量 RegularExpressionLiteral

正则表达式由Body和Flags两部分组成，例如：

```js
/RegularExpressionBody/ig
```

其中Body部分至少有一个字符，第一个字符不能是 `*`（因为 `/*` 跟多行注释有词法冲突）。

正则表达式有自己的语法规则，在词法阶段，仅会对它做简单解析。

正则表达式并非机械的见到/就停止，在正则表达式 `[ ]` 中的 `/` 就会被认为是普通字符，例如：

```js
/[/]/.test("/"); // true
```

除了 `\`、`/` 和 `[` 三个字符之外，JS表达式中的字符都是普通字符。

用 `\` 和 一个非换行符 可以组成一个转义，`[ ]` 中也支持转义。正则表达式中的 **flag** 在词法阶段不会限制字符。

虽然只有 **ig** 几个是有效的，但是任何IdentifierPart（Identifier中合法的字符）序列在词法阶段都会被认为是合法的。

#### 4.1.10 字符串模板 Template

在词法结构上，Template是个整体，其中的 `${}` 是并列关系。
实际上，在JS词法中，包含${}的Template，是被拆开分析的。例如：

```js
`a${b}c${d}e`
```

在JS中被认为是

```js
`a${
b
}c${
d
}e`
```

它被拆成了五个部分：

- **`a${** : 这个被称为模板头
- **}c${** : 被称为模板中段
- **}e`**  : 被称为模板尾
- **b、d** : 普通标识符

实际上，这里的词法分析过程已经与语法分析深度耦合了。

模板支持添加处理函数的写法，这时模板的各段会被拆开，传递给函数当参数

```js
function f(){
  console.log(arguments);
}

var a = "world"
f`Hello ${a}!`; // [["Hello", "!"], world]
```

> 模板字符串不需要关心大多数字符的转义，但是 **${** 和 **`** 还是需要处理的。
> 模板中的转义跟字符串几乎完全一样，都是使用 \。

### 4.2 语法

#### 4.2.1 自动插入分号

> 行尾使用分号的风格来自于 Java，也来自于 C 语言和 C++，这一设计最初是为了降低编译器的工作负担。
> 但是，从今天的角度来看，行尾使用分号其实是一种语法噪音，恰好 JS 语言又提供了相对可用的分号自动补全规则，所以，很多 JS 的程序员都是倾向于不写分号。

自动插入分号规则独立于所有语法产生式定义，规则：

- 有换行符，且下一个符号是不符合语法的，那么就尝试插入分号
- 有换行符，且语法中规定此处不能有换行符，那么就自动插入分号
- 源代码结束处，不能形成完整的脚本或模块结构，那么就自动插入分号

![语法](./HTML演示文件/语法.html)

#### 4.2.2 no LineTerminator here 规则

no LineTerminator here 规则表示它所在的结构中的这一位置不能插入换行符。

自动插入分号规则的第二条：有换行符，且语法中规定此处不能有换行符，那么就自动插入分号。跟no LineTerminator here 规则强相关。

JS语法中定义了以下 no LIneTerminator here 规则：

- 带标签的 continue 语句，不能在 continue 后插入换行
- 带标签的 break 语句，不能再break后插入换行
- return 后不能插入换行
- 后自增、后自减前不能插入换行
- throw 和 Exception 之间不能插入换行
- 凡是 async 关键字后面，都不能插入换行
- 箭头函数的箭头前，都不能插入换行
- yield之后，不能插入换行

![语法](./HTML演示文件/语法.html)

> no LineTerminator here 规则的存在，多数情况下是为了保证自动插入分号行为是符合预期的，但是在JS设计的最初，遗漏了一些重要的情况，所以有一些不符合预期的情况出现，需要格外注意

**不写分号需要注意的情况**:

- 以括号开头的语句

  ```js
  (function(a){
      console.log(a);
  })()/*这里没有被自动插入分号*/
  (function(a){ // 看似是两个独立执行的函数表达式，但是第三组括号被理解为传参，导致抛出错误
      console.log(a);
  })()
  ```

- 以数组开头的语句

  ```js
  var a = [[]] /*这里没有被自动插入分号*/
  // 这段代码本意是一个变量 a 赋值，然后对一个数组执行 forEach，但是因为没有自动插入分号，被理解为下标运算符和逗号表达式
  [3, 2, 1, 0].forEach(e => console.log(e)) // 这里不会抛出错误，代码排查非常困难
  ```

- 以正则表达式开头的语句

  ```js
  var x = 1, g = {test:()=>0}, b = 1 /*这里没有被自动插入分号*/
  /(a)/g.test("abc") // 本意是声明三个变量，然后测试一个字符串中是否含有字母 a，但是因为没有自动插入分号，正则的第一个斜杠被理解成了除号，后面的意思就都变了
  console.log(RegExp.$1) // 这里不会抛出错误，代码排查非常困难
  ```

- 以 Template 开头的语句

  ```js
  var f = function(){
    return "";
  }
  // 这段代码本意是声明函数 f，然后赋值给 g，再测试 Template 中是否含有字母 a。但是因为没有自动插入分号，函数 f 被认为跟 Template 一体的，进而被莫名其妙地执行了一次。
  var g = f/*这里没有被自动插入分号*/
  `Template`.match(/(a)/);
  console.log(RegExp.$1)
  ```

#### 4.2.3 语法

JS有两种源文件：一. 脚本 二. 模块。这个区分是在ES6引入了模块机制开始的，ES6以前只有脚本。

脚本可以由浏览器或node引入执行的，而模块只能由JS代码用 `import` 引入执行

从概念上，可以认为脚本具有主动性的JS代码，是控制宿主完成一定任务的代码；而模块是被动性的代码，是等待被调用的库。

> 实际上模块和脚本之间的区别仅仅在于是否包含 `import` 和 `export`。

浏览器支持用 `<script>` 引入模块，但必须给 `<script>` 标签添加 `type="module"`。如果引入脚本，则不需要 type。

```js
<script type="module" src="xxxxx.js"></script>
```

> `<script>` 标签如果不加 `type=“module”` ，默认加载的文件是脚本而非模块，如果在脚本中写了 `export`，会抛错。

脚本中可以包含语句，模块中可以包含3种内容：

- import声明
- export声明
- 语句

##### 4.2.3.1 import声明

import 声明有两种用法

1. 直接import一个模块

    ```js
    import "mod"; //引入一个模块
    ```

    这样只能保证这个代码模块被执行，引用它的模块是无法获得它的任何信息的。

2. 带from的import
  带from的import的意思是引入模块中的一部分信息，可以把它们变成本地的变量。
  带from的import又有三种细分：

    ```js
    // 1. 引入模块中导出的默认值
    import x from "./a.js";
    // 2. 引入模块中的变量
    import {a as x, modify} from "./a.js";
    // 3. 把模块中所有的变量以类似对象属性的方式引入
    import * as x from "./a.js";

    // 第一种方式还可以跟后面两种组合使用
    // 语法要求不带 `as` 的默认值永远在最前。
    // 注意这里的变量实际上仍然可以受到原来模块的控制
    import d,{a as x, modify} from "./a.js";
    import d,* as x from "./a.js";
    ```

##### 4.2.3.2 export声明

export承担的是导出的任务

导出变量的方式有两种：

1. 独立使用export声明

    ```js
    export {a,b,c};
    ```

2. 直接在声明型语句前加 `export` 关键字，这里的 `export` 可以加在任何声明性质的语句前，整理如下：

    - var
    - function(含async和generator)
    - class
    - let
    - const

    export 还有一种特殊的用法，就是跟 default 联合使用。`export default` 表示导出一个默认变量值，它可以用于 `function` 和 `class`。这里导出的变量是没有名称的，可以使用 `import x from "./a.js"` 这样的语法，从模块中引入。
    export default 还支持一种语法，后面跟一个表达式，例如：

      ```js
      var a = {};
      export default a; // 这里导出的是值，以后a的变化与导出的值无关
      ```

> import 语句前无法加入 export，但是可以直接使用 `export from` 语法

  ```js
  export x from "a.js";
  ```

##### 4.2.3.3 函数体

执行函数的行为通常是在 JS代码 执行时，注册宿主环境的某些事件触发的，而执行过程，就是执行函数体（函数的花括号中间的部分）。

宏任务可能执行的代码包括 "脚本(script)" 、"模块(module)" 和 "函数体(function body)"。

函数体其实也是一个语句的列表。跟脚本和模块相比，函数体的语句列表中多了 return 语句可用。

函数体实际上有以下四种：

- 普通函数体

  ```js
  function foo(){
      //Function body
  }
  ```

- 异步函数体

  ```js
  async function foo(){
      //Function body
  }
  ```

- 生成器函数体

  ```js
  function *foo(){
      //Function body
  }
  ```

- 异步生成器函数体

  ```js
  async function *foo(){
      //Function body
  }
  ```

> 这四种函数体的区别在于：能否使用 `await` 或 `yield` 语句

![模块、脚本和函数体能使用的语句](./image/模块、脚本和函数体能使用的语句.jpg)

##### 4.2.3.4 预处理

JS执行前会对，脚本、模块和函数体中的语句进行预处理，预处理的过程将会提前处理 **var、函数声明、class、const、let** 这些语句，以确定其中变量的含义。

###### 4.2.3.4.1 var声明

var声明永远作用于脚本、模块、函数体这个级别，在预处理阶段，不关心赋值的部分，只管在当前作用域声明这个变量。
var的作用域能够穿透一切语句结构，它只认脚本、模块和函数体这三种语法结构。

###### 4.2.3.4.2 function声明

function声明的行为原本跟 var 非常相似，但在最新的JS标准中，对它进行了一定的修改。

在全局（模块、脚本和函数体），function声明表现跟 var 相似，不同之处在于，function声明不仅在作用域中加入变量，还会给它赋值。

function声明出现在 if 等语句中的情况有点复杂，它仍然作用于脚本、模块和函数体级别的，在预处理阶段，仍然会产生变量，但它不再被提前赋值

```js
// function 在预处理阶段仍然发生了作用，在作用域中产生了变量，没有产生赋值，赋值行为发生在了执行阶段
console.log(foo); // undefined
if(true) {
    function foo(){

    }
}
```

出现在 if 等语句的function，在if创建的作用域中仍然会被提前赋值。

###### 4.2.3.4.3 class声明

class声明在全局的行为跟 function 和 var 都不一样。

在class声明前使用class名会抛错

```js
console.log(c); //  c is not define
class c{

}
```

试图在 class 前打印变量 c，得到了个错误，这个行为很像是 class 没有预处理，但是实际上并非如此。

```js
var c = 1;
function foo(){
    console.log(c);
    class c {}
}
foo();
```

执行后，我们看到，仍然抛出了错误，如果去掉 class 声明，则会正常打印出 1，也就是说，出现在后面的 class 声明影响了前面语句的结果。
说明了，class声明也是会被预处理的，它会在作用域中创建变量，并且要求访问它时抛出错误。

> class声明的作用不会穿透if等语句结构，所以只有写在全局环境才会有声明作用。
> 这样的 class设计 比 function 和 var 更符合直觉，而且遇到一些比较奇怪的用法时，倾向于抛出错误。
> 按照现代语言设计的评价标准，及早抛错是好事，它能帮助在开发阶段就发现代码的可能问题。

##### 4.2.3.5 指令序言机制

脚本和模块都支持一种特别的语法，叫做指令序言（Directive Prologs）。

这里的指令序言最早是为 **use strict** 设计的，它规定了一种给JS代码添加元信息的方式。

"use strict" 是JS标准中规定的唯一一种指令序言，但是指令序言的目的是，留给JS的引擎和实现者一些统一的表达方式，在静态扫描时指定JS代码的一些特性。

```js
// 假设要设计一种声明本文件不需要进行 lint 检查的指令，可以这样设计
"no lint";
"use strict";
function doSth(){
    //......
}
//......
```

JS的指令序言是只有一个字符串直接量的表达式语句，它只能出现在脚本、模块和函数体的最前面。

#### 4.2.4 语句

JS遵循了一般编程语言的 "语句-表达式" 结构。
在JS标准中，把语句分成了两种：**声明** 和 **语句**，这两种语句最大的区别就是声明型语句响应预处理过程，普通语句只有执行过程。

**普通语句**
![JS普通语句的种类](./image/JS普通语句的种类.png)

**声明型语句**
![JS声明型语句的种类](./image/JS声明型语句的种类.jpg)

##### 4.2.4.1 语句块

```js
{
  var x,y;
  x = 10;
  y = 20;
}
```

语句块的意义和好处在于：可以把多行语句视为同一行语句，这样if、for等语句定义起来就比较简单。

> 需要注意：语句块会产生作用域

##### 4.2.4.2 空语句

空语句就是一个独立的分号，实际上没什么大用。

```js
;
```

> 空语句的存在仅仅是从语言设计完备性的角度考虑，容许插入多个分号而不抛出错误。

##### 4.2.4.3 if语句

if语句是条件语句。

```js
if(a < b) {
  console.log(a);
}
```

> **作用** : 在满足条件时执行它的语句内容，这个语句可以是一个语句块，这样就可以实现有条件地执行多个语句。

if语句还有else结构，用于不满足条件时执行，常见的用法是：利用语句的嵌套能力，把if和else连写成多分支条件判断。

##### 4.2.4.4 switch语句

switch 语句继承自 Java，Java 中的 switch 语句继承自 C 和 C++，原本 switch 语句是跳转的变形，所以我们如果要用它来实现分支，必须要加上 break。

```js
switch(num) {
  case 1:
    print 1;
    break;
  case 2:
    print 2;
    break;
  case 3:
    print 3;
    break;
}
```

在 C 时代，switch 生成的汇编代码性能是略优于 if else 的，但是对 JS 来说，则无本质区别。

##### 4.2.4.5 循环语句

###### 4.2.4.5.1 while循环 和 do while循环

```js
let a = 100
while(a--) {
  console.log("*");
}
```

```js
let a = 101;
do {
    console.log(a);
} while(a < 100)
```

> while循环与do while循环的区别在于do while循环至少执行一次。

###### 4.2.4.5.2 普通for循环

```js
for(i = 0; i < 100; i++)
    console.log(i);

for(var i = 0; i < 100; i++)
    console.log(i);

for(let i = 0; i < 100; i++)
    console.log(i);
```

###### 4.2.4.5.3 for in 循环

for in 循环枚举对象的属性，这里体现了属性的 enumerable 特征。

```js
let o = { a: 10, b: 20}
Object.defineProperty(o, "c", {enumerable:false, value:30})

for(let p in o)
    console.log(p);
```

###### 4.2.4.5.4 for of 循环和 for await of 循环

for of 循环是非常棒的语法特性，它背后机制是 **iterator 机制**
可以给任何一个对象添加 iterator，使它可以用于 for of 语句

  ```js
  let o = {
      [Symbol.iterator]:() => ({
          _value: 0,
          next(){
              if(this._value == 10)
                  return {
                      done: true
                  }
              else return {
                  value: this._value++,
                  done: false
              };
          }
      })
  }
  for(let e of o)
      console.log(e);
  ```

这段代码展示了如何为一个对象添加 iterator。但是，在实际操作中，一般不需要这样定义 iterator，可以使用 generator function。

  ```js
  function* foo(){
    yield 0;
    yield 1;
    yield 2;
    yield 3;
  }
  for(let e of foo())
    console.log(e);
  ```

此外，JavaScript 还为异步生成器函数配备了异步的 for of

```js
function sleep(duration) {
  return new Promise(function(resolve, reject) {
    setTimeout(resolve,duration);
  })
}
// 定义了一个异步生成器函数，异步生成器函数每隔一秒生成一个数字，这是一个无限的生成器。
async function* foo(){
  i = 0;
  while(true) {
    await sleep(1000);
    yield i++;
  }
}
// 使用 for await of 来访问这个异步生成器函数的结果，可以看到，这形成了一个每隔一秒打印一个数字的无限循环。
for await(let e of foo())
  console.log(e);
```

##### 4.2.4.6 return

return语句用于函数中，它终止函数的运行，并且返回函数的指定值

##### 4.2.4.7 break 和 continue

break用于 跳出循环语句 或 switch语句，continue 语句用于结束本次循环并继续循环。

这两个语句都是控制型语句。都有带标签的用法

```js
outer:for(let i = 0; i < 100; i++)
  inner:for(let j = 0; j < 100; j++)
    if( i == 50 && j == 50)
      break outer;
outer:for(let i = 0; i < 100; i++)
  inner:for(let j = 0; j < 100; j++)
    if( i >= 50 && j == 50)
      continue outer;
```

> 带标签的break和continue可以控制自己被外层的哪个语句结构消费，这可以跳出复杂的语句结构。

##### 4.2.4.8 try 语句和 throw语句

try语句和throw语句用于处理异常，它们是配合使用的。在大型的应用中，异常机制非常重要。

```js
try {
    throw new Error("error");
} catch(e) {
    console.log(e);
} finally {
    console.log("finally");
}

```

一般来说，throw用于抛出异常，但是单纯从语言的角度，它可以抛出任何值，不一定是异常逻辑，但是为了保证语义清晰，不建议用throw表达任何非异常逻辑。

try语句用于捕获异常，用 throw 抛出的异常，可以在try语句的结构中被处理掉：try部分用于标识捕获异常的代码段，catch部分用于捕获异常后做一些处理，而finally则是用于执行后做一些必须执行的清理工作。

catch 结构会创建一个局部的作用域，并且把抛出的错误当做参数写入其中。

在 catch 中重新抛出错误的情况非常常见，在设计比较底层的函数时，常常会这样做，保证抛出的错误能被理解。

finally语句一般用于释放资源，它一定会被执行，即使再try中出现return，finally中的语句也一定要被执行。

##### 4.2.4.9 debugger语句

debugger语句的作用：通知调试器在此断点。在没有调试器挂载时，它不产生任何效果。

##### 4.2.4.10 var

var声明语句是古典的JS中声明变量的方式。而现在，在绝大多数情况下，let 和 const 都是更好的选择。

把它当做一种“保障变量是局部”的逻辑，遵循以下三条规则：

- 声明同时必定初始化
- 尽可能在离使用的位置近处声明
- 不要在意重复声明

##### 4.2.4.11 let和const

let和const都是变量的声明，它们的特性都非常相似。let和const的作用范围是if、for等结构型语句。

let和const语句在重复声明时会抛错，这能够有效地避免变量名无意中冲突。

let和const声明虽然看上去是执行到了才生效，但是实际上，它们还是会被预处理。如果当前作用域内有声明，就无法访问到外部的变量。

```js
const a = 1;
if(true){
  // 在 if 的作用域中，变量 a 声明执行到之前，访问了变量 a，这时会抛出一个错误，这说明 const 声明仍然是有预处理机制的。
  console.log(a); // 报错
  const a = 2;
}
```

##### 4.2.4.12 class声明

class最基本的用法只需要 class关键字、名称和一对大括号。它的声明特征跟const和let类似，都是作用于块级作用域，预处理阶段则会屏蔽外部变量。

```js
const a = 2;
if(true){
  console.log(a); //抛错
  class a {

  }
}
```

class内部，可以使用 `constructor` 关键字定义构造函数，还能定义 `getter/setter` 和方法

```js

class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
  // Getter
  get area() {
    return this.calcArea();
  }
  // Method
  calcArea() {
    return this.height * this.width;
  }
}
```

> 以目前的兼容性，class 中的属性只能写在构造函数中，class默认内部的函数定义都是 **strict模式** 的。

##### 4.2.4.13 函数声明

函数声明使用 `function` 关键字。

```js
function foo(){

}

// 生成器函数可以理解为返回一个序列的函数，它的底层是 iterator 机制。
function* foo(){
    yield 1;
    yield 2;
    yield 3;
}

// async 函数是可以暂停执行，等待异步操作的函数，它的底层是 Promise 机制。
async function foo(){
    await sleep(3000);

}

// 异步生成器函数则是二者的结合。
async function* foo(){
    await sleep(3000);
    yield 1;
}

```

函数的参数，可以只写形参名，现在还可以写默认参数和指定多个参数。

```js
function foo(a = 1, ...other) {
    console.log(a, other)
}
```

#### 4.2.5 表达式语句

表达式语句实际上就是一个表达式，它是由 运算符连接变量 或 直接量 构成。

一般来说，表达式语句要么是函数调用、赋值、自增、自减，否则表达式计算的结果没有任何意义。但是，在语法上没有这样的限制，任何合法的表达式都可以当做表达式语句使用。

##### 4.2.5.1 PrimaryExpression 主要表达式

表达式的原子项：**Primary Expression**。它是表达式的最小单位，它所涉及的语法结构也是优先级最高的。

PrimaryExpression 包含了各种"直接量"，直接量就是用某种语法写出来的具有特定类型的值。在运行时有各种值，比如：数字123，字符串Hello，所以通俗的讲，直接量就是在代码中把它们写出来的语法。

```js
"abc";
123;
null;
true;
false;
```

JS不仅能以直接量的形式定义基本类型，还能够以直接量的形式定义对象，针对函数、类、数组、正则表达式等特殊对象类型，JS提供了语法层面的支持。

```js
({});
(function(){});
(class{ });
[];
/abc/g;
```

> 注意：在语法层面，`function`、`{` 和 `class` 开头的表达式语句和声明语句有语法冲突，所以，要想使用这样的表达式，必须加上括号来回避语法冲突。

PrimaryExpression还可以是 this 或 变量，在语法上，把变量称为 **"标识符引用"**。

```js
this;
myVar;
```

任何表达式加上圆括号，都会被认为是 Primary Expression，这个机制使得圆括号成为改变运算优先级的手段。

##### 4.2.5.2 Member Expression 成员表达式

Member Expression通常用于访问对象成员，它有几种形式：

```js
a.b; // 标识符的属性访问
a["b"]; // 字符串的属性访问
new.target; // new.target 是个新加入的语法，用于判断函数是否是被 new 调用
super.b; // super 则是构造函数中，用于访问父类的属性的语法
```

Member Expression 最初设计是为了属性访问的，不过从语法结构需要，以下两种在 JavaScript 标准中当做 Member Expression

```js
// 带函数的模板，这个带函数名的模板表示把模板的各个部分算好后传递给一个函数。
f`a${b}c`;
// 带参数列表的 new 运算，注意，不带参数列表的 new 运算优先级更低，不属于 Member Expression。
new Cls();
```

> 实际上，这两种被放入 Member Expression，仅仅意味着它们跟属性运算属于同一优先级，没有任何语义上的关联

##### 4.2.5.3 New Expression New表达式

Member Expression 加上 new 就是 New Expression，(当然，不加 new 也可以构成New Expression，JS中默认独立的高优先级表达式都可以构成低优先级表达式)。

> 注意 : 这里的 New Expression 特指没有参数列表的表达式。

##### 4.2.5.4 call Expression 函数调用表达式

除了New Expression，Member Expression 还能构成 call Expression。

它的基本形式是Member Expression后加一个括号里的参数列表，或者可以用上 `super` 关键字替代 Member Expression

```js
a.b(c);
super();

// 还有一些变体
a.b(c)(d)(e);
a.b(c)[3];
a.b(c).d;
a.b(c)`xyz`;
```

> 这些变体的形态，跟Member Expression几乎是一一对应的。实际上，可以理解为，Member Expression中的某一个子结构具有函数调用，那么整个表达式就成为了 call Expression。
> 而 call Expression 就失去了比 New Expression 优先级高的特性，这是一个主要的区分。

##### 4.2.5.5 LeftHandSideExpression 左值表达式

New Expression 和 Call Expression 统称 LeftHandSideExpression，左值表达式。
左值表达式就是可以放到等号左边的表达式，语法如下：

```js
a() = b;
```

原生的JS函数，返回值都不能被赋值。因此，多数时用到的赋值是Call Expression的其他形式，比如：

```js
a().c = b;
```

> 另外，根据JS运行时的设计，不排除某些宿主会提供返回引用类型的函数，这时候，赋值是有效的。
> 左值表达式最经典的用法是用于构建赋值表达式，在JS标准中，它出现在各种场合，凡是需要"可以被修改的变量"的位置，都可以见到它。

##### 4.2.5.6 AssignmentExpression 赋值表达式

AssignmentExpression赋值表达式也有多种形态，最基本的是使用等号赋值：

```js
a = b;
```

上面的等号是可以嵌套的：

```js
a = b = c = d;
// 等价于
// 这不是一个好的代码风格，不建议这样写代码;
a = ( b = (c = d)); // 先把 d 的结果赋值给 c，再把整个表达式的结果赋值给 b，再赋值给 a
```

赋值表达式的使用，还可以结合一些运算符。

```js
a += b;
// 相当于
a = a + b;
```

能这样使用的还有下面几种：

```js
*=、/=、%=、+=、-=、<<=、>>=、>>>=、&=、^=、|=、**=
```

##### 4.2.5.7 Expression 表达式

赋值表达式可以构成 Expression 表达式的一部分。在JS中，表达式就是用逗号运算符连接的赋值表达式。

在JS中，比赋值运算优先级更低的就是逗号运算符。可以把逗号理解为一种小型的分号。

```js
a = b,b = 1, null;
```

逗号分隔的表达式会顺次执行，就像不同的表达式语句一样。"整个表达式的结果" 就是 "最后一个表达式的表达式结果"。上面的例子的表达式结果就是 null。

> 在很多场合，都不允许使用带逗号的表达式，比如：export后只能跟赋值表达式，意思就是表达式中不能含逗号。

##### 4.2.5.8 ConditionalExpression 条件表达式

在一些通用的计算机语言设计理论中，能够出现在赋值表达式的右边，叫做：右值表达式（RightHandSideExpression），而在JS标准中，规定了在等号右边表达式叫做：条件表达式（ConditionalExpression），不过，在JS标准中，从未出现过右值表达式字样。

JS标准也规定了左值表达式同时都是条件表达式（也就是右值表达式），此外，左值表达式也可以通过跟一定的运算符组合，逐级构成更复杂的结构，直到成为右值表达式。

对于右值表达式来说，可以理解为以左值表达式为最小单位开始构成的。

##### 4.2.5.9 UpdateExpression 更新表达式

左值表达式搭配 ++ --运算符，可以形成更新表达式。

```js
--a; ++a; a--; a++;
```

更新表达式会改变一个左值表达式的值，分为前后自增，前后自减一共四种。

> 在ES2018中，跟早期版本有所不同，前后自增自减运算被放到同一优先级。

##### 4.2.5.10 UnaryExpression 一元运算表达式

更新表达式搭配一元运算符，可以形成一元运算表达式

```js
delete a.b;  void a;  typeof a;  - a;  ~ a;  ! a;  await a;
```

> 特点就是一个更新表达式搭配了一个一元运算符。a本身就是一个更新表达式。

##### 4.2.5.11 ExponentiationExpression 乘方表达式

乘方表达式也是由更新表达式构成的。它使用 `**` 号。

```js
2 ** 3  // 正确
-2 ** 3 // 错误
(-2)**3 // 正确
```

> -2 这样的一元运算表达式，是不可以放入乘方表达式的，如果需要表达类似的逻辑，必须加括号（消除运算符优先级的歧义）。
> `**` 运算是右结合的，这跟其他正常的运算符都不一样。

```js
4 ** 3 ** 2
// 事实上被这样运算
4 ** (3 ** 2)
```

##### 4.2.5.12 MultiplicativeExpression 乘法表达式

更新表达式也可以构成乘法表达式，用乘号、除号、取余符号连接即可。它们的优先级是一样的。

```js
x * 2;
```

##### 4.2.5.13 AdditiveExpression 加法表达式

加法表达式可以由乘法表达式用 加号(+) 或 减号(-) 连接构成。

```js
a + b - c
```

##### 4.2.5.14 ShiftExpression 移位表达式

移位表达式由加法表达式构成，移位是一种运算，分成3种：

```js
<< 向右位移
>> 向左位移
>>> 无符号向右位移
```

移位运算把操作数看做二进制表示的整数，然后移动特定位数。所以左移n位相当于乘以2的n次方，右移n位相当于除以2取整n次。

```js
10 << 2; // 40
11 >> 2; // 2
```

普通位移会保持正负数，无符号位移会把减号视为符号位 1，同时参与位移：

```js
-1 >>> 1; // 2147483647，也就是 2 的 31 次方，跟负数的二进制表示法相关
```

> 在JS中，二进制操作整数并不能提高性能，移位运算这里也仅仅是作为一种数学运算存在，这些运算存在的意义仅仅是为了照顾C系语言的用户的习惯。

##### 4.2.5.15 关系表达式 RelationalException

关系表达式就是大于、等于、小于、大于等于、小于等于等运算符号连接，统称为关系运算。

```js
<=
>=
<
>
instanceof
in
```

> 注意：这里的 <= 和 >= 关系运算，完全是针对数字的，所以 <= 并不等价于 <或==。

##### 4.2.5.16 相等表达式 EqualityExpression

在语法上，相等表达式是由关系表达式用相等表达式用相等比较运算符连接构成，所以，可以像下面这段代码一样使用，而不需要加括号：

```js
a instanceof "object" == true
```

相等表达式可以由四种运算符和关系表达式构成：

- ==
- ===
- !=
- !==

相等表达式又包含一个JS中著名的设计失误，那就是 == 的行为。类型不同的变量比较时 == 运算只有三条规则：

- undefined 和 null相等
- 字符串和boolean都转为数字再比较
- 对象转换成primitive类型再比较

这样就可以理解一些不太符合直觉的例子，比如：

- false == "0" // false
- true == "true" // false
- [] == 0 // true
- [] == false // true
- new Boolean("false") == false // false

这里不太符合直觉的有两点：

- 即使是字符串与boolean比较，也要转换成数字
- 对象如果转换成了 primitive 类型跟等号另一边类型恰好相同，则不需要转换成数字

此外，==的行为也经常跟 if 的行为（转换成boolean）混淆。

== 最好只在 Number 与 String 类型之间时使用，比如：

```js
// 等号左边必然是 string，右边的直接量必然是 number
document.getElementsByTagName("input")[0].value == 100
```

##### 4.2.5.17 位运算表达式

位运算表达式含有3种：

- 按位与表达式 BitwiseANDExpression
- 按位或表达式 BitwiseXORExpression
- 按位或表达式 BitwiseORExpression

1. 按位与表达式：按位与表达式由按位与运算符（`&`）连接按位异或表达式构成，按位与表达式把操作数视为二进制整数，然后把两个操作数按位做与运算。

2. 按位异或表达式：按位异或表达式由按位异或运算符（^）连接按位与表达式构成，按位异或表达式把操作数视为二进制整数，然后把两个操作数按位做异或运算。异或两位相同时得0，两位不同时得1。
  异或运算有个特征，那就是两次异或运算相当于取消。所以有一个异或运算的小技巧，就是用异或运算来交换两个整数的值。

    ```js
    let a = 102, b = 324;

    a = a ^ b;
    b = a ^ b;
    a = a ^ b;

    console.log(a, b);
    ```

3. 按位或表达式：按位或表达式由按位或运算符（|）连接相等表达式构成，按位或表达式把操作数视为二进制整数，然后把两个操作数按位做或运算。
  按位或运算常常被用在一种叫 位掩码 (BitMask) 的技术上。BitMask 相当于使用一个整数来当做多个布尔型变量，现在已经不提倡了。不过，一些比较老的API还是会这样设计，比如：DOM中的 iterator API 。

##### 4.2.5.18 逻辑与表达式和逻辑或表达式

逻辑与表达式：由按位或表达式经逻辑与运算符连接构成。
逻辑或表达式：由逻辑与表达式经逻辑或运算符连接构成。

> 注意：这两种表达式都不会做类型转换，所以尽管是逻辑运算，但是最终的结果可能是其他类型。

```js
false || 1; // 1
false || undefined; // undefined
```

逻辑表达式具有短路的特性。

```js
// 这里的 foo 将不会被执行，这种中断后面表达式执行的特性就叫做短路。
true || foo();
```

#### 4.2.5.19 TernaryOperatorExpression 三目运算符

三目运算符由逻辑或表达式和条件运算符构成，条件运算符又称三目运算符，它有三个部分，由两个运算符 ? 和 : 配合使用。

```js
condition ? branch1 : branch2
```

> 注意：条件表达式也像逻辑表达式一样，可能忽略后面表达式的计算。这一点跟C语言的条件表达式是不一样的。
> 三目运算实际上就是JS中的右值表达式 RightHandSideExpression，是可以放到赋值运算后面的表达式。

----

<span id="__proto__"> 1. `[[prototype]]`
: `[[prototype]]` 是对象的私有属性，而 prototype 是只有函数才有的属性，`[[prototype]]` 是JS的非标准但许多浏览器实现的属性，即 __proto__ ，`Object.[[prototype]] === Object.getPrototypeOf(someObject) === someObject.__proto__` (`Object.[[prototype]]` 浏览器不支持这样操作，Object.getPrototypeOf()是ES6的方法)
所有的JS对象都有一个指向它的原形对象的内部链接 `[[prototype]]`，但只有函数才有 prototype 这个属性
</span>