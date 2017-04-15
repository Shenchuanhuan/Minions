# Minions
Minions made by html5, css3.

### 知识点概括
-	兼容于各浏览器内核的css3写法
	-	-webkit ：chrome & safari
	-	-moz：firefox
	-	-ms：ie
	-	-o：opera

-	各浏览器内核
	-	Trident内核代表产品Internet Explorer，又称其为IE内核。Trident（又称为MSHTML），是微软开发的一种排版引擎。使用Trident渲染引擎的浏览器包括：IE、傲游、世界之窗浏览器、Avant、腾讯TT、Netscape 8、NetCaptor、Sleipnir、GOSURF、GreenBrowser和KKman等。
	-	Gecko内核代表作品Mozilla FirefoxGecko是一套开放源代码的、以C++编写的网页排版引擎。Gecko是最流行的排版引擎之一，仅次于Trident。使用它的最著名浏览器有Firefox、Netscape6至9。
	-	WebKit内核代表作品Safari、Chromewebkit 是一个开源项目，包含了来自KDE项目和苹果公司的一些组件，主要用于Mac OS系统，它的特点在于源码结构清晰、渲染速度极快。缺点是对网页代码的兼容性不高，导致一些编写不标准的网页无法正常显示。主要代表作品有Safari和Google的浏览器Chrome。
	-	Presto内核代表作品OperaPresto是由Opera Software开发的浏览器排版引擎，供Opera 7.0及以上使用。它取代了旧版Opera 4至6版本使用的Elektra排版引擎，包括加入动态功能，例如网页或其部分可随着DOM及Script语法的事件而重新排版。

****
###	一些在IE6里常见的兼容性问题及解决方案
-	在IE6及以下的版本里，如果往div中插入图片，图片会将div下方撑大三像素。
	>hack：将<img>转为块级元素，display:block;
-	当IE6及更低版本浏览器在解析浮动元素时，会加倍浮动边距。
	>hack：给浮动元素添加声明：display:inline;
-	表单元素行高表现不一致。
	>hack:给表单元素添加声明：float:left;
-	按钮元素默认大小不一致。
	>hack: 1、用a标签模拟按钮元素；2、用一个标签包住input标签，去掉input边框样式，所有按钮样式加在外包的标签上。
-	子元素没有浮动属性，设置margin-top属性后，会错误地把该属性值添加给父级元素。
	>hack:给父元素添加声明：overflow:hidden;
-	H5标签不支持ie9以下版本浏览器
	>hack:引用html5shiv.js
	```javascript
	<script src="js/html5shiv.js"></script>
	```
	
###	Animation
-	八条属性
	1.	animation-name      //定义动画名称
	2.	animation-duration  //定义动画执行时间
	3.	animation-delay		//定义延时执行动画时间
	4.	animation-iteration-count //定义动画执行次数
	5.	animation-direction //方向
	6.	animation-play-state	//暂停或播放动画 
	7.	animation-fill-mode		//设置在动画之前或之后应用
	8.	animation-timing-function //动画运动函数
	
想深入了解的话，可以参考css-tricks上的文章，我参考的是[这篇](https://css-tricks.com/almanac/properties/a/animation/)	
	       



