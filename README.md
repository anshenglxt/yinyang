#第11课，旋转段阴阳图

##html 代码
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>11课：阴阳图</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <p>11课：旋转的太极阴阳图</p>
    <div class="circle">
        <div class="circle-left">
            <div class="circle-left-inside">
            </div>
        </div>
        <div class="circle-right">
            <div class="circle-right-inside"></div>
        </div>
    </div>
</body>
</html>
```
##css 代码
```css
body{
    background: aqua;
}

p{
    text-align: center;
    margin-top: 20px;
    font-size: 30px;
    font-weight: bold;
}

.circle{
    border-top:100px solid gray;
    border-bottom: 100px solid white;
    border-radius: 50%;
    width:200px;
    background-color:black;
    position: relative;
    animation:spin 4s linear infinite;
    margin:50px auto;
}

@keyframes spin { 
    100% { 
        transform:rotate(360deg); transform-origin: 50% 50%; 
    } 
}

.circle-left{
    width: 100px;
    height: 100px;
    background:gray;
    border-radius: 50%;
    position: absolute;
    left:0;
    top:-50px;
    z-index: 10;
}
.circle-left-inside{
    width:20px;
    height: 20px;
    background: white;
    border-radius: 50%;
    margin: 50px auto;
}
.circle-right{
    width: 100px;
    height: 100px;
    background:white;
    border-radius: 50%;
    position: absolute;
    left:100px;
    top:-50px;
    z-index: 10;
}
.circle-right-inside{
    width:20px;
    height: 20px;
    background: gray;
    border-radius: 50%;
    margin: 50px auto;
}

```

