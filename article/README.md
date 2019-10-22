This repository was used to create the pdf of our submitted article.

As recommended by the ReScience team, we typed this to build the pdf:

```
pandoc --standalone --filter ~/.cabal/bin/pandoc-crossref --template=rescience-template.tex --pdf-engine=xelatex --biblatex --bibliography=bibliography.bib -M "crossrefYaml=crossref.yaml" --output Bavard-Thero-2018.tex Bavard-Thero-2018.md
xelatex Bavard-Thero-2018
biber Bavard-Thero-2018
xelatex Bavard-Thero-2018
xelatex Bavard-Thero-2018
```
