---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Supprimer une page externe d’un tableau de bord
description: Vous pouvez supprimer une page externe d’un tableau de bord si elle n’est plus nécessaire.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 37%

---

# Supprimer une page externe d’un tableau de bord

Vous pouvez supprimer une page externe d’un tableau de bord si elle n’est plus nécessaire.

Cependant, vous ne pouvez pas supprimer une page externe une fois qu’elle a été créée dans Adobe Workfront. Vous ne pouvez supprimer une page externe qu’à l’aide de l’API. Pour plus d’informations sur l’API Workfront, reportez-vous à la section [Principes de base de l’API](../../../wf-api/general/api-basics.md). Pour plus d’informations sur la création de pages externes, voir [Incorporation d’une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Forfait Adobe Workfront*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations en gestion pour le tableau de bord</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Suppression d’une page externe d’un tableau de bord

1. Cliquez sur l&#39;icône **Menu principal** ![](assets/main-menu-icon.png), puis sur **Tableaux de bord**.
1. Sélectionnez le tableau de bord à partir duquel vous souhaitez supprimer la page externe, puis cliquez sur **Modifier** ![](assets/edit-icon.png).

   ![Sélectionnez l’icône Modifier.](assets/nwe-editdashboard2021-350x188.png)

1. Sur le côté droit de l’écran, recherchez la page externe à supprimer, puis cliquez sur l’icône **Supprimer** ![](assets/delete.png) .

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Cliquez sur **Enregistrer + Fermer** dans le coin inférieur gauche.

   Cette opération supprime la page externe du tableau de bord sélectionné. La page externe reste dans Workfront et est accessible à partir d’un rapport. Pour plus d’informations, reportez-vous à la section &quot;Affichage des pages externes dans un rapport&quot; de l’article [ Intégration d’une page web externe dans un tableau de bord ](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
