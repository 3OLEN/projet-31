---
layout: intermediary_deliverable
title: "Livrable intermédiaire - Planification"
slug: planification

assessment: planning

milestone_comment: "Certains livrables manquent actuellement de détail. Si ces jalons n'ont pas une liste de tâches
complète, vous ne serez pas impactés sur la note. Mais n'oubliez pas de les compléter dès lors que vous avez ces
informations manquantes."
planning_danger: Interdiction formelle de fournir un diagramme de Gantt.
---

Afin de mieux vous organiser, il est essentiel de définir des éléments de base sur la conduite du projet. Il ne vous
sera pas demandé de prendre le rôle de « chef·fe de projet », ni de réaliser de la gestion de projet.

Si une personne souhaite s'y essayer, pourquoi pas, mais ce sera hors évaluation et si le reste de son travail n'est
pas suffisant, sa note en sera impactée.

## 🗓 Planification

Un projet est composé d'un ensemble de tâches (macro et sous-tâches) qui sont définies par une estimation de temps et
des relations entre elles (si la tâche A doit être terminée avant de commencer la tâche B). De cette manière, il est
possible de définir une durée de réalisation du projet, c'est la durée prévisionnelle.

Lorsque les différentes ressources humaines du projet réalisent leurs tâches, on définit une durée réelle. Il y a alors
des mesures qui sont remontées à propos du différentiel entre le prévisionnel et le réel pour se rendre compte de
l'état d'avancement du projet à un instant T. On sait ainsi si on prend du retard ou si on bénéficie d'une avance.

Ces aspects font partie de la gestion de projet (avec bien d'autres comme les chemins critiques, la gestion de risques,
le parallélisme, etc.). Comme indiqué au-dessus, vous n'aurez pas à vous en occuper, ou en tout cas pas de manière
poussée.

### Tâches

Avec les spécifications fonctionnelles et techniques, vous allez devoir dresser une liste des tâches à réaliser : pour
les « Dev », pour les « Infra » ou pour l'ensemble de l'équipe (les kick-off, les réunions régulières, la conception,
etc.).

L'idéal, c'est d'organiser ces tâches d'une façon hiérarchique en définissant des domaines d'application (techniques
ou fonctionnelles). Vous aurez alors des tâches parentes, dites « macro », et des tâches enfants, dites « sous-tâches »,
plus précises. 

Faites attention à ne pas définir des tâches trop globales (« Réaliser l'application » / « Gestion des livres » /
« Dockeriser l'infrastructure »), soit vous n'arriverez pas à définir exactement ce que vous devrez faire, soit vous
définirez une hiérarchie de tâches trop profonde (> au niveau 2).

À l'inverse, ne soyez pas trop précis dans la définition de vos tâches (« Champ "Titre" du formulaire des livres »
/ « Installation des dépendances PHP dans le Dockerfile applicatif » / « Définir la couleur des boutons Ajouter »), vous
aurez alors pléthore de tâches et vous vous perdrez dans la gestion de celles-ci.

Il faut trouver un équilibre. À savoir, qu'il vous est tout à fait possible en cours de projet de créer de nouvelles
tâches, de les redéfinir, de les supprimer ou de définir des sous-tâches. La liste n'est pas gravée dans le marbre.

Dans un contexte professionnel, il faut vous rapprocher de votre chef·fe de projet pour lui demander des modifications
sur la liste des tâches, afin qu'il·elle soit au courant et puisse suivre correctement le projet.

#### Récapitulatif

- Listez l'ensemble des choses à faire pour réaliser le projet.
  <br>Prenez en compte la réalisation, mais aussi la conception et les points réguliers.
  - N'hésitez pas à définir des tâches macro et des sous-tâches.
  - Étiquetez vos tâches : Application web / Infrastructure / Conception / Réunion / Documentation / etc.
- Organisez les tâches selon leur domaine d'application, notamment grâce aux spécifications techniques et
  fonctionnelles.
  <br>Cela vous permettra de suivre l'état d'avancement d'une "partie" du projet (Supervision / Backup / CRUD Livres).
- Vous pouvez vous essayer à l'exercice d'estimation de temps, mais ce n'est pas obligatoire.

#### Outils

Le tableau Kanban est un outil de base pour suivre l'état d'avancement des tâches à travers des "swimlanes" (colonnes) :
- À faire (backlog).
- En cours.
- À tester.
- Terminé.

Selon les organisations, vous trouverez des colonnes supplémentaires (« En attente de validation » / « À déployer » /
« À sélectionner pour la version » / ...).

Plusieurs outils collaboratifs en ligne vous permettent de créer des tableaux Kanban : [Trello](https://trello.com/),
[Kanboard](https://kanboard.org/), [Jira](https://www.atlassian.com/software/jira), [GitLab](https://about.gitlab.com/),
etc.

Certains outils sont plus adaptés pour suivre l'avancement des tâches, notamment si vous en avez un certain nombre et
vous pourrez facilement vous y perdre. À vous de voir ce qui convient le mieux et la façon dont vous souhaitez utiliser
ces outils pour l'organisation de vos tâches.

### Jalons

Un jalon est un point de contrôle planifié dans le temps afin de s'assurer qu'un état spécifique du projet est atteint
ou que certaines tâches sont terminées pour cette date, notamment en vue d'un livrable.

Vous aurez à reprendre les livrables demandés dans le calendrier et les définir en tant que jalons. Pour chacun de ces
jalons, et à partir de la liste des tâches définies, vous devrez définir les tâches à réaliser pour atteindre ce jalon.

Autrement dit, chaque jalon contient une liste de tâches à réaliser. On ne prendra en compte que les tâches
spécifiquement à ce jalon. Mais ça ne signifie pas que les autres tâches ne doivent pas être réalisées. C'est seulement
qu'elles ne sont pas impératives pour ce jalon.

Rien ne vous empêche de définir d'autres jalons pour vous aider à organiser le travail de votre groupe.

{% include _templates/panel/_comment.liquid text=page.milestone_comment %}

### Planning

À partir de la liste des tâches et de la liste des jalons, vous allez pouvoir définir un planning trivial et succinct.

L'objectif, c'est de définir le programme de chaque semaine jusqu'à la fin du projet, et de faire apparaître les
jalons. Vous pouvez également renseigner les réunions régulières si vous trouvez que c'est pertinent ou que le rendu
visuel de ce "planning" est satisfaisant.

{% include _templates/panel/_danger.liquid text=page.planning_danger %}

## ✅ Notation

* Une note globale sera attribuée à l'ensemble du groupe.
  - Si des tâches essentielles sont manquantes, vous serez pénalisés.
  - S'il manque des jalons, vous n'aurez pas la moyenne.
  - Si le planning semble irréaliste, vous serez pénalisés.
* N'hésitez pas à utiliser des annexes pour vous assurer de la lisibilité de vos éléments.
* Soignez votre maîtrise de la langue ; des points malus seront appliqués dans le cas contraire.
