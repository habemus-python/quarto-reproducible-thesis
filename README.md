# <span class="emoji">🎓</span> Quarto template for reproducible BEng/MSc/PhD theses using Python <span class="emoji">🐍</span>

(project maintained at and exemplified with a titlepage for [AGH University of Krakow](https://www.agh.edu.pl/en))

This template aims to (by design!):
- <span class="emoji">📦</span> encapsulate all components of a BEng/MSc thesis into a single Jupyter/Python notebook,
- <span class="emoji">✏️ </span> leverage the best of Markdown and LaTeX for hassle-free quality typesetting,
- <span class="emoji">🔄</span> automate generation of plots, tables and in-text numerical values,
- <span class="emoji">📈</span> enforce vector graphics for matplotlib plots,
- <span class="emoji">🔗</span> orchestrate clickable hyperlinks (incl. to the bibliography and from there to the citing locations),
- <span class="emoji">💻</span> offer code listings with syntax-highlighting,
- <span class="emoji">🌍</span> handle multi-lingual content (Polish letters, etc),
- <span class="emoji">📑</span> exemplify a robust bibliography setup,
- <span class="emoji">📐</span> provide reasonable defaults for line spacing, font sizes, margins, etc.

## <span class="emoji">🚀</span> How to use it

To start a new project, execute `quarto use template habemus-python/quarto-reproducible-thesis`.

To render it to a pdf, do: `quarto render thesis.ipynb`.

With the [default notebook unchanged](https://github.com/habemus-python/quarto-reproducible-thesis/blob/main/thesis.ipynb), the resultant pdf looks like this (generated on CI):

<p align="center">
    <img 
        src="https://github.com/habemus-python/quarto-reproducible-thesis/releases/download/tip/thesis.gif" 
        alt="pdf converted to animated gif"
        width="50%"
    />
</p>

## <span class="emoji">⚙️ </span> Dependencies

To get information on how to install Quarto, [read the friendly manual](https://quarto.org/docs/get-started/).

The template requires `quarto` to be executed in an environment with the following tools available (in `$PATH`):
- [Jupyter](https://jupyter.org/) and some common Python packages:
   * using `pip`: `pip install jupyter matplotlib pyyaml nbformat nbclient`
   * on Debian/Ubuntu using APT: `apt-get install jupyter python3-matplotlib python3-yaml`
- [LuaTeX](https://en.wikipedia.org/wiki/LuaTeX) and several [LaTeX packages](https://ctan.org/):
   * on Debian/Ubuntu using APT: `apt-get install texlive-luatex texlive-latex-recommended texlive-lang-polish texlive-latex-extra`
   * on macOS using Homebrew: `brew install texlive`
   * on Linux/macOS/Windows using Quarto: `quarto install tinytex` (optionally with the `--update-path` option to augment `$PATH`)
- [Biber](https://en.wikipedia.org/wiki/Biber_(LaTeX)):
   * on Debian/Ubuntu using APT: `apt-get install biber`
   * on macOS using Homebrew: `brew install biber`
- [Biblatex](https://biblatex.org/):
   * on Debian/Ubuntu using APT: `apt-get install texlive-bibtex-extra`  
- [rsvg-convert](https://en.wikipedia.org/wiki/Librsvg):
   * on Debian/Ubuntu using APT: `apt-get install librsvg2-bin`
   * on macOS using Homebrew: `brew install librsvg`
   * on Windows using Chocolatey: `choco install rsvg-convert`

The above installation steps are tested on CI with [this workflow](https://github.com/habemus-python/quarto-reproducible-thesis/blob/main/.github/workflows/test.yml).

## <span class="emoji">📚</span> Further reading

<span class="emoji">🇬🇧</span> In English:
- [Software Carpentry](https://software-carpentry.org/) lessons on: 
  * [The Unix Shell](https://swcarpentry.github.io/shell-novice/),
  * [Plotting and Programming in Python](https://swcarpentry.github.io/python-novice-gapminder/),
  * [Version Control with Git](https://swcarpentry.github.io/git-novice/), 
- books on research software engineering:
  * [The Turing Way](https://book.the-turing-way.org/) handbook on reproducible, ethical and collaborative data science,
  * [Object-oriented Programming in Python for Mathematicians](https://object-oriented-python.github.io/) book by David Ham (imperial.ac.uk),
  * [Research Software Engineering with Python](https://third-bit.com/py-rse/) book by Damien Irving (csiro.au) et al.,
- Graphics, references and math typesetting:
  * [Vector graphics](https://en.wikipedia.org/wiki/Vector_graphics) article on Wikipedia,
  * [Tips on open source scientific illustration](https://holdenlab.github.io/blog/2024/scientific-illustration/) by Séamus Holden (warwick.ac.uk),
  * [Biblatex Cheat Sheet](https://tug.ctan.org/info/biblatex-cheatsheet/biblatex-cheatsheet.pdf),
  * [Mathematical typesetting guidelines](https://direct.mit.edu/DocumentLibrary/SubGuides/NECO-math-typesetting.pdf) from MIT,
  * [Typefaces for Symbols in Scientific Manuscripts](https://physics.nist.gov/cuu/pdf/typefaces.pdf) from NIST,
- [Quarto template docs](https://quarto.org/docs/extensions/starter-templates.html#using-a-template) 
  (to learn more about using, tuning and developing Quarto templates).

<span class="emoji">🇵🇱</span> In Polish:
- [Jak przygotowywać i prezentować prace dyplomowe inżynierskie i magisterskie](https://www.fis.agh.edu.pl/home/wfiis/wfiis/import/Wzory_dokumentow/thesis.pdf) by Andrzej Lenda (fis.agh.edu.pl),
- [Wymagania stawiane pracom magisterskim i licencjackim](https://www.fuw.edu.pl/tl_files/studia/dyplomy/wymagania_prac_mag_lic.pdf) from fuw.edu.pl,
- [MWCLS: podręcznik użytkownika polskich klas dokumentów LaTeXa](https://ctan.math.illinois.edu/macros/latex/contrib/mwcls/mwclsdoc.pdf) by Marcin Woliński (uw.edu.pl).

## <span class="emoji">👥</span> Credits

Title page based on [Overleaf template](https://www.overleaf.com/latex/templates/praca-dyplomowa/kbwcrcmczypy) 
  by [Krzysztof Malarz](https://home.agh.edu.pl/~malarz/).
