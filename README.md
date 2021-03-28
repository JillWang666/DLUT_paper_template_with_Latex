# DLUT_paper_template_with_Latex  
于2020/12/30首次上传   
任何问题反馈：  
Email:  hebefans@163.com  
   QQ:  2635217964   
   
---------------------------------------------  
老版本环境：win10，texlive2018，texstudio（2.12.16） 编译器选择pdflatex，在texstudio里直接修改全域字体为12pt宋体和125%行距    
新版本环境：win10，texlive官方最新版，vscode   
后面你还能看到老版的编译环境    
---------------------------------------------  
大家好，你现在看到的是由我编写的  
大连理工大学本科生毕业设计论文的Latex模板  
基于的版本是2019年10月的官方word模板，你可以在项目文件里找到它，我已经把它转成了.pdf文件    
  
你需要安装gbt7714-2019的文献引用格式，它同时支持中英文文献  
访问：https://github.com/CTeX-org/gbt7714-bibtex-style 应该可以解决你关于这个包的全部问题  
 
欢迎大家一起帮我更新迭代，感兴趣的话就点个赞和watch~
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
---------------------------------------------    
---------------------------------------------  
2020年12月31日更新：  
修改了目录里的“参考文献”没有空格的问题
---------------------------------------------    
---------------------------------------------  
2020年12月31日更新：  
上传了视频说明（已删除）  
---------------------------------------------    
---------------------------------------------  
2021年2月24日更新：   
添加了对应的三个封面页，目前还处于脚手架版，完善可用的版本将尽快发布
---------------------------------------------    
---------------------------------------------  
2020年3月20日更新：  
加入了新版本代码，移植到了vscode上  
将不再维护老版本的代码  
示例正文后面的“结论”，“参考文献”等部分还没改动，和前面时一样的，大家自己操作吧，主要是为了代码一致性，不改也行  
目前的BUG：  
1. 页码的样式和少部分序号不对  
2. 目录还需要手动改  
3. 英文有莫名的加粗  
4. 整体使用伪加粗，会比正常的粗体看起来更粗一点  
5. 无法解决的一个问题，换行逻辑和word不同，不会像word里一样自动适配，将文字挤在一行  
---------------------------------------------    
---------------------------------------------  

