# ieee-MTT-latex
Short script for creating markdown to MTT latex format

* [Already done](https://miki725.com/2019/10/15/markdown-to-pdf-ieee.html)
* [more ieee ](https://blog.kdheepak.com/writing-papers-with-markdown.html)

```
pandoc -s -S --latex-engine=pdflatex \
--template=./templates/ieee-latex.template \
--filter pandoc-fignos \
--filter pandoc-eqnos \
--filter pandoc-tablenos \
--filter pandoc-citeproc \
--csl=./styles/ieee.csl \
--bibliography=./bib/research.bib \
-o ieee-paper.pdf paper.md
```

https://ineed.coffee/post/how-to-write-an-acm-styled-conference-paper-using-markdownpandoc.html


# Consise but not right
[asdf](https://github.com/miki725/md2pdf-ieee)
