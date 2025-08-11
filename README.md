# typst-githubrun-template

This repository provides a template for a GitHub Action that automates the process of compiling **Typst** documents into PDFs. When you push changes to your repository, this workflow automatically generates a PDF from your `.typ` files and uploads it as a **GitHub Artifact**.

# What is Typst?

**Typst** is a new, web-first markup-based typesetting system. It's designed to be powerful and easy to use, providing a modern alternative to traditional tools like LaTeX. You can learn more about it on the [official Typst website](https://typst.app/).

# Getting Started

1.  **Use this template:** Click the "Use this template" button at the top of this repository to create a new repository based on this template.
2.  **Add your Typst files:** Place your `.typ` files in your repository.
3.  **Customize the workflow (Optional):** Edit the `.github/workflows/build.yml` file to change the input file names or output paths if needed. The default configuration will compile all `.typ` files in the repository.
4.  **Push your changes:** The workflow will run automatically on the first push and subsequent pushes. You can find the generated PDF in the **Actions** tab of your repository.

# LICENSE 
I provide this with MIT LICENSE.
