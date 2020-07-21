##element.getAttribute('属性')
```html
<body>
    <div id="demo" index="1"></div>
    <script>
        var div = document.querySelector('div')
        console.log(div.id)

        //2 自定义属性
       console.log(div.getAttribute('index'))
    </script>
</body>
```

##element.属性 = 值
##element.setAttribute('属性','值')
```
       div.setAttribute('index',2)
```
