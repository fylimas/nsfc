# YSF - 国家自然基金青年项目 LaTeX 模板

NSFC 官方只有 Word 模版，民间有南开大学程明明教授的 LaTeX [模版](http://www.latexstudio.net/archives/9308)和南京航空航天大学戴一冕博士的 [iNSFC](https://github.com/YimianDai/iNSFC)模版。

本 YSF 模版即修改自 2019 年的 iNSFC 模版，原来 iNSFC 已经许久不更新，貌似也没有继续更新计划了。
经历 3 年的使用和打磨，特别为 macOS 系统做适配，同时应同行鼓励，对windows系统做适配，这里公布出来给潜在用户做参考。

macOS用户应该在`2022正文.tex`使用以下两个宏包的option即可：

```latex
%macOS用户
\documentclass[UTF8, punct,fontset=mac,oneside]{ctexbook}
\usepackage{nsfcysf}
```

windows用户应该在`2022正文.tex`使用以下两个宏包的option即可：

```latex
%windows用户
\documentclass[UTF8, punct,fontset=windows,oneside]{ctexbook}
\usepackage[windows]{nsfcysf}
```

注意：

1. 每年模版的文字可能会有略微改动，请仔细对照文字是否有改动，有的话可提交更改；
2. 本人及好友使用过程中未出现格式审查错误，但并不保证未来情况，请自行决定是否使用。