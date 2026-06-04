---
title: Dupliquer les enregistrements
description: Vous pouvez dupliquer un enregistrement existant dans la vue Tableau. Une copie identique de l’enregistrement existant est ajoutée à la page du type d’enregistrement.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/yk-q-wKrbIgyxw3WAz9un5HTNpwtdwFqaPFUQ6PzhT0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 547
ht-degree: 17%

---

# Dupliquer des enregistrements


<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Dans Adobe Workfront Planning, un enregistrement est une instance d’un type d’enregistrement.

Vous pouvez dupliquer un enregistrement existant dans la vue Tableau. Une copie identique de l’enregistrement existant est ajoutée à la page du type d’enregistrement.

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


## Dupliquer une <!--in a record type table (I don't think you can create them elsewhere right now)--> d’enregistrement

Vous pouvez créer des enregistrements dans la vue Tableau d&#39;une page de type d&#39;enregistrement en dupliquant une page existante. Un enregistrement identique à l&#39;enregistrement existant est créé et ajouté sous l&#39;enregistrement d&#39;origine.


{{step1-to-planning}}

1. Cliquez sur l’espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrements s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page de type d’enregistrement s’ouvre dans la vue à laquelle vous avez accédé pour la dernière fois. Par défaut, une page de type d’enregistrement s’ouvre en mode Tableau.
Tous les enregistrements du type sélectionné s&#39;affichent dans la vue.

1. (Conditionnel) Sélectionnez une vue de tableau.

1. Utilisez l’une des méthodes suivantes :

   * Pointez sur le nom d’un enregistrement, puis cliquez sur le menu **Plus** aligné avec le nom d’enregistrement, puis cliquez sur l’icône **Dupliquer** ![icône Dupliquer grise](assets/duplicate-icon-gray.png) .

     ![Menu Plus de l’enregistrement en mode Tableau](assets/more-menu-from-record-in-table-view.png)

   * Sélectionnez un enregistrement, puis cliquez sur l&#39;icône **Dupliquer** ![Icône Dupliquer en blanc et bleu](assets/duplicate-icon-white-and-blue.png) dans la barre d&#39;outils située en bas de la page.

     ![ Icône Dupliquer dans la barre d’outils en mode Tableau ](assets/duplicate-icon-in-toolbar-in-table-view.png)

   Un enregistrement identique avec un nom identique est créé sous l’enregistrement d’origine. Tous les champs du nouvel enregistrement sont remplis avec les mêmes informations que dans l&#39;enregistrement d&#39;origine.

1. (Facultatif) Commencez à mettre à jour les informations sur le nouvel enregistrement dans les champs disponibles en mode Tableau ou cliquez sur l’enregistrement et mettez à jour les informations dans la page ou l’aperçu de l’enregistrement.

   >[!NOTE]
   >
   >  * Il n’y a pas de champs obligatoires pour les enregistrements. Toutefois, nous vous recommandons d&#39;ajouter des informations pour le champ principal d&#39;un enregistrement, car il est utile d&#39;identifier les enregistrements lors de la liaison d&#39;enregistrements entre eux. Pour plus d’informations sur les champs principaux, consultez [Gérer la vue du tableau](/help/quicksilver/planning/views/manage-the-table-view.md) et la présentation des champs de Principal [](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Les champs qui renvoient à d’autres types d’enregistrements ou à des champs calculés sont en lecture seule.

   Pour plus d&#39;informations sur la modification des enregistrements, voir [Modifier les enregistrements](/help/quicksilver/planning/records/edit-records.md).

1. (Facultatif) Utilisez les raccourcis clavier suivants pour annuler ou rétablir l’ajout de nouveaux enregistrements ou de leurs informations lors de leur ajout en mode Tableau :

   * Ctrl + Z (⌘ + Z pour Mac) pour annuler une modification
   * Ctrl+Maj+Z (⌘+Maj+Z pour Mac) pour rétablir une modification.
