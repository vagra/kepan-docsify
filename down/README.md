#1 Kepan Docsify 下载

不定期更新，请下载最新版本。

#2 最新版本

* 2020-11-02
[kepan-docsify.4.11.6.1.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.6.1.zip)

    * Docsify 官方版本有了一些比较重大的更新，其中关键的一项，是吧它引用的 marked 库的版本，从 ^0.7 更新到了 ^1.1 ，也就是说，从此跟上了 marked 的最新版本。

    * 因此我相应的对最新版的 marked 打了 patch 。而且呢过去修改的 marked 只支持 `#1, #2, #3` 这样的 kepan markdown 标题，不支持传统的 markdown 标题 `#, ##, ###` 了，在这次更新中，做了改进，让它同时可以支持传统的 markdown 标题和 kepan markdown 标题，这样有很多好处。

    * 修改 marked 的方式，是 markdown 的标题格式本来有两种，一种叫 heading ，一种叫 lheading ，我给它加了第三种叫 kheading ，k 就是 kepan 的首字母，现在这三种标题格式可以共存。

    * 但是 marked 还有个设置，就是 pedantic 模式，它是传统的、原始的 markdown 模式，我并没有把 kheading 的支持加入进去，所以如果 pedantic 模式打开时，不会支持 `#1, #2, #3` 格式的标题。

    * 这次我对 kepan docsify 的侧边栏也做了关键变更，侧边栏的折叠和展开不再是跟随主页面全自动展开折叠，而是手动点击标题旁边的箭头来折叠和展开。今后 kepan docsify 的操作方式将会向 pdf 、 word 那种传统方式看齐。

    * 目前来说 kepan docsify 还剩下一个关键的待解决问题，就是为用户记录每个节点的折叠和展开状态，甚至记录上次浏览到的位置。

#2 尚待改进
> * 2020-05-26
希望增加侧边栏可以左右拖动调整大小的功能。以及侧边栏状态记忆，记忆住侧边栏每个条目的打开和关闭状态。

> * 2020-05-09
Kepan Docsify 的设计目标，是尽量把侧边栏的阅读体验，做得跟 Word 、 PDF 基本一致。因为大家都非常习惯 Word 和 PDF 的阅读体验了，只是 Word 只支持九级标题， PDF 实际上是支持无限级标题的，只是似乎一直没有被好好利用，让大家误以为 PDF 也只能支持六级或九级标题。

> * 2020-04-26
手机上的侧边栏，一直一来是只要点击侧边栏上的任何地方，侧边栏都会自动折叠。现在希望点击 `+` `-` 号的时候侧边栏不要折叠起来，只有点击链接的时候侧边栏才折叠。

#2 更新方法
> 1. 下载；
> 2. 解压缩；
> 3. 覆盖。
> 其实你通常只需要更新里面的 js 和 css 两个文件夹里的文件。用它们覆盖你原来的 js 和 css 文件夹即可。

#2 Git 代码库
* github（国外）
    * https://github.com/vagra/kepan-docsify
* gitee（国内）
    * https://gitee.com/pinsa/kepan-docsify

#2 历史版本

* 2020-05-26
[kepan-docsify.4.11.3.10.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.10.zip)

    * Docsify 官方代码更新了一些内容，我跟进了这些更新，其它没做什么改动。这个月的主要精力用来开发[在线转换工具](https://kepan.org/convert) 。

* 2020-05-09
[kepan-docsify.4.11.3.9.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.9.zip)

    * Docsify 官方代码更新了一些内容，我跟进了这些更新。另外侧边栏有小小的优化，一个条目如果没有子节点，前面就不显示 '+/-' 图标。

* 2020-04-26
[kepan-docsify.4.11.3.8.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.8.zip)

    * 左边栏的目录展开层次太深的时候，之前，目录只能自动向下滚动，现在做了改进，让目录也能够自动向右滚动，这样使得当前条目总是会自动保持在侧边栏可见区域之内。

* 2020-04-25
[kepan-docsify.4.11.3.7.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.7.zip)

    * 放弃了引入谷歌字体。
    * 优化了在手机上的界面表现，主要是正文标题和侧边栏。
    * 鉴于 Python 的安装使用不一定方便，增加了 Ran 作为网页服务器，是一个只有 4M 多的 exe ，下载后解压到 kepan-docsify 目录下就可以使用了。

* 2020-04-24
[kepan-docsify.4.11.3.6.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.6.zip)

    * 在侧边栏的目录条目旁边添加了 `+` `-` 按钮，点击可以展开和折叠下级目录。
    * 修正了点击链接再刷新页面后，不会同步滚动的问题。

* 2020-04-21
[kepan-docsify.4.11.3.5.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.5.zip)
    * 增进了侧边栏的功能，让侧边栏可以同步滚动、可以点击展开和折叠。

* 2020-04-16
[kepan-docsify.4.11.3.4.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.4.zip)
    * 修改了一些 css 以更好地适配手机浏览器。稍微调大了手机访问时的字体，并且解决了安卓手机上粗体不能正常显示的问题。

* 2020-04-16
[kepan-docsify.4.11.3.3.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.3.zip)
    * 修改 marked 之后产生了一些 BUG ，这些 BUG 造成了 7 个单元测试失败。现在我已解决了这些问题，单元测试全部通过。直观的表现，就是你能体会到网页加载快了很多。

* 2020-04-15
[kepan-docsify.4.11.3.2.zip](https://kepan.org/docsify/down/kepan-docsify.4.11.3.2.zip)


#2 网页服务器 Ran （燃）
[ran.0.1.4.zip](https://kepan.org/docsify/down/ran.0.1.4.zip)
    * 使用方法参见：[使用 ran 来做网页服务器](../help/ran)
