# css笔记

css最广泛的版本  css2.1

css3开始分模块

检验特性兼容哪些浏览器方法：

使用caniuse.com

## 

CSS  查询

后面加张鑫旭

素材下载

365psd

## 文档流

inline 元素从左到右

block 元素独占一行

inline-block  也是从左到右（注意：这里不会分成两块）

**警告 ！不要在inline元素里面加上block元素。**

**永远不要写width: 100%**

### 宽度的确定

inline元素尽可能的窄，block元素尽可能的宽，inline-block和inline相似但是可以设置width。

### 高度的确定

inline元素的实际高度是由line-height间接确定的，block元素是由里面的文档流元素确定的，可以设置height.

inline-block元素和block元素很像。

##### overflow  溢出:

auto超出时显示滚动条

hidden 直接隐藏溢出部分

visible  直接显示溢出部分

scroll  永远显示滚动条

默认显示第一页的内容，不会随着滚动条变换显示内容。

##### 脱离文档流

position : absolute/fixed  定位

float   浮动 

## 盒模型

如果宽度只包含内容，则称为content box 

如果宽度包含border则称为border-box.

### margin合并

只在上下边距合并

取消合并  : 给父盒子加boder 或者加padding 、overflow ：hidden。

