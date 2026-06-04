---
title: Restaurer les enregistrements supprimés
description: Vous pouvez récupérer les enregistrements supprimés de la zone Récemment supprimés dans Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6F-GarlW1gY0gHEZIC-CgSiN75EMd2RcZZUGgyOgqxU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 455
ht-degree: 15%

---

# Restaurer des enregistrements supprimés


<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
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
   <td>   <p>Accorder des autorisations supérieures ou égales à un espace de travail, un type d’enregistrement et <span class="preview">gérer les autorisations d’un enregistrement</span> </p>    
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr>   
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:
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
</table>
-->

## Considérations relatives à la récupération des enregistrements supprimés

* Vous pouvez restaurer les enregistrements que vous ou d&#39;autres utilisateurs avez supprimés.
* Les enregistrements sont stockés dans la classe Récemment supprimés pendant 30 jours. Au bout de 30 jours, les enregistrements sont définitivement supprimés de Workfront Planning.
* Lorsque des enregistrements supprimés sont liés à d’autres enregistrements, ces enregistrements liés restent intacts, bien que les informations de l’enregistrement supprimé soient éliminées. La restauration des enregistrements supprimés restaurera les informations des enregistrements connectés.
* Vous pouvez restaurer des enregistrements en bloc.
* Lorsque les enregistrements sont supprimés, les informations suivantes sont stockées dans la classe Récemment supprimés :
   * **Nom** : il s’agit des informations figurant dans le champ de Principal de l’enregistrement. Pour plus d’informations sur les champs de Principal d’enregistrement, consultez la présentation des champs de Principal [](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Date de suppression** : l’heure et la date de suppression de l’enregistrement.
   * **Temps écoulé depuis la suppression récente** : temps écoulé depuis la suppression de l’enregistrement. Les enregistrements supprimés plus de 30 jours avant la date actuelle ne s&#39;affichent pas dans la classe Récemment supprimés.
   * **Supprimé par** : nom de l’utilisateur qui a supprimé l’enregistrement.

## Restaurer des enregistrements supprimés

1. Accédez à la page de type d’enregistrement dans laquelle vous avez supprimé des enregistrements.
1. Cliquez sur l’icône **Annuler** ![Icône Annuler](assets/undo-icon.png) dans le coin supérieur droit de n’importe quel type d’enregistrement affiché sur la page, puis cliquez sur **Récemment supprimé**.

   La zone **Récemment supprimé** s’affiche.

   ![Zone récemment supprimée](assets/recently-deleted-box.png)

1. Sélectionnez les enregistrements à supprimer, puis cliquez sur **Restaurer** > **Restaurer**. Vous pouvez sélectionner plusieurs enregistrements.

   Si la restauration a réussi, vous recevez une notification de succès en bas de l’écran.
1. Accédez à la vue Tableau et passez en revue les enregistrements restaurés.
