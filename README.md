自用的一个 LaTeX 配置宏包

## 用法

+ 将 xyzsettings.sty 文件和 \*.tex 源文件放在同一目录下。
+ 在导言区加上：`\usepackage{xyzsettings}`

+ 用`xelatex`命令编译源文件。

## 关于字体

配置宏包里使用的中文字体是免费的方正书宋简体（FZSSJ.OTF）、方正黑体简体（FZHTJ.OTF）、方正楷体简体（FZKTJ.OTF）。需要在[方正字库官网](https://www.foundertype.com/)下载这三款字体，放置在 \*.tex 源文件的目录下，再进行编译，否则会出错。若要使用 LaTeX 发行版默认的字体，那么将 xyzsettings.sty 中的`\setCJKmainfont`命令、`\setCJKfamilyfont`命令以及相关的`\newcommand`命令注释掉。

## 注

严格意义上讲，这并不能算是一个模板，只是我在学习使用 LaTeX 写作的过程中，将多个源文件导言区部分的配置分离出来，写成一个配置宏包，方便调用和修改。

此外，模板更适合写成 \*.cls 文档类的形式；在 \*.sty 中导入很多宏包（不管最终有没有用到）也不是特别妥。但受限于我的技术水平，目前还不能做到尽善尽美。但人总是会成长的对不，希望我的 LaTeX 模板能写得越来越好。

O(∩_∩)O~