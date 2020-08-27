#### **SVG标签**


#### 一，SVG标签基础

##### 1.1 简介
* SVG 意为可缩放矢量图形（Scalable Vector Graphics）。
* SVG 使用 XML 格式定义图像，它是使用 XML 来描述二维图形和绘图程序的语言。
* SVG 图像在放大或改变尺寸的情况下其图形质量不会有所损失
* SVG 是万维网联盟的标准
* SVG 与诸如 DOM 和 XSL 之类的 W3C 标准是一个整体

##### 1.2 SVG的优势
* SVG 可被非常多的工具读取和修改（比如记事本）
* SVG 与 JPEG 和 GIF 图像比起来，尺寸更小，且可压缩性更强
* SVG 是可伸缩的
* SVG 图像可在任何的分辨率下被高质量地打印
* SVG 可在图像质量不下降的情况下被放大
* SVG 图像中的文本是可选的，同时也是可搜索的（很适合制作地图）
* SVG 可以与 Java 技术一起运行
* SVG 是开放的标准
* SVG 文件是纯粹的 XML

##### 1.3 SVG在HTML的使用
* SVG 文件可通过以下标签嵌入 HTML 文档：`<embed>`、`<object>` 或者` <iframe>`
* SVG的代码可以直接嵌入到HTML页面中，或您可以直接链接到SVG文件

>eg:
```html
<svg xmlns="http://www.w3.org/2000/svg" version="1.1">
   <circle cx="100" cy="50" r="40" stroke="black" stroke-width="2" fill="red" />
</svg>
```
* 可以用`<a>`标签链接到一个SVG文件
>eg:
`<a href="circle1.svg">View SVG file</a>`


