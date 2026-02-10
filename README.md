# nsfc- 国家自然科学基金项目 非官方LaTeX 模板
![Feature](https://img.shields.io/badge/编译器-XeLaTeX-brightgreen)
![Feature](https://img.shields.io/badge/特性-模板更新与用户设置完全分离-brightgreen)

## 使用方法

**【编辑正文】**

修改文件夹中`sections/`,`figures/`,`ref.bib`文件内容，然后编译得到PDF。**不需要修改`xx项目-正文-2026.tex`文件**

**【常规设置】**

阅读并修改`sections/个性化设置.sty`文件。
```latex
%【1】标题颜色
\definecolor{HighLight}{RGB}{0,0,0}
%【2】正文字体设置
\global\MS@kaitrue\global\MS@songfalse%楷体正文
%\global\MS@kaifalse\global\MS@songtrue%宋体正文
%【3】是否屏蔽正文
%\global\MS@offtrue\global\MS@onfalse%屏蔽正文
\global\MS@ontrue\global\MS@offfalse%不屏蔽正文
%【4】设置数学字体
\global\def\selectedmathfont{latinmodern-math}
%可选字体：latinmodern-math，asana-math，cambria-math，
%texgyrebonum-math，texgyreschola-math，
%texgyredejavu-math，texgyretermes-math，texgyrepagella-math
```
**【高阶设置】**

阅读并修改`nsfc.sty`文件。**如非必要，不建议修改。**
如若修改，只建议修改`nsfc.sty`文件的环境{MS}内部的命令。
修改其他地方可能会影响浅蓝色字体部分，这个需要自己小心观察命令间的调用关系。

## 常见问题

**(1) 初次下载方法**

- 🔥点击页面右上部分绿色【<>Code】按钮，点击【Download ZIP】，下载整个项目。

**(2) 后续更新方法**

- 🔥对于后续的小细节更新，一般只需要下载`nsfc.sty`和`xxxx-2026.tex`即可，不需要下载整个项目。
- 🔥平时也可以不更新，定稿前重新下载项目，替换自己的`sections/`,`figures/`,`ref.bib`即可。

**(3) 不能编译**
- （1）对于overleaf用户，要上传所有文件夹到云端；
- （2）要手动设置`XeLaTeX`编译器。
- 清理辅助文件，重新编译

**(4) 不出内容**

- 请回头阅读【常规】部分的设置内容。


每年模版的文字虽然大差不差，保不齐会有略微改动，请仔细对照文字是否有改动；遇到问题可以提issues，可以进群交流，由于无法扫码进群，请加fylimas微信进群备注latex。

## 历史信息

NSFC 官方只有 Word 模版。2019年时，民间有南开大学程明明教授的 LaTeX [模版](http://www.latexstudio.net/archives/9308)和南京航空航天大学戴一冕博士的 [iNSFC](https://github.com/YimianDai/iNSFC)模版🫡。本模版的制作，便始于 2019 年的 iNSFC 模版，原来 iNSFC 许久不更新，后于2024年重启更新。这期间，热心老师也制作了不少其他模版，包括：[Ruzim](https://github.com/Ruzim/NSFC-application-template-latex)、[Readon](https://github.com/Readon/NSFC-application-template-latex)、[huangwb8](https://github.com/huangwb8/ChineseResearchLaTeX)等🫡。

本模版从 2020～2025 共 6 年一直在使用，未出现形式审查问题，windows、macOS、overleaf、linux用户都可以使用。这里公布出来给潜在用户做参考。

- 根据20260104基金委公布的青年基金2026版新模版进行更新。
- 根据20260105最新版青年基金2026版、面上基金2026版进行更新。
- 根据20260118指南发布后的面上、地区、青C、青B、青A模版更新。
- 20260124：取消release下载，避免下载到历史版本。
- 20260201：增加多个数学字体的可选项
