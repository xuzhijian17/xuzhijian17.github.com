Asm.js: JavaScript的编译目标
==========================
期待已久的Asm.js终于出来了，我也像许多开发者一样激动不已。你要是对此感兴趣，想要了解更多近期的信息请访问[Asm.js is now in Firefox nightly ](https://blog.mozilla.org/luke/2013/03/21/asm-js-in-firefox-nightly/)。这里也有大量你所感兴趣的资料[ Mozilla and Epic announced](https://blog.mozilla.org/blog/2013/03/27/mozilla-is-unlocking-the-power-of-the-web-as-a-platform-for-gaming/)，而且他们已经把虚拟引擎3（Unreal Engine 3）移植到了Asm.js上了-并且它运行的很好。

Asm.js通过使用WebGL渲染，能让一个基于C++引擎的游戏运行在JavaScript上面，这是一个非常大的壮举，而且很大程度上是因为有大量的工具链才能让Mozilla的开发人员将它变为可能。

自从发布了Asm.js的虚拟引擎3接口后，我就一直从Twitter,博客和其它一些地方关注着大家对此的反应，而一些开发者通过自己掌握的公开技术将它们有趣的结合在一起，并且已经取得了一些进步，同时也帮我解决了许多的困惑，比如:Asm.js是一个插件吗？Asm.js是否真能定期的使我的JavaScript变快？是否能在所有的浏览器中工作？我觉得Asm.js能够把这些技术相关联起来是一件非常了不起的事。我也试着通过我自己对它的一些理解来告诉大家Asm.js是怎么实现的以及它能给大家带来什么好处。同时在我这篇简短的研究报告中，我也问了[David Herman](http://calculist.org/)（Mozilla研究院高级研究员）一个关于Asm.js是怎样把各个零件都连在一起的问题。

什么是Asm.js?
-------------------
在理解Asm.js之前，你需要先知道它安装在浏览器中的什么地方和它来自哪里以及为什么存在。

Asm.js是JavaScript应用程序中的一个新的分类:C/C++应用程序通过JavaScript进行编译。它是整个JavaScript应用程序中的一个新的类型，并由[Mozilla Emscripten 项目](https://github.com/kripken/emscripten)发起。

Emscripten通过LLVM将C/C++代码转换生成LLVM字节码并放在JavaScript中运行（特别说明下，Asm.js是JavaScript的一个子集）。
![Asm.js Compilation & Execution Pipeline](./images/1yoy1Fal.png)

如果编译Asm.js代码去做一些执行过程中的渲染的话，那么大部分情况很可能都是通过WebGL来负责实现的（已经渲染的则使用OpenGL来实现）。在这种方法中，整个过程在技术上使用了JavaScript和浏览器，但是几乎绕过了整个真实的，正常的代码执行过程，并获取一个网页中的js渲染路径。

因为Asm.js是JavaScript的一个子集，因此它在操作使用上都会极大的受限。这样做，以便编译Asm.js代码可以运行尽可能快做尽可能少的假设，直接转换Asm.js代码到集合中。



## License

[MIT](http://opensource.org/licenses/MIT)
=======
=======
>>>>>>> fce28c9474279911a895b3ca6d0fd46723766e55
[xuzhijian17.github.io](http://xuzhijian17.github.io)
======================

test blog
<<<<<<< HEAD
>>>>>>> b8e49fca4de400bcc7bf901f0ed64f7c237c81c0
=======
>>>>>>> fce28c9474279911a895b3ca6d0fd46723766e55
