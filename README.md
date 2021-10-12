# SDD I Module 2 : Workflow en biologie

## Avant-propos

Il est possible que ce document évolue au cours du temps. N'hésitez pas à aller vérifier le lien suivant afin de voir les modifications dans les consignes : <https://github.com/BioDataScience-Course/A02Ga_21_workflow>

## Objectif

Ce projet est un projet **en binôme**, **court** et **cadré** qui doit être terminé pour la fin du module 2.

L'objectif est de s'intéresser R Markdown pour écrire des documents scientifiques de manière à ce qu'ils soient reproductibles et faciles à mettre à jour.

## Consignes

Vous êtes dans la peau de biologistes qui analyse des données de biométrie humaine. Vous avez à votre disposition deux jeux de données répartis en deux fichiers, disponibles à partir du sous-dossier `data` de ce projet.

- `biometry_2014.xlsx`
- `biometry_2016.xlsx`

Ces fichiers comprennent 7 variables :

- gender : homme (H) ou femme (F)
- db : date de naissance
- yb : année de naissance
- weight : masse en kg
- height : taille en cm
- wrist : circonférence du poignet en mm
- measurement_date : année de la prise de mesure

### Analyse de `biometry_2014.xlsx`

Le tableau `biometry_2014.xlsx` comprend des mesures biométriques collectées en 2014. 

**Vous avez une succession d'étape à réaliser par le premier ou le second collaborateur. Il y a plusieurs commit, pull, push à réaliser. Nous vous conseillons pour ce premier projet en groupe de réaliser les étapes ensemble.**

1. Réalisez 4 graphiques dans le script `biometry_graphe.R` qui est dans le sous-dossier `R`.
    + Le premier collaborateur réalise 2 graphiques. Il fait ensuite un commit et un push.
    + Le second collaborateur commence par faire un pull. Il réalise ensuite 2 graphiques différents. Il termine par un commit et un push.

2. Réalisez un rapport d'analyse avec Microsoft Word Online < www.umons.ac.be/office365> ou Google docs. Ce document doit se nommer biometry_word_NOMDUGROUPE. Ce document doit être structuré. Il doit comprendre un `titre général`, une section `introduction` et une section `analyses`. Il faut intégrer un graphique pertinent dans la section analyses de ce rapport. Ce graphique doit être décrit en 3 à 5 phrases. Vous pouvez utiliser une capture d'écran pour extraire votre graphique de RStudio et l'incorporer sous la forme d'une image dans votre document. Vous devez partager ce document afin qu'il soit téléchargeable. Le lien pour accéder à ce document doit se trouver dans `biometry_online.Rmd`. Réalisez un Pull, un commit et un push.


3. Réalisez un rapport d'analyse avec R Markdown.
    + Le second collaborateur réalise un pull.
    + Le second collaborateur édite `biometry.Rmd`. Ce document doit être identique au document en ligne. Il doit comprendre un `titre général`, une section `introduction` et une section `analyses`. 
    + Le second collaborateur incorpore un graphique pertinent dans la section analyse de ce rapport. Ce graphique doit être décrit en 3 à 5 phrases. Vous devez ajouter un chunk contenant le code qui permet de générer ce document.
    + Le second collaborateur vérifie que son document est compilable. Le document doit être compilé en "HTML", "PDF" et "Word".
    + Le second collaborateur réalise un commit et un push.
  
### Nouvelles données `biometry_2016.xlsx`

Après avoir réalisé une première version de vos rapports, l'un dans Word, et l'autre dans R Markdown, avec les données de `data/biometry_2014.xlsx`, vous recevez de nouvelles données (celles dans`data/biometry_2016.xlsx`).

4. Le premier collaborateur réalise un pull,  actualise le rapport sous R Markdown, réalise un commit et un push.

5. Le second collaborateur réalise un pull, actualise le rapport sous Microsoft Word Online. Vous devez bien évidemment actualiser le graphique, ce qui revient donc à remplacer l'ancienne version par un graphique recalculé. 

### Comparaison des deux méthodes

À la suite de vos analyses, répondez aux questions ci-dessous pour cadrer votre réflexion sur le workflow et la recherche reproductible.

6. Utilisez un fichier RMarkdown (`.Rmd`) pour y consigner vos réponses et placez-le dans votre projet RStudio. Nommez ce fichier `workflow.Rmd`

- Quel workflow vous semble le plus simple à l'utilisation, et pourquoi ?

- Comparez la façon dont les graphiques sont gérés dans les deux cas.

- Quel workflow vous semble le plus pertinent lorsque les données arrivent progressivement ?

- Quel workflow vous semble le plus simple et le plus approprié lorsque plusieurs personnes collaborent pour rédiger un rapport ? 

### État de progression 

À la fin de ce module, vous devez avoir :

- un script R nommé `biometry_graphe.R` (dans le dossier `R`) qui comprend vos premiers graphiques

- un fichier au format .doc ou .docx nommé `biometry_online.docx` (dans le dossier `docs`) qui comprend le nuage de point le plus à jour.

- un fichier au format .Rmd nommé `biometry.Rmd` (dans le dossier `docs`) qui comprend le nuage de point le plus à jour.

- un fichier au format .Rmd nommé `workflow.Rmd` (dans le dossier `docs`) qui comprend votre comparaison des workflows.
