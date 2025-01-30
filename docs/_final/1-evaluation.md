---
layout: linked_pages/final
title: Grille d'évaluation
slug: evaluation

description: Éléments de notation lors des passages de groupe et en individuel.
---

Vous serez évalués sur votre soutenance orale individuelle.

La présentation de groupe et la démonstration globale ont pour objectif de valider votre solution et de vérifier qu'elle
est fonctionnelle de bout en bout.

## Oral de groupe

L'oral de groupe ne donne pas lieu à une note en tant que telle, mais il peut avoir un impact négatif sur la note de la
soutenance individuelle, donc ne prenez pas cet oral à la légère. Si le jury n'est pas convaincu par votre solution, il
pourra forcer le rattrapage du Projet 31.

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

-----

## Soutenance individuelle

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
