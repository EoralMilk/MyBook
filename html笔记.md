
# HTML笔记
###  <p align="right">————EoralMilk： 2020, 1, 21</p>

<br/>
<br/>

## **一个简单的html实例：**

---
<!-- 一个简单的html实例。-->

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>菜鸟教程(runoob.com)</title>
    </head>
    <body bgcolor="AliceBlue">
        <h1>我的第一个标题</h1>
        <p>我的第一个段落。</p>
        <hr>
        <br/>
        <p><a href=https://www.runoob.com/html/html-formatting.html">点击<br/>链接了解更多标签
        </a></p>
        <p>
        <img src="lily_white_cat.jpg" width="153" height="240" />
        <br/>
        <b>加粗文本</b><br><br>
        <i>斜体文本</i><br><br>
        <code>电脑自动输出</code><br><br>
        这是 <sub> 下标</sub> 和 <sup> 上标</sup>
        </p>
    </body>
</html>

<br/>
<br/>
<br/>
<br/>

```html
实例解析：
<!DOCTYPE html> 声明为 HTML5 文档
<html> 元素是 HTML 页面的根元素
<head> 元素包含了文档的元（meta）数据，如 <meta charset="utf-8"> 定义网页编码格式为 utf-8。
<title> 元素描述了文档的标题
<body> 元素包含了可见的页面内容
<h1> 元素定义一个大标题
<p> 元素定义一个段落
<a href="http://www.bing.com">点击链接</a> 插入一个链接
<img src="lily_white_cat.jpg" width="307" height="480" /> 插入一个图片
<br/> 空元素，会产生换行
<hr> 分割线
<!-- 注释 -->
<!--
    注释
-->
```

---
<br/>
<br/>

# HTML 速查列表  
<br/>
<br/>

## 1. HTML 基本文档：
---

<!DOCTYPE html>
<html>
<head>
<title>文档标题</title>
</head>
<body>
可见文本...
</body>
</html>


<br/>
<br/>
<br/>
<br/>

## 2. 基本标签（Basic Tags）：

---

<h1>最大的标题</h1>
<h2> . . . </h2>
<h3> . . . </h3>
<h4> . . . </h4>
<h5> . . . </h5>
<h6>最小的标题</h6>
 
<p>这是一个段落。</p>
<br> （换行）
<hr> （水平线）
<!-- 这是注释 -->

<br/>
<br/>
<br/>
<br/>

## 3.文本格式化（Formatting）：

---

<b>粗体文本</b>  
<code>计算机代码</code>  
<em>强调文本</em>  
<i>斜体文本</i>  
<kbd>键盘输入</kbd>   
<pre>预格式化文本</pre>  
<small>更小的文本</small>  
<strong>重要的文本</strong>  
<abbr> （缩写） </abbr>  
<address> （联系信息） </address>   
<bdo> （文字方向） </bdo>  
<blockquote> （从另一个源引用的部分） </blockquote>   
<cite> （工作的名称） </cite>      

<del> （删除的文本） </del>  
<ins> （插入的文本） </ins>   
<sub> （下标文本） </sub>   
<sup> （上标文本） </sup>   


<br/>
<br/>
<br/>
<br/>

## 4. 链接（Links）:
---

普通的链接：<a href="http://www.example.com/">链接文本</a>  

图像链接： <a href="http://www.example.com/"><img src="URL" alt="替换文本"></a>  

邮件链接： <a href="mailto:webmaster@example.com">发送e-mail</a>  

<br/>
<br/>
<br/>
<br/>

## 5. 书签：
---

<a id="tips">提示部分</a>
<a href="#tips">跳到提示部分</a>

<br/>
<br/>
<br/>
<br/>

## 6. 图片（Images）:
---

<img src="URL" alt="替换文本" height="42" width="42">  

<br/>
<br/>
<br/>
<br/>
<br/>

## 7. 样式/区块（Styles/Sections）:
---

<style type="text/css">
h1 {color:Black;}
h2 {color:Green;}
p {color:Gray;}

</style>

<div>文档中的块级元素</div>
<span>文档中的内联元素</span>  

### 无序列表:
<ul>
    <li>项目</li>
    <li>项目</li>
</ul>  

### 有序列表:
<ol>
    <li>第一项</li>
    <li>第二项</li>
</ol>

### 定义列表:
<dl>
  <dt>项目 1</dt>
    <dd>描述项目 1</dd>
  <dt>项目 2</dt>
    <dd>描述项目 2</dd>
</dl>
<br/>
<br/>
<br/>
<br/>

## 8. 表格（Tables）:
---
<table border="1">
  <tr>
    <th>表格标题</th>
    <th>表格标题</th>
  </tr>
  <tr>
    <td>表格数据</td>
    <td>表格数据</td>
  </tr>
</table>
<br/>
<br/>
<br/>
<br/>

## 9. 框架（Iframe）:
---

<iframe src="demo_iframe.htm"></iframe>
<br/>
<br/>
<br/>
<br/>

## 10. 表单（Forms）:
---
<form action="demo_form.php" method="post/get">
    <input type="text" name="email" size="40" maxlength="50">
    <input type="password">
    <input type="checkbox" checked="checked">
    <input type="radio" checked="checked">
    <input type="submit" value="Send">
    <input type="reset">
    <input type="hidden">
    <select>
        <option>苹果</option>
        <option selected="selected">香蕉</option>
        <option>樱桃</option>
    </select>
    <textarea name="comment" rows="10" cols="20"></textarea>
</form>
<br/>
<br/>
<br/>
<br/>

## 11. 实体（Entities）:
---
```
&lt; 等同于 <
&gt; 等同于 >
&#169; 等同于 ©
```