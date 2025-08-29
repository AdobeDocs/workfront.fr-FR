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
source-git-commit: dc820b4012fec494ce5ebb1baefb4ee0df214916
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 56%

---

# Configurer les taux de change

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer des taux de change de devise dans Workfront. Cela inclut les éléments suivants :

* Définir la devise par défaut pour le système Workfront
* Mettre à jour les taux de change dans Workfront pour les faire correspondre aux taux de change actuels
* Configurer les taux de change pour plusieurs devises (pour ainsi permettre aux utilisateurs et utilisatrices de choisir une devise par défaut pour des projets individuels)

Les taux de change ont un impact sur tous les éléments financiers de Workfront. La devise de base est la devise par défaut pour tous les projets du système, sauf si elle est remplacée pour un projet ou une fonction spécifique. La devise de base ou par défaut actuelle est indiquée par une icône ![Icône de devise par défaut](assets/default-icon.png) dans la liste. Vous pouvez également choisir d’afficher les informations financières dans des devises disponibles dans votre système qui sont différentes de la devise de base ou de celle du projet, lors de leur affichage dans un rapport ou une liste. Pour plus d’informations, voir [Créer des rapports de données financières avec des taux de change uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Pour plus d’informations sur le remplacement de la devise de base dans Workfront pour les projets et les fonctions, consultez les articles suivants :

* [Modifier la devise du projet](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

La manière dont vous configurez les taux de change détermine si les utilisateurs et utilisatrices peuvent modifier les taux de change d’un projet donné.

>[!IMPORTANT]
>
>Les taux de change dans Workfront ne sont pas dynamiques ; la valeur que vous définissez doit être mise à jour en cas de modification des taux de change.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

     La nouvelle devise par défaut est mise à jour avec l’icône .

     >[!NOTE]
     >
     >La devise par défaut apparaît toujours en premier dans la liste, quelle que soit la manière dont la liste est triée.

1. (Facultatif) Pour supprimer une devise, cochez la case en regard du nom de la devise et sélectionnez **Supprimer** dans la barre d’actions située en bas de l’écran. Impossible de supprimer la devise par défaut.

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


<!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->
