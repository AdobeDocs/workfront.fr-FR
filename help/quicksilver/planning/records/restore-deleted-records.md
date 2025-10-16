---
title: Restaurer les enregistrements supprimés
description: Vous pouvez récupérer les enregistrements supprimés de la zone Récemment supprimés dans Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 5%

---

# Restaurer les enregistrements supprimés

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->

{{planning-important-intro}}

Vous pouvez récupérer les enregistrements supprimés de la zone Récemment supprimés dans Adobe Workfront Planning.

Pour plus d&#39;informations sur la suppression d&#39;enregistrements, voir [Supprimer des enregistrements](/help/quicksilver/planning/records/delete-records.md).

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout Workfront et tout package Planning</p> <p>Tout workflow et tout package Planning</p>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations de niveau Contribution ou supérieur à un espace de travail et à un type d’enregistrement  </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr>   
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Considérations relatives à la récupération des enregistrements supprimés

* Vous pouvez restaurer les enregistrements que vous ou d&#39;autres utilisateurs avez supprimés.
* Les enregistrements sont stockés dans la classe Récemment supprimés pendant 30 jours. Au bout de 30 jours, les enregistrements sont définitivement supprimés de Workfront Planning.
* Si les enregistrements supprimés sont liés à d&#39;autres enregistrements, les enregistrements liés ne sont pas supprimés, mais les informations de l&#39;enregistrement supprimé sont également supprimées. La restauration des enregistrements supprimés restaurera les informations des enregistrements connectés.
* Vous pouvez restaurer des enregistrements en bloc.
* Lorsque les enregistrements sont supprimés, les informations suivantes sont stockées dans la classe Récemment supprimés :
   * **Nom** : il s’agit des informations figurant dans le champ de Principal de l’enregistrement. Pour plus d’informations sur les champs de Principal d’enregistrement, consultez la présentation des champs de Principal [](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Date de suppression** : l’heure et la date de suppression de l’enregistrement.
   * **Temps écoulé depuis la suppression récente** : temps écoulé depuis la suppression de l’enregistrement. Les enregistrements supprimés plus de 30 jours avant la date actuelle ne s&#39;affichent pas dans la classe Récemment supprimés.
   * **Supprimé par** : nom de l’utilisateur qui a supprimé l’enregistrement.

## Restaurer les enregistrements supprimés

1. Accédez à la page de type d’enregistrement dans laquelle vous avez supprimé des enregistrements.
1. Cliquez sur l’icône **Annuler** ![Icône Annuler](assets/undo-icon.png) dans le coin supérieur droit de n’importe quel type d’enregistrement affiché sur la page, puis cliquez sur **Récemment supprimé**.

   La zone **Récemment supprimé** s’affiche.

   ![Zone récemment supprimée](assets/recently-deleted-box.png)

1. Sélectionnez les enregistrements à supprimer, puis cliquez sur **Restaurer** > **Restaurer**. Vous pouvez sélectionner plusieurs enregistrements.

   Si la restauration a réussi, vous recevez une notification de succès en bas de l’écran.
1. Accédez à la vue Tableau et passez en revue les enregistrements restaurés.
