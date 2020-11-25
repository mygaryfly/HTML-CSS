#### **CSS3 弹性盒子(Flex Box)**

[**flex快速通道**](https://www.zhangxinxu.com/wordpress/2018/10/display-flex-css3-css/) —— 来自张鑫旭

#### **一，定义**
弹性盒子是 CSS3 的一种新的布局模式。

CSS3 弹性盒（ Flexible Box 或 flexbox），是一种当页面需要适应不同的屏幕大小以及设备类型时确保元素拥有恰当的行为的布局方式。

引入弹性盒布局模型的目的是提供一种更加有效的方式来对一个容器中的子元素进行排列、对齐和分配空白空间。

* 弹性盒子由弹性容器(Flex container)和弹性子元素(Flex item)组成。

* 弹性容器通过设置 display 属性的值为 flex 或 inline-flex将其定义为弹性容器。

* 弹性容器内包含了一个或多个弹性子元素。

<br>

#### **二，flex的属性**

##### **2.1 - 作用在flex容器上的属性**

##### **2.1-1 - flex-direction**
语法：`flex-direction: row | row-reverse | column | column-reverse`

flex-direction的值有:

* row：横向从左到右排列（左对齐），默认的排列方式。
* row-reverse：反转横向排列（右对齐，从后往前排，最后一项排在最前面。
* column：纵向排列。
* column-reverse：反转纵向排列，从后往前排，最后一项排在最上面。

##### **2.1-2 - justify-content**
语法：`justify-content: flex-start | flex-end | center | space-between | space-around
`

* flex-start：
弹性项目向行头紧挨着填充。这个是默认值。第一个弹性项的main-start外边距边线被放置在该行的main-start边线，而后续弹性项依次平齐摆放。

* flex-end：
弹性项目向行尾紧挨着填充。第一个弹性项的main-end外边距边线被放置在该行的main-end边线，而后续弹性项依次平齐摆放。

* center：
弹性项目居中紧挨着填充。（如果剩余的自由空间是负的，则弹性项目将在两个方向上同时溢出）。

* space-between：
弹性项目平均分布在该行上。如果剩余空间为负或者只有一个弹性项，则该值等同于flex-start。否则，第1个弹性项的外边距和行的main-start边线对齐，而最后1个弹性项的外边距和行的main-end边线对齐，然后剩余的弹性项分布在该行上，相邻项目的间隔相等。

* space-around：
弹性项目平均分布在该行上，两边留有一半的间隔空间。如果剩余空间为负或者只有一个弹性项，则该值等同于center。否则，弹性项目沿该行分布，且彼此间隔相等（比如是20px），同时首尾两边和弹性容器之间留有一半的间隔（1/2*20px=10px）。

![](./images/justify-content.png)
 