# 05 Flex Panel Gallery

## 涉及知识
1. `flex`属性
是一个简写属性，包括了`flex-grow`, `flex-shrink`, `flex-basis`三个属性. <br/>
> `flex-grow`: 值为数字，设置弹性盒子的伸展值（和主尺寸`main size`相比），类似分数占比 <br/>
> `flex-shrink`: 值为数字，设置弹性盒子的收缩值
> `flex-basis`: 值为一个有效的宽度值，用于指定flex 元素在主轴方向上的初始大小
<br/>

2. `classList.toggle()`方法
有则移除，无则添加。
<br/>

## 思路
1. 给panel类设置弹性布局，声明flex值为1
2. 监听panel盒子的点击事件，动态替换`open`选择器（flex值修改为5）
3. 制造文字上下飞入的效果：先把上下文字利用`transform`移开，点击时移回来，注意要设置`transition-delay`值，否则文字会比图片的伸展先变化。
