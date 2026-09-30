# Thomas Vaudescal

Consultant développeur en finance quantitative · Quantitative Developer & Financial Engineering Consultant

## CV

| Version | PDF | Sources LaTeX |
| --- | --- | --- |
| Français | [CV français, 2 pages](out/CV_Thomas_Vaudescal_FR.pdf) | [french/](french/) |
| English | [English CV, 2 pages](out/CV_Thomas_Vaudescal_EN.pdf) | [english/](english/) |
| English, quant | [Quant Developer / Researcher CV, 2 pages](out/CV_Thomas_Vaudescal_Quant_Graduate.pdf) | [quant-graduate/](quant-graduate/) |

## Structure

```
english/          CV anglais : resume.tex, rubriques dans cv/, classe russell.cls
french/           CV français : resume.tex, rubriques dans cv/, classe russell.cls
quant-graduate/   CV quant : resume.tex, rubriques dans cv/, classe russell-ats.cls (lisible par les ATS)
fonts/            polices partagées par les trois versions
out/              PDF compilés
```

Les versions anglaise et française utilisent le gabarit Russell original. La version quant utilise `russell-ats` : pas d'icônes, polices Roboto intégrées.

The English and French versions use the original Russell template. The quant version uses `russell-ats`: no icons, embedded Roboto fonts.

## Compilation

Utiliser XeLaTeX. Les versions anglaise et française demandent aussi les packages Source Sans Pro, Font Awesome 5 et Babel français. Lancer la commande depuis le dossier de la version.

Use XeLaTeX. The English and French versions also need Source Sans Pro, Font Awesome 5 and French Babel. Run the command from the version's folder.

```bash
cd english        && xelatex -interaction=nonstopmode -halt-on-error -output-directory=../out -jobname=CV_Thomas_Vaudescal_EN resume.tex
cd french         && xelatex -interaction=nonstopmode -halt-on-error -output-directory=../out -jobname=CV_Thomas_Vaudescal_FR resume.tex
cd quant-graduate && xelatex -interaction=nonstopmode -halt-on-error -output-directory=../out -jobname=CV_Thomas_Vaudescal_Quant_Graduate resume.tex
```
