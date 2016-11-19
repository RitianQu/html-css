# html-css
#### 常见标签学习
     p 段落
     h1-h6 标题
     hr 水平线
     br 换行
     font 文本样式
     b/strong 加粗
     i/em 倾斜
     s/del 删除线
     u/ins 下划线
#### img
     <img src="" title="" alt="">
     title 标题
     src 路径
     alt 图片不正常显示时文本提示
#### 创建超链接
      <a href="跳转目标" target="窗口弹出方式">文本或者图像</a>
#### 锚点链接
     创建锚点链接分为两部：
     1 使用”链接文本“创建链接文本
     2 使用相应的id名标注跳转目标的位置
#### 列表
###  无序列表ul
     <ul>
        <li>列表以</li>
        <li>列表二</li>
        <li>列表三</li>
      </ul>
###  有序列表ol
###  定义列表dl
     <dl>
         <dt>名词1</dt>
         <dd>名词1解释1</dd>
         <dd>名词1解释2</dd>
         
         <dt>名词2</dt>
         <dd>名词2解释1</dd>
         <dd>名词2解释2</dd>
      </dl>
#### 表格
     <table>
        <tr>
        <td>单元格内的文字</td>
        ...
        </tr>
        ...
     </table>
#### 标签的属性
     border 设置表格的边框（默认border=”0“无边框） 像素值
     cellspacing 设置单元格与单元格边框之间的空白间距 像素值（默认为2像素）
     cellpadding 设置单元格内容与单元格边框之间的空白间距 像素值
     width 设置表格的宽度 像素值
     height 设置表格的高度 像素值
     align 设置表格在网页中的水平对齐方式 left.center.right
#### caption标签
     caption标签必须紧随table标签之后。您只能对每个表格定义一个标题。通常这个标题回被居中于表格之上
#### th标签
     th替代相应的单元个标记
#### 表单
     <form action="" method=""(get post)>
     <input type="" name="" value="">
     ...
     </form>
     action,属性用于指定接受并处理表单数据的服务器程序的url地址。
     method，属性用于设置表单数据的提交方式，其取值为get或post。
     name，属性用于指定表单的名称，以区分同一个页面中的多个表单。
#### input控件
     <input type="">
     type text 单行文本输入框
          password 密码输入框
          radio 单选按钮
          checkbox 复选框
          button 普通按钮
          submit 提交按钮
          reset 重置按钮
          image 图像形式的提交按钮
          hidden 隐藏域
          file 文件域
     name 由用户自定义 控件的名称
     value 由用户自定义 input控件中的默认文本值
     size 正整数 input控件在页面中的显示宽度
     readonly 该控件内容为只读（不能编辑修改）
     disabled 第一次加载页面是禁用该控件（显示为灰色）
     checked 定义选择控件默认被选中的项
     maxlength 正整数 控件允许输入的最多字符数
#### textarea控件
     <textarea cols="列数" rows="行数">
     ...
     </textarea>
#### select控件
     <select>
       <option>选项1</option>
       <option>选项2</option>
       <option>选项3</option>
       ...
     </select>
     select size 指定下拉菜单的可见选项数（取值为正整数）
            multiple 定义multiple="multiple"时，下拉菜单将具有多项选择的功能，方法为暗处ctrl键的同事选择多项
     option selected 定义selected="selected"时，当前项即为默认选中项
#### filedset组合控件
     用于将form中的控件进行分组，filedset没有必须或唯一的属性
     legend用于给filedset定义标题
     <form action="" method="">
      <filedset>
       <legend>title</legend>
       <input type="radio" id="radio">
      </filedset>
     </form>
