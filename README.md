# 📄 Research LaTeX Template

A clean, modular, and professional LaTeX template tailored for academic theses, dissertations, and research documents. This template is designed to support structured writing, semantic clarity, and reproducible formatting across a variety of disciplines and institutional styles.

## ✨ Key Features

- **📚 Modular structure** – Chapters, metadata, references, and appendices are split for clarity and ease of use
- **🔄 BibLaTeX + Biber citation system** – Easily switch between APA, IEEE, Chicago, and other citation styles
- **🧠 Semantic macros** – Includes academic shorthand like `\eg`, `\ie`, `\cf`, and `\theory{}` for consistent expression
- **🎓 Thesis-ready layout** – Configurable for Master's or PhD theses with university branding
- **📝 Glossary and acronyms** – Built-in support using the `glossaries` package
- **🧱 Figure/table styling** – Pre-styled captions, cross-referencing, and alignment with academic publishing standards
- **⚙️ Automated build** – Works with `latexmk`, `Makefile`, or Overleaf
- **☁️ Overleaf compatible** – Fully portable for cloud-based editing

## 📁 Directory Structure

```
research-latex-template/
├── main.tex              # Entry point
├── metadata.tex          # Title, author, degree, institution
├── preamble.tex          # Package imports, styling, macros
├── structure/            # Modular content
│   ├── abstract.tex
│   ├── introduction.tex
│   ├── literature.tex
│   ├── methodology.tex
│   ├── results.tex
│   ├── discussion.tex
│   ├── conclusion.tex
│   └── appendix.tex
├── references/
│   └── references.bib    # Bibliographic database
├── images/               # Figures and diagrams
│   └── sample-fig.png
├── glossary.tex          # Glossary and acronym entries
├── Makefile              # Automate build (optional)
├── latexmkrc             # Configuration for latexmk (optional)
├── LICENSE               # License (e.g., MIT or CC-BY)
├── .gitignore
└── README.md             # You're here
```

## 🚀 Getting Started

### Option 1: Compile Locally

**Requirements:**
- A LaTeX distribution (TeX Live or MiKTeX)
- `latexmk` (recommended)
- `biber` for bibliography processing

**To build:**

```bash
latexmk -pdf main.tex
```

Or if you have the provided Makefile:

```bash
make
```

### Option 2: Use with Overleaf

1. Download the repository as a `.zip` file
2. Go to [Overleaf](https://www.overleaf.com)
3. Select "Upload Project"
4. Upload the `.zip` archive and start editing

## ✍️ Customization Guide

1. **Modify your thesis details** in `metadata.tex` (title, author, institutional details)
2. **Edit content** in `structure/*.tex` files to write your content by chapter
3. **Add figures** to the `images/` directory
4. **Update references** in `references/references.bib`
5. **Define terms and acronyms** in `glossary.tex`

## 🔗 Citation Styles

To switch citation styles, modify the `biblatex` option in `preamble.tex`:

```latex
\usepackage[style=apa, backend=biber]{biblatex}
```

Change `style=apa` to `ieee`, `authoryear`, `numeric`, or any other supported style.

## 📒 Glossary and Acronyms

Define terms and acronyms in `glossary.tex` like this:

```latex
\newglossaryentry{liminality}{
    name=liminality,
    description={The transitional state between two stages}
}

\newacronym{RWI}{RWI}{Remote Work Intensity}
```

Use `latexmk` to automatically build glossary entries, or run `makeglossaries` manually.

## 💡 About This Template

This template was originally developed for a PhD thesis exploring Liminal Spaces in Remote Work. It aims to reduce friction in long-form academic writing by enforcing structure, semantic markup, and professional typesetting practices.

## 📄 License

This project is licensed under the MIT License (see `LICENSE` file). You are free to use, modify, and distribute this template for academic or commercial purposes with attribution.

## 🛠️ Contributing

Contributions are welcome via issues or pull requests. Feature suggestions, bug fixes, and improvements are appreciated.

## 📬 Contact

For questions or feedback, please open an issue on GitHub or reach out via email (contact details in the repo or profile).
