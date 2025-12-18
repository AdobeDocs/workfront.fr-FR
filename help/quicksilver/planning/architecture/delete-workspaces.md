---
title: Supprimer les espaces de travail
description: Vous pouvez supprimer des espaces de travail lorsqu’ils ne sont plus pertinents.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 37%

---


# Supprimer des espaces de travail

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Dans Adobe Workfront Planning, les espaces de travail sont des emplacements centralisés permettant aux équipes de planifier le travail.
 Pour plus d’informations, voir [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).

Vous pouvez supprimer les espaces de travail qui ne sont plus pertinents.

Avant de supprimer un espace de travail, nous vous recommandons de créer à nouveau certains ou tous les types d’enregistrements, enregistrements, champs et vues associés à l’espace de travail dans un autre espace de travail.

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
<ul> 
<li><p>Tout Workfront et tout package Planning</p></li>
Ou
<li><p>Tout workflow et tout package Planning</p></li></ul>
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations d’un espace de travail</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Remarques relatives à la suppression des espaces de travail

* Lorsque vous supprimez des espaces de travail, tous les types d’enregistrements, enregistrements, champs associés et vues sont également supprimés.
* Les espaces de travail supprimés et les informations qu’ils contiennent ne peuvent pas être récupérés.

## Supprimer un espace de travail

{{step1-to-planning}}

1. (Conditionnel) Si vous êtes un administrateur Workfront, cliquez sur l’une des options suivantes :

   * **Espaces de travail sur lesquels je travaille** pour accéder aux espaces de travail que vous avez créés
   * **Autres espaces de travail** pour accéder aux espaces de travail que d’autres ont partagés avec vous
Ou
     <span class="preview">**Tous les espaces de travail** pour accéder aux espaces de travail partagés avec vous ou que vous avez créés</span>

1. (Facultatif) Cliquez sur **Tout afficher** pour afficher des espaces de travail supplémentaires. Le lien **Tout afficher** s’affiche uniquement lorsque vous disposez de plus de deux lignes de cartes d’espace de travail.
1. (Facultatif) Cliquez sur K **Afficher moins** pour limiter le nombre d’espaces de travail affichés à l’écran.
1. Pour supprimer un espace de travail, effectuez l’une des opérations suivantes :

   * Pointez sur la carte de l’espace de travail, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans le coin supérieur droit de la carte
Ou
   * <span class="preview"> Cliquez sur l’icône **rechercher** ![Icône Rechercher](assets/search-icon.png) dans le coin supérieur droit de la page Espaces de travail pour rechercher un espace de travail par nom</span> puis cliquez sur une vignette d’espace de travail pour ouvrir l’espace de travail, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’espace de travail.
1. Cliquez sur **Supprimer**.

   ![Confirmation de suppression définitive de l’espace de travail](assets/permanently-delete-workspace-confirmation.png)

1. Saisissez « **delete** » dans l’espace prévu à cet effet, puis cliquez sur **Supprimer définitivement**. Cette opération n’est pas sensible à la casse.

   L’espace de travail est supprimé de manière irréversible. Les types d’enregistrement, enregistrements, champs et vues qui leur sont associés sont également supprimés. <!--ensure this is right at or before GA-->


