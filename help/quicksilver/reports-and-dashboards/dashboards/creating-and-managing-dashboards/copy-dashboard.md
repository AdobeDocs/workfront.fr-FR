---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copier un tableau de bord
description: Vous pouvez copier un tableau de bord et tout son contenu (rapports, calendriers et pages externes). Lorsque vous copiez le contenu d’un tableau de bord, vous pouvez choisir de le conserver tel qu’il apparaît dans le tableau de bord d’origine ou de créer de nouveaux éléments qui sont des copies de ceux du tableau de bord d’origine. Vous pouvez également choisir de ne pas transférer ni copier d’éléments dans le nouveau tableau de bord.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 100%

---

# Copier un tableau de bord

Vous pouvez copier un tableau de bord et tout son contenu (rapports, calendriers et pages externes). Lorsque vous copiez le contenu d’un tableau de bord, vous pouvez choisir de le conserver tel qu’il apparaît dans le tableau de bord d’origine ou de créer de nouveaux éléments qui sont des copies de ceux du tableau de bord d’origine. Vous pouvez également choisir de ne pas transférer ni copier d’éléments dans le nouveau tableau de bord.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Accès en affichage à un tableau de bord</p> <p>Vous obtiendrez l’accès en gestion au tableau de bord copié.</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Conditions préalables

Vous devez créer un tableau de bord avant de pouvoir le copier.

Pour plus d’informations sur la création de tableaux de bord, voir [Créer un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copier un tableau de bord

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png), puis cliquez sur **Tableaux de bord**.

1. Sélectionnez le tableau de bord à copier, puis cliquez sur **Copier** ![](assets/copy-icon.png).\
   Ou\
   Ouvrez le tableau de bord à copier, puis cliquez sur **Actions du tableau de bord** > **Copier**.\
   La boîte de dialogue Copie du tableau de bord s’affiche. Tous les éléments du tableau de bord d’origine s’affichent.

1. Dans le champ **Nom du tableau de bord**, indiquez un nouveau nom au tableau de bord.
1. Pour sélectionner tous les éléments du tableau de bord existant et les copier dans le tableau de bord copié, laissez **Sélectionner tout** sélectionné. Par défaut, les rapports, calendriers ou listes du tableau de bord existant seront copiés dans le nouveau tableau de bord.\
   Ou\
   Pour transférer uniquement des éléments spécifiques du tableau de bord d’origine vers le nouveau, désélectionnez les éléments que vous ne souhaitez pas afficher dans le nouveau tableau de bord puis, pour chaque élément sélectionné, choisissez l’une des options suivantes :

   * **Effectuer une copie :** l’élément est copié à partir du tableau de bord d’origine et une nouvelle version de cet élément s’affiche sur le nouveau tableau de bord. Les modifications apportées à l’élément dans le nouveau tableau de bord ne sont pas répercutées dans l’élément du tableau de bord d’origine. De même, les modifications apportées à l’élément dans le tableau de bord d’origine ne sont pas répercutées dans l’élément du nouveau tableau de bord.\
     Utilisez cette option lorsque vous souhaitez modifier le rapport d’origine sur le tableau de bord d’origine.\
     Par exemple, vous copiez un tableau de bord appelé « Équipe B » et le renommez en « Équipe A ». Sur le tableau de bord « Équipe B » se trouve un rapport intitulé « Rapport de l’équipe B ». Ce rapport contenant des données spécifiques à l’équipe B, vous sélectionnez l’option permettant d’en faire une copie afin de pouvoir le personnaliser pour l’équipe A et de le renommer ultérieurement « Rapport de l’équipe A ».\
     Avec cette option, vous supprimez les autorisations de partage du rapport d’origine du rapport copié. L’option Exécuter ce rapport avec les droits d’accès aux informations reste intacte sur le rapport copié.

   * **Utiliser l’original :** affiche l’élément d’origine dans le nouveau tableau de bord. Les modifications apportées à l’élément dans le nouveau tableau de bord sont également répercutées dans l’élément du tableau de bord d’origine. De même, les modifications apportées à l’élément sur le tableau de bord d’origine sont répercutées dans l’élément du nouveau tableau de bord.\
     Cette option permet de conserver les autorisations de partage du rapport d’origine. L’option Exécuter ce rapport avec les droits d’accès aux informations reste également intacte.

1. (Facultatif) Renommez les éléments que vous avez sélectionnés.
1. Cliquez sur **Copier le tableau de bord**.
1. (Facultatif) Si vous souhaitez modifier l’un des rapports, calendriers et pages externes copiés dans le tableau de bord copié, effectuez l’une des opérations suivantes :

   * Pour modifier les informations d’un des rapports copiés, cliquez sur le nom du rapport dans le tableau de bord, puis sur **Actions de rapport** > **Modifier**.

     Par exemple, vous pouvez modifier l’affichage, le filtre, le regroupement, l’invite ou le graphique ou un rapport copié.

   * Pour rétablir les autorisations sur les rapports copiés, cliquez sur le nom du rapport dans le nouveau tableau de bord, puis cliquez sur **Actions de rapport** > **Partage** et mettez à jour les autorisations du rapport.

     Lorsque vous copiez un rapport lors de la copie d’un tableau de bord, les autorisations de ce rapport sont supprimées.

   * Pour modifier l’option Exécuter le rapport avec les droits d’accès aux informations, cliquez sur le nom du rapport dans le nouveau tableau de bord, puis sur **Actions de rapport** > **Modifier** > **Options de rapport**.\
     Après la copie d’un rapport, les autorisations Exécuter ce rapport avec les droits d’accès ne sont conservées que dans les cas suivants :

     (Si aucune de ces conditions n’est vraie, les autorisations Exécuter ce rapport avec les droits d’accès sont supprimées et la nouvelle option Exécuter ce rapport avec les droits d’accès est modifiée pour la personne qui a créé le rapport copié.)

     Si la personne qui copie le tableau de bord et ses rapports dispose des droits d’accès Administration.

      * Si la personne qui copie le tableau de bord et ses rapports dispose des droits d’accès Administration.
      * Si la personne qui copie le tableau de bord et ses rapports est actuellement définie comme l’option Exécuter ce rapport avec les droits d’accès pour les rapports en cours de copie.
      * Si la personne qui copie le rapport dispose des autorisations de gestion sur le rapport.
