# Research Paper - Wikipedia Bias Analysis

This directory contains the LaTeX source for my **CPSC-298 research paper** on systematic bias and multilingual representation on Wikipedia.

## File Structure
paper/
├── main.tex                    # Main document file
├── references.bib              # Bibliography (BibTeX format)
├── sections/                   # Individual sections
│   ├── abstract.tex
│   ├── introduction.tex
│   ├── related-work.tex
│   ├── methodology.tex
│   ├── results.tex
│   ├── discussion.tex
│   ├── conclusion.tex
│   └── appendix-AI-usage.tex
└── figures/                    # Place your figures here

Compiling the Paper
Option 1: Latex in Vscode
This is my preferred method.

Setup (do this once):

Install a LaTeX distribution (this provides the actual LaTeX compiler tools like pdflatex and bibtex):

macOS: Install MacTeX (large download, ~4GB)
# Or via Homebrew:
brew install --cask mactex
Windows: Install MiKTeX
Linux: Install TeX Live
# Ubuntu/Debian:
sudo apt-get install texlive-full
# Fedora:
sudo dnf install texlive-scheme-full
Install the LaTeX Workshop extension in VS Code:

Open VS Code
Go to Extensions (Cmd+Shift+X on macOS, Ctrl+Shift+X on Windows/Linux)
Search for "LaTeX Workshop" by James Yu
Click Install
The extension acts as an interface between VS Code and the LaTeX distribution you installed in step 1.

Btw, talking about extensions, also get the Markdown All in One extension.

Usage:

Files should compile in VS Code automatically upon saving. In case this does not happen, you can compile from the commandline:

cd paper/
pdflatex main.tex
If the references changed:

pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
Option 2: Overleaf
Overleaf is convenient to get started and for collaboration. But your official version will be the one on in your git repo. So in case you use Overleaf, make sure that your work is copied back.

Go to Overleaf
Create a new project → Upload Project
Upload all files from this paper/ directory
The PDF will compile automatically
To download: Menu → PDF (or Source for all files)