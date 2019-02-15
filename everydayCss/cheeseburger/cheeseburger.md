## 芝士汉堡制作
最近看到有人翻译这篇英文文章,正好还年后还没开始上班,在家没事也饿了,也打算自己好好做一个这样的芝士汉堡,品尝一下

[参考原文链接](https://www.lesscake.com/cheeseburger-css-div)

那么绘制如下

## HTML
html绘制非常简单
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Cheeseburger</title>
    <link rel="stylesheet" href="cheeseburger.css">
</head>
<body>
    <div class="cheeseburger"></div>
</body>
</html>
```

## CSS
由于汉堡包含内容比较多,我们想在一个div上绘制汉堡的话,会想到用伪类来扩大我们的绘制面积,废话不多说,基本构造如下

```
.cheeseburger{
    /* 整个汉堡 */
}

.cheeseburger::before{
    /* 上下两层面包 */
}

.cheeseburger::after{
    /* 芝麻 */
}
```