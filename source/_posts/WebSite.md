# JavaScript的学习

***

## 初步了解js

***

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>一个需要加工的网页</title>    
    <style>
        .pink{
            background-color: pink;
        }
    </style>
</head>
<body>
    <h1>1级标题</h1>
        <p>
        原力刀法
        </p>
        <p>
        快慢<br>刀法
        </p>
    <h2>2级标题</h2>
    <h3>3级标题</h3>
    <h4>4级标题</h4>
    <h5>5级标题</h5>
    <h6>6级标题</h6>
    <button style="color: green" class="pink">按钮1</button>
    <button style="color: black">按钮2</button>
    <button style="color: red">按钮3</button>
    <button style="color: purple">按钮4</button>

    <script>
        let btns=document.querySelectorAll('button')
        for (let i = 0; i <= btns.length; i++) {
            btns[i].addEventListener('click',function(){
                document.querySelector('.pink').className=''
                this.className='pink'
            })
        }
    </script>
</body>
</html>
```

这个是一个网页情况运行会变成

![](E:\Personal%20blog\Blog1\Web%20Site\parallaxScrollingWebsite01\images\Snipaste_2023-01-21_16-30-40.png)

![](E:\Personal%20blog\Blog1\Web%20Site\parallaxScrollingWebsite01\images\Snipaste_2023-01-21_16-31-14.png)
