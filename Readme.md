## plugin

* Markdown Preview    `ctrl+shift+p  ==> mp`
* zencoding	`ctrl+alt+enter`
* jsFormat 选中代码后按快捷键	`{ "keys": ["ctrl+alt+f"], "command": "js_format"}`
* Clipboard History
	-  OSX: Press ctrl-alt-super-v to show the history.
	- Windows: Press ctrl-alt-v to show the history.

## 代码提示包(放入package内)

* jQuery Package for Sublime Text `snippet`
* [sublime-kissy-snippets](https://github.com/zfkun/sublime-kissy-snippets#readme)


## 颜色主题

加入了MarkDown配色文件 `Monokai-custom.tmTheme`

* Janblus.tmTheme
* Obsidian.tmTheme

	"color_scheme": "Packages/User/Monokai-custom.tmTheme"

##  主题

黑色主题	`Default.sublime-theme`


## 建立自己的代码片段库

写代码，都少不了自己一些常用的代码片段，Sublime Text也提供了设置代码片段的方法。
在Tools->New Snippet 中可以新建自己的代码片段
新建snippet会默认显示如下代码，可以这个为模板进行修改。

	<snippet>
	    <content><![CDATA[
	Hello, ${1:this} is a ${2:snippet}.
	]]></content>
	    <!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	    <!-- <tabTrigger>hello</tabTrigger> -->
	    <!-- Optional: Set a scope to limit where the snippet will trigger -->
	    <!-- <scope>source.python</scope> -->
	</snippet>

使用时，先取消注释的内容。

* content标签包含的内容就是需要显示的代码片段。其中${1:this} 是表示产生代码片段后，光标停在this这个位置。${2:snippet}表示，产生代码片段后，按tab健光标跳到 snippet位置。
*tabTrigger标签 相当于快捷键，比如上面代码hello：输入hello然后按tab键即可显示content标签的内容。
*scope标签可选，默认不写则对所有文件格式生效，如果设置了，则对相应的文件或文件格式生效。

最后设置好后， 将文件保存在”packages/User”目录下，以sublime-snippet为扩展名。重启sublime text 2，该snippet即可使用了。
关于snippet的详细内容可参看文章：http://sublimetext.info/docs/en/extensibility/snippets.html


## 破解方法

目前最新版本的Sublime Text2破解方法：将sublime_text.exe复制一份改名为sublime_text_cracked.exe，用sublime text2打开这个sublime_text_cracked文件（新版sublime text貌似无法二进制写入，导致保存后无法识别为有效win32应用程序）用支持二进制写入的编辑器来改，搜索3342，改为3242保存，打开sublime_text_cracked文件，在help菜单里enter license，把下面注册码贴进去，包括begin和end那两行，完。

测试环境：sublime text2 32bit在win7 ultimate 64bit sp1，xp professional 32bit sp2，windows server 2003 32bit，BackTrack 5。

linux和mac下的sublime text破解过程与windows下的同理。

	—–BEGIN LICENSE—–
	hiwanz
	Unlimited User License
	EA7E-26838
	5B320641E6E11F5C6E16553C438A6839
	72BA70FE439203367920D70E7DEB0E92
	436D756177BBE49EFC9FBBB3420DB9D3
	6AA8307E845B6AB8AF99D81734EEA961
	02402C853F1FFF9854D94799D1317F37
	1DAB52730F6CADDE701BF3BE03C34EF2
	85E053D2B5E16502F4B009DE413591DE
	0840D6E2CBF0A3049E2FAD940A53FF67
	—–END LICENSE—–
