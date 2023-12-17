---
layout: intermediary_deliverable
title: "Livrable intermédiaire - Diagrammes UML"
slug: uml

assessment: uml

comment: "Même si le module a été mené pour les « Dev », nous attendons aussi une participation de la part des
« Infra » (au moins un chacun). Collaborez avec les « Dev » et apprenez de l'enseignement qu'ils ont reçu."
---

Dans le cadre de votre phase de conception, vous aurez à produire des diagrammes UML afin de mieux appréhender le sujet
et d'avoir à disposition ces "schémas" vous permettant de visualiser les fonctionnalités attendues et les solutions
décidées à mettre en place.

Pour le dossier de conception, vous devrez fournir les diagrammes désignés ci-dessous. Vous pouvez compléter votre
dossier avec d'autres diagrammes si vous le souhaitez, à condition qu'ils soient pertinents. Si c'est bien le cas, vous
pourrez être éligibles à des points bonus. Mais ne faites pas ces diagrammes dans le but d'espérer des points bonus ;
vous gaspilleriez du temps pour des éléments obligatoires à la notation du dossier.

Plusieurs outils sont à disposition comme [StarUML](https://staruml.io),
[Visual Paradigm](https://online.visual-paradigm.com/fr/), ou encore [draw.io](https://draw.io).

{% include _templates/panel/_comment.liquid text=page.comment %}

-----

Liens rapides vers les spécifications fonctionnelles :

{% include _templates/list/_pages.html pages=site.specifications %}

## 📝 Diagrammes à fournir

### Diagrammes des cas d'utilisation

En reprenant les spécifications fonctionnelles, vous définirez les différents "acteurs" de l'application et leurs
interactions avec le système. Vous devrez fournir un ou plusieurs diagramme·s de cas d'utilisation pour représenter
les différents rôles utilisateur et ce qu'ils pourront faire à travers l'application.

Il existe plusieurs façons d'appréhender les cas d'utilisation.

- Soit vous définissez l'ensemble dans un seul diagramme. Cette solution permet de voir l'ensemble des acteurs et ce
que chacun peut ou ne peut pas faire. Cependant, cela peut vite devenir illisible et complexe à maintenir.
- Soit vous définissez un diagramme par acteur. Cette solution permet de se consacrer essentiellement à ce qu'un
utilisateur peut faire. Cependant, cela peut vite devenir redondant et complexe à maintenir.
- Soit vous définissez un diagramme par fonctionnalité ou domaine fonctionnel. Cette solution permet d'avoir une vision
de l'ensemble des cas d'utilisation d'une fonctionnalité ou d'un domaine fonctionnel.

Gardez en tête qu'un diagramme doit être exploitable, c'est pourquoi il est important qu'il soit lisible. Par ailleurs,
vous pourrez réutiliser ces diagrammes dans votre soutenance.

### Diagrammes d'activité

Généralement, chaque cas d'utilisation permet de définir un diagramme d'activité (ou un ensemble de diagrammes selon
la complexité). Ce diagramme permet de définir les différentes étapes de l'action et les conditions de passage d'une
étape à une autre. Il permet aussi de relier des activités ensemble ou de créer des pointeurs vers d'autres diagrammes.

### Diagrammes de séquences

Afin d'avoir une meilleure vision de l'implémentation technique de certaines fonctionnalités et de l'utilisation des
diverses briques de développement, chaque « Dev » devra enrichir une fonctionnalité avec un diagramme de séquences.

Chacun doit choisir une fonctionnalité différente afin de ne pas avoir de doublons.

Ce diagramme sera le seul annoté avec le nom de l'étudiant.

### Diagramme de déploiement

Afin de représenter l'infrastructure à mettre en place, et respectant les contraintes techniques définies, vous
fournirez un diagramme de déploiement.

Ce diagramme permet de représenter les différents éléments de l'infrastructure et leurs relations. Il permet aussi de
représenter les différents environnements (intégration, recette, production) et les flux de déploiement.

## ✅ Notation

* Une note globale sera attribuée pour l'ensemble des diagrammes fournis :
  - Chaque type de diagramme demandé doit être fourni. Si un type est manquant, la note ne dépassera pas la moyenne.
  <br>Mais ce n'est pas parce que vous fournissez tous les types que vous atteindrez la moyenne !
  - Aucun aspect fonctionnel ne doit être oublié. Si un aspect est manquant, la note ne dépassera pas la moyenne.
* Une note personnelle pour les « Dev » concernant leur propre diagramme de séquences.
* Chaque diagramme doit être bien présenté, lisible et compréhensible. Si ce n'est pas le cas, le diagramme sera rejeté.
* Soignez votre maîtrise de la langue ; des points malus seront appliqués dans le cas contraire.

N'oubliez pas que chaque membre du groupe doit avoir pris la responsabilité d'au moins un diagramme.
