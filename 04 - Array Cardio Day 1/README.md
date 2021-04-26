# 04 Array Cardio Day 1

## 涉及知识
### [Array](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array)<br/>
**1. [Array.prototype.filter()](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)**
> 语法： `arr.filter(callback(element, index, array), this.arg);` <br/>

`filter()`返回一个数组，其元素通过callback函数的测试。 <br/>
`callback(element, index, array)`的三个传参中element表示原数组的元素，index表示元素下标，array表示原数组对象，其中element为必选参数。
<br/><br/>


**2. [Array.prototype.map()](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/map)**
> 语法： `arr.map(callback(element, index, array), this.arg);` <br/>

`map()`返回一个数组，其中每个元素都是原元素调用callback函数后的结果。 <br/><br/>

**3. [Array.prototype.sort()](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)**
> 语法： `arr.sort(compareFunction(a, b));` <br/>

compareFunction为可选传参，比较函数中若返回结果<0，则a在b之前；>0则b在a之前，=0则排位不变。<br/><br/>

**4. [Array.prototype.reduce()](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)** 
> 语法： `arr.reduce(callback(accumulator, currentValue[, index[, array]])[, initialValue])` <br/>

`reduce()`返回一个值，由遍历各个数组元素执行定义好的callback函数而汇总成的终值。<br/>
`accumulator`表示当前累计值，调用`reduce()`函数时可以传一个初始值`initialValue`进去。<br/><br/>
