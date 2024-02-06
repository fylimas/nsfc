# nsfc- 国家自然基金项目(青年+面上) LaTeX 模板

NSFC 官方只有 Word 模版，民间有南开大学程明明教授的 LaTeX [模版](http://www.latexstudio.net/archives/9308)和南京航空航天大学戴一冕博士的 [iNSFC](https://github.com/YimianDai/iNSFC)模版。

本 YSF 模版即修改自 2019 年的 iNSFC 模版，原来 iNSFC 已经许久不更新，貌似也没有继续更新计划了【2024年重启更新】。
经历 4 年的使用和打磨，特别为 macOS 系统做适配，同时应同行鼓励，也对windows系统做适配，这里公布出来给潜在用户做参考。

## 使用方法

windows和macOS用户都可以在`xx正文.tex`使用以下设置设置：

```latex
%windows、macOS用户都可用
\documentclass[UTF8, punct, oneside]{ctexbook}
\usepackage[windows]{nsfc}
```

macOS用户还可以使用本机自带的字体，在`xx正文.tex`使用以下设置即可：

```latex
%macOS用户独享
\documentclass[UTF8, punct, oneside]{ctexbook}
\usepackage{nsfc}
```

## 核对与官方区别

为了方便大家对比本模版和官方模版编译效果的区别，可以使用下述设置：

```latex
%用来对比模版有无变化，正常使用时，请注释掉
\renewcommand{\input}[1]{\vspace{\baselineskip}}
```

免责声明（狗头保命）：

1. 每年模版的文字虽然大差不差，保不齐会有略微改动，请仔细对照文字是否有改动，有的话可提issues，发邮件`fylimas@mail.ustc.edu.cn`，发微信`fylimas`；

2. 本人及好友使用过程中未出现格式审查错误，但并不保证未来情况，请自行决定是否使用（狗头保命）。

   
   

## 保持最新

如果本模版有更新，但是你已经写了很多自己的东西了，怎么办呢，更新会不会覆盖掉你自己的东西呢？

方法1: 手动选择把哪个文件拷贝到自己文件夹里替换到相应的文件，这样子你觉得放心，但是可能心累。

方法2: 利用`.gitignore`机制。其中以`⚠︎`和`⚠︎*/*`，即以⚠︎开头的文件、文件夹均被`git`忽略，所以你个人文件和文件夹只需要以⚠︎开头进行命名即可。`git`下到的文件也不可能覆盖你的⚠︎开头文件和文件夹。