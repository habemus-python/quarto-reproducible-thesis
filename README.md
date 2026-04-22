# Quarto template for AGH BEng/MSc theses

To start a new blank project, execute `quarto use template habemus-python/quarto-agh-thesis`.

To render it to a pdf, do: `quarto render thesis.ipynb`.

Note: to make it work, `quarto` needs to be executed in an environment with the following tools available (in `$PATH`):
- [Jupyter](https://jupyter.org/) and some common Python packages:
   * using `pip`: `pip install jupyter matplotlib pyyaml nbformat nbclient`
   * on Debian/Ubuntu using APT: `apt-get install jupyter python3-matplotlib python3-yaml`
- [LuaTeX](https://en.wikipedia.org/wiki/LuaTeX) and several [LaTeX packages](https://ctan.org/):
   * on Debian/Ubuntu using APT: `apt-get install texlive-luatex texlive-latex-recommended texlive-lang-polish texlive-latex-extra`
   * on macOS using Homebres: `brew install texlive`
   * on Windows using Quarto: `quarto install tinytex`
- [Biber](https://en.wikipedia.org/wiki/Biber_(LaTeX)):
   * on Debian/Ubuntu using APT: `apt-get install biber`
   * on macOS using Homebrew: `brew install biber`
- [Biblatex](https://biblatex.org/):
   * on Debian/Ubuntu using APT: `apt-get install texlive-bibtex-extra`  
- [rsvg-convert](https://en.wikipedia.org/wiki/Librsvg):
   * on Debian/Ubuntu using APT: `apt-get install librsvg2-bin`
   * on macOS using Homebrew: `brew install librsvg`
   * on Windows using Chocolatey: `choco install rsvg-convert`

See [Quarto docs](https://quarto.org/docs/extensions/starter-templates.html#using-a-template) 
  to learn more about using templates.

Template based on [Overleaf template](https://www.overleaf.com/latex/templates/praca-dyplomowa/kbwcrcmczypy) 
  by [Krzysztof Malarz](https://home.agh.edu.pl/~malarz/).
