---
layout: page
title: Évaluation finale
permalink: /final

description: Intitulé de l'épreuve finale et points d'attention.
---

L'épreuve finale du « Projet 31 » consiste en une démonstration de groupe et une soutenance de projet individuelle
devant un jury d'examen composé de professionnels et des anciens diplômés de l'ORT.

Pendant le passage de groupe, vous devrez vous présenter, rappeler le contexte et faire une démonstration totale de la
solution permettant de répondre aux problématiques et spécifications indiquées pour le projet. Cela permettra de
valider si le projet est réalisé et fonctionnel.

Lors de la soutenance individuelle, vous expliquerez votre contribution et détaillerez votre réalisation personnelle.
Votre expertise et vos connaissances techniques seront évaluées, notamment à travers un entretien auprès d'un jury.

## ⚠️ Points d'attention

* Vous fournirez une prestation **professionnelle** face à d'autres professionnels. Ils seront intransigeants.
  - Vous serez considérés comme des professionnels présentant votre solution auprès d'un comité d'expert du numérique
    agissant pour le compte du client final.
  - Votre tenue vestimentaire doit être soignée : pas de t-shirt, pas de sweat, pas de veste à capuche, pas de
    survêtement. Un effort aussi sur les chaussures.
    - Messieurs : a minima la chemise. Le _must_ c'est le costume, pour la meilleure des impressions et pour faire
      plaisir au jury.
    - Pour information, le jour de la soutenance professionnelle du 9 septembre, c'est une tenue exemplaire et
      irréprochable !
  - Votre stature et votre expression orale doivent être soignées et travaillées.
* Votre présentation et vos démonstrations sont préparées en amont et doivent être fluides et d'une qualité
  professionnelle.
  - Imaginez que vous faites la présentation de la solution à mettre en production et que le client doit valider votre
    prestation. Il faut que la décision du client soit "Go". Si c'est un "no go", c'est que vous avez échoué.

## 📑 Éléments de l'épreuve

<div class="final-content-list simple-list">
    {% assign final_pages = site.final | where_exp: "page", "page.slug != 'index'" %}
    {% include _templates/list/_final_pages.liquid final_pages=final_pages %}
</div>
