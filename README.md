
该内容主要集合了html/css/JavaScript的初级笔记
对所知内容进行一定的收集并进行整理

* name: 铭心
* time: 2021/3/15
* 该内容会持续更新

# html/css 模块
### 1. html 基本结构
   - html 标签是由<>包围的关键词。
   - html 标签通常成对出现，分别为标签开头和标签结尾。
   - 有部分标签是没有结束标签的，为单标签，单标签必须使用 / 结尾。
   - 页面所有的内容都在 html 标签中。
   - html标签分为三部分：标签名称，标签内容，标签属性。
   - html标签具有语义化，可通过标签名能够判断出该标签的内容，语义化的作用是网页。
   - 结构层次更清晰，更容易被搜索引擎收录，更容易让屏幕阅读器读出网页内容。
   - 标签的内容是在一对标签内部的内容。
   - 标签的内容可以是其他标签。
### 2. 标签属性
   - class属性：用于定义元素的类名
   - id属性：用于指定元素的唯一id，该属性的值在整个html文档中具有唯一性
   - style属性：用于指定元素的行内样式，使用该属性后将会覆盖任何全局的样式设定
   - title属性：用于指定元素的额外信息
   - accesskey属性：用于指定激活元素的快捷键
   - tabindex属性：用于指定元素在tab键下的次序
   - dir属性：用于指定元素中内容的文本方向，属性只有`ltr`或`rtl`两种
   - lang属性：用于指定元素内容的语言
### 3. 事件属性
   - (1) window窗口事件，onload，在网页加载结束之后触发，onunload，在用户从网页离开时发生（点击跳转，页面重载，关闭浏览器窗口等）
   - (2) form表单事件，onblur，当元素失去焦点时触发，onchange，在元素的值被改变时触发，onfocus，当元素获得焦点时触发，onreset，当表单中的重置按钮被点击时触发，onselect，在元素中文本被选中后触发，onsubmit，在提交表单时触发
   - (3) keyboard键盘事件，onkeydown，在用户按下按键时触发，onkeypress，在用户按下按键后，按着按键时触发。该属性不会对所有按键生效，不生效的有，alt,ctrl,shift,esc
   - (4) mouse鼠标事件，onclick，当在元素上发生鼠标点击时触发，onblclick，当在元素上发生鼠标双击时触发，onmousedown，当元素上按下鼠标按钮时触发，onmousemove，当鼠标指针移动到元素上时触发，onmouseout，当元素指针移出元素时触发，onmouseup，当元素上释放鼠标按钮时触发。Media媒体事件，onabort，当退出时触发，onwaiting，当媒体已停止播放但打算继续播放时触发。
### 4. 文本标签
   - (1) 段落标签 `<p></p>`，段落标签用来描述一段文字
   - (2) 标题标签 `<hx></hx>`，标题标签用来描述一个标题，标题标签总共有六个`<h1>~<h6>`级别，`<h1></h1>`标签在每个页面中通常只出现一次
   - (3) 强调语句标签， `<em></em>`，用于强调某些文字的重要性
   - (4) 更加强调标签， `<strong></strong>` 和 `<em>` 标签一样，用于强调文本，但它强调的程度更强一些
   - (5) 无语义标签 `<span></span>` ，标签是没有语义的
   - (6) 短文本引用标签 `<q></q>` ，简短文字的引用
   - (7) 长文本引用标签 `<blockquote></blockquote>` ，定义长的文本引用
   - (8) 换行标签`<br/>`
### 5. 多媒体标签
   - (1) 链接标签: `<a></a>`
   - (2) 图片标签: `<img/>`
   - (3) 视频标签: `<video></video>`
   - (4) 音频标签: `<audio></audio>`
### 6. 列表
   - (1) 无序列表标签，ul,li, `<ul></ul>` 列表定义一个无序列表，`<li></li>` 代表无需列表中的每一个元素
   - (2) 有序列表，ol,li
   - (3) 定义列表， `<dl></dl>`，定义列表通常和 `<dt></dt>` 和 `<dd></dd>` 标签一起使用
### 7. 表格
   - (1) 表格标签 `<table></table>`
   - (2) 表格的一行 `<tr></tr>`
   - (3) 表格的表头 `<th></th>`
   - (4) 单元格 `<td></td>`
   - (5) 表格合并，同一行内，合并几列 colspan="2" ，同一列内，合并几行 rowspan="3"
### 8. 表单标签
   - (1) 表单标签 `<from>`
     - `<form></form>` 表单是可以把浏览者输入的数据传送到服务器端，这样服务器端程序就可以处理表单传过来的数据。
     - `<formmethod="传送方式"action="服务器文件">` 
     - action,浏览者输入的数据被传送到的地方method，数据传送的方式
   - (2) 输入标签<input/>
     - name：为文本框命名，用于提交表单，后台接收数据用。
     - value：为文本输入框设置默认值。
     - type：通过定义不同的type类型，input的功能有所不同。
        - text单行文本输入框
        - password密码输入框（密码显示为***)
        - radio单选框（checked属性用于显示选中状态）
        - checkbox复选框（checked属性用于显示选中状态）
        - file上传文件
        - button普通按钮
        - reset重置按钮（点击按钮，会触发form表单的reset事件）
        - submit提交按钮（点击按钮，会触发form表单的submit事件）
        - email专门用于输入e-mail
        - url专门用于输入url
        - number专门用于number
        - range显示为滑动条，用于输入一定范围内的值
        - date选取日期和时间（还包含：month、week、time、datetime、datetime-local）
        - color选取颜色
     - button按钮，下拉选择框 `<select></select>`
        - `<optionvalue="提交值">` 选项 `</option>` 是下拉选择框里面的每一个选项
   - (3)文本域：`<textarea></textarea>`，当用户想输入大量文字的时候，使用文本域。cols，多行输入域的列数，rows，多行输入域的行数。
### 9. 其他语义化标签
   - (1)盒子`<div></div>`
   - (2) 网页头部 `<header></header>` ，html5新增语义化标签，定义网页的头部，主要用于布局，分割页面的结构
   - (3) 底部信息` <footer></footer>`，html5新增语义化标签，定义网页的底部，主要用于布局，分割页面的结构
   - (4) 导航 `<nav></nav>` ，html5新增语义化标签，定义一个导航，主要用于布局，分割页面的结构
   - (5) 文章 `<article></article>` ，html5新增语义化标签，定义一篇文章，主要用于布局，分割页面的结构
   - (6) 侧边栏 `<aside></aside>` ，语义化标签，定义主题内容外的信息，主要用于布局，分割页面的结构。
   - (7) 时间标签 `<time></time>` ，语义化标签，定义一个时间。

### 10. 网页结构

  - (1) `<!DOCTYPE html>`定义文档类型，告知浏览器用哪一种标准解释HTML
  - (2) `<html></html>` 可告知浏览器其自身是一个HTML文档
  - (3) `<head></head>` 标签用于定义文档的头部，它是所有头部元素的容器
  - (4) `<title></title>` 元素可定义文档的标题
  - (5) `<link>` 标签将css样式文件链接到HTML文件内
  - (6) `<meta>` 定义文档的元数据
  - (7) `<body></body>` 标签之间的内容是网页的主要内容
### 11. 模块划分
  - (1) 常见的企业网站，多由头部区，展示图片区域，主题区域，底部信息区域组成
  - (2) 网页拆分原则:–由上到下-由内到外
### 12. CSS代码语法
  - (1) CSS全称为层叠样式表(CascadingStyleSheets)，它主要是用于定义HTML内容在浏览器内的显示样式，如文字大小、颜色、字体加粗等。
  - (2) css代码通常存放在 `<style></style>` 标签内
  - (3) css样式由选择符和声明组成，而声明又由属性和值组成
  - (4) 选择符{属性:值}
  - (5) 选择符：又称选择器，指明网页中要应用样式规则的元素
### 13. CSS放置位置
  - (1) 行内样式，不建议使用
  - (2) 内联式样式表
  - (3) 外联样式表
### 14. CSS的继承
  - (1) CSS的某些样式是具有继承性的，继承是一种规则，它允许样式不仅应用于某个特定html标签元素，而且应用于其后代。
  - (2) 不可继承样式：display、margin、border、padding、background、height、min-height、max-height、width、min-width、max-width、overflow、position、left、right、top、bottom、z-index、float、clear
  - (3) 可以继承的样式：letter-spacing、word-spacing、white-space、
line-height、color、font、font-family、font-size、font-style、font-variant、font-weight、text-decoration、text-transform、direction、visibility、cursor
### 15. 选择器的种类
  - (1) 标签选择器:通过标签的名字，修改css样式
  - (2) 通配符选择器:选择页面中所有的元素
  - (3) 属性选择器
  - (4) 后代选择器:选择某个父元素下面所有的元素
  - (5) 一级子元素选则器:选择某个父元素的直接子元素，后代选择器是选择父元素的所有子孙元素，一级子元素原则器只选择第一级子元素，不会再向下查找元素
  - (6) id选择器：通过id查找页面中唯一的标签
  - (7) class选择器:通过特定的class（类）来查找页面中对应的标签，以.class名称
  - (8) 伪类选择器:
    - :hover鼠标移入某个元素;
    - :before在某个元素的前面插入内容;
    - :after在某个元素的后面插入内容
  - (9)群组选择器:可以对多个不同的选择器设置相同的样式
### 16. 选择器的优先级
  - (1) 当有不同的选择器对同一个对象进行样式指定时，并且两个选择器有相同的属性被赋予不同的值时。
  - (2) 通过测算那个选择器的权重值最高，应用哪一个选择器的样
  - (3) 权重计算方式:
  - 标签选择器：1
  - class选择器：10
  - id选择器：100
  - 行内样式：1000
  - `!important` 最高级别，提高样式权重，拥有最高级别
### 17. 背景样式
  - (1) 背景颜色 `background-color`
  - (2) 背景图片 `background-image`
    -  `background-image: url(bg01.jpg)`
  - (3) 背景图片位置 `background-position`
    -  `background-position: 10px100px` //代表坐标x，y轴
  - (4) 背景图片重复 `background-repeat`
    -  `background-repeat: no-repeat` //no-repeat设置图像不重复，常用 //round自动缩放直到适应并填充满整个容器 //space以相同的间距平铺且填充满整个容器
  - (5) 背景图片定位 `background-attachment`
    -  `background-attachment: fixed` //背景图像是否固定或者随着页面的其余部分滚动 //background-attachment 的值可以是 scroll（跟随滚动），fixed（固定）
  - (6) background缩写
    -  `background: #ff0000url(bg01.jpg)no-repeatfixedcenter`
### 18. 字体样式
  - (1) 字体族 font-family
    - font-family:"微软雅黑","黑体";
  - (2) 字体大小 font-size
    - font-size: 12px;网页默认字体大小是16px
  - (3)字体粗细 font-weight
    - font-weight: 400;
      - normal（默认）
      - bold（加粗）
      - bolder（相当于 `<strong>` 和 `<b>` 标签）
      - lighter（常规）
      - 100~900整百（400=normal，700=bold）
  - (4) 字体颜色color
    - 颜色的英文单词color: red;
    - 十六进制色：color: #FFFF00;
    - RGB(红绿蓝) color: rgb(255,255,0)
    - RGBA（红绿蓝透明度）A是透明度在0~1之间取值。color: rgba(255,255,0,0.5)
  - (5)字体斜体font-style
    - font-style: italic
### 19. 文本属性
  - (1) 行高 line-height 
    - line-height: 50px; 可以将父元素的高度撑起来
  - (2) 文本水平对齐方式text-align
    - left 左对齐
    - center 文字居中
    - right 右对齐
  - (3) 文本所在行高的垂直对齐方式 vertical-align
    - baseline 默认
    - sub 垂直对齐文本的下标，和 `<sub>` 标签一样的效果
    - super 垂直对齐文本的上标，和 `<sup>` 标签一样的效果
    - top 对象的顶端与所在容器的顶端对齐
    - text-top 对象的顶端与所在行文字顶端对齐
    - middle 元素对象基于基线垂直对齐
    - bottom 对象的底端与所在行的文字底部对齐
    - text-bottom 对象的底端与所在行文字的底端对齐
  - (4) 文本缩进text-indent
    - text-indent: 2em; 通常用在段落开始位置的首行缩进
  - (5) 字母之间的间距letter-spacing
  - (6)单词之间间距word-spacing
  - (7)文本的大小写text-transform
    - capitalize 文本中的每个单词以大写字母开头
    - uppercase 定义仅有大写字母
    - lowercase 定义仅有小写字母
  - (8) 文本的装饰 text-decoration
    - none 默认
    - underline 下划线
    - overline 上划线 
    - line-through 中线
  - (9) 自动换行 word-wrap
      - word-wrap: break-word;
### 20. 基本样式
  - (1) 宽度 width
    - width: 200px; 定义元素的宽度
  - (2) 高度 height
    - height: 300px; 元素默认没有高度,需要设置高度,可以不定义高度，让元素的内容将元素撑高
  - (3) 鼠标样式 cursor
    - 定义鼠标的样式 cursor: pointer
      - default 默认
      - pointer 小手形状 // 常用
      - move 移动形状
