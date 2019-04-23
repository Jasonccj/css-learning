# CSS绘制各种几何形状

Github地址:https://github.com/Jasonccj/css-learning/tree/master/everydayCss/polygon  
掘金地址:https://juejin.im/post/5c68375d5188252a160efdec  
慕课地址:https://www.imooc.com/article/278712  

## 正方形
```
.square {
    width: 100px;
    height: 100px;
    background-color: green;
}
```

<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/polygon/square.png" />
</div>

## 长方形
```
.rectangle {
    width: 200px;
    height: 100px;
    background-color: green;
}
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/polygon/rectangle.png" />
</div>

## 锐角三角形
```
.triangle-acute {
    width: 0;
    height: 0;
    border-left: 50px solid transparent;
    border-right: 50px solid transparent;
    border-bottom: 100px solid green; 
}
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/polygon/triangle-acute.png" />
</div>

## 直角三角形
```
.triangle-right {
    width: 0;
    height: 0;
    border-left: 50px solid green;
    border-right: 50px solid transparent;
    border-top: 50px solid transparent;
    border-bottom: 50px solid green; 
}
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/polygon/triangle-right.png" />
</div>

## 平行四边形
```
.rhomboid {
    width: 200px;
    height: 100px;
    margin-left: 30px;
    background-color: green;
    transform: skewX(30deg)
}
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/polygon/rhomboid.png" />
</div>

## 梯形
```
.trapezoid {
    width: 100px;
    height: 0;
    border-bottom: 100px solid green;
    border-left: 50px solid transparent;
    border-right: 50px solid transparent;
}
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/polygon/trapezoid.png" />
</div>

## 圆形
```
.circle {
    width: 100px;
    height: 100px;
    background-color: green;
    border-radius: 50%;
}
```
<div align="left">
    <img src="https://jasonccj.oss-cn-beijing.aliyuncs.com/css-learning/polygon/circle.png" />
</div>

其他图形后续不断更新中!

# 最后
- 喜欢的记得点个star.鼓励一下,谢谢!
- 微信 cuixianseni
- qq群号 424072183

<div align="left">
    <img src="https://jason-1255999874.cos.ap-beijing.myqcloud.com/img/mpvue%2Cjava%2C%E5%B0%8F%E7%A8%8B%E5%BA%8F%E7%BE%A4%E8%81%8A%E4%BA%8C%E7%BB%B4%E7%A0%81.png" width="200px" />
</div>