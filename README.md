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

## Rappel du formulaire d'enquête

### Votre profil
Question | Réponse(s)
-----------------------------------|--------------------------------------------
Quelle est votre tranche d'age ? * | `integer`
Quel est votre sexe ? * | Femme,  Homme, Autre
Quel est votre plus haut diplôme obtenu ? (si pas dans la liste, sélectionner équivalent) * | Bac, BTS/DUT/DEUG, Licence, Master/DEA/DESS, Doctorat
Votre métier de bioinformaticien(ne) a * | Une dominante vers la biologie, Une dominante vers l'informatique, Un juste milieu entre les deux domaines
Combien d'année(s) d'expérience cumulez-vous aujourd'hui ? * | `integer`
Parmi ces années, combien d'année(s) à l'étranger ? * | `integer`

### Votre environnement de travail
Question | Réponse(s)
-----------------------------------|--------------------------------------------
Etes-vous actuellement en France ou à l'étranger ? * | France, Étranger (Europe), Étranger (hors Europe)
Etes-vous dans le public ou dans le privé ? * | Public, Privé, Aucun des deux
Etes-vous actuellement en * | Recherche d'emploi, Stage/alternance, CDD/doctorat, CDI
Nombre de biologistes travaillant avec vous * | `integer`
Nombre de bioinfos travaillant avec vous * | `integer`
Autres collègues proches * | `integer`
Quel est le titre de votre poste actuel ? * | `char`
Votre salaire annuel brut actuel en euros se situe entre * | [15;20[, [20;25[, [25;30[, [30;35[, [35;40[, [40;45[, [45;50[, [50;55[, [55;60[, [60;65[, [65;70[, [70;75[, [80;++[

### Le coin techno
Question | Réponse(s)
-----------------------------------|--------------------------------------------
Votre/vos OS du quotidien * | Windows, Windows + VM GNU/Linux, GNU/Linux + VM Windows, GNU/Linux, macOS, macOS + VM Windows
Quel(s) langages de programmation utilisez-vous quotidiennement * | `char`
Quels sont les contextes dans lequels vous utilisez les langages que vous avez spécifié ? * | développement web, base de données, scripting, analyses/statistiques, admin systeme, développement d'application, au



