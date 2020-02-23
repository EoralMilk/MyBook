# Markdown基础教程
### <p align="right">————**EoralMilk**： 2020, 2, 23</p>

## **简介：**
- Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档。

- Markdown 语言在 2004 由约翰·格鲁伯（英语：John Gruber）创建。

- Markdown 编写的文档可以导出 HTML 、Word、图像、PDF、Epub 等多种格式的文档。

- Markdown 编写的文档后缀为 .md, .markdown。 

- Markdown 能被使用来撰写电子书，如：Gitbook。

- 当前许多网站都广泛使用 Markdown 来撰写帮助文档或是用于论坛上发表消息。例如：GitHub、简书、reddit、Diaspora、Stack Exchange、OpenStreetMap 、SourceForge等。
  
- 咱个人使用的编辑器是<abbr title="Visual Studio Code">vscode</abbr>可以写代码的同时观察到实现效果，除此之外还有很多其他编辑器，例如Typora，gitbook editor等等。  

## **目录：**
> [1. 标题与分割线](#1)  
> [2. 字体与换行：](#2)  
> [3. 列表：](#3)  
> [4. 区块：](#4)  
> [5. 代码：](#5)  
> [6. 链接：](#6)  
> [7. 图片：](#7)  
> [8. 表格：](#8)  

------
## <div id="1">1. 标题与分割线：</div>
###  **样例：**
# 大标题
## 次级标题
### 次次级标题
---
- - -
******
### **代码：**

```markdown
# 大标题
## 次级标题
### 次次级标题
---
- - -
******
<!-- 你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线： -->
```
## <div id="2">2. 字体与换行：</div>
### **样例：**
第1行  
第2行  
第3行

*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___  
\*\* 正常显示星号 \*\*
### **代码：**
```markdown
第1行  
第2行  
第3行
<!-- 第1行和第2行后面都有2个空格，表示换行 -->
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___ 
\*\* 正常显示星号 \*\*

<!-- 
可以转义的字符：
\   反斜线
`   反引号
*   星号
_   下划线
{}  花括号
[]  方括号
()  小括号
#   井字号
+   加号
-   减号
.   英文句点
!   感叹号

 -->
```
### **其他样式：**
GOOGLE.COM  
~~BAIDU.COM~~  
<u>用html标签生成带下划线文本</u>  

使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑  

某些时候是不支持md脚注的[^jz]，这时的脚注经常会被认为是链接  

但是可以用html标签实现<sup>这种脚注可以实现</sup>  

还有就是标记一个缩写：The <abbr title="People's Republic of China">PRC</abbr> was founded in 1949.  

<bdo dir="rtl">也可以让某段落文字从右到左显示。</bdo>  

### **代码：**
```markdown
<!-- 删除线效果 -->
~~BAIDU.COM~~  

<u>用html标签生成带下划线文本</u>  

<!-- 按键效果 -->
使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑  

<!-- 脚注 -->
某些时候是不支持脚注的[^jz]，这时的脚注经常会被认为是链接  

但是可以用html标签实现<sup>这种脚注可以实现</sup>  

<!-- 缩写 -->
- 标记一个缩写：The <abbr title="People's Republic of China">PRC</abbr> was founded in 1949.
<bdo dir="ltr/rtl">内容</bdo>

<!-- 显示方向 -->
- <bdo dir="rtl">该段落文字从右到左显示。</bdo>   

<!-- 
<bdo>标签中文本内容的方向由“dir”属性规定；
“dir”属性值可以是ltr和rtl，分别代表不同的方向；
“ltr”是英文“left to right”的缩写，即“从左到右”；
“rtl”是英文“right to left”的缩写，即“从右到左” 
-->

```


## <div id="3">3. 列表：</div>
### **样例：**
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项

- 第一项
- 第二项
- 第三项

1. 第一项
2. 第二项
3. 第三项

1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素

### **代码：**
```markdown
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项

- 第一项
- 第二项
- 第三项

1. 第一项
2. 第二项
3. 第三项

1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
```

## <div id="4">4. 区块：</div>
### **样例：**
> 区块引用  
> 第二行 
> 继续第二行

> 最外层
> > 第一层嵌套
> > > 第二层嵌套

> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> * 第二项
> - 第三项
### **代码：**
```markdown
> 区块引用  
> 第二行 
> 继续第二行

> 最外层
> > 第一层嵌套
> > > 第二层嵌套

> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> * 第二项
> - 第三项
```
## <div id="5">5. 插入代码：</div>
### **样例：**  

这个`print('输出')`是用于输出的代码
<!-- 这行是注释 -->
#### 在代码前加上制表符<kbd>Tab</kbd>即可构建代码块

    import something
    def func(x):
        pass
#### 下面是指定所使用的语言的代码块，结构请看下方代码讲解部分
```python
import something
def func(x):
   pass
```     
### **代码：**
```markdown
这个`print('输出')`是用于输出的代码
<!-- 这行是注释 -->
"-->|"代表Tab键，第二种使用时前面没有"> " 

-->|import something
-->|def func(x):
-->|    pass

这里也可以不指定语言
> ```python
> import something
> def func(x):
>     pass
> ```  
```
## <div id="6">6. 链接：</div>
### **样例：**  
[GitHublink](www.github.com)  
<www.github.com>  
[GoToGitHub]  
[Google][1]  
<a href="https://github.com/EoralMilk/HelloOpenCV/blob/master/skly1.jpg">这是一个链接</a>  

### **代码：**
```markdown
[GitHublink](www.github.com)  
<www.github.com>
[GoToGitHub]

使用方法：
[链接名称](链接地址)
或者
<链接地址>

链接也可以用变量来代替，文档末尾附带变量地址：
这个链接用 1 作为网址变量 [Google][1]
这个链接用自己作为网址变量 [GoToGitHub]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [GoToGitHub]: http://www.github.com/

html的链接写法也可以在md中使用：
<a href="https://github.com/EoralMilk/HelloOpenCV/blob/master/skly1.jpg">这是一个链接</a>
```  

## <div id="7">7. 图片：</div>  

```markdown
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")
```
- 开头一个感叹号 !
- 接着一个方括号，里面放上图片的替代文字
- 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。

### **样例：**  

![picture1](https://github.com/EoralMilk/HelloOpenCV/blob/master/skly1.jpg?raw=true "噗！")
#### 图片同样也可以作为可点击的链接
[![picture1](https://github.com/EoralMilk/HelloOpenCV/blob/master/skly1.jpg?raw=true "噗！")](https://github.com/EoralMilk/HelloOpenCV/blob/master/skly1.jpg)  
#### 缩小50%等操作需要使用html语法来达成
[<img src="https://github.com/EoralMilk/HelloOpenCV/blob/master/skly1.jpg?raw=true" width="50%">](https://github.com/EoralMilk/HelloOpenCV/blob/master/skly1.jpg)


## <div id = "8">8. 表格：</div>
#### Markdown 制作表格使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。

**语法格式如下：**

    |  表头   | 表头  |
    |  ----  | ----  |
    | 单元格  | 单元格 |
    | 单元格  | 单元格 |  
**效果：**
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |  

---
#### 对齐方式：
我们可以设置表格的对齐方式： 

    -: 设置内容和标题栏居右对齐。
    :- 设置内容和标题栏居左对齐。
    :-: 设置内容和标题栏居中对齐


**效果：**

| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单——元——格 | 单——元——格 | 单——元——格 |
| 单元格 | 单元格 | 单元格 |

#### **代码：**
```markdown
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单——元——格 | 单——元——格 | 单——元——格 |
| 单元格 | 单元格 | 单元格 |
```

-----------------------------------------------

<!-- 变量声明 -->
[GoToGitHub]: http://www.github.com/
[^jz]: 注释文本