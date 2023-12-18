---
layout: intermediary_deliverable
title: "Livrable intermédiaire - Dossier de conception"
slug: dossier-conception

assessment: design-document
description: |
  Dans le cadre de votre phase de conception, vous produirez un document
  (`nom_groupe-dossier-conception.pdf`) qui présentera votre réflexion sur le sujet et votre organisation.

  N'hésitez pas à recourir à des "annexes" pour inclure des documents de conception. Ces annexes peuvent être intégrés
  au document (en fin de document) ou fournies à part (archives / pages web). Rappelez-vous que ces documents doivent
  être accessibles quelle que soit la plateforme.
  
  Par ailleurs, n'oubliez pas le sommaire, les index, les numérotations, les en-têtes et pieds de page, etc.

  Il sera composé des éléments suivants :

document_model:
  - title: "Projet"
    description: "Cette partie contiendra les informations globales du projet afin de le présenter ainsi que son
contexte. Vous présenterez également votre groupe."
    sections:
    - title: "Contexte"
      description: "Vous rappellerez le contexte du projet Bibli'OLEN, c'est-à-dire le sujet et le besoin énoncé."
    - title: "Groupe"
      description: "Vous présenterez votre groupe de projet, c'est-à-dire les membres qui le composent et leurs
      rôles respectifs."
    - title: "Notes de réunion"
      description: |
        Afin de vous motiver à collaborer ensemble et à entreprendre des points réguliers (organiser
        des réunions hebdomadaires courtes pour faire l'état d'avancement, par exemple) vous allez devoir justifier la
        conduite d'au moins **deux** réunions ayant servi à la conception du projet, et donc à la rédaction de ce
        document.

        Cette partie vous sert d'apprentissage dans les bonnes pratiques de la conduite de réunions. Dès lors que vous
        organisez ou que vous participez à une réunion, prenez des notes afin de garder une trace écrite de ce qui
        a été dit et demandé/décidé. Cette note est ensuite à partager avec les participants (ou en tout cas les
        personnes concernées/intéressées/impliquées) afin de valider ce qui a été dit et de pouvoir prouver
        des décisions.
      related_pages:
      - type: "assessment"
        identifier: "notes-reunion"
        title: "Aide à la prise de notes"
        blank: true
  - title: Étude
    description: "Cette partie traitera de votre étude fonctionnelle du sujet et des documents de conception qui en
    résultent."
    sections:
    - title: Utilisateurs
      description: "Vous définirez les différents rôles utilisateur de l'application et leurs interactions avec 
      l'application par le biais d'un ou plusieurs diagramme·s de cas d'utilisation."
    - title: Actions utilisateur
      list:  
      - "Pour chaque action déterminée par les cas d'utilisation, vous définirez des sous-parties fonctionnelles (et
        éventuellement sous-sous-parties) avec les diagrammes d'activité correspondants."  
      - "En complément de ces diagrammes, chaque « Dev » enrichira une fonctionnalité (différente pour chacun) avec
       le diagramme de séquences correspondant."
      related_pages:
        - type: "assessment"
          identifier: "uml"
          title: "Détail des diagrammes UML à fournir"
          blank: true
      comment: "Même si le module a été mené pour les « Dev », nous attendons aussi une participation de la part des
      « Infra » (au moins un chacun). Collaborez avec les « Dev » et apprenez de l'enseignement qu'ils ont reçu."
    - title: MCD
      description: |
        Avant de créer la BDD, il est nécessaire de concevoir le modèle conceptuel de données (MCD) pour lister
        les tables, les champs et les relations.

        La deuxième séance sera co-animée avec M. Gilot. Donc prévoyez de travailler sur le MCD avant cette séance afin
        de pouvoir en discuter avec lui et ainsi le critiquer (positif et négatif).
      related_pages:
        - type: "assessment"
          identifier: "mcd"
          title: "Informations complémentaires sur le MCD"
          blank: true
  - title: Solution
    description: "Cette partie apportera des éléments plus techniques sur la solution qui sera mise en place."
    sections:
    - title: "Description"
      description: "Présentez globalement la solution telle qu'elle sera définie dans la finalité. N'hésitez pas à
      intégrer éventuellement un schéma, si cela vous semble pertinent."
    - title: "Infrastructure"
      description: "Cette partie décrit l'infrastructure du projet en se basant sur les contraintes techniques fournies." 
      sections:
      - title: Diagramme de déploiement
        description: Représentation graphique de la solution technique qui devra être mise en place.
        related_pages:
        - type: "assessment"
          identifier: "uml"
          title: "Détail des diagrammes UML à fournir"
          blank: true
      - title: Exploitation
        description: "Vous indiquerez l'ensemble des outils et demandes pour l'exploitation de l'infrastructure."  
    - title: "Application"
      description: "Cette partie concerne l'application web et la façon dont elle sera développée."
      sections:
      - title: Architecture applicative
        description: Étude menée sur l'architecture applicative selon le concept MVC.
        related_pages:
        - type: "assessment"
          identifier: "archi-web"
          title: "Attentes sur l'étude de l'architecture applicative"
          blank: true
      - title: Aspect graphique
        description: "Rappelez les contraintes définies sur l'aspect graphique et l'exploitation de l'application web
        par les futurs utilisateurs."
        related_pages:
        - type: "assessment"
          identifier: "charte-graphique"
          title: "Charte graphique et maquettes"
          blank: true
  - title: Planification
    description: |
      Vous n'aurez pas à réaliser de la gestion de projet dans le cadre de ce projet transverse. Néanmoins,
      certains éléments de base sont à prendre en compte et à définir afin de conduire au mieux le projet.

      Vous pouvez prendre en charge la gestion de projet, mais ce ne sera pas du tout un critère d'évaluation.
    sections:
    - title: Tâches
      description: "Il est essentiel de définir l'ensemble des tâches « Dev » / « Infra » / « Projet » à réaliser tout
      au long du projet afin de savoir ce que vous avez à faire, ainsi que pouvoir suivre ce qui a été fait."
    - title: Jalons
      description: "Comme vous l'avez vu dans le calendrier, il y a des dates importantes avec des livrables à rendre
      concernant la production. Vous devez donc en définir des jalons : des points de contrôle vous assurant que vous
      avez effectué les tâches critiques pour le livrable."
    - title: Planning
      description: "À partir des deux éléments précédents, vous pourrez définir un planning trivial afin d'organiser
      le travail à réaliser."
    related_pages:
    - type: "assessment"
      identifier: "planification"
      title: "Détail et informations sur la planification"
      blank: true
---

{% include _pages/assessments/content/_document_model.liquid model_content=page.document_model %}
