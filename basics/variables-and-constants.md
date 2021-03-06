# 变量和常量

变量和常量是储存数据的方式。

## 变量

你可以这样定义一个变量：

```js
var myVariable;
```

这条语句定义了一个变量，`myVariable`，它没有储存的数据，因此代表 `undefined`。`var` 是用于定义变量的关键字。

## 赋值

你可以通过赋值运算符给 `myVariable` 赋值：

```js
myVariable = 6;
```

此时，`myVariable` 就代表 `6`。在这以后，你就可以通过 `myVariable` 调用其值。

JavaScript 是动态类型语言，这也就意味着，变量的数据类型不是固定的，而是可以通过赋值，更改它数据类型。

`=` 是赋值运算符，它可以对变量执行赋值操作。它有固定的方向，只会先运算右侧表达式的值，然后赋值给左侧的变量。因此，这样的语句也是合法的：

```js
myVariable = myVariable + 3;
```

对于 `=`，你还需注意它无法判断左侧与右侧的值是否相等。所以，以下语句虽然是合法的，但可能不会按你的预期运行：

```js
if ( myVariable = 9 ) { /* do something */ }
```

这样做，无论 `myVariable` 的值是多少，都会执行 `{` 和 `}` 之间的语句。如果将其作为循环语句的条件，跟可能导致无限循环。

## 常量

常量用于储存不变的数据，它可以这样定义：

```js
const pi = 3.1415926535;
```

这样，我们就定义了一个名为 `pi` 的常量。常量的值必须在定义时指定，否则会报出错误。同时，常量一旦定义，就无法再为之赋值。因此，以下语句是非法的：

```js
pi = 3.4151;
```

## 命名

每个变量或常量都有一个名称，用于调用此变量的值。对于这样的变量名或常量名，有以下命名规则：

- 名称中不得含有运算符，如 `[a`、`<b`。
- 名称不得以数字起头，如 `3c`。
- 名称不得与关键字相同，如 `var`、`if`。
- 名称中不得含有空格。

## 参考文献

- [var 描述 - JavaScript | MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/var)
- [const - JavaScript | MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/const)
