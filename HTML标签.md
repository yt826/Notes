# HTML标签

## 层级

[TOC]

section   章节标签

header  头部

footer  脚部

main 主要内容

aside 旁支内容

div 做划分

pre   保留空格，回车等

code  默认里面的字体等宽

hr  分割线

br 换行



## 全局属性

class 

contenteditble  使任何元素都可以被编辑

hidden  显示或者隐藏



## 重点标签

#### a标签

<a href ="#" target>

target  指定在哪个窗口打开

rel = noopener   防止BUG

##### href的值：

http//xxx.com

https//xxx.com

//xxx.com(以后就使用这个)

路径  a/b/c

伪协议 ：javascript:;

#xxx  id

邮件伪协议：mailto:邮箱

tel:手机号(点击后直接拨打号码)；

##### target的值：

_blank 在新的页面打开

_top 在最上面的窗口打开

_parent 在当前链接所在的上一层打开

_self  在当前一层打开

_xxx 创建一个新窗口并命名为xxx



#### table标签

```html
<table>
    <thead>
        <tr>				//table里面的一行A
            <th>英语</th>		//表头
             <th>翻译</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>hyper</td>//一行里面的一格
            <td>超级</td>
        </tr>
        <tr>
        <td>target</td>
        <td>
            目标</td></tr>
         <tr>
        <td>
             reference</td>
        <td>
             引用</td>
        </tr>   <table>
        <thead>
            <tr>
                <!--table里面的一行A -->
                <th>英语</th>
                <!--表头 -->
                <th>翻译</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>hyper</td>
                <!--一行里面的一格 -->
                <td>超级</td>
            </tr>
            <tr>
                <td>target</td>
                <td>目标</td>
            </tr>
            <tr>
                <td>reference</td>
                <td>引用</td>
            </tr>
        </tbody>
        <troot></troot>
    </table>
    </tbody>
    <tfoot></tfoot>
</table>
```



thead 	头部

tr 	table 里面的一行

td    一行里面的一格

tbody 	身体

troot 	尾部

##### 相关的样式

table-layout 设置计算宽度的算法

boder-spacing  每一格之间的间隙

border-collapse 设置边框是否合并

#### img标签

作用：发出一个请求，展示一张图片

属性：

- alt   加载失败时输出文字
- width 宽度
- heigth 高度
- src 路径

max-sizing 响应式


#### form 标签

##### input标签

作用 : 发出一个get或post请求，然后刷新页面

属性 ：

name 表单的名字

type 表单的类型     **注意: 一个表单里面必须要有一个type="submit"的东西**

type 的值：

|  type值  | 含义                       |
| :------: | -------------------------- |
| password | 不显示输入的内容           |
|  radio   | 单选按钮                   |
| checkbox | 多选按钮                   |
|   file   | 选择文件  +mutiple可以多选 |
|  hidden  | 看不见的input              |

 action 提交到什么位置

autocomplete 推荐曾经的用户名

**input里面的 submit 和button标签的区别**

input不可以加东西

button里面还可以加其他的东西 如标签等。

##### select  选择

<option value = "">  </option>

