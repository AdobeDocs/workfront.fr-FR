---
title: Supprimer des types d’enregistrements
description: Vous pouvez supprimer des types d’enregistrement lorsqu’ils ne sont plus pertinents. La suppression des types d’enregistrement supprime également toutes les informations associées aux types d’enregistrement, telles que leurs enregistrements, champs et vues.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 66%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Supprimer des types d’enregistrements

{{planning-important-intro}}

Vous pouvez supprimer des types d’enregistrement lorsqu’ils ne sont plus pertinents.

Cependant, la suppression des types d’enregistrement supprime également toutes les informations associées aux types d’enregistrement. Pour plus d’informations, consultez la section [Remarques concernant la suppression de types d’enregistrement](#considerations-when-deleting-record-types) de cet article.

Pour plus d’informations sur les types d’enregistrement, voir [Présentation des types d’enregistrement](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite à l’étape d’accès anticipé pour la planification Workfront </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Nouvelle : standard</p>
   <p>Actuelle : formule</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gérer les autorisations d’un espace de travail</a> </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Votre administrateur ou administratrice Workfront ou de groupes doit ajouter la zone Planning dans votre modèle de disposition. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Vue d’ensemble des accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Remarques concernant la suppression de types d’enregistrement

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Vous ne pouvez supprimer que les types d’enregistrement des espaces de travail pour lesquels vous disposez d’autorisations de gestion.
* La suppression des types d’enregistrement supprime les informations suivantes qui leur sont associées :

   * Tous les enregistrements de ce type
   * Tous les champs associés au type d’enregistrement
   * Toutes les vues (y compris les filtres, les regroupements et les critères de tri) du type d’enregistrement
* Le type d’enregistrement est supprimé pour toutes les personnes accédant à l’espace de travail.
* La suppression des types d’enregistrements et leurs informations associées est irréversible.
* Il est recommandé de recréer les champs et les enregistrements associés au type d’enregistrement que vous souhaitez supprimer sur un autre type d’enregistrement avant de les supprimer.

## Supprimer des types d’enregistrements

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les types d’enregistrements,

   Ou

   Dans un espace de travail, développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   L’espace de travail et les types d’enregistrement s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Passez la souris sur la carte de type enregistrement, cliquez sur le menu Plus, puis **Supprimer**.
   * Cliquez sur la carte du type d’enregistrement que vous souhaitez supprimer, puis, dans la page du type d’enregistrement, cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du nom du type d’enregistrement, puis cliquez sur **Supprimer**.

   ![](assets/permanently-delete-record-type-confirmation.png)

1. Saisissez **delete** dans la boîte de confirmation, puis cliquez sur **Supprimer définitivement**. Ceci n’est pas sensible à la casse.

   Le type d’enregistrement sélectionné, ainsi que leurs champs, enregistrements associés et vues, sont supprimés.
