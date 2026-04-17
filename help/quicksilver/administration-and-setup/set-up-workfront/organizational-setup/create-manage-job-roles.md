---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Créer et gérer des fonctions
description: En tant qu’administrateur ou administratrice  [!DNL Adobe Workfront]  ou en tant que personne disposant d’un accès administratif aux fonctions, vous pouvez créer des fonctions qui peuvent être affectées à des personnes et supprimer les fonctions par défaut qui ne concernent pas votre organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: d8a01839b8f1332741f87be766f3ccb7d08cef96
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 28%

---

# Créer et gérer des fonctions

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Avec la version 25.11, la devise de remplacement pour les fonctions a été abandonnée dans la production. (L’obsolescence a eu lieu le 30 octobre dans l’environnement de prévisualisation.) Au lieu d’avoir une devise de base et de remplacer les devises, une devise est désormais disponible pour les fonctions, et les taux de coût et de facturation sont définis à l’aide de cette devise.

En tant qu’administrateur [!DNL Adobe Workfront] ou utilisateur standard disposant d’un accès en modification aux fonctions, vous pouvez créer des fonctions qui peuvent être affectées à des utilisateurs et supprimer les fonctions par défaut qui ne sont pas pertinentes pour votre organisation. Pour plus d’informations sur l’accès administratif dans [!DNL Workfront], voir [Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>Les fonctions font partie intégrante de la gestion des ressources. Pour utiliser les outils de planification des ressources, les fonctions doivent comporter un coût et un taux de facturation qui leurs sont associés. Pour plus d’informations, voir [Commencer avec la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Pour créer ou modifier une fonction : tout Workfront ou package de workflow</p>
   <p>Pour appliquer des attributs de taux et ajouter des formulaires personnalisés à la fonction : Workflow Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Modifier l’accès aux fonctions</td>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une fonction

Pour créer une fonction, procédez comme suit :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Fonctions]**.
1. Cliquez sur **[!UICONTROL Nouvelle fonction] > Créer une nouvelle fonction**.
1. Renseignez les champs suivants :

   * **Nom** : indiquez un nom pour la fonction. Il s’agit du nom qui s’affiche partout dans Workfront où s’affiche le champ Fonction .

     >[!TIP]
     >
     >Le nom d’une fonction peut contenir jusqu’à 255 caractères. Toutefois, les noms plus longs peuvent être tronqués dans certaines zones de Workfront.

   * **Description** : saisissez une description du rôle qui indique ce qui est unique à son sujet.
   * **Est actif** : sélectionnez **Oui** si vous souhaitez que le rôle soit actif et disponible partout dans Workfront pour être associé aux utilisateurs et utilisatrices, aux tâches, etc. Sélectionnez **Non** si vous souhaitez que le rôle soit désactivé et qu’il ne soit pas disponible pour être affecté aux utilisateurs, aux éléments de travail, etc.

     Pour plus d’informations sur la désactivation des fonctions, voir la section [Désactiver des fonctions](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

1. Cliquez sur **[!UICONTROL Créer une fonction]**. La fonction peut désormais être affectée à des tâches, des problèmes et des approbations. Vous pouvez aussi partager avec elle des modèles de mise en page ou d’autres objets. Pour plus d’informations sur tous les usages des fonctions dans [!DNL Workfront], voir [Vue d’ensemble des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Pour plus d’informations sur la suppression d’une fonction, voir [Supprimer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

## Ajouter des taux et des attributs à une fonction

Les taux de facturation et de coûts d’une fonction sont utilisés dans les calculs financiers.

Les attributs de taux sont pris en charge dans les zones de Workfront où il existe des taux, comme les fonctions et les utilisateurs. Lorsque des attributs sont appliqués à une fonction, leurs affectations sont automatiquement résolues aux taux corrects.

Pour plus d’informations, voir [Définir des attributs de taux](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Fonctions]**.
1. Cliquez sur le nom d’une fonction existante pour la modifier.
1. Pour mettre à jour les détails de la fonction, cliquez sur **Détails** dans le panneau de gauche.
1. (Facultatif) Pour joindre un formulaire personnalisé à la fonction, cliquez sur le champ **Ajouter un formulaire personnalisé** dans le coin supérieur droit de la page Détails, puis sélectionnez un formulaire personnalisé dans la liste qui s’affiche.

   Pour plus d’informations sur l’ajout d’un formulaire personnalisé, voir [Ajouter un formulaire personnalisé à un objet](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Cliquez sur [!UICONTROL **Taux**] dans le panneau de gauche.
1. Cliquez sur [!UICONTROL **Facturation**] ou [!UICONTROL **Coût**] pour sélectionner le type de taux.
1. Cliquez sur [!UICONTROL **Ajouter des taux**] pour ajouter un nouveau taux.

   Ou

   Sélectionnez un taux existant et cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) pour le mettre à jour.

   >[!NOTE]
   >
   >Comme chaque taux est associé à la combinaison du rôle et des attributs pour créer un taux unique, les attributs ne peuvent pas être modifiés lorsque vous modifiez un taux.

1. Dans la zone **Nouveau taux**, sélectionnez des attributs pour le taux, tels que Agence, Lieu ou Centre de coûts.

   >[!NOTE]
   >
   >Ces attributs sont définis séparément et peuvent affecter les calculs de produits et de coûts. Pour plus d’informations, voir [Définir des attributs de taux](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Sélectionnez la **Devise** pour le taux. L’administrateur Workfront ajoute la devise de base dans la zone Configuration . Vous pouvez remplacer la sélection par une autre devise disponible et modifier la devise sur les périodes effectives.

   >[!TIP]
   >
   >Seules les devises disponibles dans la zone Taux de change de votre système sont disponibles dans ce champ. Si une seule devise est configurée, seule cette devise est disponible.

   Pour plus d’informations sur la configuration de la devise de base dans Workfront, voir [Configurer des taux de change](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Pour plus d’informations sur la modification de la devise d’un projet, voir [Modifier la devise du projet](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. (Conditionnel) Pour un taux de facturation, saisissez le **Taux de facturation** pour cette fonction.

   Il s’agit du taux horaire de facturation de la fonction. Cette valeur calcule les revenus prévus et réels des tâches et des problèmes associés au rôle et, par conséquent, les revenus prévus et réels des projets. Entrez le taux en utilisant la devise sélectionnée.

   Si vous utilisez des attributs, les attributs et la fonction se combinent pour définir un taux unique. Par exemple, un rôle Designer à New York pour l’Agence A peut avoir un taux distinct d’un rôle Designer à Paris pour l’Agence B.

   Pour connaître les taux de facturation effectifs par date, cliquez sur **Ajouter un taux**. Saisissez la valeur de la facturation/heure pour la période, puis affectez une date de début et une date de fin, si nécessaire. Le premier taux de facturation ne comporte pas de date de début et le dernier taux de facturation ne comporte pas de date de fin.

   <!-- Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.-->

   Workfront vous permet de laisser des espaces entre les périodes, mais vous recevrez un avertissement pour confirmer que c’est intentionnel.

   Pour plus d’informations sur le calcul du chiffre d’affaires par Workfront, voir [Présentation de la facturation et du chiffre d’affaires](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Lors de la modification d’une fonction existante, vous pouvez trier la liste pour afficher la date de début la plus récente en haut de la liste des taux.

1. (Conditionnel) Pour un taux de coût, saisissez le **Taux de coût** pour cette fonction.

   Il s’agit du coût horaire de la fonction. Cette valeur calcule les coûts prévus et réels des tâches et des problèmes associés au rôle et, par conséquent, les coûts prévus et réels des projets. Entrez le taux en utilisant la devise sélectionnée.

   Si vous utilisez des attributs, les attributs et la fonction se combinent pour définir un taux unique. Par exemple, un rôle Designer à New York pour l’Agence A peut avoir un taux distinct d’un rôle Designer à Paris pour l’Agence B.

   Pour connaitre les taux de dépenses effectifs par date, cliquez sur **Ajouter un taux**. Saisissez la valeur du coût/heure pour la période, puis affectez une Date de début et une Date de fin, le cas échéant. Le premier taux de coût ne comporte pas de date de début et le dernier taux de coût ne comporte pas de date de fin.

   Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de coût n&#39;a pas de date de fin et que vous ajoutez un second taux de coût avec une date de début fixée au 1er mai, une date de fin fixée au 30 avril est ajoutée au premier taux de coût afin qu&#39;il n&#39;y ait aucun écart.

   Pour plus d’informations sur la façon dont Workfront calcule les coûts, voir [Suivre les coûts](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >Lors de la modification d’une fonction existante, vous pouvez trier la liste pour afficher la date de début la plus récente en haut de la liste des taux.

1. Cliquez sur [!UICONTROL **Enregistrer**].

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->


<!--

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

-->



