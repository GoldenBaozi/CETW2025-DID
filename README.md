# CETW-2025 论文笔记和汇报模板

请将笔记写在`./didNotes.tex`中，将slides写在`./didSlides.tex`中，也可以写成单独的文件放在`./src/`目录下，然后`\input`进入这两个文件，便于维护。

若希望本地编译文件，请确保安装了`./package-requirements.txt`中写明的latex包，以及系统中安装了 Times New Roman, Arial 和 KaiTi 等字体（MacOS可能没有这些字体，或者名字不一样）

强烈建议安装`latexmk`（用`tlmgr`即可安装），然后使用我设置好的`.latexmkrc`进行一键快速编译（xelatex -> xelatex -> biber -> xelatex）

在该目录下运行：
- `latexmk <filename>` 编译文件得到pdf
- `latexmk -C` 清除编译文件

可以把引用的论文用纯文本写在tex文件里，如果希望精细一点，可以用biblatex来引用，把bibitem写在`./src/ref.bib`里面