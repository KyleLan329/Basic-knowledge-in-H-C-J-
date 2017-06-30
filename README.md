# Basic-knowledge-in-H-C-J-
Collect basic knowledge that is easily ignored in HTML/CSS/Javascript

## HTML/CSS

(1)
常用的页面的图片格式有三种，GIF、JPG、PNG。 GIF 意为Graphics Interchange format（图形交换格式）； JPEG 代表Joint Photograhic Experts Group（联合图像专家组），这种格式经常写成JPG，JPG图片的扩展名为jpg；流式网络图形格式(Portable Network Graphic Format，PNG)名称来源于非官方的“PNG's Not GIF”，是一种位图文件(bitmap file)存储格式，读成“ping”。PNG用来存储灰度图像时，灰度图像的深度可多到16位，存储彩色图像时，彩色图像的深度可多到48位，并且还可存储多到16位的α通道数据。
标签图像文件格式 （ Tagged Image File Format ，简写为 TIFF ）是一种灵活的 位图 格式，主要用来存储包括照片和艺术图在内的图像。 TIFF文件格式适用于在应用程序之间和计算机平台之间的交换文件，它的出现使得图像数据交换变得简单。 TIFF文件以 .tif 为扩展名。其数据格式是一种3级体系结构，从高到低依次为：文件头、一个或多个称为IFD的包含标记指针的目录和数据。 


(2)运用css3动画，需要运用@keyframes规则和animation属性


(3)bootstrap3支持: IOS 与 Android 上的opera浏览器

(4)
H5新增标签：
article: 标签定义外部的内容。
aside:标签定义 article 以外的内容。a
audio:h5新增音频标签。没有高宽属性。
canvas:h5新增画布标签。
command: 定义命令按钮(未测试)
datalist：标签定义选项列表。
datalist 及其选项不会被想显示出来，它仅仅是合法的输入值列表。
details：标签用于描述文档或文档某个部分的细节。
figure：标签用于对元素进行组合。
figcaption：定义 figure 元素的标题。
footer：定义 section 或 document 的页脚。
header：定义 section 或 document 的页眉。
hgroup：用于对网页或区段（section）的标题进行组合。
keygen:标签规定用于表单的密钥对生成器字段
mark：标签定义带有记号的文本。
meter：通过min="0" max="20"的方式定义度量衡。仅用于已知最大和最小值的度量。
nav：定义document或section或article的导航。
output：定义不同的输出类型，比如脚本。
progress：定义任何类型的任务的进度。
rp:定义若浏览器不支持 ruby 元素显示的内容
rt：定义 ruby 注释的解释
ruby：定义 ruby 注释
section：标签定义文档中的节、区段。比如章节、页眉、页脚或文档中的其他部分。
source:audio和video的属性之一。为audio和video定义媒介源。
summary:为details定义标题。
time:定义日期或时间。
video：h5新增视频标签。具有高宽属性。

(5)

      <pre>定义预格式文本，保持文本原有的格式
      <meta> 元素可提供有关页面的元信息（meta-information），比如针对搜索引擎和更新频度的描述和关键词。
      <meta> 标签位于文档的头部，不包含任何内容。
      <meta> 标签的属性定义了与文档相关联的名称/值对。

(6)
可以对元素的margin设置百分数，百分数是相对于父元素的width计算，不管是margin-top/margin-bottom还是margin-left/margin-right。（padding同理）

如果没有为元素声明width，在这种情况下，元素框的总宽度包括外边距取决于父元素的width，这样可能得到“流式”页面，即元素的外边距会扩大或缩小以适应父元素的实际大小。如果对这个文档设置样式，使其元素使用百分数外边距，当用户修改浏览窗口的宽度时，外边距会随之扩大或缩小。

为什么margin-top/margin-bottom的百分数也是相对于width而不是height呢？

CSS权威指南中的解释：

我们认为，正常流中的大多数元素都会足够高以包含其后代元素（包括外边距），如果一个元素的上下外边距时父元素的height的百分数，就可能导致一个无限循环，父元素的height会增加，以适应后代元素上下外边距的增加，而相应的，上下外边距因为父元素height的增加也会增加，如果循环。

(7)
display: none和visibility:hidden的区别就是visibility:hidden会保留元素的空间
repaint(重绘) ，repaint发生更改时，元素的外观被改变，且在没有改变布局的情况下发生，如改变outline,visibility,background color，不会影响到dom结构渲染。
reflow(渲染)，与repaint区别就是他会影响到dom的结构渲染，同时他会触发repaint，他会改变他本身与所有父辈元素(祖先)，这种开销是非常昂贵的，导致性能下降是必然的，页面元素越多效果越明显。
所以display:none才会产生reflow
visibility:hidden只会出发repaint

(8)

    在网页中嵌入多媒体，如电影，声音等用到的标记是:
    <embed> 标签是 HTML 5 中的新标签。
    浏览器支持
    所有主流浏览器都支持 <embed> 标签。
    定义及使用说明
    <embed> 标签定义了一个容器，用来嵌入外部应用或者互动程序（插件）。
    实例
    被嵌入的 flash 动画片：
      <embed src="helloworld.swf">


(9)单元格垂直合并所用的属性是Rowspan ；单元格横向合并所用的属性是  Colspan

(10)
    
     HTML技术中使文字滚动的方法是使用双标签<marquee></marquee>。在HTML代码中可使其作用区文字滚动，默认为从右到左，循环滚动。 <marquee direction="left">default scroll direction</marquee>
    

(11) 在使用table表现数据时，有时候表现出来的会比自己实际设置的宽度要宽，为此需要设置下面哪些属性值？
- 单元格边距(表格填充)(cellpadding) -- 代表单元格外面的一个距离,用于隔开单元格与单元格空间单；
- 元格间距(表格间距)(cellspacing) -- 代表表格边框与单元格补白的距离,也是单元格补白之间的距离.

(12)
请阅读以下代码：
    
      <div style=”width:400px;height:200px;”>
    <span style=”float:left;width:auto;height:100%;”>
     <i style=”position:absolute;float:left;width:100px;height:50px;”>hello</i>
    </span>
      </div>

问题：span标签的width和height分别为多少？
width = 0px，height = 200px
首先span不是块级元素，是不支持宽高的，但是style中有了个float：left；就使得span变成了块级元素支持宽高，height:100%;即为，200，宽度由内容撑开。
但是内容中的 i 是绝对定位，脱离了文档流，所以不占父级空间，所以span的width=0



## JavaScript

（1）
$.post(url)是ajax请求；
ajax的事件是：
ajaxComplete(callback)
ajaxError(callback)
ajaxSend(callback)
ajaxStart(callback)
ajaxStop(callback)
ajaxSuccess(callback)   $.post(url)不属于ajax事件


（2）
Yahoo! User Interface  库  (YUI)  包含一个  bucketload 。
和  YUI  一样， ExtJS  包含大量开箱即用的组件，其中有很多功能强大的网格控件，支持内联编辑、分页、筛选、分组、汇总、缓冲和数据绑定。
MooTools  和  Prototype 、 jQuery  不包含开箱即用的  UI  控件和小部件.

(3)
JavaScript中的保留字：别用它们来命名！！
abstract
boolean break byte
case catch char class const continue
debugger default delete do double
else enum export extends
false final finally float for function
goto
if implements import in instanceof int interface
long
native new null
package private protected public
return
short static super switch synchronized
this throw throws transient true try typeof
var void volatile
while with

(4)Flash提供了ExternalInterface接口与JavaScript通信，ExternalInterface有两个方法，call和addCallback，call的作用是让Flash调用js里的方法，addCallback是用来注册flash函数让js调用。

(5)
  console.log(Number(""));           //0
  console.log(Number(null));         //0
  console.log(Number(undefined));    //NaN

  console.log(parseInt(""));        //NaN
  console.log(parseInt(null));      //NaN
  console.log(parseInt(undefined)); //NaN

  console.log(null == 0); //false
  console.log(undefined == 0); //false

(6) 如果需要匹配包含文本的元素，用下面哪种方法来实现？

contains()
text()是jQuery中的方法，可是设置或返回被选元素的文本内容

：contains选择器，选取包含指定字符串的元素，字符串也可以是文本

:input()选择器，选取表单元素
attr(name,value)属性操作，设置或返回被选元素的属性和属性值

(7)

(8)
md5()函数将一个字符串进行md5加密计算，md5()函数使用RSA数据安全，包括MD5报文摘要算法。 语法：md5(string,raw)，第一个参数string必需，表示待处理字符串，第二个参数raw可选，布尔型数值，默认为false，false表示返回32位的十六进制字符串，true表示返回16位二进制数。 sha1()函数计算字符串sha-1散列，使用哈希安全算法。 语法：sha1(string,raw)，同md5。 str_rot13()函数对字符串执行rot13编码。 crc32()函数计算字符串的32位crc（循环冗余校验），该函数可以用于验证数据完整性。

(9)
type              result
Undefined   "undefined"
Null             "object"
Boolean     "boolean"
Number      "number"
String           "string"
Symbol           "symbol"
Host object      Implementation-dependent
Function         "function"
Object           "object"

(10)
当在 HTML 页面中执行脚本时，页面的状态是不可响应的，直到脚本已完成。 web worker 是运行在后台的 JavaScript，独立于其他脚本，不会影响页面的性能。您可以继续做任何愿意做的事情：点击、选取内容等等，而此时 web worker 在后台运行。

(11)
    
    	function test(){
    var n = 4399;
    
    function add(){
      n++;
      console.log(n);
    }
    
    return {n:n, add:add}
     	 }
    
      var result = test();
      var result2 = test();
      result.add(); //4400
      result.add(); //4401
      console.log(result.n) //4399;
      result2.add(); //4400


首先，题中定义了一个函数，名为test，这个函数内部分别又定义了一个数值变量n和一个闭包函数add，test函数的最后一行代码return{n:n,add:add}，实际上是返回了一个object，而这个object中有一个属性n，它的值是n，还有一个方法add，它的值是add。
好了，函数解释清楚，再来看输出的问题。函数外部分别定义了两个变量，result和result2，他们都指向test函数，但是分属两个不同的作用域，这也就解释了答案中1和4,4不会在2的基础上继续n++。
1和2属于闭包函数的问题，可参考阮一峰老师的一篇博文（http://www.ruanyifeng.com/blog/2009/08/learning_javascript_closures.html），简单易懂，借用阮老师博客中所写，闭包的两个最大的用处：一个是可以读取到函数内部的变量，另一个就是让这些变量的值始终保持在内存中，具体可以测试。第二个用途就解释了同一个作用域中答案2会在1的基础上进行+1操作。
答案3是比较令人困惑的一项，追本溯源，前面提到过第6行代码返回了一个有着值为n的属性n和值为add的方法add的匿名对象，在这里，在这个匿名对象中，属性n和方法add是互不相关的，即使在闭包add中改变了变量n的值，result.n的值依然不变。

(12)

	  var bb = 1;
	  function aa(bb) {
	      bb = 2;
	      alert(bb);
	  };
	  aa(bb); //2
	  alert(bb); //1

记住一句话就好了：“ECMA中所有函数的参数都是按值传递的”。
值传递：把把一个值类型（也叫基本类型）传递给另一个变量时，其实是分配了一块新的存储空间，因此就本题来说，在内部改变这个值时，其实在函数外部对这个值没有影响。

函数体内，bb并没有使用var来定义，按理说这个bb在预处理的时候应该是window的属性。但在这里，函数声明的时候，带了一个参数bb，也就是相当于在函数体内声明了var bb。所以，函数里的bb就是函数活动对象的属性。所以函数执行时会输出2。函数执行完后，函数的活动对象被销毁，也就是局部的这个bb被删除了，执行流进入到window，再输出bb，值就是1了。如果声明函数时，把参数那里的bb去掉，这段代码执行起来，结果就是弹出 2 2


(13)
可以使用preventDefault()阻止默认行为，例如a链接的跳转，在a链接跳转中，需要先对a链接绑定点击事件，然后在a链接的事件对象中调用该方法即可.

stopPropagation()用于阻止事件冒泡

(14)
AMD是"Asynchronous Module Definition"的缩写，意思就是"异步模块定义"。它采用异步方式加载模块，模块的加载不影响它后面语句的运行。所有依赖这个模块的语句，都定义在一个回调函数中，等到加载完成之后，这个回调函数才会运行。
AMD也采用require()语句加载模块，但是不同于CommonJS。
主要有两个Javascript库实现了AMD规范：require.js和curl.js。
参考链接：http://www.ruanyifeng.com/blog/2012/10/asynchronous_module_definition.html

    AMD 是 RequireJS 在推广过程中对模块定义的规范化产出。
    CMD 是 SeaJS 在推广过程中对模块定义的规范化产出。
    区别：
    1. 对于依赖的模块，AMD 是提前执行，CMD 是延迟执行。
    2. CMD 推崇依赖就近，AMD 推崇依赖前置。
    // CMD
      define(function(require, exports, module) {
      var a = require('./a')
      a.doSomething()
      // 此处略去 100 行
      var b = require('./b') // 依赖可以就近书写
      b.doSomething()
      // ...
      })
    
      // AMD 默认推荐的是
      define(['./a', './b'], function(a, b) { // 依赖必须一开始就写好
      a.doSomething()
      // 此处略去 100 行
      b.doSomething()
      ...
      })

(15) 只要 协议 、 域名 、 端口 有任何一个 不同, 都被当作是 不同 的域。

(16)
all（）方法和apply（）方法的作用相同，他们的区别在于接收参数的方式不同。对于call（），第一个参数是this值没有变化，变化的是其余参数都直接传递给函数。（在使用call（）方法时，传递给函数的参数必须逐个列举出来。使用apply（）时，传递给函数的是参数数组）如下代码做出解释：
    
      function add(c, d){
    
      return this.a + this.b + c + d;
    
      }
    
      var o = {a:1, b:3};
      add.call(o, 5, 7); // 1 + 3 + 5 + 7 = 16
      add.apply(o, [10, 20]); // 1 + 3 + 10 + 20 = 34

(17)

    下列代码，页面打开后能够弹出alert(1)的是
    
      <iframe src=”javascript: alert(1)”></iframe> //页面加载时触发
    
    
      <img src=”” onerror=”alert(1)”/> //图片载入失败时触发
    
    
      IE下<s style=”top:expression(alert(1))”></s>  // 在ie 7下会连续弹出， IE5及其以后版本支持在CSS中使用expression，用来把CSS属性和Javascript表达式关联起来，这里的CSS属性可以是元素固有的属性，也可以是自定义属性。就是说CSS属性后面可以是一段Javascript表达式，CSS属性的值等于Javascript表达式计算的结果。 在表达式中可以直接引用元素自身的属性和方法，也可以使用其他浏览器对象。这个表达式就好像是在这个元素的一个成员函数中一样。参考资料 http://www.blueidea.com/tech/site/2006/3705.asp
    
      <div onclick=”alert(1)”></div>  // 不可以,因为div里没有内容，盒子的宽度为0所以点击不了
 
（18）以下符合 ES6 写法的有：

    A．	class Foo
    {
    	constructor() {return Object.create(null);}
    }
    Foo()
    B．	var m=1;
    export m;
    export var firstName=’Michael’;
    在A模块中export{readFile}后，在B模块中import readFile from ‘A’可以获取到readFil

 
A、Fun() 把 class 当成方法来用？ var fun = new Func() 这样用就对了
B、export 后面变量没加括号；
D、import readFile 没加括号，是导入 default 的用法，但是前面不是 export 为 default

参照 export 和 import 用法：
1、https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/export
2、https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import

    
    export {name1,name2, …,nameN};
    export {variable1asname1,variable2asname2, …,nameN};
    export letname1,name2, …,nameN; // also var
    export letname1= …,name2= …, …,nameN; // also var, const
    
    export expression;
    export default expression;
    export default function (…) { … } // also class, function*
    export default function name1(…) { … } // also class, function*
    export {name1as default, … };
    
    export * from …;
    export {name1,name2, …,nameN} from …;
    export {import1asname1,import2asname2, …,nameN} from …;
    
     import defaultMember from "module-name";
    import * as name from "module-name";
    import { member } from "module-name";
    import { member as alias } from "module-name";
    import { member1 , member2 } from "module-name";
    import { member1 , member2 as alias2 , [...] } from "module-name";
    import defaultMember, { member [ , [...] ] } from "module-name";
    import defaultMember, * as name from "module-name";
    import "module-name"
    
 (19) 先事件捕获从windows > document 往下级直到 特定的事件节点，然后进行事件处理，再事件冒泡，从特定节点往上级，这个完整的过程
 
