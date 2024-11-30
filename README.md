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
