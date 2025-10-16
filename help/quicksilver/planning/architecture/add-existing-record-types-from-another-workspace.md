---
title: Ajouter des types d’enregistrements existants à partir d’un autre Workspace
description: Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Dans Workfront Planning, vous pouvez ajouter un type d’enregistrement existant créé dans un autre espace de travail.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 9%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Ajouter des types d’enregistrements existants depuis un autre espace de travail

{{planning-important-intro}}

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

En tant que responsable d’espace de travail, vous pouvez ajouter un type d’enregistrement qui existe dans un autre espace de travail à un espace de travail que vous gérez dans Adobe Workfront Planning.

Un gestionnaire d’espace de travail doit d’abord désigner un type d’enregistrement en tant que type d’enregistrement global avant de pouvoir l’ajouter aux espaces de travail que vous gérez en tant que type d’enregistrement existant. Les responsables Workspace peuvent désigner un type d’enregistrement comme global lors de sa création ou de sa modification en définissant les paramètres de l’espace de travail du type d’enregistrement.

Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Cet article décrit comment ajouter un type d’enregistrement à partir d’un type existant.

Avant d’ajouter des enregistrements à un espace de travail à partir d’un type d’enregistrement global, consultez également l’article [Présentation des types d’enregistrements sur l’ensemble des espaces de travail](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<ul><li><p>Tout package Workfront et un package Planning Plus</p></li>
<p>Ou</p>
<li><p>Packages Prime et Ultimate de workflow et de planification</p></p></li></ul>
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

  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## Créer un type d’enregistrement en ajoutant un type existant à partir d’un autre espace de travail

>[!NOTE]
>
>Assurez-vous qu’au moins un type d’enregistrement est désigné comme global dans au moins un autre espace de travail.

1. Commencez à créer un type d’enregistrement, comme décrit dans l’article [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md), puis cliquez sur **Ajouter un existant**. <!--check this - the option might have been renamed in the UI-->

   ![Modal pour ajouter un type d’enregistrement avec la possibilité d’ajouter depuis un autre espace de travail](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Lorsqu’aucun type d’enregistrement n’est configuré pour être ajouté à d’autres espaces de travail de votre système, l’option **Ajouter existant** ne s’affiche pas.

1. Cliquez sur **Continuer**.
1. Dans la zone **Choisir le type d’enregistrement**, cliquez sur la carte correspondant au type d’enregistrement à ajouter à partir d’un espace de travail existant, puis cliquez sur **Ajouter**.

   Le type d’enregistrement est ajouté à l’espace de travail que vous avez sélectionné et l’icône **type d’enregistrement global** s’affiche ![](assets/global-icon.png) sur la carte du type d’enregistrement.

   Les événements suivants se produisent :

   * Les informations suivantes sont également ajoutées à partir du type d’enregistrement global existant :

      * Tous les champs d’origine
      * Toutes les connexions aux enregistrements
   * Vous pouvez afficher les enregistrements ajoutés à partir d&#39;autres espaces de travail qui utilisent le même type d&#39;enregistrement global, uniquement si vous disposez au moins des autorisations d&#39;affichage pour ces espaces de travail.
   * Le champ en lecture seule **Workspace** est ajouté à la nouvelle vue de tableau de type d&#39;enregistrement. Le champ affiche l’espace de travail dans lequel chaque enregistrement a été créé.

     >[!NOTE]
     >
     >Vous ne pouvez pas modifier l’aspect, les paramètres supplémentaires ou les champs d’origine du nouveau type d’enregistrement. Vous ne pouvez modifier le type d’enregistrement et tous ses champs et paramètres d’origine qu’à partir de l’espace de travail d’origine.

1. (Facultatif) Cliquez sur le type d’enregistrement nouvellement ajouté et déposez-le dans n’importe quelle section de l’espace de travail.
1. (Facultatif) Cliquez sur le menu **Plus** sur la carte du nouveau type d’enregistrement ou à droite du nom du type d’enregistrement sur sa page, puis cliquez sur **Supprimer**.

   Pour plus d’informations, consultez la section « Supprimer des types d’enregistrements globaux » de l’article [Supprimer des types d’enregistrements](/help/quicksilver/planning/architecture/delete-record-types.md).

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—vérifier auprès de Lilit si nous pouvons ajouter des automatisations ou des formulaires de demande aux RT globaux secondaires??—ajouter une étape avec des liens vers ces articles si / lorsque oui—>







