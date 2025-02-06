---
layout: linked_pages/jury
title: Grille d'évaluation
slug: evaluation

description: Éléments de notation lors des passages de groupe et en individuel.
warning_group_oral: |
  L'oral de groupe peut faire appliquer des malus sur les notes individuelles de l'équipe : projet non fini, oral de
  groupe ou démonstration non préparés, manque de sérieux, etc.
---

Chaque étudiant·e sera noté sur sa soutenance individuelle.

L'oral de groupe permet au jury de découvrir l'équipe et la solution réalisée.

{% include _templates/panel/_warning.liquid text=page.warning_group_oral %}

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
  aucun scrupule à lui mettre un 0.
- Si l'étudiant·e s'est impliqué·e, a fait plus que sa part, a porté le groupe en solitaire ou à bout de bras,
  récompensez son mérite.

## 📊 Notation des soutenances

### Oral de groupe

{% assign group_introduce_step = site.data.defense.group_steps | where_exp: "step", "step.name == 'Présentation groupe'" | first %}
{% assign group_introduce_duration = group_introduce_step.duration | floor %}
{% assign group_proof_step = site.data.defense.group_steps | where_exp: "step", "step.name == 'Démonstration'" | first %}
{% assign group_proof_duration = group_proof_step.duration | floor %}

{% assign group_oral_duration = group_introduce_duration | plus: group_proof_duration | append: " min" %}
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
{% assign student_oral_duration = student_oral_step.duration | floor | append: " min" %}
{% assign student_interview_step = site.data.defense.student_steps
    | where_exp: "step", "step.name == 'Entretien'"
    | first
%}
{% assign student_interview_duration = student_interview_step.duration | floor | append: " min" %}

{% assign student_comment = "**Rappel** : L'oral individuel dure "
    | append: student_oral_duration
    | append: " (avec une potentielle démonstration), suivi de "
    | append: student_interview_duration
    | append: " d'entretien avec le jury."
%}
{% include _templates/panel/_comment.liquid text=student_comment %}

{% comment %} <!-- Grille d'évaluation « Individuel » --> {% endcomment %}
{% include _pages/final/_evaluation_grid.liquid grid=site.data.final_evaluation.student_defense jury_view=true %}
