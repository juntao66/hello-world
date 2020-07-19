#jquery
#事件注册
1. 单个事件注册
```
$("div").click(function(){事件处理程序})
```
1. 多个事件
```
$("div").on({
	mouseenter: function(){
		$(this).css("background","skyblue");
	},
		click: function(){
			$(this).css("background","blue");
			}
})
```

1. 事件委托
```
$("ul").on("click","li",function(){
		alert('11')
})
```
click是绑定在ul上的，但是触发对象是ul里的li

1. 动态创建
```
var li = $("<li>后来创建的</li>")
$("ul").append(li)
```
#off()解绑事件
```
$("div").off("click")
$("div").off("click","li")//解绑事件委托
```

##one()只能触发事件一次
