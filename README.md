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
#### css规则
     css主要目的：控制网页中元素的样式
     css可以让我们从HTML结构和样式分离出来
     css可以让我们专注结构。代码更少，语义更好，搜索更容易
#### css选择器
###  标签选择器
     标记选择器是指用html标记名称作为选择器，按标记名称分类，为页面中某一类标记指定统一的css样式。其基本语法格式如下
     表签名（属性1：属性值1；属性2：属性值2；属性3：属性值3；）
     标记选择器最大的优点是能快速为页面中同类型的标记统一样式，同时这也是她的缺点，不能色剂差异化样式
###  类选择器
     类选择器使用”.“（英文点号）进行标识，后面紧跟类名，其基本语法格式如下：
     .classname{属性1：属性值1；属性2：属性值2；属性3：属性值3}
     类选择器最大的优势是可以为元素对象定义单独或相同的样式
###  id选择器
     id选择器使用"#"进行标识，后面紧跟id名，其基本语法格式入戏：
     #idname{属性1：属性值1；属性2：属性值2；属性3：属性值3；}
     该语法中，id名即为html元素的id属性值，大多数html元素都可以定义id属性，元素的id值是唯一的，只能对应于文档中某一个具体的元素
###  统配选择器
     通配符选择器用”*“号表示，他是所有选择器中作用范围最广的，能匹配页面中素有的元素，其基本语法格式如下：
     *{属性1：属性值1；属性2：属性值2；属性3：属性值3；}
     如果：清楚当前文档中所有的元素的外边距和内边距
     *{
     margin:0;
     padding:0;
     }
#### css样式属性
###  font字体属性
##   font-size
     font-size属性用于设置字号，该属性的值可以使用相对长度单位，也可以使用绝对长度单位。其中，相对长度单位比较常用，推荐使用像素单位px，绝对长度单      位使用较少
##   font-family字体
##   font-weight
     font-weight属性用于定义字体的粗细，其可用属性值：normal、bold、bolder、lighter、100~900（100的整数倍）
##   font-style
     font-style属性用于定义字体风格，如设置斜体、倾斜或正常字体。其可用属性值如下：
     normal：默认值，浏览器会显示标准的字体样式
     italic:浏览器会显示斜体的字体样式
     oblique:浏览器会显示倾斜的字体样式
##   font综合设置
     font属性用于对字体样式进行综合设置，其基本语法格式如下：
     选择器{
     font:font-style font-weight font-size/line-height font-family;
     }
     使用font属性时，必须按上面语法格式中的顺序书写，各个属性以空格隔开
     其中不需要设置的属性可以省略（取默认值），但必须保留font-size和font-family属性，否则font属性将不起作用
#### 文本外观属性
###  文本颜色color
     color属性用于定义文本的颜色，其取值方式有如下3种：
     预定义的颜色值，如red，green，bule等。
###  字间距letter-spacing
     letter-spacing属性用于定义字间距，所谓字间距就是字符与字符之间的空白。其属性值可为不同单位的数值，允许使用复值，默认为normal
###  单词间距word-spacing
     word-spacing属性用于定义英文单词之间的间距，对中文字符无效。和letter-spacing一样，其属性值可为不同单位的数值，允许使用负值，默认为normal
     word-spacing和letter-spacing均可对英文进行设置。不同的是letter-spacing定义的字母之间的间距，二word-spacing定义的为英文单词之间的间距
###  行间距line-height
     line-height属性用于设置行间距，就是行与行之间的距离，即字符的垂直间距，一般称为行高。line-height常用的属性值单位有三种
     分别为像素px，相对值em和百分比%，实际工作中使用最多的是像素px
#### 文本装饰text-decoration
     text-decoration属性用于设置文本的下划线，上划线，删除线等装饰效果，其可用属性值如下：
     none：没有装饰（正常文本默认值）
     underline：下划线
     oveline：上划线
     line-through：删除线
###  水平对齐方式text-align
     text-align属性用于设置文本内容的水平对齐，相当于html中的align对齐属性。其可用属性值如下：
     left：左对齐（默认值）
     right：右对齐
     center：居中对齐
#### 
     

     
