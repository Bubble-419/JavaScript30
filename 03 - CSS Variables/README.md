# 03 CSS Variables

## 涉及知识
**1. `:root`根伪类**
<br/>
`:root`这个 CSS 伪类匹配文档树的根元素。对于 HTML 来说，`:root` 表示 `<html>` 元素，除了优先级更高之外，与 html 选择器相同。通常与声明全局CSS变量搭配使用。
<br/>

**2. CSS变量**
<br/>
CSS变量是由开发者自定义的属性，当相同的属性值在文档中多次出现时，可以利用CSS变量动态赋值，避免修改时的困难。<br/>
变量的属性名需要以“--”开头，例如`--main-bg-color`，且和普通属性一样需要被声明在规则集内，规则集指定的选择器定义了变量的可见域。当我们把变量声明在`:root`里时，变量是全局可访问的。 <br/>
当我们需要使用变量时，只需要用`var()`函数包裹即可，例如`background-color: var(--main-bg-color);`<br/>
<br/>
**3. HTML滑块控件** `<input type='range'>`
<br/>
<br/>
**4. JS中`element.setAttribute()`和`element.setProperty()`的区别**
<br/>
前者用于修改标签属性值，后者用于修改样式属性值

## 实现思路
1. 利用css变量事先声明好img的背景色、blur()值和边框大小，这样修改时只需要修改变量值即可<br/>
2. 定义修改变量值的函数<br/>
3. 监听控件元素的change（值立刻改变）和mousemove事件（值随鼠标移动而改变）
