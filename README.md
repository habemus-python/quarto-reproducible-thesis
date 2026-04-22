# Quarto template for AGH BEng/MSc theses

This template aims to:
- encapsulate all components of a BEng/MSc thesis into a single Jupyter/Python notebook,
- ensure code-generated plots are in-sync with the code,
- enforce vector graphics for matplotlib plots,
- provide clickable references - with links from the text to the bibliography, as well as from the bibliography to the citing locations,
- offer code listings with syntax-highlighting,
- handle correctly multi-lingual content (Polish letters, etc),
- provide reasonable defaults for line spacing, font sizes, margins, etc.

To start a new blank project, execute `quarto use template habemus-python/quarto-agh-thesis`.

To render it to a pdf, do: `quarto render thesis.ipynb`.

Note: to make it work, `quarto` needs to be executed in an environment with the following tools available (in `$PATH`):
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

The above installation steps are tested on CI with [this workflow](https://github.com/habemus-python/quarto-agh-thesis/blob/main/.github/workflows/test.yml).

See [Quarto docs](https://quarto.org/docs/extensions/starter-templates.html#using-a-template) 
  to learn more about using templates.

Template based on [Overleaf template](https://www.overleaf.com/latex/templates/praca-dyplomowa/kbwcrcmczypy) 
  by [Krzysztof Malarz](https://home.agh.edu.pl/~malarz/).
