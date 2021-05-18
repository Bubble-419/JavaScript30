# Array Cardio Day 2
## 涉及知识
### 1. Array.prototype.some()
> 语法：`arr.some(callback(element[, index[, array]])[, thisArg])` <br/>

`some()`返回一个布尔值，告诉我们该数组中是否至少有一个元素通过了回调函数的测试。<br/>

### 2. Array.prototype.every()
> 语法：`arr.every(callback(element[, index[, array]])[, thisArg])` <br/>

`every()`返回一个布尔值，告诉我们该数组中是否全部元素都通过回调函数的测试。<br/>
当数组为空时，也会返回`true`。<br/>

### 3. Array.prototype.find()&findIndex()
> 语法：`arr.find(callback(element[, index[, array]])[, thisArg])`, arr.findIndex(callback(element[, index[, array]])[, thisArg]) <br/>

`find()`查找通过回调函数测试的**第一个**元素的**值**，如果没有则返回`undefined`，`findIndex()`则是查找其**索引值**。<br/>
注意`findIndex()`是查找通过函数测试的第一个元素的索引值，而有个类似的方法`indexOf()`是查找给定元素的索引值。
