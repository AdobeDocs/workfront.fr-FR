---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Configurer les taux de change
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer des taux d’exchange de devise dans Workfront.
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: b0cf0a5ec6b932267c8714b966638d8da93331b8
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 22%

---

# Configurer les taux de change

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

En tant qu’administrateur Adobe Workfront, vous pouvez configurer des taux d’exchange de devise dans Workfront. Cela inclut les éléments suivants :

* Définition de la devise par défaut pour le système Workfront
* Mise à jour des taux d’exchange dans Workfront pour qu’ils correspondent aux taux d’exchange actuels
* Configuration des taux d’exchange pour plusieurs devises (ce qui permet aux utilisateurs de choisir une devise par défaut pour des projets individuels)

Les taux d’Exchange ont un impact sur tous les éléments financiers de Workfront. La devise de base est la devise par défaut de tous les projets du système, sauf si elle est remplacée pour un rôle de projet ou de tâche donné. Vous pouvez également choisir d’afficher les informations financières dans des devises disponibles dans votre système qui sont différentes de la devise de base ou de celle du projet lors de leur affichage dans un rapport ou une liste. Pour plus d’informations, voir [Création de rapports de données financières avec des taux d’exchange uniques](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Pour plus d’informations sur le remplacement de la devise de base dans Workfront pour les projets et les rôles de tâche, consultez les articles suivants :

* [Modification de la devise du projet](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

La manière dont vous configurez les taux d’exchange affecte la possibilité pour les utilisateurs de modifier les taux d’exchange d’un projet donné.

>[!IMPORTANT]
>
>Les taux d’Exchange dans Workfront ne sont pas dynamiques ; la valeur que vous définissez doit être mise à jour en cas de modification des taux d’exchange.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurer les taux de change

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Préférences du projet** > **Taux d’Exchange.**

1. Cliquez sur **Ajouter une devise.**
1. Commencez à saisir le nom de la devise, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.

1. Dans le champ fourni, indiquez le taux de la devise que vous avez sélectionnée, en fonction de la devise définie comme devise de base dans le système.
1. (Facultatif) Définissez la devise comme devise de base (par défaut) pour Workfront.

   Il s’agit de la devise utilisée par défaut pour tous les projets et rapports du système.

1. Cliquez sur **Enregistrer** pour enregistrer vos modifications.

## Permet aux utilisateurs de modifier la devise par défaut d’un projet.

Les utilisateurs peuvent modifier la devise par défaut d’un projet lorsque les conditions suivantes sont remplies :

* L’utilisateur dispose d’une licence Plan avec l’accès administratif aux taux d’Exchange.

  Pour plus d’informations, voir [Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Plusieurs devises sont activées sur le système Workfront.

Pour plus d’informations sur la manière dont les utilisateurs peuvent modifier la devise par défaut sur un projet donné, voir [Modification de la devise du projet](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permet aux utilisateurs de modifier la devise par défaut d’un rôle de tâche

Les utilisateurs peuvent modifier la devise d’un rôle de tâche lorsque les conditions suivantes sont remplies :

* L’utilisateur dispose d’une licence Plan avec un accès administratif aux rôles de tâche.

  Pour plus d’informations, voir [Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Plusieurs devises sont activées dans le système Workfront.

Pour plus d’informations sur la manière dont les utilisateurs peuvent modifier la devise par défaut pour un rôle de tâche donné, voir [Création et gestion des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
