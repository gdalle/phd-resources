---
permalink: /tutorials/latex/
title: LaTeX
---

[LaTeX](https://www.latex-project.org/) is the reference software to edit scientific documents and articles.

## Setting up LaTeX

There are two main ways to create LaTeX documents: online and offline.

### Online use

The online way is easier at first. [Overleaf](https://www.overleaf.com/) is an online collaborative editor that takes the pain out of LaTeX. All the necessary packages are automatically installed and up-to-date, while collaboration is made easy by the comment system and the possible GitHub synchronization.

### Offline install

However, using LaTeX offline has its benefits too. In that case, you will need two ingredients: a LaTeX distribution and an editor.

To install a distribution, go to [this page](https://www.latex-project.org/get/) and download the one corresponding to your OS. I recommend:

- [Texlive](https://www.tug.org/texlive/quickinstall.html) for Linux
- [MacTex](https://www.tug.org/mactex/mactex-download.html) for OSX
- [MikTex](https://miktex.org/download) for Windows
  
If you have enough disk space, download the full distribution at once, so that you don't have to install additional packages one by one when you need them.

As for the editor, there are specialized LaTeX editors such as [TeXMaker](https://www.xm1math.net/texmaker/) or [TexStudio](https://www.texstudio.org/). However, I would recommend using a general-purpose IDE such as [VSCode](../tutorials/vscode.md) with the [LaTeX Workshop extension](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop), in order to have a single tool for all of your writing and programming needs.

## Learning LaTeX

Unlike WYSIWYG alternatives such as Microsoft Word and LibreOffice Writer, LaTeX separates the content from the form. As a result, writing LaTeX is a bit like writing source code. Overleaf has a series of great [tutorials](https://fr.overleaf.com/learn) that will teach you the basics, but the only way to get fluent is through practice! If you prefer interactive tutorials where you can test and modify code to experiment, [learnlatex.org](https://www.learnlatex.org/en/) is the way to go.

If you come from the social sciences, check out [LaTeX appliqué aux sciences humaines](http://tug.ctan.org/info/latex-sciences-humaines.pdf).

## Advanced tips

### Configuration and packages

- A detailed collection of [LaTeX tips](https://github.com/RiMillo/LaTeX_tips) gathered by a fellow student
- My personal LaTeX [configuration](https://github.com/gdalle/LaTeX-packages)

### Templates

Overleaf hosts a great [collection of templates](https://www.overleaf.com/latex/templates). I found a few interesting things there, most notably:

- A simple model for [conference posters](https://fr.overleaf.com/articles/decaf-poster/ryfhdpmwcnpd)
- A nice two-column [resume](https://github.com/liantze/AltaCV)

### Drawing

The [Tikz](https://www.overleaf.com/learn/latex/TikZ_package) package allows you to draw anything you want. Take a look at the [Overleaf tutorial](https://www.overleaf.com/learn/latex/LaTeX_Graphics_using_TikZ%3A_A_Tutorial_for_Beginners_(Part_1)%E2%80%94Basic_Drawing) to learn more.

If you are too lazy to use Tikz directly, there are WYSIWYG alternatives such as [Tikzit](https://tikzit.github.io/). The same goes for [equations](https://latex.codecogs.com/eqneditor/editor.php) by the way.
