# nsfc- 国家自然基金项目(面、青、地) LaTeX 模板

## 历史信息

NSFC 官方只有 Word 模版。2019年时，民间有南开大学程明明教授的 LaTeX [模版](http://www.latexstudio.net/archives/9308)和南京航空航天大学戴一冕博士的 [iNSFC](https://github.com/YimianDai/iNSFC)模版。本模版的制作，便始于 2019 年的 iNSFC 模版，原来 iNSFC 许久不更新，后于2024年重启更新。这期间，热心老师也制作了不少其他模版，包括：[Ruzim](https://github.com/Ruzim/NSFC-application-template-latex)、[Readon](https://github.com/Readon/NSFC-application-template-latex)、[huangwb8](https://github.com/huangwb8/ChineseResearchLaTeX)等。

本模版从 2020～2024 共 5 年一直在使用，未出现形式审查问题，这里公布出来给潜在用户做参考。本人 2025 年将继续维护和使用本项目。

## 使用方法

- windows、macOS、overleaf用户都可以在`xx正文.tex`使用以下设置设置；编译器用XeLaTeX；overleaf用户需要注意的是，字体文件夹也要上传到云端：

```latex
%windows、macOS用户都可用
\documentclass[UTF8, punct, oneside]{ctexbook}
\usepackage[windows]{nsfc}
```

- macOS用户还可以使用本机自带的字体，在`xx正文.tex`使用以下设置即可：

```latex
%macOS用户独享
\documentclass[UTF8, punct, oneside]{ctexbook}
\usepackage[macos]{nsfc}
```

## 核对与官方word区别

为了方便大家对比本模版编译后效果和官方word模版的区别，可以使用下述设置：

```latex
%用来对比模版有无变化，正常使用时，请注释掉
\renewcommand{\input}[1]{\vspace{\baselineskip}}
```

免责声明（狗头保命）：

1. 每年模版的文字虽然大差不差，保不齐会有略微改动，请仔细对照文字是否有改动；遇到问题进群交流，或加我微信`fylimas`拉进群（请备注latex）：

   <img src="./figures/IMG.JPG" alt="Image" width="166">

2. 本人及好友在 2020～2024 使用过程中未出现格式审查错误，但并不保证未来情况，请自行决定是否使用（狗头保命）。



## 保持最新（github使用者）

如果本模版有更新，但是你已经写了很多自己的东西了，怎么办呢，更新会不会覆盖掉你自己的东西呢？

方法1: 手动选择把哪个文件拷贝到自己文件夹里替换到相应的文件，这样子你觉得最放心，但是可能心累。

方法2: 利用`.gitignore`机制。其中以`⚠︎`和`⚠︎*/*`，即以⚠︎开头的文件、文件夹均被`git`忽略，所以你个人文件和文件夹只需要以⚠︎开头进行命名即可。`git`下到的文件也不可能覆盖你的⚠︎开头文件和文件夹。

注意：本github仓库为主仓库[https://github.com/fylimas/nsfc](https://github.com/fylimas/nsfc)，gitee仓库[https://gitee.com/fylimas/nsfc](https://gitee.com/fylimas/nsfc)是镜像，方便不可靠网络环境下的访问。