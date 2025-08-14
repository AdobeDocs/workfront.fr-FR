---
title: Ajouter des types d’enregistrements sur plusieurs espaces de travail
description: Les types d’enregistrements sont les types d’objets d’Adobe Workfront Planning. Dans Workfront Planning, vous pouvez importer un type d’enregistrement existant à partir d’un autre espace de travail.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 17%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Ajouter des types d’enregistrements entre les espaces de travail

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

En tant que responsable d&#39;espace de travail, vous pouvez importer ou ajouter un type d&#39;enregistrement existant dans un autre espace de travail.

Vous devez d&#39;abord désigner un type d&#39;enregistrement comme centralisé avant que les responsables d&#39;espace de travail puissent l&#39;importer dans d&#39;autres espaces de travail.

Vous pouvez désigner un type d’enregistrement comme centralisé lorsque vous le créez ou le modifiez, car vous définissez ses paramètres sur plusieurs espaces de travail.

Pour plus d’informations, voir [Configuration des fonctionnalités de plusieurs espaces de travail pour les types d’enregistrements](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer des autorisations relatives à un espace de travail</a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Présentation des types d’enregistrements centralisés

Remarques concernant l’ajout de types d’enregistrements existants depuis un autre espace de travail

* Lorsqu’aucun type d’enregistrement n’est configuré pour être ajouté à un autre espace de travail, l’option permettant de les importer depuis un autre espace de travail ne s’affiche pas lors de la création d’un type d’enregistrement. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* Après avoir ajouté le type d’enregistrement à partir d’un autre espace de travail, les informations suivantes sont également ajoutées à partir du type d’enregistrement existant :

   * Champs
   * Enregistrements
   * Connexions d’enregistrement

* Vous ne pouvez modifier le type d’enregistrement, y compris ses champs, que dans son espace de travail d’origine. Vous ne pouvez pas le modifier à partir des espaces de travail où il a été ajouté.

## Créer un type d’enregistrement à partir d’un type d’enregistrement existant

1. Commencez à créer un type d’enregistrement, comme décrit dans l’article [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md), puis cliquez sur **Ajouter un existant**. <!--check this - the option might have been renamed in the UI-->

   ![Boîte de dialogue modale pour ajouter un type d’enregistrement avec la possibilité d’importer depuis un autre espace de travail](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Cliquez sur **Continuer**.
1. Dans la zone **Choisir le type d’enregistrement**, cliquez sur la carte correspondant au type d’enregistrement à ajouter à partir d’un espace de travail existant, puis cliquez sur **Ajouter**.

   Le type d’enregistrement est ajouté à l’espace de travail que vous avez sélectionné et les événements suivants se produisent :

   * L’icône **type d’enregistrement entre espaces de travail** ![icône de connexion entre espaces de travail](assets/global-icon.png) est ajoutée à la carte du type d’enregistrement importé.
   * Le champ en lecture seule **Workspace** est ajouté au type d’enregistrement importé. Le champ affiche l’espace de travail dans lequel chaque enregistrement a été créé.

     >[!NOTE]
     >
     >* Vous ne pouvez pas modifier le type d&#39;enregistrement importé ou ses champs. Vous pouvez modifier le type d’enregistrement et ses champs à partir de l’espace de travail d’origine.

1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) dans la carte du type d’enregistrement importé, ou à droite du nom du type d’enregistrement sur sa page, puis cliquez sur **Supprimer**.
1. (Conditionnel) Saisissez **delete** dans le champ fourni, puis cliquez sur **Supprimer définitivement**.

   Le type d’enregistrement importé est alors supprimé de l’espace de travail sélectionné. Le type d’enregistrement d’origine et ses champs restent dans leur espace de travail d’origine.

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



