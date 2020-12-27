# Custom LaTeX template for theses

**Custom** [LaTeX](https://www.latex-project.org/) template – created for my thesis at the [Beuth University of Applied Sciences Berlin](https://www.beuth-hochschule.de/en/).

> **This is not an official template for the Beuth University!**

## How to Typeset (build LaTeX & view PDF files)

- install LaTeX and an editor/previewer (comes often bundled) from e.g. the [LaTeX Project](https://www.latex-project.org/get/)
- clone this repo
- open the `main.tex` file with your installed LaTeX editor/previewer
- run the `Typeset` action or the equivalent in your editor/previewer
- (optionally run the `Typeset` action again if errors/warnings appear in the console on the first pass. They might disappear.)
- open the preview area of your editor/previewer or open the `main.pdf` file to see the typeset/generated result

## How to navigate

- `main.tex` is your root entry point of your LaTeX document
- `main.pdf` is always the latest _generated_ PDF file of your typeset document
- `1_frontmatter/` includes everything that comes _before_ your actual content (see [front matter](https://en.wiktionary.org/wiki/front_matter))
- `2_bodymatter/` includes everything that is your personal content (see [body matter](https://en.wiktionary.org/wiki/body_matter))
- `3_backmatter/` includes everything that comes _after_ your actual content (see [back matter](https://en.wiktionary.org/wiki/back_matter))
- `images/` is where all images belong (I recommend vector-based `.eps` files for graphics and diagrams etc.)
- `libraries/` is where the bibliography and glossary store their entries
- `packages.tex` is a list of all added LaTeX packages & some of their settings 

### Disclaimer

- _This template still has bugs. Be aware._  
Like this workaround in the `main.tex` file, you need to know about:

```tex
% restore roman page numbering for secondary pages
\pagenumbering{roman}
\setcounter{page}{42} % WORKAROUND: update number manually depending on the glossary length!
```

- I have only tested it on UNIX-based operating systems and in a _very small_ selection of editors.

- It is normal that LaTeX generates a lot of additional files. They should be ignored by Git.

- Please ask your educational institution if this template meets their standards before using it.

## How to Support

You are very welcome to fix bugs within this project.

1. Create a pull request for this repo
2. Include an explanation of your changes (what, why & how)
3. Always make it nicer (not harder) for the next person

Thank you & keep studying!
