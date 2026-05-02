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

To render it to a pdf, do: `quarto render` (or `quarto render thesis.ipynb`).

With the [default notebook unchanged](https://github.com/habemus-python/quarto-reproducible-thesis/blob/main/thesis.ipynb), 
  the [resultant pdf](https://github.com/habemus-python/quarto-reproducible-thesis/releases/download/tip/thesis.pdf) looks like this (generated on CI):

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

## <span class="emoji">🛠️</span> Notes for contributors

- [pre-commit documentation](https://pre-commit.com/#3-install-the-git-hook-scripts)
- [Quarto template docs](https://quarto.org/docs/extensions/starter-templates.html#using-a-template) 

## <span class="emoji">👥</span> Credits

Title page based on [Overleaf template](https://www.overleaf.com/latex/templates/praca-dyplomowa/kbwcrcmczypy) 
  by [Krzysztof Malarz](https://home.agh.edu.pl/~malarz/).
