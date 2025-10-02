---
title: Ajouter des types d’enregistrements existants à partir d’un autre Workspace
description: Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Dans Workfront Planning, vous pouvez ajouter un type d’enregistrement existant créé dans un autre espace de travail.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 8%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Ajouter des types d’enregistrements existants depuis un autre espace de travail

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

En tant que responsable d’espace de travail, vous pouvez ajouter un type d’enregistrement qui existe dans un autre espace de travail à un espace de travail que vous gérez dans Adobe Workfront Planning.

Cet article décrit comment ajouter un type d’enregistrement à partir d’un enregistrement existant et comment le supprimer, s’il n’est plus nécessaire.

Un gestionnaire d’espace de travail doit d’abord désigner un type d’enregistrement comme centralisé avant de pouvoir l’ajouter aux espaces de travail que vous gérez en tant que type d’enregistrement existant.

Vous pouvez désigner un type d&#39;enregistrement comme centralisé lorsque vous le créez ou le modifiez, au fur et à mesure que vous définissez ses paramètres avancés.

Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Avant d’ajouter des enregistrements à un espace de travail à partir d’un type d’enregistrement centralisé, consultez l’article [Présentation des types d’enregistrements sur l’ensemble des espaces de travail](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<ul><li><p>Tout package Workfront</p></li>
<p>Et</p>
<li><p>Tout package Planning permettant de créer des types d'enregistrements connectables</p></li>
<li><p>Package Planning Plus pour créer des types d'enregistrements centralisés</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre gestionnaire de compte Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Créer un type d’enregistrement à partir d’un type d’enregistrement existant

1. Commencez à créer un type d’enregistrement, comme décrit dans l’article [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md), puis cliquez sur **Ajouter un existant**. <!--check this - the option might have been renamed in the UI-->

   ![Modal pour ajouter un type d’enregistrement avec la possibilité d’ajouter depuis un autre espace de travail](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Cliquez sur **Continuer**.
1. Dans la zone **Choisir le type d’enregistrement**, cliquez sur la carte correspondant au type d’enregistrement à ajouter à partir d’un espace de travail existant, puis cliquez sur **Ajouter**.

   Le type d’enregistrement est ajouté à l’espace de travail que vous avez sélectionné.

   >[!TIP]
   >
   >Si aucun type d’enregistrement n’est configuré pour être ajouté à un autre espace de travail, l’option permettant de les ajouter à partir d’un autre espace de travail ne s’affiche pas.

   Les événements suivants se produisent :

   * Les informations suivantes sont également ajoutées à partir du type d’enregistrement centralisé existant :

      * Tous les champs d’origine
      * Toutes les connexions aux enregistrements
   * Vous pouvez afficher les enregistrements ajoutés à partir d&#39;autres espaces de travail qui utilisent le même type d&#39;enregistrement centralisé, uniquement si vous disposez au moins des autorisations d&#39;affichage pour ces espaces de travail.
   * L’icône **type d’enregistrement centralisé** ![icône de type d’enregistrement centralisé](assets/global-icon.png) est ajoutée à la carte du nouveau type d’enregistrement.
   * Le champ en lecture seule **Workspace** est ajouté à la nouvelle vue de tableau de type d&#39;enregistrement. Le champ affiche l’espace de travail dans lequel chaque enregistrement a été créé.

     >[!NOTE]
     >
     >Vous ne pouvez pas modifier l’aspect, les paramètres avancés ou les champs d’origine du nouveau type d’enregistrement. Vous ne pouvez modifier le type d’enregistrement et tous ses champs et paramètres d’origine qu’à partir de l’espace de travail d’origine.

1. (Facultatif) Cliquez sur le type d’enregistrement nouvellement ajouté et déposez-le dans n’importe quelle section de l’espace de travail.

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

## Supprimer un type d’enregistrement centralisé d’un espace de travail secondaire

Vous pouvez supprimer un type d’enregistrement que vous avez ajouté à partir d’un autre espace de travail si nécessaire. Si vous le supprimez, il sera uniquement supprimé de l’espace de travail secondaire et les enregistrements ajoutés à partir de cet espace de travail. Le type d’enregistrement d’origine reste dans son espace de travail d’origine et dans les autres espaces de travail où il a été ajouté.

Pour supprimer un type d’enregistrement centralisé d’un espace de travail secondaire :

1. Accédez au type d’enregistrement centralisé dans l’espace de travail secondaire.

1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) sur la carte du type d’enregistrement ou à droite du nom du type d’enregistrement sur sa page, puis cliquez sur **Supprimer**.
1. (Conditionnel) Saisissez **delete** dans le champ fourni, puis cliquez sur **Supprimer définitivement**.

   Les événements suivants se produisent :

   * Le type d’enregistrement créé à partir d’un type d’enregistrement centralisé est supprimé de l’espace de travail sélectionné.
   * Le type d’enregistrement d’origine et ses champs restent dans leur espace de travail d’origine.
   * Le type d’enregistrement reste dans tous les autres espaces de travail où il a été ajouté.
   * Les enregistrements ajoutés au type d’enregistrement de l’espace de travail actuel sont supprimés. Tous les autres enregistrements ajoutés à partir d’espaces de travail supplémentaires où le type d’enregistrement centralisé a été ajouté sont conservés.





