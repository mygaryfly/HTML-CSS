#### **HTML表格**

##### **一，定义**
表格由 `<table>` 标签来定义。每个表格均有若干行（由 `<tr>` 标签定义），每行被分割为若干单元格（由 `<td>` 标签定义）。字母 td 指表格数据（table data），即数据单元格的内容。数据单元格可以包含文本、图片、列表、段落、表单、水平线、表格等等。

```html
<table border="1">
    <tr>
        <td>row 1, cell 1</td>
        <td>row 1, cell 2</td>
    </tr>
    <tr>
        <td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
    </tr>
</table>
```
>图例：
<table border="1">
    <tr>
        <td>row 1, cell 1</td>
        <td>row 1, cell 2</td>
    </tr>
    <tr>
        <td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
    </tr>
</table>

##### **二，边框属性**
如果不定义边框属性，表格将不显示边框。有时这很有用，但是大多数时候，我们希望显示边框。

使用边框属性来显示一个带有边框的表格：
```html
<table border="1">
    <tr>
        <td>Row 1, cell 1</td>
        <td>Row 1, cell 2</td>
    </tr>
</table>
```
>图例:
<table border="1">
    <tr>
        <td>Row 1, cell 1</td>
        <td>Row 1, cell 2</td>
    </tr>
</table>

##### **三，表格表头**
表格的表头使用 `<th>` 标签进行定义。

大多数浏览器会把表头显示为粗体居中的文本：
```html
<table border="1">
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>row 1, cell 1</td>
        <td>row 1, cell 2</td>
    </tr>
    <tr>
        <td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
    </tr>
</table>
```
>图例：
<table border="1">
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>row 1, cell 1</td>
        <td>row 1, cell 2</td>
    </tr>
    <tr>
        <td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
    </tr>
</table>


##### **四，表格标签**
<table border="1">
    <tr>
        <th>标签</th>
        <th>描述</th>
    </tr>
    <tr>
        <td>&lt table &gt</td>
        <td>定义表格</td>
    </tr>
    <tr>
        <td>&lt th &gt</td>
        <td>定义表格的表头</td>
    </tr>
    <tr>
        <td>&lt tr &gt</td>
        <td>定义表格的行</td>
    </tr>
    <tr>
        <td>&lt td &gt</td>
        <td>定义表格单元</td>
    </tr>
    <tr>
        <td>&lt caption &gt</td>
        <td>定义表格标题</td>
    </tr>
    <tr>
        <td>&lt colgroup &gt</td>
        <td>定义表格列的组</td>
    </tr>
        <tr>
        <td>&lt col &gt</td>
        <td>定义用于表格列的属性</td>
    </tr>
    <tr>
        <td>&lt thead &gt</td>
        <td>定义表格的页眉</td>
    </tr>
        <tr>
        <td>&lt tbody &gt</td>
        <td>定义表格的主体</td>
    </tr>
    <tr>
        <td>&lt tfoot &gt</td>
        <td>定义表格的页脚</td>
    </tr>    
</table>
