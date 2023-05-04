# MD-to-PDF

MD-to-PDF is a toolkit to convert a markdown file into a PDF file using a LaTeX template.

# Installation

## LaTeX renderer

The compilation script should be adapted to your system depending on the LaTeX installation, on my current installation I use MikTex, so I can compile a LaTeX file into PDF using the command

```
texify --pdf -q --clean --engine=xetex main.tex
```

Since the template uses custom fonts you should use XeLaTeX or LuaLaTeX to compile the template. If you are using a different LaTeX distribution, you should adapt the template.

## Fonts

The template uses the fonts [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) and [Source Code Pro](https://fonts.google.com/specimen/Source+Code+Pro), so those should be installed on your computer.

## SVG rendering

If you want to embed SVG images in your markdown file, you need to install the [Inkscape](https://inkscape.org/) terminal tools and add them to your PATH. On MacOS you can use

```
brew install inkscape
```
