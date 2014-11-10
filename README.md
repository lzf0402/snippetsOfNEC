snippet，你用活了么?——Sublime代码片段，提高你的开发效率
=============

> 作为一名前端coder，[Sublime Text](http://www.sublimetext.com/)这款编辑器应该不会陌生啦，简单轻量功能强大，真心好用~ 再说说它提供的snippet功能，可以一定程度的把我们从*复制粘贴*的重复劳动中解放出来。把经常会拷贝的代码片段，存成一个snippet文件，然后借助触发键快速生成，这在提升编码效率方面可是杠杠的，也让你的开发工作瞬间有滋有味~

##  轻松几步，制作你自己的代码片段  ##

**1. Sublime text ——> tools ——> New Snippet**

![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show1.png)

新建一个Snippet，保存成`.sublime-snippet`后缀的文件，Sublime Text默认会保存到`C:\Users\yourname\AppData\Roaming\Sublime Text 2\Packages\User`此目录下。当然你也可以在此目录下新建文件夹，把代码片段进行分类，比如可以把css和html的代码片段分别放到对应的目录，如下图：

![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show2.png)


**2. 修改snippet文件**

把你自定义的代码片段放到合适的区域，并指定一个触发键（tabTrigger）和片段可以触发的文件范围（scope），也可以指定描述文本，如下：
![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show5.png)


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

![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show3.png)

**3.注意事项**

如果在css文件里不能触发上图所示的代码提示框，那该如何？ 下文来支招：

**可通过修改配置文件开启代码自动提示功能**：
在菜单栏中选择Preferences >> Settings - Default,打开该文件搜索找到"auto_complete_selector",将该行注释掉，如下图所示：

![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/tip.jpg)

还不赶紧把你常用的各类代码（CSS、HTML、JS等）整理成代码片段，解放你的“Ctrl+C/V”。

**4.snippet Of NEC**

本着一人分享、造福众码农的无私精神，把咱大网易大名鼎鼎的NEC（什么？你不知道NEC，你来，我保证不打死你！还不赶紧猛戳[NEC官网](http://nec.netease.com/)）的框架、布局、模块、元件代码做成了snippet，供前端攻城狮们下载（[下载请猛戳](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/NEC-snippet.rar)），请叫我雷锋^_^~
 
![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show9.png)
![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show6.png)
![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show7.png)
![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show8.png)

把下载的NEC版的代码片段
在Sublime Text编辑器的菜单栏中选择 Preferences >> Browse Packages...，在打开的Packages目录下找到User目录，将你下载的NEC版的代码片段解压在此目录下，就大功告成啦~
回到编辑器，新建一个html文件，当你在敲下 `NEC-html`触发键后生成了一整片html模板代码，有没有小小激动一下~

![](https://raw.githubusercontent.com/lzf0402/snippetsOfNEC/master/imgs/show10.png)

另外，随着CSS预处理器在项目中的广泛实践应用，以上的NEC版代码片段里也包含了模块和元件的MCSS版。说到[MCSS](https://github.com/leeluolee/mcss)，目前已在多个产品中实践，鉴定好用，所以小伙伴们还不赶紧mcss一下~；自从有了mcss，妈妈再也不用担心我写css慢啦~
