#DOM
处理HTML或xml的编程接口
W3C已经定义一系列dom

##DOM树
![](https://upload-images.jianshu.io/upload_images/16749538-64b1ae6106efded7.png)

- 文档：一个页面就是一个文档
- 元素：页面中所以标签都是元素
- 节点：网页中所以内容都是节点

**DOM把以上内容都看作是对象**

1. getElementById
*返回对拥有指定 id 的第一个对象的引用。*
```HTML
<div id='time'>2019</div>
<script>
	var timer = document.getElementById('time')
	console.log(timer)
</script>
```
1. getEelementsByTagName
*返回带有指定标签名的对象集合。*
```HTML
<li>1</li>
<li>2</li>
<script>
	var lis = document.getEelementsByTagName('li')
	console.log(lis)
</script>
```
1. getElementsByClassName
*返回文档中所有指定类名的元素集合，作为 NodeList 对象。*
1. querySelector
*返回指定选择器的第一个元素*
1. querySelectorAll
*返回指定选择器的所有元素*
1. body
*返回body*
1. documentElement
*返回HTML*


##事件源 ：要触发的对象  （一般是名词，事件发起者，比如开关按钮）

##事件类型：怎么触发这个事情  （一般是动词，触发事件，比如点击开关）

##事件处理程序:发生了什么事情 （处理结果，比如灯亮了）
###获取事件源 —>> 注册事件（绑定事件）—>> 添加事件处理函数

```
<button id="btn">按钮</button>

<script>
	// 获取事件源
	var btn = document.querySelector('#btn')
	// 注册事件
	 btn.onclick = function () { // 添加事件处理函数
	 	alert('触发了事件！')
	 }
</script>
```
#操作元素
1. innerText
*innerText 打印标签之间的纯文本信息，会将标签过滤掉*
1. innerHtml
*打印标签之间的内容，包括标签和文本信息*
1. src，herf
1. id，alt，title
1. 表单元素：type，value，checked，selected，disabled
1. 样式：element.style   element.className

```
<script>
var btn = document.querySelector('.close-btn')
var box = document.querySelector('.box')
btn.onclick = function(){
	box.style.display = 'none'
}
</script>
```
1. this.className = 'change'
改类名
