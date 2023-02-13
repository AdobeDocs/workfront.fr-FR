---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Créer et modifier des risques sur les projets
description: Les risques sont des événements ou des facteurs possibles qui empêchent un projet de se terminer à temps ou dans les limites du budget. Les risques peuvent être enregistrés dans le cadre de la création de l’Analyse de cas d’un projet ou à l’aide de l’onglet Risques . Les risques ne sont créés que sur un projet. Vous ne pouvez pas associer des risques à des tâches ou des problèmes.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 8611c7bf8be6405f8ec8462ff2fd0f5998e8a995
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# Créer et modifier des risques sur les projets

Les risques sont des événements ou des facteurs possibles qui empêchent un projet de se terminer à temps ou dans les limites du budget. Les risques peuvent être enregistrés dans le cadre de la création de l’Analyse de cas d’un projet ou à l’aide de l’onglet Risques . Les risques ne sont créés que sur un projet. Vous ne pouvez pas associer des risques à des tâches ou des problèmes.

Les risques peuvent être associés au coût, mais le coût réel du risque n’a aucune incidence sur le coût réel du projet.

>[!NOTE]
>
>Cet article définit les risques associés au projet, tels que vous les définissez dans l’ Analyse de cas du projet ou tels que vous les ajoutez dans l’onglet Risques du projet. Pour plus d’informations sur le champ Risque disponible lors de la modification d’un projet, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets et aux données financières</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p> Gérer les autorisations qui incluent Gérer les finances sur le projet pour lequel vous souhaitez créer ou modifier des risques </p> <p>Pour plus d’informations sur les autorisations de projet, voir l’article <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Partage d’un projet dans Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Créer et modifier des risques dans l’Analyse de cas

Vous pouvez créer des risques dans le cadre de la planification de l’analyse de cas d’un projet. Vous pouvez ensuite les modifier dans l’Analyse de cas, lorsque des modifications sont apportées à leur probabilité, à leur plan d’atténuation ou à leur coût, par exemple. Pour plus d’informations sur la création d’un cas d’entreprise, voir [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Votre administrateur Workfront ou l’administrateur de groupe doit activer la fonction **Risques** avant de pouvoir l’afficher au niveau du projet dans la section Analyse de cas . Pour plus d’informations sur la définition des préférences de projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

La création et l&#39;édition des risques dans l&#39;Analyse de cas sont identiques.

Pour créer ou modifier un risque dans l’Analyse de cas :

1. Accédez au projet pour lequel vous souhaitez créer des risques.
1. Cliquez sur **Analyse de cas** dans le panneau de gauche.
1. Dans le **Risques** , cliquez sur **Modifier les risques**.
1. Saisissez ou modifiez les informations suivantes :

   * **Description :** décrire le risque ;

   * **Coût potentiel**: indiquer le coût estimé si le risque doit survenir ;

   * **Probabilité**: indiquent la probabilité que le risque se produise en pourcentage.

   * **Type :** indiquer la catégorie du risque.
   * **Plan d’atténuation**: mettre à jour la description du plan pour atténuer le risque.

   * **Coût de réduction**: indiquer le coût du plan d’atténuation que vous devez mettre en place pour éviter que le risque ne se produise.

   ![](assets/crp1-350x117.png)

1. (Facultatif) Cliquez sur **Ajouter un autre risque** ajouter des risques supplémentaires.
1. Cliquer sur **Enregistrer**.

## Créer et modifier des risques dans la zone Risques

Outre la création et la modification de risques dans l’Analyse de cas, vous pouvez le faire à l’aide de la variable **Risques** d’un projet.

* [Créer des risques dans la zone Risques](#create-risks-in-the-risks-area)
* [Modifier les risques dans la zone Risques](#edit-risks-in-the-risks-area)

### Créer des risques dans la zone Risques {#create-risks-in-the-risks-area}

1. Accédez au projet pour lequel vous souhaitez créer des risques.
1. Cliquez sur **Risques** dans le panneau de gauche.

   ![Section Risques de la tâche](assets/risks-section-on-project-2022.png)

1. Cliquez sur **Commencer à ajouter des risques** et créer des risques en éditant en ligne leurs informations.

   Ou

   Cliquez sur **Nouveau risque**. Le **Nouveau risque** s’ouvre.

1. Renseignez les informations suivantes :

   * **Description**: décrire le risque ;
   * **Type de risque**: indiquer la catégorie du risque.\
      Votre administrateur Workfront définit les types de risque disponibles dans votre environnement. Pour plus d’informations sur la définition des types de risque, voir l’article [Modifier et créer des types de risque](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Probabilité**: indiquent la probabilité que le risque se produise en pourcentage.
   * **Coût potentiel**: indiquer le coût estimé si le risque doit survenir ;
   * **Coût de réduction**: indiquer le coût du plan d’atténuation que vous devez mettre en place pour éviter que le risque ne se produise.
   * **Coût réel**: indiquer le coût réel du risque en cas de risque.
   * **Plan d’atténuation**: mettre à jour la description du plan pour atténuer le risque.

1. (Conditionnel) Cliquez sur **Entrée** si vous créez le risque en ligne.

   Ou

   Cliquez sur **Enregistrer** si vous modifiez les informations dans la variable **Nouveau risque** de la boîte de dialogue

1. (Facultatif) Sélectionnez une **État** pour le risque, dans la variable **État** lors de l’application de la variable **Standard** pour connaître la liste des risques.

   Par défaut, le Statut du risque est **Identifié**.

### Modifier les risques dans la zone Risques {#edit-risks-in-the-risks-area}

Vous pouvez modifier les risques pendant la durée de vie d’un projet, lorsque des changements se produisent dans leur probabilité, leur coût potentiel ou leur statut, par exemple.

Vous pouvez modifier un risque à la fois ou plusieurs risques en bloc.

Pour modifier les risques :

1. Accédez à un projet pour lequel vous souhaitez modifier les risques existants.
1. Cliquez sur **Risques** dans le panneau de gauche.
1. Commencez à éditer en ligne les champs correspondant aux risques que vous voyez dans la liste pour éditer un risque à la fois.

   Ou

   Sélectionnez un ou plusieurs risques, puis cliquez sur **Modifier** pour modifier plusieurs risques en même temps.

   >[!NOTE]
   >
   >Vous appliquez les mêmes informations à tous les risques sélectionnés lorsque vous modifiez simultanément plusieurs risques. Les informations associées à chaque risque avant vos modifications sont remplacées par une modification en masse.

1. Si vous avez cliqué sur **Modifier**, la variable **Modifier le risque** s’ouvre.

   Envisagez de modifier les champs suivants :

   * **Description**: modifiez la description du risque.
   * **Type de risque**: indiquer la catégorie du risque.
   * **Probabilité**: indiquent la probabilité que le risque se produise en pourcentage.
   * **Coût potentiel**: indiquer le coût estimé si le risque doit survenir ;
   * **Coût de réduction**: indiquer le coût du plan d’atténuation que vous devez mettre en place pour éviter que le risque ne se produise.
   * **Coût réel**: indiquer le coût réel du risque en cas de risque.
   * **Plan d’atténuation**: mettre à jour la description du plan pour atténuer le risque.

1. Cliquez sur **Enregistrer les modifications**.
1. (Facultatif) Modifiez la variable **État** pour un risque, dans la variable **État** lors de l’application de la variable **Standard** pour connaître la liste des risques.

   >[!NOTE]
   >
   >Vous ne pouvez pas modifier la variable **État** de risques dans la **Modifier le risque** de la boîte de dialogue Vous ne pouvez le faire que dans une modification en ligne.
