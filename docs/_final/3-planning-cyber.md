---
layout: linked_pages/final
title: Planning - CYBER
slug: planning-cyber

description: Planification de la journée d'examen et ordres de passage des Cyber et du projet « Contr'OLEN ».
full_size: true

shortcut_links:
- type: final
  identifier: planning-dev
  title: Afficher le planning des DEV
  badge: calendar
---

{% include _templates/list/_related_pages.liquid pages=page.shortcut_links %}

{% include _pages/final/_planning.liquid scope=site.data.defense._parameters._scopes._student.scope project='cyber' %}
