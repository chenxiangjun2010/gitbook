# 第1节：常用的css

#### css 写法规范

```css
Positioning position top right bottom left z-index

Box mode	display box-sizing width height padding border border-radius float overflow

Typographic font lin-height text-align

Visual 		background color opacity
```



#### 渐变的写法

```css
background: linear-gradient(to right, yellow 0% 10%, blue 10% 25%, red 25%);
```

表示 0%-10%显示yellow，10%-25%显示blue，25%-100%显示red

``` css
`background：linear-gradient(to right, yellow 10%, blue  25%, red 40%);`
```

表示 0%-10%显示yellow，10%-25%显示yellow-blue的渐变，25%-40%显示blue-red的渐变，40%-100%显示red

#### 阴影的写法

``` css
box-shadow: 5px 10px 10px #888888 inset;
```

 表示 X轴 Y轴 Rpx（模糊程度） color 内阴影

#### 动画的写法

```css
animation:mymove 5s infinite;
```

``` css
animation: slidein 3s ease-in 1s infinite reverse both running;
```

表示 动画名称 运行时间 运行的时间函数 延迟 运行次数 运行方向   在执行之前和之后如何将样式应用于其目标   运行状态

里面有个step函数，适合做常背景的

#### font-size 适配比较好的

``` css
html {

 font-size: 16px;

}

@media screen and (min-width: 375px) {

 html {

  */\* iPhone6的375px尺寸作为16px基准，414px正好18px大小, 600 20px \*/*

  font-size: calc(100% + 2 * (100vw - 375px) / 39);

  font-size: calc(16px + 2 * (100vw - 375px) / 39);

 }

}

@media screen and (min-width: 414px) {

 html {

  */\* 414px-1000px每100像素宽字体增加1px(18px-22px) \*/*

  font-size: calc(112.5% + 4 * (100vw - 414px) / 586);

  font-size: calc(18px + 4 * (100vw - 414px) / 586);

 }

}

@media screen and (min-width: 600px) {

 html {

  */\* 600px-1000px每100像素宽字体增加1px(20px-24px) \*/*

  font-size: calc(125% + 4 * (100vw - 600px) / 400);

  font-size: calc(20px + 4 * (100vw - 600px) / 400);

 }

}

@media screen and (min-width: 1000px) {

 html {

  */\* 1000px往后是每100像素0.5px增加 \*/*

  font-size: calc(137.5% + 6 * (100vw - 1000px) / 1000);

  font-size: calc(22px + 6 * (100vw - 1000px) / 1000);

 }

}
```





### 全屏灰

```css
-webkit-filter: grayscale(100%);
-moz-filter: grayscale(100%);
-ms-filter: grayscale(100%);
filter: grayscale(100%);
filter: progid:DXImageTransform.Microsoft.BasicImage(grayscale=1);  /* ie */
filter: gray; /* ie6~ie9 */
```

