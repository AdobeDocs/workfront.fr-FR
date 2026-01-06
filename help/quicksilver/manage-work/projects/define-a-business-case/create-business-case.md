---
navigation-topic: business-case-and-scorecards
title: Créer une analyse de rentabilité pour un projet
description: Vous pouvez utiliser le business case pour demander un projet et définir l’objectif, le budget et le bénéfice potentiel du projet. La personne gestionnaire de portfolio ou la personne sponsor de projet utilise les informations du business case pour analyser le projet et établir sa priorité avant de l’approuver.
author: Becky
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 63%

---

# Créer une analyse de rentabilité pour un projet

<!--Audited: 6/2025-->

Vous pouvez utiliser le business case pour demander un projet et définir l’objectif, le budget et le bénéfice potentiel du projet. La personne gestionnaire de portfolio ou la personne sponsor de projet utilise les informations du business case pour analyser le projet et établir sa priorité avant de l’approuver.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader"><p>Formule Adobe Workfront</p></td> 
   <td> 
   <p>Prime ou version ultérieure</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
   <p>Standard </p> 
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td> <p>Accès Modifier aux Projets, aux Données financières et à la Gestion des ressources</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Autorisations Gérer ou supérieures sur le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Tenez compte des points suivants lorsque vous demandez un projet par le biais d’un business case :

* Votre administrateur ou administratrice Adobe Workfront ou de groupes doit activer les sections du business case avant qu’elles n’apparaissent sur votre projet.\
  Pour plus d’informations sur l’activation des sections dans le business case au niveau du système, consultez l’article [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Pour plus d’informations sur les zones du business case, consultez l’article [Vue d’ensemble des zones du business case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Si vous souhaitez que votre projet reçoive un score dans l’optimisateur de portfolio, vous devez renseigner toutes les zones du business case, à l’exception de la zone Objectifs. Le renseignement de la zone Objectifs est facultatif. Le projet reçoit un score dans l’optimisateur de portfolio, même si cette zone n’est pas renseignée.

  Pour plus d’informations sur l’utilisation des cartes de performance et de l’optimisateur de portfolio, consultez l’article [Appliquer une carte de performance à un projet et générer un score d’alignement](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Créer un business case

{{step1-to-projects}}

1. Cliquez sur **Nouveau projet**, puis sélectionnez **Demander le projet** dans la liste déroulante qui s’affiche. Le projet est créé et le statut **Idée** est attribué par défaut.

   >[!CAUTION]
   >
   >Si le statut Idée a été supprimé dans votre instance Workfront, le projet est placé dans le statut par défaut pour les nouveaux projets, comme défini dans la zone Préférences du projet. Pour plus d’informations sur la configuration des préférences de projet, voir [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Saisissez un nom dans le champ Titre du projet .
1. (Facultatif) Cliquez sur l’icône **Plus** ![Icône Plus](assets/qs-more-icon-on-an-object.png), puis **Joindre un modèle** pour créer la structure de répartition du travail de votre projet.

   Ou

   Commencez à ajouter manuellement des tâches au projet.

1. (Conditionnel) Si vous avez choisi de joindre un modèle, continuez à joindre le modèle au projet.
1. Dans le volet de gauche, cliquez sur **Analyse de rentabilité**.
1. (Facultatif) Pour modifier la section **Informations sur le projet**, cliquez sur **Modifier les informations du projet**.

   Pour plus d’informations sur la modification des champs de section **Informations sur le projet**, consultez la section [Informations sur le projet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) dans l’article [Présentation des domaines de l’analyse de rentabilité](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facultatif) Pour modifier la section **Objectifs**, cliquez sur **Modifier les objectifs**.

   Pour plus d&#39;informations sur la modification de la section **Objectifs** de l&#39;Analyse de rentabilité, reportez-vous à la section [Objectifs](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) de l&#39;article [Aperçu des aspects de l&#39;Analyse de rentabilité](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facultatif) Pour modifier la section **Dépenses**, cliquez sur **Modifier les dépenses**.

   Pour plus d&#39;informations sur la modification de la section **Dépenses** de l&#39;Analyse de rentabilité, reportez-vous à la section [Dépenses](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) de l&#39;article [Aperçu des domaines de l&#39;Analyse de rentabilité](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Facultatif) Cliquez sur **Modifier l&#39;établissement du budget de ressources** pour budgéter vos ressources et obtenir le coût budgété de la main-d&#39;œuvre associé aux fonctions du projet. Pour plus d’informations, voir [Établissement du budget des ressources dans le business case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >Les informations affichées ici sont les mêmes que celles affichées dans les outils de budgétisation des ressources au niveau du système.

1. (Facultatif) Cliquez sur **Modifier les risques** pour ajouter des risques potentiels à ce projet. Pour plus d’informations sur l’ajout de risques au business case, voir la section [Risques](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) dans l’article [Vue d’ensemble des zones du business case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (Facultatif) Sélectionnez une **Carte de performance** dans le menu déroulant **Ajouter une carte de performance à ce projet**.

   Les cartes de performances doivent être créées avant de pouvoir être jointes aux projets.

   Pour plus d’informations sur les cartes de performances, voir l’article [Appliquer une carte de performances à un projet et générer un sore d’alignement](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Facultatif) Sélectionnez un **formulaire personnalisé** dans le menu déroulant **Formulaires personnalisés**.

   Les formulaires personnalisés doivent être créés avant de pouvoir être associés à des projets.

   Pour plus d’informations sur Custom Forms, consultez l’article [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur **Envoyer**. Le statut du projet passe à **Demandé** et il est soumis pour approbation du business case.

   Pour plus d’informations sur l’approbation d’un business case, voir l’article [Approuver un business case](../../../manage-work/projects/define-a-business-case/approve-business-case.md).


>[!TIP]
>
> Une fois l’analyse de rentabilité terminée, vous pouvez en exporter une copie dans un fichier .pdf. Pour plus d’informations sur l’exportation de l’analyse de rentabilité dans un fichier .pdf, voir [Exporter l’analyse de rentabilité d’un projet](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md).


