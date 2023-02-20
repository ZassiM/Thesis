# LaTeX Template
Inofficial template for bachelor and master theses at ika.

# Why
Why should I use this template instead of the so called "official"
[one](https://gitlab.ika.rwth-aachen.de/latex-templates/latex-thesis-template) ?

This template uses `pdflatex` instead of `lualatex` in the "official template".
`pdflatex` is much faster than `lualatex`. The difference compiling a large
document can be of [factor 5](https://tex.stackexchange.com/a/635807). Why wait
25s instead of 5 seconds?

# Cover sheet
Use Word to open and edit the cover sheet template. Insert your data and save
cover sheet as `CoverSheet.pdf` in the root directory.

# Thesis Number
Ask your supervisor for the thesis number and insert it in `main.tex`.

# Glossaries
The glossaries `List of Symbols` and `List of Abbreviations` are automatically
build using the package:

```latex
\usepackage[automake]{glossaries}
```

If you still experience problems building the glossaries you should try the
`automake=immediate` option, which will use the shell escape at the start of
`\makeglossaries` to build the glossaries.

# Bibliography
Bibliography uses `biber` and it is automatically build if you use `latexmk`
for building `main.tex`. The build tool `latexmk` is the standart build command
 for VSCODE and other LaTeX Tools.

# Build instructions with VSCODE
Install the extension `LaTeX Workshop`, naviagte to any `.tex` file, press
<kbd>CTRL</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> and use 
`LaTeX Workshop: Build LaTeX project` to build the main document.


