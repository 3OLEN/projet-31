---
layout: intermediary_deliverable
title: "Livrable intermédiaire - Version 1"
slug: livraison-version-1

assessment: version-1
description: |
  Une version complète et fonctionnelle doit être mise à disposition par chacun des groupes afin d'avoir une version
  initiale entièrement intégrée et disponible pour avoir une première approche du projet dans son ensemble.
  <br><br>Cette version 1.0 pourra servir de solution de repli au cas où la version finale de fin de projet ne soit pas
  fonctionnelle et disponible.

acceptance_testing_comment: "Ce document est à la charge de **TOUTE** l'équipe et ce pour **chaque** partie, même les
parties concernant les fonctionnalités de l'application."
---

# ☑️ Attentes

Pour cette date, une version 1.0 des sources applicatives sera déployée sur l'infrastructure du groupe. Il sera possible
d'utiliser l'application dans son ensemble en tant que « beta-test ».

Cette livraison doit tenir lieu de démonstration professionnelle auprès des clients.

## 💻️ Application web

Les principaux éléments de l'application doivent être réalisés et le maximum de fonctionnalités doivent être livrés.

L'utilisateur doit pouvoir exploitation l'application de la manière la plus "normale" et cohérente vis-à-vis de ses
attentes, aussi bien sur l'UX que l'UI ou que les fonctionnalités globales.

Le jeu de données doit être totalement en accord avec le jeu de données final, lorsque l'application sera officiellement
mise à disposition.

### Quelques conseils

* Vérifiez vos scénarios utilisateurs.
  - Création d'un compte utilisateur.
  - Première connexion d'un utilisateur.
  - Droits d'accès aux écrans.
  - etc.
* Utilisez les *tags* de Git pour figer votre version 1.0.
  - <span class="text-danger">‼️</span> Respectez le `semantic versioning`.
  - Certaines applications indiquent la version exacte du produit dans le *footer*.

## 🏗️ Infrastructure

Les trois environnements (intégration / recette / production) doivent être déployés et fonctionnels. La version
applicative de chacun de ces environnements peut être différente (`1.0` sur la production, `1.1` sur la recette et
`1.1.1` sur l'intégration, par exemple), tant que la version de production est mise à disposition du client.

Les principales contraintes de l'infrastructure doivent être réalisées et disponibles sur le serveur.

Le compte d'accès doit être fourni et une démonstration des éléments devra être présentée.

## 📝 Recette

Afin de valider la solution, il faut mener une recette, c'est-à-dire une phase durant laquelle toutes les
fonctionnalités et toutes les contraintes sont vérifiées (implémentées, intégrées, fonctionnelles).

La recette s'effectue à travers un document fourni au client : le cahier de recette. Il tient lieu de preuve officielle
de la réalisation et du fonctionnement du produit.

Ce document professionnel présente les différents éléments du projet et valide le fait que toutes les demandes et les
contraintes sont implémentées et fonctionnelles (OK).

{% include _templates/panel/_comment.liquid text=page.acceptance_testing_comment %}

### Instructions

* Un rendu Moodle par groupe : `nom_groupe-cahier_recette-v1.0`.
* Je vous conseille de le faire sur Word.
  - Utilisez l'orientation paysage pour vos tableaux.
  - Vous fournirez un PDF, bien évidemment.
* Vous pouvez le faire sur Excel, mais pour rappel, je n'ai pas la suite Office, donc à vos risques et périls...
* Vous pouvez le faire sur un outil en ligne.
  - Vous pouvez fournir le lien de consultation ou un PDF de la page ou éventuellement la page HTML.
  - Pour le lien de consultation : si j'ai un doute sur le différentiel entre la date de rendu et le moment où je le
    visualise, je me réserve le droit de vous refuser le cahier de recette.
* N'oubliez pas que vous fournissez un travail d'une qualité professionnelle, comme si vous étiez en entreprise et que
  vous vous adressiez à un client.

## 📋️ Reste à faire

Tout ne sera pas forcément terminé pour cette version 1.0. Il est de votre devoir de lister les éléments traités et les
éléments manquants. Vous devez fournir une liste des éléments restants, leur priorité et s'ils seront prêts pour la
version finale lors de la soutenance de projet (logiquement la version 2.0 ou la version 3.0 si vous prévoyez une
nouvelle livraison intermédiaire de votre propre chef).

Pour rappel, l'ORT vous reste accessible pendant votre période entreprise.

# ✅ Notation

Cette version initiale sera soumise à une notation complémentaire pour le « projet transverse 1 ».

* Une note de groupe pour définir si le projet est bien livré et déployé en "production".
  - Avec le cahier de recette.
  - La qualité du produit sera évidemment un critère important.
* Une note pour les Dev et une note pour les Infra sur le travail fourni.
* Si le projet n'est pas déployé, la note sera un chiffre rond : 0.
