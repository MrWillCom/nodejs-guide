# 数组

数组用于存储一组有序数据。

要定义一个数组，应使用 `[` 和 `]` 包装数据，用 `,` 分割每个数组元素：

```js
var myArray = [1, 2, 4, 7];
```

这是一个只包含数的数组。接着，我们试着打印其中的第一个元素 “`1`”：

```js
console.log(myArray[0]);
```

此时控制台会输出 `1`。

数组的每一个元素都有一个索引，索引从 0 起始，依次往后递增。

你可通过 `console.table` 方法以表格的形式输出数组：

```output
> console.table(myArray);
┌─────────┬────────┐
│ (index) │ Values │
├─────────┼────────┤
│    0    │   1    │
│    1    │   2    │
│    2    │   4    │
│    3    │   7    │
└─────────┴────────┘
undefined
```

在 JavaScript 中，数组元素的类型不受限制，你可以混合各种数据类型。如：

```js
var arrayWithDifferentTypesOfItems = [1, "string", ["array", "in", "array"], { name: "also objects", description: 3 }];
```

要调用数组的长度，你可以使用 `length` 方法：

```js
console.log(myArray.length);
```

这将会输出一个数。另外，如果为 `length` 赋值，数组也会随之被修改：

```output
> myArray.length = 5; myArray;
[ 1, 2, 4, 7, <1 empty item> ]
> myArray.length--; myArray;
[ 1, 2, 4, 7 ]
```

因此，当你要取数组长度的递减值时，不能使用 `--` 运算符，这将删除数组的最后一个元素。

除此之外，还有一种新建数组的方法：

```js
var newArrayCreatedWithNew = new Array();
```

这也就揭露了在 JavaScript 中，数组的本质实际上是一个对象。
