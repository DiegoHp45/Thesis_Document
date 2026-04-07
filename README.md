# Thesis Manuscript Repository

## Overview

This repository contains the complete LaTeX source code for a scientific thesis. It is designed to support a structured, modular, and reproducible workflow for the preparation of an academic manuscript in physics. The repository integrates version control practices to ensure transparency, traceability of changes, and collaborative potential.

## Objectives

The primary objectives of this repository are:

* To maintain a well-organized and scalable LaTeX project
* To facilitate reproducible document compilation
* To ensure consistency in formatting, notation, and referencing
* To support the integration of figures, tables, and computational results
* To enable efficient version control using Git

## Repository Structure

The project is organized as follows:

```
thesis/
│── Thesis.tex                % Root document
│── preamble.tex            % Packages, formatting, and custom commands
│── references.bib          % Bibliographic database (BibTeX)
│── chapters/               % Individual chapter files
│── figures/                % Figures and graphical assets
│── tables/                 % Tabular data (optional)
│── appendices/             % Supplementary material
│── .gitignore              % Excluded build artifacts
```

Each chapter is developed as an independent file and incorporated into the main document via `\input{}`, promoting clarity and maintainability.

## Compilation

The document can be compiled using standard LaTeX tools. A typical compilation sequence is:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Alternatively, automated compilation may be performed using:

```bash
latexmk -pdf main.tex
```

## Bibliographic Management

References are managed using BibTeX. Entries should be maintained in `references.bib` and cited within the text using standard LaTeX citation commands (e.g., `\cite{key}`). Consistent citation practices should be followed throughout the manuscript.

## Figures and Tables

All graphical materials should be stored in the `figures/` directory and included using the `graphicx` package. Tables may be defined within the text or maintained separately in the `tables/` directory if needed.

## Version Control

This repository uses Git for version control. Temporary and auxiliary files generated during compilation (e.g., `.aux`, `.log`, `.toc`) are excluded via the `.gitignore` file. Users are encouraged to commit regularly with clear and descriptive messages.

## Current Status

The repository is currently under active development. Content, structure, and formatting are subject to refinement as the manuscript progresses.

## Author

Diego Fernando Hernandez Porras

