---
title: Création de hiérarchies Workspace
description: En tant que gestionnaire d'espace de travail, vous pouvez créer plusieurs hiérarchies d'espaces de travail entre les types d'enregistrements dans Adobe Workfront Planning. Après avoir connecté des types d’enregistrements dans un espace de travail et créé une hiérarchie, les types d’enregistrements sont connectés les uns aux autres, un type d’enregistrement étant désigné comme parent et jusqu’à 6 autres types d’enregistrements étant configurés comme enfants.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 5%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Créer des hiérarchies d’espace de travail

En tant que gestionnaire d&#39;espace de travail, vous pouvez créer plusieurs hiérarchies d&#39;espaces de travail entre les types d&#39;enregistrements dans Adobe Workfront Planning.


Une fois les types d’enregistrements connectés dans un espace de travail, vous pouvez créer une hiérarchie qui organise ces connexions. Les hiérarchies organisent les types d&#39;enregistrements en relations parent-enfant et peuvent contenir jusqu&#39;à quatre niveaux de types d&#39;objets.

S’il n’existe pas encore de connexion entre deux types d’enregistrements, elle peut être créée lorsque vous configurez la hiérarchie. Une fois définie, la hiérarchie établit un chemin d’accès structuré entre les types d’enregistrements associés dans l’espace de travail.

Les hiérarchies génèrent des chemins de navigation pour les types d’enregistrements et les <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> d’enregistrements qui s’affichent dans leurs en-têtes. Ainsi, les utilisateurs savent où ils se trouvent dans la hiérarchie à n’importe quelle étape de leur workflow.

Pour obtenir des informations générales sur les hiérarchies et les chemins de navigation, voir [ Présentation des hiérarchies et des chemins de navigation ](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Conditions d’accès

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ Développez pour afficher les exigences d’accès afin d’effectuer les étapes de cet article :  

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

## Créer une hiérarchie d’espace de travail

{#step1-to-planning}

1. Cliquez sur une carte d’espace de travail.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’espace de travail, puis cliquez sur **Paramètres**.
La section **Hiérarchies** s’ouvre par défaut.
1. Cliquez sur **Nouvelle hiérarchie** dans le coin supérieur droit de la page **Hiérarchies**.
1. Cliquez sur **Ajouter un objet** et sélectionnez un objet dans le menu déroulant. Il s&#39;agira du premier objet parent dans votre hiérarchie.
Le premier parent ne peut être qu&#39;un type d&#39;enregistrement Planning. Les projets Workfront ne peuvent pas être sélectionnés en tant que parents d&#39;autres types d&#39;objets dans une hiérarchie.
1. Cliquez sur **Ajouter un objet** pour ajouter un second objet qui est le premier enfant de votre hiérarchie, puis sélectionnez un autre objet dans le menu déroulant.
   ![Nouvelle zone de hiérarchie sans champ sélectionné](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. Cliquez sur **Sélectionner le champ connecté** pour indiquer quel champ connecte les deux objets.
1. (Conditionnel) S’il existe un champ connecté entre les deux types d’objet, sélectionnez-le dans la liste. Sinon, cliquez sur **Ajouter une nouvelle connexion**.

   >[!WARNING]
   >
   >Si le champ **Créer le champ correspondant sur le type d’enregistrement lié** n’a pas été sélectionné lors de la création du champ connecté, vous devez d’abord modifier le champ avant de pouvoir continuer.

1. (Conditionnel) Si vous ajoutez une nouvelle connexion, procédez comme suit :

   1. Ajoutez un nom pour votre champ connecté dans la zone **Nom**.
   1. Sélectionnez l’un des types de connexion suivants :

      * **Plusieurs à plusieurs**
      * **Un à plusieurs**
      * **Plusieurs à un**
      * **Un à un**
   1. Sélectionnez l’un des types d’apparences d’enregistrement suivants :

      * **Nom et image**
      * **Nom**
      * **Image**
Pour plus d’informations, voir [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
   1. Cliquer sur **Enregistrer**.
1. (Facultatif) Continuez à ajouter jusqu’à 4 types d’objets à vos hiérarchies en suivant les étapes ci-dessus. Vous pouvez d’abord ajouter tous vos types d’objets, puis ajouter les champs de connexion entre eux.
1. (Facultatif) Cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/minus-icon.png) pour supprimer une connexion.
1. Cliquez sur **Enregistrer** pour enregistrer votre hiérarchie.

   >[!TIP]
   >
   >Le bouton **Enregistrer** est grisé si tous les champs connectés ne sont pas en place.

   Les événements suivants se produisent :

   * La hiérarchie est ajoutée à la section **Hiérarchies** de l’espace de travail.
   * Les enregistrements qui renseignent les champs de connexion affichent toutes les connexions dans leurs chemins de navigation, lorsque vous accédez à la page d&#39;un enregistrement.
1. (Facultatif) Pointez sur une hiérarchie, puis cliquez sur le menu **Plus**, puis sur l’une des options suivantes :

   * **Modifier** : permet d’ouvrir la boîte de dialogue **Modifier la hiérarchie** dans laquelle vous pouvez apporter des modifications.
   * **Supprimer** : supprime définitivement la hiérarchie. Les hiérarchies supprimées ne peuvent pas être récupérées. Les champs de connexion ne sont pas supprimés.





