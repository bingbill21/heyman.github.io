今天给大家介绍一款最近发现的功能十分强大，颜值非常高的一款终端工具。这个神器我是在其他公众号文章上看到的，但他们都没把它的强大之处介绍明白，所以我自己体验一波后，再向大家分享自己的体验。

这款神器就是—— `WindTerm` ！

之前我也用过很多终端工具，比如 SecurCRT 、XShell、Putyy、MobaXterm。但我第一眼看到 `WindTerm` ，还是被深深吸引住了。

![](https://pic2.zhimg.com/v2-99a59eb06b6e51dd99e8f25c0debc13d_b.jpg)

![](https://pic2.zhimg.com/80/v2-99a59eb06b6e51dd99e8f25c0debc13d_720w.webp)

它是一款 C 语言开发的跨平台（Windows、MacOS、Linux） SSH 客户端，完全免费用于商业和非商业用途，没有限制。 所有发布的源代码（第三方目录除外）均在 Apache-2.0 许可条款下提供。

**主要功能特性：**

- 支持 SSH、Telnet、Tcp、Shell、Serial
    
- 支持 SSH v2、Telnet、Raw Tcp、串行、Shell 协议。
    
- 会话认证时支持 SSH 自动执行。
    
- 支持 SSH ControlMaster。
    
- 支持 SSH ProxyCommand 或 ProxyJump。
    
- 支持 SSH 代理转发。
    
- 支持使用密码、公钥、键盘交互、gssapi-with-mic 的 SSH 自动登录。
    
- 支持 X11 转发。
    
- 支持直接/本地端口转发、反向/远程端口转发和动态端口转发。
    
- 支持 XModem、YModem 和 ZModem。
    
- 集成 sftp、scp 客户端，支持下载、上传、删除、重命名、新建文件/目录等。
    
- 集成本地文件管理器，支持移动到、复制到、复制自、删除、重命名、新建文件/目录等。
    
- 支持 Windows Cmd、PowerShell 和 Cmd、PowerShell 作为管理员。
    
- 支持 Linux bash、zsh、powershell core 等。
    
- 支持 MacOS bash、zsh、powershell core 等。
    

结合我这几天的使用体验，跟大家分享一些着实让我震撼的特性。

> 以下动图来自作者博客，本想自己录制，结果录出来 gif 文件很大，有木有小伙伴教教我？

## 一、WindTerm强大之处

### 1\. 自动补全功能

自动补全功能简直是我们程序员的福音！想想我们在写代码的时候，自动补全功能节约了我们多少时间？

`WindTerm` 居然也自带自动补全功能，这我还是第一次在终端工具里见到。之前我们敲命令，都通过不断敲击 `Tab` 键来补全命令，这下好了，都不用敲 `Tab` 键了。

![](https://pic4.zhimg.com/v2-47fa224c85ab01dd7ff60630d50be193_b.gif)

![动图封面](https://pic4.zhimg.com/v2-47fa224c85ab01dd7ff60630d50be193_b.jpg)

### 2\. 强大的历史回溯功能

一般情况下，我们需要查看之前输入过的命令，都是使用 `history` 命令。而 `WindTerm` 则直接在右侧给你带了一个历史命令的窗口，你连 `history` 命令也都省了！

![](https://pic1.zhimg.com/v2-77c642e9150252a3dedf94c1d9c98154_b.jpg)

![](https://pic1.zhimg.com/80/v2-77c642e9150252a3dedf94c1d9c98154_720w.webp)

而且它还有筛选功能，你甚至都不用再 `grep` 了，这贴心程度简直了！

你要重新执行某条命令，就双击一下对应的命令就行了。而在之前，我们还需要记住历史命令的编号，再用 `!` 重新执行。

当然你依然也可以使用 `!` ，只不过他又顺带给你加强了。你不仅可以重新执行当前会话的命令，还可以回溯其它会话你输入过的命令！

![](https://pic4.zhimg.com/v2-bd6ff5da76e90ac2042d06d1c5cc3563_b.gif)

![动图封面](https://pic4.zhimg.com/v2-bd6ff5da76e90ac2042d06d1c5cc3563_b.jpg)

### 3\. 快速命令

所谓的快速命令，就是类似于脚本，你可以把要执行的命令放在快速命令里，然后执行这个快速命令，它就会把里面的命令按次序执行。

有点拗口是不是？给个图大家就明白了。

![](https://pic1.zhimg.com/v2-07ab364c27e854bb9d16f1ddd42e1234_b.jpg)

![](https://pic1.zhimg.com/80/v2-07ab364c27e854bb9d16f1ddd42e1234_720w.webp)

（这个窗口怎么出来的？点击右下角的小齿轮就可以了）

然后，点击左下角你起的快速命令的名称，就可以自动按顺序执行你刚刚输入的那些命令了。

![](https://pic3.zhimg.com/v2-9295a8128dce65a8de7847e5cd2f1e7e_b.jpg)

![](https://pic3.zhimg.com/80/v2-9295a8128dce65a8de7847e5cd2f1e7e_720w.webp)

如果你不会写脚本的话，那这个功能也是一个福音。（还有程序员不会写脚本？？赶紧拍一拍我文末的课程吧【笑脸】）

### 4\. 自由输入模式

在其它终端工具里，我们输入命令的时候，只能从按顺序来敲字母，如果中间忘记敲某个选项或参数，就需要移动光标回去补一下。

早期计算机没有鼠标，这样的操作无可厚非。

但现在，几乎所有的文本编辑器都支持鼠标操作，比如点击某个位置再输入文字，选中文字删除，拖动文字到其它位置等等。

我所见过的其它终端工具基本也不支持这样的操作，但是 `WindTerm` 它居然支持！！不仅仅在命令窗口，也支持 `Vim` 、`Emac` 等等编辑器！

使用起来的效果，跟 Word 极其类似！

想怎么插入就怎么插入，想怎么删就怎么删，想怎么拖动就怎么拖动，就是这么方便！

### 5\. 高度自定义界面

我们可以看到，`WindTerm` 的界面含有非常多的内容，但有些栏目可能不是我们所需要的，那就可以去掉，或者自定义。

这种可订制的界面真的也十分强大！

**自定义栏目：**

![](https://pic4.zhimg.com/v2-00f2219eedd8ccef3fd9bca771c0adc3_b.gif)

![动图封面](https://pic4.zhimg.com/v2-00f2219eedd8ccef3fd9bca771c0adc3_b.jpg)

**自定义Dock：**

![](https://pic1.zhimg.com/v2-871393c7003e187ae905a9963fac9a60_b.gif)

![动图封面](https://pic1.zhimg.com/v2-871393c7003e187ae905a9963fac9a60_b.jpg)

**分屏功能：**

![](https://pic3.zhimg.com/v2-f91f18894c5683eb7121021feea41b7e_b.gif)

![动图封面](https://pic3.zhimg.com/v2-f91f18894c5683eb7121021feea41b7e_b.jpg)

### 6\. 同步输入功能

如果是运维工程序员的话，可能会有这样的需求，就是对多台服务器同时输入某条命令。

其它终端工具不知道（我用过的还没见到过），`WindTerm` 已经实现了这样的需求，又是一大神奇的功能！

![](https://pic3.zhimg.com/v2-cc22677ff8f0389129c0b8561ed74036_b.gif)

![动图封面](https://pic3.zhimg.com/v2-cc22677ff8f0389129c0b8561ed74036_b.jpg)

其实 `WindTerm` 还有很多强大的功能，比如文件上传下载、自动锁屏、跳板机、XModem、YModem、ZModem，等等。

限于篇幅，这些特性就不展开了，大家可以自行使用感受一下。

## 二、常用设置

**创建会话**

菜单 --> 会话 --> 新建会话

在弹出的窗口里输入主机名，其余的默认即可。当然你如果想设置标签，想分组，它也是支持的。

![](https://pic2.zhimg.com/v2-b743417b04b05c27ed45ad7f05b99335_b.jpg)

![](https://pic2.zhimg.com/80/v2-b743417b04b05c27ed45ad7f05b99335_720w.webp)

再输入用户名：

![](https://pic1.zhimg.com/v2-feb43b10d498d8cce3dbdfebfe7293bc_b.jpg)

![](https://pic1.zhimg.com/80/v2-feb43b10d498d8cce3dbdfebfe7293bc_720w.webp)

**自动复制选中内容**

我一般使用习惯是，鼠标选中文字自动复制，然后右击自动粘贴。不过现在很多终端都没有默认开启这样的功能，需要手动开启。

菜单栏 --> 会话 --> 首选项 --> 设置

![](https://pic3.zhimg.com/v2-c80fa2eb2d885ae3f92a734f871f4a1e_b.jpg)

![](https://pic3.zhimg.com/80/v2-c80fa2eb2d885ae3f92a734f871f4a1e_720w.webp)

**开启右键点击粘贴文本功能**

菜单栏 --> 会话 --> 首选项 --> 设置

![](https://pic4.zhimg.com/v2-e914189c7be7ad1e83b74199d56de797_b.jpg)

![](https://pic4.zhimg.com/80/v2-e914189c7be7ad1e83b74199d56de797_720w.webp)

**关闭鼠标悬停在标签上自动激活标签功能**

`WindTerm` 有个功能我不是很喜欢，就是你把鼠标放在标签上，它就自动激活那个标签。我们可以手动关闭这个功能。

菜单栏 --> 会话 --> 首选项 --> 设置

![](https://pic4.zhimg.com/v2-67b0a974ee48d5e9e05f1f7b00349c9f_b.jpg)

![](https://pic4.zhimg.com/80/v2-67b0a974ee48d5e9e05f1f7b00349c9f_720w.webp)

## 三、小结