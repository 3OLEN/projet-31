---
layout: linked_pages/final
title: Grille d'évaluation
slug: evaluation

description: Éléments de notation lors des passages de groupe et en individuel.
---

Vous serez évalués à la fois sur la soutenance orale de groupe, mais aussi sur la soutenance orale individuelle.

Le coefficient de la soutenance individuelle est plus élevé que celui de la soutenance de groupe. Cependant, l'oral de
groupe permettra au jury d'avoir une première impression sur votre travail d'équipe et donc de votre implication.

## Oral de groupe

{% assign group_oral_step = site.data.defense.group_steps | where_exp: "step", "step.name == 'Oral groupe'" | first %}
{% assign group_oral_duration = group_oral_step.duration | floor | append: " min" %}
{% assign group_comment = "**Rappel** : L'oral de groupe dure "
    | append: group_oral_duration
    | append: " (avec la démonstration)."
%}
{% include _templates/panel/_comment.liquid text=group_comment %}

{% comment %} <!-- Grille d'évaluation « Groupe » --> {% endcomment %}
{% include _pages/final/_evaluation_grid.liquid grid=site.data.final_evaluation.group_defense student_view=true %}

-----

## Oral individuel

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
    | append: " (avec la démonstration), suivi de "
    | append: student_interview_duration
    | append: " d'entretien avec le jury."
%}
{% include _templates/panel/_comment.liquid text=student_comment %}

{% comment %} <!-- Grille d'évaluation « Individuel » --> {% endcomment %}
{% include _pages/final/_evaluation_grid.liquid grid=site.data.final_evaluation.student_defense student_view=true %}
