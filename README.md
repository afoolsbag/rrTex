# zhengrr 所知的 TeX

[*TeX*](https://tug.org/ "TeX, 1978")

Donald Ervin Knuth（高德纳）

[*LaTeX*](https://latex-project.org/ "LaTeX, 1983")

Leslie Lamport（莱斯利·兰波特）

## 参考

[*CTAN*](https://ctan.org/ "Comprehensive TeX Archive Network, 1992") <sub>
    [*mirrors*](http://mirrors.ctan.org/) </sub>

[*CTeX*](http://ctex.org/ "Chinese TeX")

TeX 发行版
| [*TeX Live*](https://tug.org/texlive/ "TeX Live, 1996")
| [*MacTeX*](https://tug.org/mactex/ "MacTeX, 2005")
| [*MiKTeX*](https://miktex.org/) <sub>
      [*proTeXt*](https://tug.org/protext/) </sub>

## 指南

| ["李东风 LaTeX 排版心得"](http://www.math.pku.edu.cn/teachers/lidf/docs/textrick/tricks.pdf)

| [*The TeXbook*](http://www.ctex.org/documents/shredder/src/texbook.pdf)
| [*LaTeX 2e - The macro package for TeX*](http://www.ctex.org/documents/shredder/src/latex2e.pdf)
| [*The Not So Short Introduction To LaTeX*](http://www.ctex.org/documents/shredder/src/lshort.pdf) <sub>
      [*zh-CN*](http://mirrors.ctan.org/info/lshort/chinese/lshort-zh-cn.pdf) </sub>

### TeXstudio 指定构建目录

*   Option > Configure TeXstudio > Commands
    *   LaTeX `latex.exe -src -interaction=nonstopmode -aux-directory=build -output-directory=dist %.tex`
    *   PdfLaTeX `pdflatex.exe -synctex=1 -interaction=nonstopmode -aux-directory=build -output-directory=dist %.tex`
    *   XeLaTeX `xelatex.exe -synctex=1 -interaction=nonstopmode -aux-directory=build -output-directory=dist %.tex`
    *   LuaLaTeX `lualatex.exe -synctex=1 -interaction=nonstopmode -aux-directory=build -output-directory=dist %.tex`
    *   ...
    *   BibTeX `bibtex.exe -include-directory=build build\%`
    *   ...
    *   Biber `biber.exe build\%`
    *   ...
*   Option > Configure TeXstudio > Build (Show Advanced Options) > Additional Search Paths
    *   Log File `build`
    *   PDF File `dist`

## 许可

项目采用 Unlicense 许可，文档采用 CC0-1.0 许可：

<p xmlns:dct="https://purl.org/dc/terms/">
  <a rel="license"
     href="https://creativecommons.org/publicdomain/zero/1.0/">
    <img src="https://licensebuttons.net/p/zero/1.0/88x31.png" style="border-style: none;" alt="CC0" />
  </a>
  <br />
  To the extent possible under law,
  <span resource="[_:publisher]" rel="dct:publisher">
    <span property="dct:title">zhengrr</span></span>
  has waived all copyright and related or neighboring rights to this work.
</p>
