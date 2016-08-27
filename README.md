# 嗨，这里是CQUThesis！
[![CTAN release](https://img.shields.io/ctan/v/cquthesis.svg?label=CTAN)](https://www.ctan.org/pkg/cquthesis)
[![GitHub release](https://img.shields.io/github/release/nanmu42/cquthesis.svg?label=Github)](https://github.com/nanmu42/CQUThesis/releases/latest)
[![GitHub commits](https://img.shields.io/github/commits-since/nanmu42/CQUThesis/v1.14.svg)](https://github.com/nanmu42/CQUThesis/commits/master)

CQUThesis表示的是**C**hong**Q**ing **U**niversity **Thesis**.

本宏包是重庆大学毕业论文的`\LaTeX{}`模板，支持学士、硕士、博士论文的排版。合理使用本宏包可以大大减轻重庆大学毕业生在毕业论文撰写过程中的排版工作量。
	
CQUThesis根据重庆大学《重庆大学本科设计（论文）撰写规范化要求（2007年修订版）》和《重庆大学博士、硕士论文撰写格式标准（2007年修订版）》编写，力求合规，简洁，易于实现，用户友好。

# 模板特色
* 支持重庆大学本科（文学、理工）、硕士（学术、专业）、博士的毕业论文格式；
* 内置封面、目录、索引、授权书等论文部件，可按需自动生成；
* 自动侦测文档页数，生成相应的单面打印/双面打印PDF文件；
* 预置一批优化过的宏包和小功能，包含中英双语题注及配套图录、表录，国际标准单位、化学式支持、三线表等，可按需开启；
* 支持基于cwl文件的代码着色和补全，makefile功能能够在Linux, Mac, Windows三平台通用。

![CQUThesis-Poster](https://cloud.githubusercontent.com/assets/8143068/15363773/68c6b380-1d4c-11e6-9627-4d892facb333.png)

# 获取CQUThesis
## 下载
版本	|	下载地址	|	描述
---	|	---		|	---
开发版	|[点我下载](https://github.com/nanmu42/cquthesis/zipball/master)	|	推荐，最新的功能，最快的BugFix
预发行版 | [Github下载页面](https://github.com/nanmu42/CQUThesis/releases) | 累计有较大更改时更新
发行版	|[CTAN下载页面](https://www.ctan.org/pkg/cquthesis)|	定期从预发行版更新，和TeX Live等发行版一同发行

排版示例和用户文档随版本发布，如果需要单独下载，请参阅后文。

## 部署
CQUThesis的安装十分便利。下载CQUThesis的.zip压缩包后请将整个文件夹解压出来，进入文件夹后：

* Windows用户可以直接双击运行`makewin.bat`
* Linux 和 Mac 用户请在Bash窗口中进行如下操作：
```
cd path/to/cquthesis
make thesis
```

即可完成 CQUThesis 的安装和示例文档的编译。以上也是CQUThesis推荐的论文编译方式。

## 编译方式
CQUThesis提供了支持全平台的Makefile来完成论文编译，大部分编译工作基于`latexmk`，能够有效利用中间文件提高编译效率，实现一键编译。

* Windows用户请在文件夹空白处按住Shift键再点击书鼠标右键，选择“在此处打开命令窗口”，运行下列命令：
```
makewin help
```
可查询makewin.bat的详细用法（推荐熟悉，事半功倍）。

* Linux用户和Mac用户可打开 Makefile 文件查看相关用法。

## 更新
CQUThesis的升级很方便，下载最新的开发版，将zip文件中的`cquthesis.dtx`和`cquthesis.ins`覆盖掉工作文件夹中的相应文件后：

* Windows用户请在文件夹空白处按住Shift键再点击书鼠标右键，选择“在此处打开命令窗口”，运行下列命令：
```
makewin extract
```

* Linux 和 Mac 用户请在 Bash 窗口中进行如下操作：
```
cd cquthesis
make cls
```
即可完成 CQUThesis 的升级。


#  文档 
文档涵盖了CQUThesis的使用方法、注意事项、实现方式，推荐阅读以快速上手：

	文档 | 描述
	--- | ---
 排版示例 |	请编译`main.tex`获得
 用户文档 |	随模板发布，也可[点我下载](https://github.com/nanmu42/CQUThesis/raw/master/cquthesis.pdf)

# 提问和支持
* [Github Issues](https://github.com/nanmu42/CQUThesis/issues)
* 加入[重庆大学TeX用户组](http://jq.qq.com/?_wv=1027&k=2HvYu95)寻求支持

# 用户协议
1. 本模板按照[LaTeX Project Public License](https://latex-project.org/lppl/lppl-1-3.txt)发布，协议版本号为1.3或以后的任何版本（随你意）。本条款不适用于重庆大学LaTeX模板工具箱（CQUThesis Toolkit）；
1. 重庆大学教务处和研究生院只提供毕业论文写作指南，不提供官方模板，也不会授权或认证第三方模板为官方模板。
这个模板是按照写作指南的参考实现，模板作者自当尽力，但不保证审查老师不提意见。任何由于本模板而引起的论文格式审查问题与本模板作者无关。

# About CQUThesis
CQUThesis stands for Chongqing University Thesis Template for LaTeX, bearing the ability to support bachelor, master, doctor dissertations with grace and speed.

# 致谢 / Acknowledgements
这个模板是站在巨人肩膀上的成果，感谢LaTeX 2e计划，感谢[CTeX社区](https://github.com/CTeX-org/ctex-kit)提供的中文解决方案，感谢薛瑞尼副教授的[先驱之作](https://github.com/xueruini/thuthesis)，感谢[中国科学技术大学TeX用户组](https://github.com/ustctug/gbt-7714-2015)。向你们致以真诚的问候和感激！

世界因你们更美好。

The author would like to acknowledge these contributors for their efforts and, essentially, beautiful mind:

* [The CTeX Community](https://github.com/CTeX-org/ctex-kit)
* [XUE, Ruini](https://github.com/xueruini/thuthesis)
* [USTC TeX User Group](https://github.com/ustctug/gbt-7714-2015)

# 关于CQUThesis Toolkit
重庆大学LaTeX模板工具箱（CQUThesis Toolkit）是为了增强CQUThesis而提供的额外文件和程序，这些内容往往是对CQUThesis易用性或功能的增强，没有它们，CQUThesis仍然可以良好地独立运行。

这些内容有着自己的授权方式和简单的用户协议，不会随本模板的CTAN版本发布，CQUThesis的Github源是这些内容唯一的官方源，程序的更新和修正都会在这里进行。
