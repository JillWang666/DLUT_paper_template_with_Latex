# DLUT_paper_template_with_Latex
于2020/12/30首次上传
---------------------------------------------
大家好，你现在看到的是由我编写的
大连理工大学本科生毕业设计论文的Latex模板
基于的版本是2019年10月的官方word模板，你可以在项目文件里找到它，我已经把它转成了.pdf文件

编译环境是：win10，texlive2018，texstudio（2.12.16）
为什么用这么老的texstduio：因为懒得更（主要是镜像没法访问QAQ）
你可以在：https://blog.csdn.net/lvshu_yuan/article/details/80468425 上下载和安装他们
我也会在项目中上传全部的支撑文件
编译器选择pdflatex，在texstudio里直接修改全域字体为12pt宋体和125%行距

你需要安装gbt7714-2019的文献引用格式，它同时支持中英文文献
访问：https://github.com/CTeX-org/gbt7714-bibtex-style 应该可以解决你关于这个包的全部问题

你可以关注b站帐号：经理和大桁
我会在近期更新这个模板的使用和思路，任何人反馈的任何问题我都会拍成视频作为答复
欢迎大家一起帮我更新迭代，现在的bug还“非常多”
---------------------------------------------
---------------------------------------------
2020/12/30更新：
目前未修复的BUG
1. \section,\subsection,\subsubsection 环境下的标题是自动加粗的；
2. CTEX的12pt宋体和word下的小四宋体“好像不一样大”；
3. 《附录A》这个标题的A，和周围的字体不一样大。
目前需要优化的代码：
1. \section,\subsection,\subsubsection 环境下的设置不是全域的，每次新增他们都要把行距和字体格式打进去；
2. 在插入图片的时候，“图1”的后面需要2个空格，目前的解决办法是\caption{\ \ }，手动把两个空格加进去，也不说全域的；
3. 目录现在为了实现要求的字体和字号，需要直接修改.toc文件再进行一次编译，麻烦而且容易出错，方法如下：
把.toc文件的 \contentsline {section}{\numberline {1}\fontsize {15}{22.5} {\heiti 示例}}{2}{section.1}
修改为       \contentsline {section}{\numberline {1} \zihao{-4}{示例}}{2}{section.1}
很麻烦对吧QAQ。

