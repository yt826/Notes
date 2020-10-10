# CSS布局

## 布局分类

1. 固定宽度布局 （960/1000/1024px)
2. 不固定宽度布局 （手机布局）
3. 响应式布局 

## 布局两种思路

- 从大到小
- 从小到大

## 布局方法

### CSS布局

![image-20201007142646411](C:\Users\17724\Desktop\前端笔记\imges\一图流)

### float布局

#### 步骤

1. 子元素用float 
2. 父元素一定要添加.clearfix 

经验 ：

一般最后一个不设宽度

float布局不用响应式

如果图片发现有东西 就用vertical - align: middle;

border有时会干扰布局，这是换成outline。

负margin:

### flex布局

#### container 容器

将一个元素变成flex

.container {

display: flex

}

| 属性            | 值                   | 作用               |
| --------------- | -------------------- | ------------------ |
| flex-direction  | row/column           | 控制主轴的方向     |
| flex-wrap       | wrap                 | 控制是否换行       |
| justify-content | center/space-between | 控制对齐的方式     |
| align-items     | center               | 控制支轴对齐的方式 |

### Grid布局

{

display: grid; 

}

| 属性                       | 值                                        | 作用                       |
| -------------------------- | ----------------------------------------- | -------------------------- |
| grid-column-start / end    | x                                         | 设置开始/结束              |
| grid-area:                 | row-start/column-start/row-end/column-end | 合并设置                   |
| order                      | 1                                         | 设置顺序                   |
| grid-template-rows/columns | 20px 40% 3em                              | 设置每一行或每一列的宽度。 |

## CSS定位

div的分层 
由下往上依次是 background border 块级子元素 浮动子元素 内联子元素

position-新属性

| position | 作用                                                       |
| -------- | ---------------------------------------------------------- |
| static   |                                                            |
| relative | 绝对定位，还在文档流里面，原来位置不变，但是显示的位置变了 |
| absolute | 相对定位                                                   |
| fixed    | 相对于视口的定位（手机上不要用）                           |
| sticky   | 粘滞定位                                                   |

white-space: no wrap控制文字不换行。

点两次hover展示hover