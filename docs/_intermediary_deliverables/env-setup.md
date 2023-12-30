---
layout: intermediary_deliverable
title: "Livrable intermédiaire - Mise en place de l'environnement"
slug: mise-en-place-environnement

assessment: env-setup
description: |
  Plusieurs environnements doivent être mis en place pour le projet par le biais de Docker :
  
  - **Développement** : Un environnement de travail mis à disposition de chaque développeur du projet, généralement en
    local pour de meilleures performances et sécurité.
  - **Intégration** : Un environnement permettant d'effectuer l'intégration continue après chaque merge sur la branche
    principale de développement.
  - **Recette** : Un environnement où sont déployées les versions à livrer au client. Cet environnement permet de
    tester les fonctionnalités et de valider la version.
  - **Production** : Un environnement où est déployée la version courante accessible par les utilisateurs finaux.

env_availability_comment: "Du fait de l'aspect incertain de la disponibilité matérielle, il ne vous sera pas forcément 
demandé d'avoir ces environnements prêts à cette date, mais dès lors qu'il vous sera possible de le faire, ces
environnements doivent être opérationnels."

production_env_danger: "N'attendez pas la livraison de la version 1 pour mettre à disposition l'environnement de
production. Celui-ci aussi doit être opérationnel le plus tôt possible."
---

## ☑️ Attentes

À partir de cette date, les développeurs doivent être en mesure de développer sur leur machine locale à travers leur
propre environnement de développement. Ils ont donc à disposition les images Docker leur permettant de monter
l'ensemble de l'infrastructure pour lancer l'application, développer et tester leurs fonctionnalités.

Cet environnement sera amené à évoluer au cours du projet, mais faites en sorte qu'il soit le plus complet possible
au plus tôt afin de réduire l'impact des problèmes techniques sur l'application : BDD, serveur de fichiers, HTTPS, etc.

### Intégration et recette

L'environnement d'intégration et l'environnement de recette doivent être montés au plus tôt et intégrés dans les chaînes
de CI/CD. 

Vous devez préparer ces environnements afin de pouvoir les mettre à disposition sur le serveur attribué à votre groupe
dès qu'il vous sera possible d'y accéder.

{% include _templates/panel/_comment.liquid text=page.env_availability_comment %}

### Production

{% include _templates/panel/_danger.liquid text=page.production_env_danger %}
