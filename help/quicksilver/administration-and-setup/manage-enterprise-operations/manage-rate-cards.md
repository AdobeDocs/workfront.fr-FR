---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gérer les cartes tarifaires
description: Une carte tarifaire représente l’accord contractuel avec votre client dans lequel des taux horaires sont définis pour les fonctions qui termineront le travail. Dans une carte tarifaire, vous pouvez définir plusieurs taux de facturation par fonction, en fonction des attributs.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 14%

---

# Gérer les cartes tarifaires

Une carte tarifaire représente l’accord contractuel avec votre client dans lequel des taux horaires sont définis pour les fonctions qui termineront le travail. Dans une carte tarifaire, vous pouvez définir plusieurs taux de facturation par fonction, en fonction d’attributs tels que l’agence, l’emplacement ou le centre de coûts. Vos attributs de taux uniques sont configurés dans la zone Configuration . Pour plus d’informations, voir [Définir des attributs de taux](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

Par exemple, vous pouvez avoir une fonction Designer basée à Paris pour l’agence A, une autre Designer basée à Paris pour l’agence B et une troisième Designer basée à New York non affectée à une agence, chacune avec des taux de facturation différents. Toutefois, les attributs ne sont pas obligatoires pour les fonctions sur une carte tarifaire. Les attributs servent d’outils pour établir des taux plus granulaires. Un taux de facturation sur une carte tarifaire peut également être valide pour une date effective, de sorte que le taux commence et se termine à des dates spécifiées.

Vous pouvez également verrouiller les taux sur une carte tarifaire pour éviter qu’ils ne soient remplacés au niveau du projet ou de la tâche. Les taux verrouillés sont les plus élevés dans la hiérarchie des taux de facturation, à l’exception des taux conservés pour un projet. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Modifier l’accès aux [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Pour modifier une carte tarifaires partagée avec vous, vous devez disposer des autorisations Gérer sur la carte tarifaire.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter une carte tarifaire

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Cartes tarifaires**].
1. Cliquez sur [!UICONTROL **Nouvelle carte tarifaire**], puis sur [!UICONTROL **Créer une carte tarifaire**].
1. Saisissez un nom et une description pour la carte tarifaire dans la zone [!UICONTROL **Nouvelle carte tarifaire**].

   Le nom doit être unique.

   ![ Boîte de dialogue Nouvelle carte tarifaire ](assets/new-rate-card-dialog.png)

1. (Facultatif) Sélectionnez un [!UICONTROL **Groupe**] pour la carte tarifaire. C&#39;est l&#39;agence qui définit la carte tarifaire.
1. (Facultatif) Sélectionnez une [!UICONTROL **Société**] pour la carte tarifaire. Il s’agit du client pour lequel les taux sont attribués par contrat.

   >[!NOTE]
   >
   >Le Groupe et la Société sont utilisés non seulement dans les détails de la carte tarifaire, mais également comme filtres lors de l&#39;association d&#39;une carte tarifaire à un projet.

1. Cliquez sur **Créer**.

   L’écran Carte tarifaire > Fonctions et taux s’affiche.

1. Cliquez sur [!UICONTROL **Ajouter une fonction**].
1. Dans la zone [!UICONTROL **Nouveau taux de facturation**], sélectionnez une [!UICONTROL **Fonction**] pour définir les taux de facturation.

   ![Boîte de dialogue du nouveau taux de facturation](assets/new-job-role-rate-on-rate-card.png)

1. (Facultatif) Sélectionnez des attributs pour le taux de facturation, tels que l’agence, l’emplacement ou le centre de coûts.

   >[!NOTE]
   >
   >Ces attributs sont définis séparément et peuvent affecter les calculs de produits et de coûts. Pour plus d’informations, voir [Définir des attributs de taux](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Sélectionnez une [!UICONTROL **Devise**] pour le taux de facturation.
1. (Facultatif) Saisissez un [!UICONTROL **alias de fonction**] pour la fonction.

   Si le nom d’alias que vous tapez n’existe pas déjà, vous pouvez l’ajouter.

   Lorsque la carte tarifaire est associée à un projet, l’alias apparaît sur des informations telles que les affectations d’espace réservé, les dépenses et les rapports, au lieu du nom de la fonction interne.

   >[!NOTE]
   >
   >* Un seul alias peut exister pour chaque combinaison de fonction et d’attribut dans une carte tarifaire unique.
   >* Un alias doit être mis à jour sur la carte tarifaire et ne peut pas être modifié sur un projet.

1. Dans le champ [!UICONTROL **Taux de facturation**], saisissez le taux de facturation pour cette fonction et ses attributs.
1. (Facultatif) Sélectionnez [!UICONTROL **Verrouiller le taux**] pour verrouiller ce taux et ne pas autoriser sa modification au niveau du projet ou de la tâche. Vous pourrez le déverrouiller ultérieurement si nécessaire.
1. (Facultatif) Cliquez sur [!UICONTROL **Ajouter un taux de validité de date**] pour appliquer des dates de validité au taux de facturation.
1. (Facultatif) Cliquez de nouveau sur [!UICONTROL **Ajouter un taux effectif à la date**] pour ajouter d’autres taux de facturation avec des dates effectives pour cette fonction et ses attributs.
1. (Conditionnel) Si vous ajoutez plusieurs taux de facturation pour cette fonction, saisissez les informations suivantes :

   * [!UICONTROL **Taux de facturation**] : valeur du taux de facturation pour la période.
   * [!UICONTROL **Date de début**] : date à laquelle le taux commence.
   * [!UICONTROL **Date de fin**] : date de fin de validité du taux.

     Il n’est pas nécessaire que le premier taux de facturation ait une date de début et il n’est pas nécessaire que le dernier taux de facturation ait une date de fin. Des écarts sont autorisés entre les dates des taux, mais les dates qui se chevauchent ne sont pas autorisées. Pendant une lacune, d’autres zones de la hiérarchie des taux de facturation sont utilisées pour déterminer le taux de facturation, en fonction du type de revenu d’une tâche. Pour plus d&#39;informations, voir [Généralités sur la hiérarchie des revenus et des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

1. Cliquez sur [!UICONTROL **Enregistrer**].
1. (Facultatif) Pour ajouter un autre taux de facturation, pour la même fonction avec des attributs différents ou pour une fonction distincte, cliquez sur [!UICONTROL **Ajouter une fonction**].

   Les taux de chaque rôle sont ajoutés à la carte tarifaire au fur et à mesure de leur création. Le taux en vigueur actuel, basé sur les dates, est indiqué par une icône ![Icône Taux actuel](assets/current-rate-icon.png).

   ![Carte tarifaire avec les taux affichés](assets/rates-on-rate-card.png)

## Modifier les détails et les taux de la carte tarifaire

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte tarifaire**].
1. Pour modifier une carte tarifaire existante, cliquez sur son nom dans la liste Cartes tarifaires.
1. Pour mettre à jour les détails de la carte tarifaire, cliquez sur [!UICONTROL **Détails**] dans le panneau de gauche.
1. (Facultatif) Pour joindre un formulaire personnalisé à la carte tarifaire, cliquez sur le champ [!UICONTROL **Ajouter un formulaire personnalisé**] dans le coin supérieur droit de la page Détails, puis sélectionnez un formulaire personnalisé dans la liste qui s’affiche.

   Pour plus d’informations sur l’ajout d’un formulaire personnalisé, voir [Ajouter un formulaire personnalisé à un objet](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Cliquez sur [!UICONTROL **Enregistrer les modifications**] après avoir modifié les détails de la carte tarifaire.
1. Cliquez sur [!UICONTROL **Fonctions et taux**] dans le panneau de gauche pour modifier les taux de facturation.
1. Pour modifier un taux, activez la case à cocher en regard du taux et cliquez sur [!UICONTROL **Modifier**] dans la barre d’actions située en bas de l’écran.

   Pour plus d’informations sur la barre d’actions, voir [ Utiliser des listes améliorées ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   >[!NOTE]
   >
   >Comme chaque taux est associé à la combinaison du rôle et des attributs pour créer un taux unique, le rôle et les attributs ne peuvent pas être modifiés lorsque vous modifiez un taux.

1. Pour supprimer un taux de facturation de la carte tarifaire, cochez la case en regard du taux et cliquez sur [!UICONTROL **Supprimer**] dans la barre d’actions.
1. Pour verrouiller un taux, activez la case à cocher en regard du taux et cliquez sur [!UICONTROL **Verrouiller**] dans la barre d’actions.

   Les taux verrouillés ne peuvent pas être modifiés au niveau du projet ou de la tâche. Une icône de verrouillage s’affiche en regard des taux verrouillés dans la liste.

   Vous pouvez également déverrouiller un taux verrouillé à partir de la barre d’actions.

1. Pour ajuster les taux d’un pourcentage, procédez comme suit :

   1. Sélectionnez tous les taux que vous souhaitez ajuster dans la Carte tarifaire > Rôles de fonction et Taux .

      Vous pouvez choisir un ou plusieurs taux. Tous seront ajustés du même pourcentage.

   1. Cliquez sur [!UICONTROL **Ajuster les taux**] dans la barre d’actions.
   1. Dans la zone [!UICONTROL **Ajuster les taux de fonctions**], choisissez si vous souhaitez que l&#39;ajustement des taux se produise au cours de la période sélectionnée (les dates de validité existantes) ou d&#39;une période personnalisée que vous définissez.

      ![Zone Ajuster les taux de fonctions](assets/adjust-job-role-rates-dialog.png)

   1. Saisissez la valeur d&#39;ajustement pour les taux.

      Cette valeur est appliquée en tant que pourcentage. Par exemple, si vous saisissez 10, les taux sélectionnés augmenteront de 10 %.

   1. Cliquez sur [!UICONTROL **Mettre à jour les taux**].
   1. Cliquez sur [!UICONTROL **Mettre à jour**] dans le message de confirmation.

      Les taux sélectionnés sont augmentés du pourcentage.

## Importer une carte tarifaire

Consultez l’article [Importer des cartes tarifaires à partir d’un modèle](/help/quicksilver/administration-and-setup/manage-enterprise-operations/import-rate-cards.md).

## Copier une carte tarifaire

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte tarifaire**].
1. Cochez la case en regard de la carte tarifaire dans la liste et cliquez sur l’icône **Copier** ![Icône Copier](assets/copy-icon.png).
1. Saisissez le nom de la nouvelle carte tarifaire dans la zone [!UICONTROL **Copier la carte tarifaire**]. Cliquez ensuite sur [!UICONTROL **Créer**].

   La nouvelle carte tarifaire est enregistrée. Modifiez les détails de la carte tarifaire, les fonctions et les taux selon les besoins.

## Supprimer une carte tarifaire entière

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte tarifaire**].
1. Cochez la case en regard de la carte tarifaire dans la liste, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete.png).

   >[!NOTE]
   >
   >Une carte tarifaire associée à un projet sera supprimée du projet.

