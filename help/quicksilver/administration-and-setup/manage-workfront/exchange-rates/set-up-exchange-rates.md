---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Configurer les taux de change
description: Les taux de change ont un impact sur tous les éléments financiers de Workfront. La devise de base est la devise par défaut pour tous les projets du système.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: b16523bf6c37747702efe3b5ecfcc33801526af1
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 41%

---

# Configurer les taux de change

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

{{highlighted-preview}}

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer des taux de change de devise dans Workfront. Cela inclut les éléments suivants :

* Définir la devise par défaut pour le système Workfront
* Mettre à jour les taux de change dans Workfront pour les faire correspondre aux taux de change actuels
* Configurer les taux de change pour plusieurs devises (pour ainsi permettre aux utilisateurs et utilisatrices de choisir une devise par défaut pour des projets individuels)

Les taux de change ont un impact sur tous les éléments financiers de Workfront. La devise de base est la devise par défaut pour tous les projets et rapports du système, sauf si elle est remplacée pour un projet ou une fonction spécifique. La devise de base ou par défaut actuelle est indiquée par une icône ![Icône de devise par défaut](assets/default-icon.png) dans la liste. Vous pouvez également choisir d’afficher les informations financières dans des devises disponibles dans votre système qui sont différentes de la devise de base ou de celle du projet, lors de leur affichage dans un rapport ou une liste. Pour plus d’informations, voir [Créer des rapports de données financières avec des taux de change uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Pour plus d’informations sur le remplacement de la devise de base dans Workfront pour les projets et les fonctions, consultez les articles suivants :

* [Modifier la devise du projet](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

La manière dont vous configurez les taux de change détermine si les utilisateurs et utilisatrices peuvent modifier les taux de change d’un projet donné.

>[!IMPORTANT]
>
>Les taux de change dans Workfront ne sont pas dynamiques ; la valeur que vous définissez doit être mise à jour en cas de modification des taux de change.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Pour configurer des taux de change : tout Workfront ou package de workflow</p>
       <p>Pour appliquer des dates de validité à des taux de change : package Workflow Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Administrateur ou administratrice système</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer les taux de change

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Taux de change**.
1. Cliquez sur **Ajouter une devise**.
1. Dans la zone **Ajouter une devise**, commencez à saisir le nom de la devise, puis cliquez dessus lorsqu’elle apparaît dans la liste déroulante.
1. Dans le champ **Taux de change**, saisissez le taux de la devise que vous avez sélectionnée, par rapport à la devise définie comme devise de base dans le système.
1. Cliquez sur **Ajouter** pour ajouter la nouvelle devise et son taux de change.
1. (Facultatif) Pour modifier la devise de base (par défaut), effectuez l’une des opérations suivantes :

   * Cochez la case en regard du nom de devise et sélectionnez **Rendre par défaut** dans la barre d’actions située en bas de l’écran.
   * Pointez sur le nom de la devise et cliquez sur le menu **Plus** qui s’affiche. Sélectionnez ensuite **Rendre par défaut**.

     La nouvelle devise par défaut est mise à jour avec l’icône ![Icône de devise par défaut](assets/default-icon.png).

     >[!NOTE]
     >
     >La devise par défaut apparaît toujours en premier dans la liste, quelle que soit la manière dont la liste est triée.

1. (Facultatif) Pour supprimer une devise, cochez la case en regard du nom de la devise et sélectionnez **Supprimer** dans la barre d’actions située en bas de l’écran. Impossible de supprimer la devise par défaut.

<div class="preview">

## Définir des dates effectives sur les taux de change d&#39;une devise

Les dates de validité des taux de change d&#39;une devise sont configurées de sorte qu&#39;une valeur de taux se termine à une date spécifique et qu&#39;un autre taux commence. Le taux de change de la date correcte est ensuite utilisé dans les calculs financiers.

{{step-1-to-setup}}

1. Cliquez sur **Préférences du projet** > **Taux de change**.
1. Sélectionnez une devise dans la liste, puis cliquez sur **Gérer les dates** dans la barre d’actions.
1. Dans la boîte de dialogue **(nom de devise) date taux de change effectifs** choisissez une **Date de fin** pour le taux de change actuel.

   Ou

   Choisissez une **Date de début** pour le nouveau taux de change.

   Le premier taux de change n&#39;aura pas de date de début et le dernier taux n&#39;aura pas de date de fin. Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux n’a pas de date de fin et que vous ajoutez un taux de change avec une date de début fixée au 1er décembre 2025, une date de fin fixée au 30 novembre 2025 est ajoutée au premier taux afin qu’il n’y ait aucun écart.

   ![Boîte de dialogue Taux de change effectifs](assets/euro-date-effective-rates.png)

1. Saisissez la nouvelle valeur **Taux de change**.
1. (Facultatif) Cliquez sur **Ajouter une date de validité du taux** pour ajouter d&#39;autres taux de change avec des dates de validité pour cette devise.
1. Cliquez sur **Enregistrer**.

</div>

## Permettre aux utilisateurs et utilisatrices de modifier la devise par défaut d’un projet

Les utilisateurs et utilisatrices peuvent modifier la devise par défaut d’un projet lorsque les conditions suivantes sont remplies :

* L&#39;utilisateur dispose d&#39;une licence Standard ou Plan avec un accès administratif aux taux de change.

  Pour plus d’informations, voir [Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Plusieurs devises sont activées sur le système Workfront.

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent modifier la devise par défaut sur un projet donné, voir [Modifier la devise du projet](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permettre aux utilisateurs et utilisatrices de modifier la devise par défaut d’une fonction

Les utilisateurs et utilisatrices peuvent modifier la devise d’une fonction lorsque les conditions suivantes sont remplies :

* L’utilisateur dispose d’une licence Standard ou Plan avec un accès administratif aux fonctions.

  Pour plus d’informations, voir [Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Plusieurs devises sont activées dans le système Workfront.

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent modifier la devise par défaut pour une fonction donnée, voir [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).



