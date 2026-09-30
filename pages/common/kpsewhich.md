# kpsewhich

> Standalone path lookup and expansion for `kpathsea`.
> More information: <https://mankier.com/1/kpsewhich>.

- Find a file in the TeX search path:

`kpsewhich {{file.sty}}`

- Print the value of a kpathsea variable:

`kpsewhich --var-value={{TEXMFHOME}}`

- Print the search path of a file type:

`kpsewhich --show-path={{tex}}`

- Print the complete path expansion of a string:

`kpsewhich --expand-path={{~/texmf}}`

- Print the variable and brace expansion of a string:

`kpsewhich --expand-braces={{$TEXMFHOME/tex/latex}}`

- Search for a file in an explicit path:

`kpsewhich --path={{/usr/share/texmf}} {{file.sty}}`

- Infer the search path from a program name:

`kpsewhich --progname={{fmtutil}} {{file.cnf}}`

- Display version information:

`kpsewhich --version`
