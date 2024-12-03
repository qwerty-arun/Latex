# Getting Started With Latex
- [Getting started](https://stackoverflow.com/questions/1017055/get-started-with-latex-on-linux)
- [Simple YT Tut](https://www.youtube.com/watch?v=uVM2FcwPCgk&list=PLv6a69CxXDO9UBLkBz7Gh-CQBtmv74Ly_&index=1&pp=gAQBiAQB)
- [Full Tutorial](https://www.youtube.com/watch?v=ydOTMQC7np0)
- [Online Editor](https://www.overleaf.com/)
- [Learn](https://www.overleaf.com/learn)
- [Neovim Setup](https://github.com/latex-lsp/texlab)

# Simple Makefile for Latex file 
```Makefile
output: %.tex
	latex test.tex	

pdf: %.dvi
	pdflatex test.tex 

view: 
	open test.pdf 
```
- Created a playground for Latex just like I did for C++
- The above makefile created some problems
- It kept displaying the old pdf even when I wrote into the file adding changes. My target was just `view`.
- This target just displays the pdf and doesn't update anything no matter what.
# New Makefile
```Makefile
view:
	latex test.tex; pdflatex test.tex; open test.pdf
```
- Yeah! That's all there is to it!
