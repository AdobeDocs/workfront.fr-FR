---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Configuration des taux d’Exchange
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer des taux de change de devise dans Workfront.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 99%

---

# Configurer les taux de change

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer des taux de change de devise dans Workfront. Cela inclut les éléments suivants :

* Définir la devise par défaut pour le système Workfront
* Mettre à jour les taux de change dans Workfront pour les faire correspondre aux taux de change actuels
* Configurer les taux de change pour plusieurs devises (pour ainsi permettre aux utilisateurs et utilisatrices de choisir une devise par défaut pour des projets individuels)

Les taux de change ont un impact sur tous les éléments financiers de Workfront. La devise de base est la devise par défaut de tous les projets du système, sauf si elle est remplacée pour un projet donné ou une fonction donnée. Vous pouvez également choisir d’afficher les informations financières dans des devises disponibles dans votre système qui sont différentes de la devise de base ou de celle du projet, lors de leur affichage dans un rapport ou une liste. Pour plus d’informations, voir [Créer des rapports de données financières avec des taux de change uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Pour plus d’informations sur le remplacement de la devise de base dans Workfront pour les projets et les fonctions, consultez les articles suivants :

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

1. Cliquez sur **Préférences du projet** > **Taux de change.**

1. Cliquez sur **Ajouter une devise.**
1. Commencez à saisir le nom de la devise, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.

1. Dans le champ fourni, indiquez le taux de la devise que vous avez sélectionnée, en fonction de la devise définie comme devise de base dans le système.
1. (Facultatif) Définissez la devise comme devise de base (par défaut) pour Workfront.

   Il s’agit de la devise utilisée par défaut pour tous les projets et rapports du système.

1. Cliquez sur **Enregistrer** pour enregistrer les modifications.

## Permettre aux utilisateurs et utilisatrices de modifier la devise par défaut d’un projet

Les utilisateurs et utilisatrices peuvent modifier la devise par défaut d’un projet lorsque les conditions suivantes sont remplies :

* L’utilisateur ou l’utilisatrice dispose d’une licence de plan avec un accès administratif aux taux de change.

  Pour plus d’informations, voir [Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Plusieurs devises sont activées sur le système Workfront.

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent modifier la devise par défaut sur un projet donné, voir [Modifier la devise du projet](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permettre aux utilisateurs et utilisatrices de modifier la devise par défaut d’une fonction

Les utilisateurs et utilisatrices peuvent modifier la devise d’une fonction lorsque les conditions suivantes sont remplies :

* L’utilisateur ou l’utilisatrice dispose d’une licence de plan avec un accès administratif aux fonctions.

  Pour plus d’informations, voir [Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Plusieurs devises sont activées dans le système Workfront.

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent modifier la devise par défaut pour une fonction donnée, voir [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
