# typst-githubrun-template

This repository provides a template for a GitHub Action that automates the process of compiling **Typst** documents into PDFs. When you push changes to your repository, this workflow automatically generates a PDF from your `.typ` files and uploads it as a **GitHub Artifact**.

## What is Typst?

`Typst` is a new, web-first markup-based typesetting system. It's designed to be powerful and easy to use, providing a modern alternative to traditional tools like LaTeX. You can learn more about it on the [official Typst website](https://typst.app/).

# Getting Started

1. Click the `Use this template` button at the top of this repository to create a new repository based on this template.
2. Set up self hosted runner. In The repository's setting tab, you can click actions and select runner setting. you will see a button of adding new self hosted runner.
3.  Put your `.typ` files in your repository.
4.  The workflow will run automatically on the first push and subsequent pushes. You can find the generated PDF in the **Actions** tab's Artifact of your repository.

# LICENSE 
I provide this with MIT LICENSE.

# Font Setting
## Default
These fonts are available
- DejaVu Sans
- DejaVu Sans Mono
- DejaVu Serif
- Libertinus Serif
- New Computer Modern
- New Computer Modern Math
- Noto Sans CJK JP
But,`Noto Sans CJK JP` is not typst default font.
So if you could use the font on Self hosted runner, you have to install(put font file in `~/.fonts`) that.You can see link of that in ReleaseBuild.yaml
If you want to use additional fonts, you can set up it.
## On Self hosted runner
Only you have to do is that download font and put it in ~/.fonts/
## On Github Runner
You have to add code of font download to workflows file.

# Release
This repo is set up for release build.
It runs on GitHub hosted runner, and static(it does not depend on the situation of self-hosted server).

## how to create release with ReleaseBuild
Create Release tag named `*.*.*`.
And create Release with that tag.
