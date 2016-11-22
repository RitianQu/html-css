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
#### 垂直对齐方式vertical-align（适用于行内元素）
     vertical-align 常用属性值
     baseline 将支持valign特性的对象的内容与基线对齐
     sub 垂直对齐文本的下标
     super 垂直对齐文本的上标
     top 将支持valign特性的对象的内容与对象顶端对齐
     text-top 将支持valign特性的对象的文本与对象顶部对齐
     middle 将支持valign特性的对象的文本与对象中部对齐
     bottom 将支持valign特性的对象的文本与对象底端对齐
     text-bottom 将支持valign特性的对象的文本与对象顶端对齐
#### 首行缩进text-indent
     text-indent属性用于设置首行文本的缩进，其属性值可为不同单位的数值。em字符宽度的倍数。或相对于浏览器窗口宽度的百分比%，允许使用负值，建议使用      em作为设置单位
#### 空白符处理white-space
     normal：常规（默认值），文本中的空格。空行无效，满行（到达区域边界）后自动换行
     pre：预格式化，按文档的书写格式保留空格。空行原样显示
     nowrap：空格空行无效，强制文本不能换行，除非遇到换行标记
     。内容超市元素的边界也不换行，若超出浏览器页面则会自动增加滚动条
#### 自动换行word-break
     normal 使用浏览器默认的换行规则
     break-all 允许在单词内换行
     科尔皮、-all 只能在半角空格或连字符处换行
#### word-wrap
     属性允许长单词或URL地址换行到下一行normal
     normal 只在允许的端子点换行（浏览器保持默认处理）
     break-word 在长单词或URL地址内部进行换行，几乎得到了浏览器的支持
#### 后代选择器
     div p {
        width: 100px;
        height: 100px;
        }
#### 交集选择器
     选择两个集合中的共同部分
     div p.boss {
     color: red;
     }
     <div>
     <p class="boss">11</p>
     </p>
#### 并集选择器
     对多个集合中的所有的内容合并在一起进行设置
     p, span {
     color: red;
     }
#### 伪类选择器
     link：标签原本样式（如果在这个属性中设置样式优先级药高于标签选择器）
     visited：标签被访问以后的样式
     hover：鼠标悬停在标签上会触犯的样式
     active：当点击（激活）标签时的样式
     a:link {
     color: blue;
     }
     a:visited {
     color: red;
     }
     a:hover {
     color: yellow
     }
     a:active {
     color: green;
     }
#### css三种样式类型
###  行内样式
     所有样式都是在写标签的内部，只能作用在这个标签上面。（一般情况下不建议使用，我们单独学习css的目的就是页面的结构和样式的分离，我们不能反其道而行      之）
###  嵌套样式
     写在head中，并且用style标签包含。这也是我们比较常用的一种。
###  外部样式
     将css编写为单独的文件，需要在head中引入
#### css的三大特性
###  继承
     就是页面中的一些标签的属性可以继承给子标签，但是继承还是限制的，比如a的颜色，块级元素的高度等等。一般情况下，所有的与文字图片的大小样式相当的属      性都可以继承：font-x，line-x，一些标签的宽高也可以继承。
     h元素的字体阿晓会受祖先元素的影响，但是字体大小是呈比例额的
###  层叠
     页面的样式是多项属性设置进行叠加的结果
     针对重复性的设置，那么后边的设置会覆盖掉之前的设置
###  优先级
     当设置发生冲突时，需要考虑优先级，优先级最高的设置有效
     基本公式：id>class>标签>继承>浏览器的默认属性
     但是运行公式需要条件：针对同一个标签的设置。
     当优先级一致时，那么最后设置的有效
     在同一个元素上设置的属性当中，行内样式的设置最终有效
     id=100，class=10，tag=1
#### 背景的具体属性
###  background-color：设置背景颜色，按照颜色的格式填写，比如red，#F00，rgb（255,0,0）
     background-color:red;
     background-color:#F00;
###  background-image:设置背景图片，url（图片路径）
     background-image:url("image/xxx.jpg");
###  background-repeat:设置背景图片是否平铺，repeat,no-repeat,repeat-x,repeat-y.
###  background-position:设置背景图片显示位置，可以使用top,bottom,left,right设置，也可以直接设置数值x轴y轴
###  background-attachement：设置背景是否固定，fixed表示固定。
#### 背景属性的综合写法
###  background: color image repeat position attachement;
     background:red url("image/xxx.png")repeat 10px 10px fixed;
#### 行高
     使用百分比，那么这个行高的基数为当前标签字体大小。
     line-height:120%; 表示行高为当前字体的1.2被，子元素会继承父元素计算出的行高
     直接使用px进行绝对设置
     line-height：30px；直接设置行高为30px
     使用em进行相对设置
     line-height：1.5em； 设置行高为当前字体大小的1.5倍，子元素会继承父元素计算出的行高
     使用不带单位的数值
     line-height：1.5；设置行高因子为1.5，子元素会继承该因子而不是继承父元素行高
#### 边框属性
     边框颜色
     border-top-width:上边框宽度
     border-right-width:右边框宽度
     border-bottom-width:下边框宽度
     border-left-width:左边框宽度
     border-width:上边框宽度[右边框宽度 下边框宽度 左边框颜色]
     边框颜色：
     border-top-color:上边框颜色
     border-right-color:右边框颜色
     border-bottom-color:下边框颜色
     border-left-color:左边框颜色
     border-color:上边框颜色【右边框颜色 下边框颜色 左边框颜色】
     边框样式：
     border-top-style:上边框样式
     border-rignt-style:右边框样式
     border-bottom-style:下边框样式
     border-left-style:左边框样式
     border-style:上边框样式【右边框样式 下边框样式 坐边框样式】
     常用样式：solid dashed dotted double
     注意：设置边框颜色时同样必须设置边框样式，如果未设置样式或设置为none，则其他的边框属性无效。
     边框属性的综合设置：
     border-top:宽度 样式 颜色
     border-top:1px solid red;
     border:宽度 样式 颜色
     borderL:1px dotted yellow;
     小技巧：border:0none;设置边框为0的方法。
#### 内边距padding属性
     padding-top:上内边距
     padding-right：右内边距
     padding-bottom：下内边距
     padding-left:左内边距
     综合设置：padding：上内边距【右内边距 下内边距 左内边距】
#### 外边距margin
     margin-top：上外边距
     margin-right：右外边距
     margin-bottom：下外边距
     margin-left：左外边距
     综合设置：margin:上外边距【右外边距 下外边距 左外边距】
     注意：
     1 外边距可以使用负值，使相邻元素重叠。
     2 可能会出现外边距合并情况
     3 为了方便操作，可以用×{margin：0；padding：0}取消浏览器的默认属性
#### 解决嵌套元素的外边距合并
     对于两个嵌套关系的块元素，如果父元素没有上内边距及边框，则父元素的上外边距会与子元素的上外边距发生合并，合并后的外边距为两者中的较大者，即使父      元素的上外边矿局为0，也会发生合并。
     如果希望外边距不和并，可以为父元素定义1像素的上边框或上内边距。这里可以定义父元素的上边框为例，在父div的CSS样式中增加如下代码：
     border：1px solid red; 或者padding-top:1px;
#### 盒子宽度和高度的计算
     Width=border-left+padding-left+width+padding-right+border-right
     Height=border-top+padding-top+height+padding-bottom+border-bottom
     一般请款下设置padding值都会影响div的大小，但是如果这个div没有设置宽度，而是继承了父亲的宽度，那么再次设置Padding值的时候不会影响这个div的宽      度

     
