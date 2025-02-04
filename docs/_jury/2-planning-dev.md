---
layout: linked_pages/jury
title: Planning - DEV
slug: planning-dev

description: Planification de la journée d'examen et ordres de passage des Dev et du projet « Disp'OLEN ».
full_size: true

shortcut_links:
- type: jury
  identifier: planning-cyber
  title: Afficher le planning des CYBER
  badge: calendar
---

{% include _templates/list/_related_pages.liquid pages=page.shortcut_links %}

{% include _pages/final/_planning.liquid scope=site.data.defense._parameters._scopes._jury.scope project='dev' %}
