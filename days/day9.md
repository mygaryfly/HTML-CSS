### Alignment - 对齐
***

#### **一， text-align**
定义和用法:
text-align 属性规定元素中的文本的水平对齐方式。
该属性通过指定行框与哪个点对齐，从而设置块级元素内文本的水平对齐方式。通过允许用户代理调整行内容中字母和字之间的间隔，可以支持值 justify；不同用户代理可能会得到不同的结果。

* 如果 direction 属性是 ltr，则默认值是 left；如果 direction 是 rtl，则为 right。
* 继承性: YES
* JavaScript 语法：	`object.style.textAlign="right"`

<table>
    <tr style="background: black;">
        <th>值</th>
        <th>描述</th>      
    </tr>
    <tr>
        <td style="text-align:center;">left</td>
        <td>把文本排列到左边。默认值：由浏览器决定。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">right</td>
        <td>把文本排列到右边</td>        
    </tr>
    <tr>
        <td style="text-align:center;">center</td>
        <td>把文本排列到中间。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">justify</td>
        <td>实现两端对齐文本效果。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">inherit</td>
        <td>规定应该从父元素继承 text-align 属性的值</td>        
    </tr>
</table>

<br>
关于justify: 最后一个水平对齐属性是 justify，它会带来自己的一些问题。

值 justify 可以使文本的两端都对齐。在两端对齐文本中，文本行的左右两端都放在父元素的内边界上。然后，调整单词和字母间的间隔，使各行的长度恰好相等。您也许已经注意到了，两端对齐文本在打印领域很常见。不过在 CSS 中，还需要多做些考虑。

要由用户代理（而不是 CSS）来确定两端对齐文本如何拉伸，以填满父元素左右边界之间的空间。例如，有些浏览器可能只在单词之间增加额外的空间，而另外一些浏览器可能会平均分布字母间的额外空间（不过 CSS 规范特别指出，如果 letter-spacing 属性指定为一个长度值，“用户代理不能进一步增加或减少字符间的空间”）。还有一些用户代理可能会减少某些行的空间，使文本挤得更紧密。所有这些做法都会影响元素的外观，甚至改变其高度，这取决于用户代理的对齐选择影响了多少文本行。

CSS 也没有指定应当如何处理连字符（注1）。大多数两端对齐文本都使用连字符将长单词分开放在两行上，从而缩小单词之间的间隔，改善文本行的外观。不过，由于 CSS 没有定义连字符行为，用户代理不太可能自动加连字符。因此，在 CSS 中，两端对齐文本看上去没有打印出来好看，特别是元素可能太窄，以至于每行只能放下几个单词。当然，使用窄设计元素是可以的，不过要当心相应的缺点。

<br>

#### **二，vertical-align**
定义和用法：
vertical-align 属性设置元素的垂直对齐方式。

该属性定义行内元素的基线相对于该元素所在行的基线的垂直对齐。允许指定负长度值和百分比值。这会使元素降低而不是升高。在表单元格中，这个属性会设置单元格框中的单元格内容的对齐方式。
* 默认值：baseline
* 继承性：NO
* JavaScript 语法：	`object.style.verticalAlign="bottom"`

<table>
    <tr style="background: black;">
        <th>值</th>
        <th>默认。元素放置在父元素的基线上。</th>        
    </tr>
    <tr>
        <td style="text-align:center;">sub</td>
        <td>把文本排列到左边。默认值：由浏览器决定。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">right</td>
        <td>垂直对齐文本的下标。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">super</td>
        <td>垂直对齐文本的上标.</td>        
    </tr>
    <tr>
        <td style="text-align:center;">top</td>
        <td>把元素的顶端与行中最高元素的顶端对齐。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">text-top</td>
        <td>把元素的顶端与父元素字体的顶端对齐。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">middle</td>
        <td>把此元素放置在父元素的中部。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">bottom</td>
        <td>把元素的顶端与行中最低的元素的顶端对齐。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">text-bottom	</td>
        <td>把元素的底端与父元素字体的底端对齐。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">length</td>
        <td>升高（正值）或降低（负值）子元素盒子。值为升高/降低的距离，如果为0，和vertical-align:baseline一样。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">%</td>
        <td>使用 "line-height" 属性的百分比值来排列此元素。允许使用负值。</td>        
    </tr>
    <tr>
        <td style="text-align:center;">inherit</td>
        <td>规定应该从父元素继承 text-align 属性的值</td>        
    </tr>
</table>
<br>

![vertical-align](./images/vertical-align.png)