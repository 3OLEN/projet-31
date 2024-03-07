---
layout: page
title: Grille d'évaluation
slug: evaluation

description: Éléments de notation lors des passages de groupe et en individuel.
warning_evaluation: |
    La note de la soutenance de groupe est individuelle. Plusieurs éléments sont communs à chaque membre du groupe, mais
    d'autres concernent exclusivement l'individu.
warning_interview: |
    Méfiez-vous, ils risquent de se plaindre de certains éléments du Projet 31 : ils n'ont pas eu le GitLab 3OLEN tout
    de suite, ils ont eu les VM école en milieu de Projet 31, il n'y a pas d'accès distant possible sur les VM école...
    <br><br>Vous pouvez couper court à leurs plaintes, sauf si c'est argumenté et pertinent. Vous n'êtes pas là pour
    écouter leurs doléances.
---

Chaque étudiant·e aura deux notes, correspondant aux deux soutenances auxquelles il·elle participera.

{% include _templates/panel/_warning.liquid text=page.warning_evaluation %}

## 🎯 Objectifs pédagogiques

Au sein des projets 3OLEN, nous souhaitons évaluer l'aspect professionnel afin de pouvoir valider que nos étudiants sont
viables pour entrer sur le marché du travail, notamment sur leur comportement / attitude et leur état d'esprit.

Par ailleurs, ils doivent se rendre compte des attentes d'un projet professionnel. Les projets transverses ne sont plus
des projets étudiants, mais des projets qui doivent être menés comme en entreprise. C'est-à-dire qu'on a une attente
forte sur la production, leur implication et l'aspect professionnel de leurs livrables.

En d'autres termes, imaginez que vous avez affaire à des prestataires dans le cadre de votre activité professionnelle.

### ✅ Réussite / ❌ Échec

N'hésitez pas à attribuer une note dans l'un des extrêmes :

- Si l'étudiant·e n'a pas une attitude professionnelle ou n'a pas une production et contribution suffisante, n'ayez
  aucun scrupule à lui mettre des 0.
- Si l'étudiant·e s'est impliqué·e, a fait plus que sa part, a porté le groupe en solitaire ou à bout de bras,
  récompensez son mérite et mettez-lui des points au max.

### 🪁 Pousser à l'amélioration

Malgré tout, notre volonté, c'est de les accompagner vers les objectifs pédagogiques des projets transverses et de leur
diplôme. Nous voulons être plus ferme avec eux pour leur faire prendre conscience que le bachelor est une étape
charnière dans leurs études et leur intégration au monde professionnel.

Cette soutenance (groupe + individuelle) est l'occasion de les mettre en situation ± réelle et de faire le maximum de
retours pour pointer ce qui ne va pas et les aider à améliorer ce qu'ils ont fait, présenté, produit.

Je vous saurai gré de définir le maximum de remarques sur l'oral, le support, l'aspect professionnel et de me les
transmettre ensuite que je puisse les faire remonter à chacun·e. J'ai aussi défini un court moment (5 minutes), intitulé
« Remarques du Jury », après chaque soutenance (groupe et individuelle) pour que vous puissiez donner les remarques les
plus importantes à chaud.

Ils doivent toutes et tous en prendre note textuellement et n'ont pas à discuter vos remarques. Faites attention à ne
pas déborder sur les 5 minutes prévues et n'utilisez pas non plus le temps alloué à l'entretien individuel pour faire
d'autres remarques.

Merci beaucoup ☺️

## 🗣️ Entretien

Lors des passages individuels (seulement), vous avez une phase d'entretien, de questions-réponses, de 10 minutes.

Mettez l'accent sur la contribution personnelle de l'étudiant·e afin de définir qui a travaillé et qui a laissé les
autres faire le travail. Plusieurs personnes se sont plaintes de leurs camarades de groupe et il y a eu des rendus
intermédiaires (dossier de conception / cahier de recette) dont la contribution de chacun·e a été assez inégale.

Concernant la gestion de projet et la communication interne, je leur ai fourni des éléments de base pour avoir un
minimum viable. C'est surtout sur le Projet 32 que l'on évaluera la gestion de projet.

Vous pouvez les titiller à ce sujet lors de l'entretien (à savoir qu'ils ont commencé les cours de gestion de projet en
plein milieu du Projet 31) et notamment voir s'ils ont commencé à y réfléchir et s'ils ont un avis ou pas encore.

{% include _templates/panel/_warning.liquid text=page.warning_interview %}

## 📊 Notation des soutenances

### Oral de groupe

{% assign group_oral_step = site.data.defense.group_steps | where_exp: "step", "step.name == 'Oral groupe'" | first %}
{% assign group_oral_duration = group_oral_step.duration | date: "%M minutes" %}
{% assign group_comment = "**Rappel** : L'oral de groupe dure "
    | append: group_oral_duration
    | append: " (avec la démonstration)."
%}
{% include _templates/panel/_comment.liquid text=group_comment %}

{% comment %} <!-- Grille d'évaluation « Groupe » --> {% endcomment %}
{% include _pages/final/_evaluation_grid.liquid grid=site.data.final_evaluation.group_defense jury_view=true %}

-----

### Oral individuel

{% assign student_oral_step = site.data.defense.student_steps
    | where_exp: "step", "step.name == 'Oral individuel'"
    | first
%}
{% assign student_oral_duration = student_oral_step.duration | date: "%M minutes" %}
{% assign student_interview_step = site.data.defense.student_steps
    | where_exp: "step", "step.name == 'Entretien'"
    | first
%}
{% assign student_interview_duration = student_interview_step.duration | date: "%M minutes" %}

{% assign student_comment = "**Rappel** : L'oral individuel dure "
    | append: student_oral_duration
    | append: " (avec la démonstration), suivi de "
    | append: student_interview_duration
    | append: " d'entretien avec le jury."
%}
{% include _templates/panel/_comment.liquid text=student_comment %}

{% comment %} <!-- Grille d'évaluation « Individuel » --> {% endcomment %}
{% include _pages/final/_evaluation_grid.liquid grid=site.data.final_evaluation.student_defense jury_view=true %}
