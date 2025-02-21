---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Supprimer une page externe d’un tableau de bord
description: Vous pouvez supprimer une page externe d’un tableau de bord si vous n’en avez plus besoin.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 83%

---

# Supprimer une page externe d’un tableau de bord

<!-- Audited: 1/2025 -->

Vous pouvez supprimer une page externe d’un tableau de bord si vous n’en avez plus besoin.

Cependant, vous ne pouvez pas supprimer une page externe une fois qu’elle a été créée dans Adobe Workfront. Vous ne pouvez supprimer une page externe qu’à l’aide de l’API. Pour plus d’informations sur l’API Workfront, voir [Principes de base de l’API](../../../wf-api/general/api-basics.md). Pour plus d’informations sur la création de pages externes, voir [Intégrer une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Formule Adobe Workfront</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront</strong></td> 
   <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès</strong></td> 
   <td> <p>Accès en modification aux rapports, tableaux de bord et calendriers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Autorisations en gestion pour le tableau de bord</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Supprimer une page externe d’un tableau de bord

1. Accédez au tableau de bord contenant la page externe à supprimer.

1. Cliquez sur **Actions du tableau de bord**, puis cliquez sur **Modifier**.

   ![Modifier le tableau de bord](assets/unshimmed-edit-dashboard.png)

1. Sur le côté droit de l’écran, recherchez la page externe à supprimer, puis cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/delete.png).

   ![Icône Supprimer la page externe dans le tableau de bord](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Cliquez sur **Enregistrer et fermer** dans le coin inférieur gauche.

   Cette opération supprime la page externe du tableau de bord sélectionné. La page externe reste dans Workfront et est accessible à partir d’un rapport. Pour plus d’informations, voir la section « Afficher des pages externes dans un rapport » de l’article [Intégrer une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
