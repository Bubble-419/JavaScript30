# 01 JavaScript Drum Kit

## 涉及知识简单回顾：
<br/>

**1. 键盘事件**
> `keydown`:按下触发，长按一直触发
<br/>

**2. 自定义属性,属性选择器**
> 给元素的自定义属性要以data开头（自定义规范）<br/>
> 属性选择器： `element[attr='']` 
<br/>

**3. HTML5 audio标签**
> 一些值得留意的属性：

|  属性   | 值  |
|  ----  | ----  |
| currentTime  | 设置或返回音频中的当前播放位置（以秒计）。 |
| ended	  | 返回音频的播放是否已结束。 |
| (default)playbackRate	 |  设置或返回音频(默认)播放的速度。 |
| (default)muted  |	设置或返回是否(默认)关闭声音。 |
| paused	|  设置或返回音频是否暂停。 |

<br/>

**4. 模板字符串**
> 使用"\`"来代替引号组成模板字符串，使用`${}`作为表达式占位符，可以使代码更优雅，且模板字符串内可换行。 <br/>
````javascript
//e.g
const a = 15;
const b = 30;
console.log('a + b = '+(a+b));
console.log(`a + b = ${a+b}`);
````
<br/>

**5. transitionend事件监听**
> transitionend事件会在css transition结束后触发。
<br/>

## 实现思路
    1. 键盘按下时，利用ASCII值和key属性的关联，找到对应的元素，修改类名为playing
    2. 同理找到对应的audio标签，播放
    3. 监听到元素的过渡事件结束后，移除类名
    4. 每次播放都改变audio的currentTime属性为0，实现长按可以连续播放
