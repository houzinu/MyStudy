#### Web标准

Web标准包括结构、表现、行为。

# 表格标签



> 表格标签

1. “<table></table>”用于定义表格的标签。
2. <tr></tr>行标签
3. <td></td>单元格标签
4. <th></th>表头单元格---经常位于第一行

> 合并单元格

1.跨行单元格：rowspan="合并单元格的个数"

2.跨列单元格：colspan="合并单元格的个数"

# 列表标签

###### 无序列表

<table>
  <ul>
    <li>榴莲</li>
    <li>菠萝</li>
    <li>西瓜</li>
  </ul>
</table>

==ul里边只能放li标签==

###### 有序列表

<table>
  <ol>
   	<li>表项1</li>
    <li>表项2</li>
    <li>表项3</li>
  </ol>
</table>

==ol里边只能放li标签==

###### 自定义列表

<table>
  <dl>
    <dt>小米售后</dt>
    <dd>新浪微博</dd>
    <dd>官方微信</dd>
    <dd>联系我们</dd>
  </dl>
</table>

==<dt>和<dd>是并列（兄弟关系）。==

# 表单标签

> 使用表单目的是为了手机用户信息。

表单由表单域、表单控件和提示信息三部分构成。

<form>
  action = "demo.php" method="POST" name="name1
</form>

#### 表单控件

1.<input>表单元素

<input type="属性值">

<form>
  username<input type='text' value="输入用户名"> <br>
  password<input type="password">
</form>

radio是单选按钮

<form>
  性别：男<input type="radio" name="sex" checked="checked">
  		 女<input type="radio" name="sex"> 
</form>

checkbox是多选按钮

<form>
  吃饭：<input type="checkbox" name="hobby">
  睡觉：<input type="checkbox" name="hobby">
</form>

==radio和checkbox按钮要有相同的*name*值才能实现多选一或者多选多。==



<form>
  <input type="submit" value="免费注册">
</form>

<form>
  <input type="reset" value="重置按钮">
</form>

<form>
  <input type="button" value="按钮">
</form>

<form>
  <input type="file" value="下载文件">
</form>

#### 表单标签

<form>
  <label for="text">用户名：</label>
  <input type="text" id="text">
</form>

#### 下拉表单标签

<form>
  <select>
    <option>云南人</option>
    <option>河北人</option>
    <option>湖北人</option>
    <option>北京人</option>
  </select>
</form>

==<select>里边至少包含一对<option>==

==在<option>中定义 selected="selected"时，是默认会选中的选项。==

> 文本域标签

<form>
  今日反馈：
  <textarea cols="50" rows="5">欢迎写反馈</textarea>
</form>





