#### **HTML表单**
<br>

##### **一，表单的定义**

* 表单是一个包含表单元素的区域
* 表单元素是允许用户在表单中输入内容,比如：文本域(textarea)、下拉列表、单选框(radio-buttons)、复选框(checkboxes)等等。
* 表单使用表单标签 <form> 来设置:
```html
<form>
.
input 元素
.
</form>
```

#### **二，表单的输入元素**
* 多数情况下被用到的表单标签是输入标签（`<input>`）。
* 输入类型是由类型属性（type）定义的。

> **1)** 文本域（Text Fields）
文本域通过`<input type="text">` 标签来设定，当用户要在表单中键入字母、数字等内容时，就会用到文本域。
eg:
```html 
<form>
First name: <input type="text" name="firstname"><br>
Last name: <input type="text" name="lastname">
</form>
```
浏览器显示如下:
<form>
First name: <input type="text" name="firstname"><br>
Last name: <input type="text" name="lastname">
</form>
<br>
<br>

> **2)** 密码字段

密码字段通过标签`<input type="password">` 来定义:
eg:
```html
<form>
Password: <input type="password" name="pwd">
</form>
```
浏览器显示如下:
<form>
Password: <input type="password" name="pwd">
</form>
<br>

> **3）** 单选按钮（Radio Buttons）

`<input type="radio">` 标签定义了表单单选框选项
eg:
```html
<form>
<input type="radio" name="sex" value="male">Male<br>
<input type="radio" name="sex" value="female">Female
</form>
```
浏览器显示如下:
<form>
<input type="radio" name="sex" value="male">Male<br>
<input type="radio" name="sex" value="female">Female
</form>
<br>

> **4）** 复选框（Checkboxes）

`<input type="checkbox">` 定义了复选框. 用户需要从若干给定的选择中选取一个或若干选项。
eg:
```html
<form>
<input type="checkbox" name="vehicle" value="Bike">I have a bike<br>
<input type="checkbox" name="vehicle" value="Car">I have a car 
</form>
```
浏览器显示效果如下:
<form>
<input type="checkbox" name="vehicle" value="Bike">I have a bike<br>
<input type="checkbox" name="vehicle" value="Car">I have a car 
</form>
<br>

> **5）** 提交按钮(Submit Button)

`<input type="submit">` 定义了提交按钮.

当用户单击确认按钮时，表单的内容会被传送到另一个文件。表单的动作属性定义了目的文件的文件名。由动作属性定义的这个文件通常会对接收到的输入数据进行相关的处理。:
```html
<form name="input" action="html_form_action.php" method="get">
Username: <input type="text" name="user">
<input type="submit" value="Submit">
</form>
```
浏览器显示效果如下:
<form name="input" action="html_form_action.php" method="get">
Username: <input type="text" name="user">
<input type="submit" value="Submit">
</form>
<br>

> **6）** 下拉列表（Select）

`<select>` 元素是一种表单控件，可用于在表单中接受用户输入。

`<select>` 元素用来创建下拉列表。
eg:
```html
<form action="">
<select name="cars"> <!-- `<select>` 元素中的`<option>` 标签定义了列表中的可用选项。-->
<option value="volvo">Volvo</option>
<option value="saab">Saab</option>
<option value="fiat">Fiat</option>
<option value="audi">Audi</option>
</select>
</form>
```
浏览器显示效果如下:
<form action="">
<select name="cars">
<option value="volvo">Volvo</option>
<option value="saab">Saab</option>
<option value="fiat">Fiat</option>
<option value="audi">Audi</option>
</select>
</form>
<br>

##### **三，属性**

<table border="1">
    <tr>
        <th style="background:black;">属性</th>
        <th style="background:black;">值</th>
        <th style="background:black;">描述</th>
    </tr>
    <tr>
        <td style="text-decoration:underline;color:darkgreen;">autofocus</td>
        <td>autofocus</td>
        <td>规定在页面加载时下拉列表自动获得焦点。</td>
    </tr>
    <tr>
        <td style="text-decoration:underline;color:darkgreen;">disabled</td>
        <td>disabled</td>
        <td>当该属性为 true 时，会禁用下拉列表</td>
    </tr>
    <tr>
        <td style="text-decoration:underline;color:darkgreen;">form</td>
        <td>form_id</td>
        <td>定义 select 字段所属的一个或多个表单</td>
    </tr>
    <tr>
        <td style="text-decoration:underline;color:darkgreen;">multiple</td>
        <td>multiple</td>
        <td>当该属性为 true 时，可选择多个选项。</td>
    </tr>
    <tr>
        <td style="text-decoration:underline;color:darkgreen;">name</td>
        <td>text</td>
        <td>定义下拉列表的名称。</td>
    </tr>
    <tr>
        <td style="text-decoration:underline;color:darkgreen;">required</td>
        <td>required</td>
        <td>规定用户在提交表单前必须选择一个下拉列表中的选项。</td>
    </tr>
    <tr>
        <td style="text-decoration:underline;color:darkgreen;">size</td>
        <td>number</td>
        <td>规定下拉列表中可见选项的数目。</td>
    </tr>                        
</table>