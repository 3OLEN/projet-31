---
layout: intermediary_deliverable
title: "Livrable intermédiaire - MCD"
slug: mcd

assessment: mcd

deliverable_comment: "Seul le MCD est attendu dans ce dossier de conception. Le reste est à faire de votre côté pour
votre propre production."
---

Pour pouvoir monter une base de données, il faut définir les tables qui la composent (avec leurs champs) et les
relations entre ces tables. De cette manière, on obtient un premier visuel de la base de données permettant alors de
mieux l'appréhender et de vérifier qu'elle est cohérente et qu'elle répond aux besoins et problématiques.

On construit alors le modèle conceptuel de données (MCD) selon la méthodologie Merise.

## 🗂️ Modèles de données

Il vous est demandé de fournir le MCD permettant de visualiser les entités et leurs relations entre elles.

C'est à partir de ce modèle que vous pourrez définir les tables (dont les tables d'association), les clefs primaires
et étrangères et les champs qui composent vos différentes tables.

Vous pourrez ensuite lister l'ensemble de vos tables avec leurs champs (ce qui se définit généralement par le
MLD : Modèle Logique de Données) vous permettant alors d'écrire vos scripts SQL de création de la BDD, puis de
l'insertion des données initiales.

{% include _templates/panel/_comment.liquid text=page.deliverable_comment %}

### Conseils

{% assign specification_page = site.html_pages | where: "path", "specifications-dev.html" | first %}

* Les [spécifications fonctionnelles]({{ specification_page.url | relative_url }}) contiennent les demandes et les
  contraintes du modèle de données.
  - À lire et **relire** sans modération !
  - Vous y trouverez toutes les informations nécessaires et la large majorité des réponses à vos questions.
  - Tout ce qui est décrit dans ces pages n'est pas anodin et très certainement à intégrer dans le modèle de données.
* Vous trouverez des outils tels que [Lucidchart](https://www.lucidchart.com/), [Draw.io](https://draw.io/) ou
  encore [Creately](https://creately.com/) pour réaliser votre MCD.
  - Gardez en tête qu'il doit être lisible.
* M. Gilot co-anime la deuxième séance du projet transverse. Il est conseillé d'avoir un MCD abouti à cette date pour
  pouvoir en discuter avec lui et ainsi le critiquer (positif et négatif).

## ✅ Notation

* La note de cette partie sera définie selon les éléments suivants :
  - Si des demandes essentielles prévues dans les spécifications fonctionnelles sont manquantes, vous serez pénalisés.
  - Selon la nature des manques (champs, tables, relations), la pénalité sera plus ou moins importante.
* Un MCD illisible et inexploitable sera **rejeté**. Utilisez annexes ou lien public de partage si besoin.
