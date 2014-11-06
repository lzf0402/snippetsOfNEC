snippetsOfNEC
=============

> 作为一名前端coder，[Sublime Text](http://www.sublimetext.com/)这款编辑器应该不会陌生啦，简单轻量功能强大，真心好用~ 再说说它提供的snippet功能，可以一定程度的把我们从*复制粘贴*的重复劳动中解放出来。把经常会拷贝的代码片段，存成一个snippet文件，然后借助触发键快速生成，这在提升编码效率方面可是杠杠的，也让你的开发工作瞬间有滋有味~

##  轻松几步，制作你自己的代码片段  ##

**1. Sublime text ——> tools ——> New Snippet**

![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/show1.png)

新建一个Snippet，保存成`.sublime-snippet`后缀的文件，Sublime Text默认会保存到`C:\Users\yourname\AppData\Roaming\Sublime Text 2\Packages\User`此目录下。当然你也可以在此目录下新建文件夹，把代码片段进行分类，比如可以把css和html的代码片段分别放到对应的目录，如下图：

![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/show2.png)


**2. 修改文件；**

把你自定义的代码片段放到合适的区域，并指定一个触发键（tabTrigger）和片段可以触发的文件范围（scope），也可以指定描述文本，如下：
![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/show5.png)


    <snippet>
	<content><![CDATA[
	//这里放你的代码片段
	.demo{font-size:12px;}
	]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>mysinppet</tabTrigger>
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<scope>source.css</scope>
	<description>测试</description>	
	</snippet>


没错，上面的代码演示了用 `mysinppet`这个触发键在css文件里，能快速生成一个名为demo的类选择器。赶紧新建一个css文件试试吧。当你在css文件里按下"my"两个字符时，神奇的事情发生了，下方出现了代码提示框，选中跟你匹配的"mysinppet"，按下回车，刚刚设置的代码片段就自动生成了，是不是很惊喜呀。如下图：

![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/show3.png)


**3.注意事项**

本着一人分享、造福众码农的无私精神，把咱大网易大名鼎鼎的NEC（什么？你不知道NEC，你来，我保证不打死你！还不赶紧猛戳xxx）的模块、元件，转成了一个MCSS版本，请叫我雷锋~

continue...