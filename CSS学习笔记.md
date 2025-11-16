# CSS 学习笔记
### 什么是CSS？
- CSS指层叠样式表(**C**ascading **S**tyle **S**heets)

- 样式定义**如何显示**HTML元素

- 样式通常存储在**样式表**中

- 把样式添加到 HTML 4.0中，是为了解**决内容与表现分离的问题**

- **外部样式表**可以极大提高工作效率

- 外部样式表通常存储在**CSS**文件中

- 多个样式可**层叠**为一个

### CSS实例
CSS规则有两个主要的部分构成：选择器，以及一条或多条声明；
![CSS实例](https://www.runoob.com/wp-content/uploads/2013/07/632877C9-2462-41D6-BD0E-F7317E4C42AC.jpg)
选择器通常是您需要改变样式的 HTML 元素。

每条声明由一个属性和一个值组成。声明每一行属性，都需要以英文分号结尾；

属性是您希望设置的样式属性。每个属性有一个值。属性和值之间被冒号隔开；所有属性和值都是以键值对这种形式出现。

![css实例](https://github.com/lixiu0816/Task/raw/main/images/CSS1.png)
### CSS 三种导入方式
1. 内联样式（inline styles）
   
当样式仅需要在一个元素上应用一次时。

`<p style="color:sienna;margin-left:20px">这是一个段落。</p>`

2. 内部样式表（internal stylesheet）

当单个文档需要特殊的样式时，就应该使用内部样式表。
```
<head>
<style>
hr {color:blue;}
p {margin-left:20px}
body {background-image:url("images/back40.gif");}
</style>
</head>
```
3. 外部样式表（external stylesheet）

当样式需要应用于很多页面时，外部样式表将是理想的选择。

浏览器会从文件 mystyle.css 中读到样式声明，并根据它来格式文档。
```
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```
**三种导入方式优先级**：
`'内联样式'>'内部样式表'>'外部样式表'`
### CSS 背景
CSS 背景属性用于定义HTML元素的背景。

CSS 属性定义背景效果:

- background

简写属性，作用是将背景属性设置在一个声明中。

- background-color

background-color 属性定义了元素的背景颜色.

- background-image

background-image 属性描述了元素的背景图像.

默认情况下 background-image 属性会在页面的水平或者垂直方向平铺。

默认情况下，背景图像进行平铺重复显示，以覆盖整个元素实体.

- background-repeat

如果你不想让图像平铺，你可以使用 background-repeat 属性:
```
body
{
background-image:url('img_tree.png');
background-repeat:no-repeat;
}
```
- background-attachment

- background-position
  
可以利用 background-position 属性改变图像在背景中的位置.
### CSS 文本格式
##### 文本颜色
颜色是通过CSS最经常的指定：

- 十六进制值 - 如: ＃FF0000

- 一个RGB值 - 如: RGB(255,0,0)

- 颜色的名称 - 如: red

一个网页的背景颜色是指在主体内的选择：
```
实例
body {color:red;}
h1 {color:#00ff00;}
h2 {color:rgb(255,0,0);}
```
**注**：对于W3C标准的CSS：如果你定义了颜色属性，你还必须定义背景色属性。
##### 文本的对齐方式
文本排列属性是用来设置文本的水平对齐方式。

文本可居中或对齐到左或右,两端对齐.

当text-align设置为"justify"，每一行被展开为宽度相等，左，右外边距是对齐（如杂志和报纸）。
```
实例
h1 {text-align:center;}
p.date {text-align:right;}
p.main {text-align:justify;}
```
##### 文本修饰
ext-decoration 属性用来设置或删除文本的装饰。

从设计的角度看 text-decoration属性主要是用来删除链接的下划线。
##### 文本转换
文本转换属性是用来指定在一个文本中的大写和小写字母。

可用于所有字句变成大写或小写字母，或每个单词的首字母大写。
```
p.uppercase {text-transform:uppercase;}
p.lowercase {text-transform:lowercase;}
p.capitalize {text-transform:capitalize;}
```
##### 文本缩进
文本缩进属性是用来指定文本的第一行的缩进。
### CSS 字体
CSS字体属性定义字体，加粗，大小，文字样式。
##### serif和sans-serif字体之间的区别
![字体](https://www.runoob.com/images/serif.gif)
**注** 在计算机屏幕上，sans-serif字体被认为是比serif字体容易阅读
#### CSS字型

在CSS中，有两种类型的字体系列名称：

- **通用字体系列** - 拥有相似外观的字体系统组合（如 "Serif" 或 "Monospace"）

- **特定字体系列** - 一个特定的字体系列（如 "Times" 或 "Courier"）

**注**: 如果字体系列的名称超过一个字，它必须用引号，如Font Family："宋体"。

多个字体系列是用一个逗号分隔指明.
#### 使用百分比和EM组合来设置字体大小

在所有浏览器的解决方案中，设置 <body>元素的默认字体大小的是百分比：
```
body {font-size:100%;}
h1 {font-size:2.5em;}
h2 {font-size:1.875em;}
p {font-size:0.875em;}
```
### CSS 链接
##### 链接样式
四个链接状态是：

- a:link - 正常，未访问过的链接

- a:visited - 用户已访问过的链接

- a:hover - 当用户鼠标放在链接上时

- a:active - 链接被点击的那一刻

**注**：当设置为若干链路状态的样式，也有一些顺序规则：

- a:hover 必须跟在 a:link 和 a:visited后面

- a:active 必须跟在 a:hover后面
### CSS 轮廓（outline）
轮廓（outline）是绘制于元素周围的一条线，位于边框边缘的外围，可起到突出元素的作用。

CSS outline 属性规定元素轮廓的样式、颜色和宽度。
![实例](https://www.runoob.com/images/box_outline.gif)
#### 所有CSS 轮廓（outline）属性
- outline：在一个声明中设置所有的轮廓属性

- outline-color:设置轮廓的颜色

- outline-style:设置轮廓的样式

- outline-width:设置轮廓的宽度
### CSS 网页布局
网页布局有很多种方式，一般分为以下几个部分：**头部区域**、**菜单导航区域**、**内容区域**、**底部区域**。
![实例](https://www.runoob.com/wp-content/uploads/2019/04/DBD1E737-47C5-445E-BFEC-7547210D88D5.jpg)
##### 头部区域
头部区域位于整个网页的顶部，一般用于设置网页的标题或者网页的 logo：
```
.header {
  background-color: #F1F1F1;
  text-align: center;
  padding: 20px;
}
```
##### 菜单导航区域

菜单导航条包含了一些链接，可以引导用户浏览其他页面.

##### 内容区域
内容区域一般有三种形式:

- 1 列：一般用于移动端

- 2 列：一般用于平板设备

- 3 列：一般用于 PC 桌面设备
![实例](https://www.runoob.com/wp-content/uploads/2019/04/D105F34E-6592-47AC-A9DF-EEDC1E2172B3.jpg)
我们将创建一个 3 列布局，在小的屏幕上将会变成 1 列布局（响应式）：
```
CSS3 实例
/* 创建三个相等的列 */
.column {
  float: left;
  width: 33.33%;
}
 
/* 列后清除浮动 */
.row:after {
  content: "";
  display: table;
  clear: both;
}
 
/* 响应式布局 - 小于 600 px 时改为上下布局 */
@media screen and (max-width: 600px) {
  .column {
    width: 100%;
  }
}
```
**提示**:要设置两列可以设置 width 为 50%。创建 4 列可以设置为 25%。

















