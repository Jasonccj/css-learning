## 一个DIV的芝士汉堡制作

项目Github地址:[点击跳转](https://github.com/Jasonccj/css-learning/tree/master/everydayCss/cheeseburger)

最近看到有人翻译这篇英文文章,正好还年后还没开始上班,在家没事也饿了,也打算自己好好做一个这样的芝士汉堡,品尝一下芝士汉堡的乐趣

<div align="center">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/cheeseburger/hanbao.jpg" width="300px" />
</div>

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

绘制上下两层面包,我们采用border绘制

```
.cheeseburger::before{
    content: '' ;
    display: block ;

    width: 300px;
    height: 60px;

    border-top: 90px solid #F5B231;
    border-bottom: 60px solid #F5B231;

}
```
<div align="left">
    <img src="
https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/cheeseburger/bread.jpg" width="300px" />
</div>

用border-radius设置圆角
```
 border-radius: 30% 30% 20% 20%;
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/cheeseburger/bread-cirtle.jpg" width="300px" />
</div>

接下来我们做肉

```
.cheeseburger{
    width: 280px;
    height: 40px;
    background-color: #962012;
    border-radius: 15px;   
}
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/cheeseburger/meat.png" width="300px" />
</div>

但是肉的位置并不是我们想要的,想要移动我们采用margin和padding,但是这样会使我们整个汉堡都移动,此时我们采用box-shadow;

```
    box-shadow: 10px 100px #962012;
```

<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/cheeseburger/meat-center.png" width="300px" />
</div>

接下来我们用同样阴影的方式将奶酪和生菜添加上

```
    box-shadow: 
    10px 70px #fddb28,
    10px 90px #1EE154,
    10px 120px #962012;
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/cheeseburger/chess.png" width="300px" />
</div>

大体已经成型,我们在撒点芝麻,同样采用box-shadow

```
box-shadow: 
        /* Top row */
        55px -200px #ffffff,
        105px -200px #ffffff,
        155px -200px #ffffff,
        205px -200px #ffffff,
        245px -200px #ffffff,

        /* Bottom row */
        25px -160px #ffffff,
        75px -160px #ffffff,
        125px -160px #ffffff,
        175px -160px #ffffff,
        225px -160px #ffffff,
        270px -160px #ffffff;
```

<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/cheeseburger/sesame.png" width="300px" />
</div>

至此汉堡已经成型,可以给奶酪加点流下来的效果

```
    content: '                ▾' ;
    color: #fddb28;
    white-space: pre;
    font-size: 45px;
    line-height: 45px;
```

<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/cheeseburger/success.png" width="300px" />
</div>

结束!

特别鸣谢! [参考链接](https://www.lesscake.com/cheeseburger-css-div)

# 最后
- 喜欢的记得点个star.鼓励一下,谢谢!
- 微信 cuixianseni
- qq群号 424072183

<div align="left">
    <img src="https://jason-1255999874.cos.ap-beijing.myqcloud.com/img/mpvue%2Cjava%2C%E5%B0%8F%E7%A8%8B%E5%BA%8F%E7%BE%A4%E8%81%8A%E4%BA%8C%E7%BB%B4%E7%A0%81.png" width="200px" />
</div>