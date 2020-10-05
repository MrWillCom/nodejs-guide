# 函数

函数是接收参数的一个语句块，以下是一个函数：

```js
function log(str) {
    console.log(str);
};
```

以上语句定义了一个名为 `log` 的函数，它和以下语句等价：

```js
var log = function (str) {
    console.log(str);
};
```

对于 `log`，你可以这样调用它：

```js
log();
```

它会向控制台输出 `undefined`。

你可以给它提供一个参数：

```js
log('Hello, World!');
```

它将会向控制台输出 `Hello, World!`。

函数可以接收若干个参数：

```js
var multipleParams = function (a, b) {
    console.log(a, b);
};
```

在定义函数时，仅需在 `(` 和 `)` 之间添加新的参数，用 `,` 分隔。然后在 `{` 和 `}` 之间的函数体中就可以调用参数。你也可以不接收参数：

```js
var noParams = function () { /* do something */ };
```

同时，函数可以通过 `return` 语句返回结果：

```js
var returnValue = function (a, b) {
    return a + b;
};
```

这样，你就可以调用这个函数并提供参数即可获得返回值，你可以将其存储在一个变量里：

```js
var addition = returnValue(1, 2);
```

那么，`addition` 的值会被赋值为 `3`。

`return` 语句只能在函数中使用，每个函数可以有多个 `return` 语句，它们可以被放在逻辑语句中。`return` 语句一旦被执行，函数的执行就完成了，因此 `return` 语句执行后的语句将不会执行。

```js
var abs = function (a) {
    if (a < 0) {
        return -a;
    } else {
        return a;
    }
};
```

这是一个取绝对值的函数，我们可以使用它取数的绝对值：

```js
var result = abs(-5);
```

这时候，`result` 的值是 `5`。

除了使用 `function` 关键字定义函数外，还可以使用箭头标记定义：

```js
var arrowDefination = (str) => {
    console.log(str);
};
```

## 参考文献

- [函数 - JavaScript | MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions)
- [箭头函数 - JavaScript | MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions/Arrow_functions)
