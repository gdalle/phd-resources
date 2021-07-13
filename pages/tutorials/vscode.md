---
layout: page
title: VSCode
subtitle: One text editor to rule them all
---

## Why you need an IDE

### The problem with multiple languages

As a researcher, especially in scientific fields, you are likely to need several programming or markup languages to get the job done. For instance, I regularly have to open

- LaTeX, Markdown and PDF files for scientific writing
- Julia and Python files for programming
- JSON and CSV files for data analysis
- HTML files for web development
  I also frequently have to run and debug programs, compile LaTeX documents or perform other commands like Git version control.

Of course, it is possible to use dedicated software for each kind of file, but it becomes tiresome after a while. Having a unique interface is not only pleasant, but it allows you to get comfortable with a single set of shortcuts, reflexes and workflows regardless of what you work on.

### What is VSCode?

This is why I recommend using an Integrated Development Environment (IDE), which is a fully customizable environment that allows you to edit and run code in basically every language. The one I use is [VisualStudio Code](https://code.visualstudio.com/), which is free but provided by Microsoft. Note that an open source version exists, it is called [VSCodium](https://vscodium.com/), which includes the exact same set of functionalities but without Microsoft telemetry.

Other well-known alternatives include [Atom](https://atom.io/) and [SublimeText](https://www.sublimetext.com/).

## Setting it up

### Installation

To download VSCode, go to the [download page](https://code.visualstudio.com/Download) and select the version corresponding to your OS. When you launch it for the first time, be sure to synchronize your settings with your GitHub account, so you can recreate the same environment on multiple computers.

To download Codium, do the same from this [download page](https://github.com/VSCodium/vscodium/releases). Usually you will need to retrieve `VSCodiumSetup-x64-?.??.?.exe` on Windows, `VSCodium.x64.?.??.?.dmg` on OSX and `codium_?.??.?-??????????_amd64.deb`.

From this point onwards, it doesn't matter which one you chose.

## Extensions

The success of VSCode is partly due to a great catalogue of extensions. For every programming language, there is usually one VSCode extension that does everything you need. Here is a list of the ones I use.

| Function     | Useful extensions                                                                                                                                                                                                                                                                                               |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Git          | [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens), [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory)                                                                                                                                      |
| Julia        | [Julia](https://marketplace.visualstudio.com/items?itemName=julialang.language-julia), [Julia Formatter](https://marketplace.visualstudio.com/items?itemName=singularitti.vscode-julia-formatter), [Julia Color Themes](https://marketplace.visualstudio.com/items?itemName=cameronbieganek.julia-color-themes) |
| Jupyter      | [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)                                                                                                                                                                                                                               |
| LaTeX        | [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop), [LTeX](https://marketplace.visualstudio.com/items?itemName=valentjn.vscode-ltex)                                                                                                                                 |
| Markdown     | [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one), [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)                                                                                     |
| Python       | [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)                                                                                                                                                                                                                                  |
| R            | [R](https://marketplace.visualstudio.com/items?itemName=Ikuyadeu.r)                                                                                                                                                                                                                                             |
| Zettelkasten | [Foam](https://foambubble.github.io/foam/)                                                                                                                                                                                                                                                                      |
| Zotero       | [Citation Picker for Zotero](https://marketplace.visualstudio.com/items?itemName=mblode.zotero)                                                                                                                                                                                                                 |
| Esthetics    | [VSCode Great Icons](https://marketplace.visualstudio.com/items?itemName=emmanuelbeziat.vscode-great-icons)                                                                                                                                                                                                     |

## Using VSCode

Although a powerful IDE can be intimidating at first, there are only a few things to remember:

- The left column contains shortcuts for the most important functionalities (file explorer, search, Git, extensions) as well as the settings and the user profile.
- The top bar contains the menu, while the bottom bar contains a lot of clickable information provided by various extensions.
- The most important keyboard shortcut is `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac), which allows you to type in what you want to do and find a command that does it.
- The second most important is `Ctrl+,` (or `Cmd+,`), which opens a searchable settings menu.
