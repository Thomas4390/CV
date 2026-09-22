# Thomas Vaudescal

Consultant développeur en finance quantitative · Quantitative Developer & Financial Engineering Consultant

## CV

| Langue / Language | PDF | Sources LaTeX |
| --- | --- | --- |
| Français | [CV français — 2 pages](french/out/CV_Thomas_Vaudescal_FR.pdf) | [french/resume.tex](french/resume.tex) |
| English | [English CV — 2 pages](out/CV_Thomas_Vaudescal_EN.pdf) | [resume.tex](resume.tex) |

Les deux versions utilisent le gabarit Russell original et présentent le même parcours. Les rubriques sont réparties dans `cv/` et `french/cv/`.

Both versions use the original Russell template and cover the same experience. Individual sections are stored in `cv/` and `french/cv/`.

## Compilation

Utiliser XeLaTeX avec les packages Roboto, Source Sans Pro, Font Awesome 5 et Babel français. Sur Overleaf, choisir XeLaTeX et le fichier principal de la langue souhaitée.

Use XeLaTeX with Roboto, Source Sans Pro, Font Awesome 5 and French Babel support. On Overleaf, select XeLaTeX and the main file for the desired language.

Version anglaise, depuis la racine du dépôt / English version, from the repository root:

```bash
xelatex -interaction=nonstopmode -halt-on-error -output-directory=out -jobname=CV_Thomas_Vaudescal_EN resume.tex
```

Version française, depuis le dossier `french/` / French version, from the `french/` directory:

```bash
xelatex -interaction=nonstopmode -halt-on-error -output-directory=out -jobname=CV_Thomas_Vaudescal_FR resume.tex
```
