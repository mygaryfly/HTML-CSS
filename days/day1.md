### HTML的结构 和标签

#### **一，HTML的结构**
> 
```html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>菜鸟教程(runoob.com)</title>
</head>
<body>
 
<h1>我的第一个标题</h1>
 
<p>我的第一个段落。</p>
 
</body>
</html>
```
##### **实例解析**
* <!DOCTYPE html> 声明为 HTML5 文档
* <html> 元素是 HTML 页面的根元素
* <head> 元素包含了文档的元（meta）数据，如 <meta charset="utf-8"> 定义网页编码格式为 utf-8。
* <title> 元素描述了文档的标题
* <body> 元素包含了可见的页面内容
* <h1> 元素定义一个大标题
* <p> 元素定义一个段落

#### **二，标签**

1. 标题标签
> HTML 标题（Heading）是通过<h1> - <h6> 标签来定义的
```html
<h1>这是一个标题</h1>
<h2>这是一个标题</h2>
<h3>这是一个标题</h3>
```

2. 段落标签
> HTML 段落是通过标签 <p> 来定义的。
```html
<p>这是一个段落。</p>
<p>这是另外一个段落。</p>
```
3. 图像标签
> HTML 图像是通过标签 <img> 来定义的
`<img src="/images/logo.png" width="258" height="39" />`

4. 链接标签
> HTML 链接由 <a> 标签定义。链接的地址在 href 属性中指定：
`<a href="http://www.mygaryfly.com">这是一个链接</a>

