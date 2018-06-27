# Analyse enquête Bioinfo-fr 2018

Enquête conduite entre le 12/03/2018 et le 30/04/2018 afin de dresser un portrait de la bioinformatique francophone.

## Infos
* Article du blog disponible [en ligne](https://bioinfo-fr.net/enquete-bioinfo-fr-2018-portrait-de-bioinfo "")
* Les scripts ont été executés avec R-3.5.0 et les packages dans la version suivant
  * dplyr_0.7.5
  * ggplot2_2.2.1
  * gridExtra_2.3
  * tm_0.7-4
  * textcat_1.0-5
  * wordcloud_2.5
* Le moins de modifications manuelles (edition d'une cellule à la main) possible ont été portées aux données afin de se mettre dans un contexte de données massives (qui sont humainement impossibles à travailler manuellement)
* Le code est actuellement encore dans une forme "brouillon" (des commentaires et des agencements du Rmd sont à revoir), mais reste parfaitement exécutable.

## Production du rapport final
`Rscript -e "library(rmarkdown); rmarkdown::render('analyse.Rmd')"`
