---
title: Création de hiérarchies Workspace
description: En tant que gestionnaire d'espace de travail, vous pouvez créer plusieurs hiérarchies d'espaces de travail entre les types d'enregistrements dans Adobe Workfront Planning. Après avoir connecté des types d’enregistrements dans un espace de travail et créé une hiérarchie, les types d’enregistrements sont connectés les uns aux autres, un type d’enregistrement étant désigné comme parent et jusqu’à 3 autres types d’enregistrements étant configurés comme enfants.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 34921b12ad902ba7390e4ea34825331280e7a8d6
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 6%

---


# Créer des hiérarchies d’espace de travail

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

En tant que gestionnaire d&#39;espace de travail, vous pouvez créer plusieurs hiérarchies d&#39;espaces de travail entre les types d&#39;enregistrements dans Adobe Workfront Planning.

Une fois les types d’enregistrements connectés dans un espace de travail, vous pouvez créer une hiérarchie qui organise ces connexions. Les hiérarchies organisent les types d&#39;enregistrements et d&#39;objets en relations parent-enfant et peuvent contenir jusqu&#39;à quatre niveaux de types d&#39;objets.

S’il n’existe pas encore de connexion entre deux types d’enregistrements, elle peut être créée lorsque vous configurez la hiérarchie. Une fois définie, la hiérarchie établit un chemin d’accès structuré entre les types d’enregistrements associés dans l’espace de travail.

Les hiérarchies génèrent des chemins de navigation pour leurs enregistrements respectifs qui s’affichent dans leurs en-têtes. Ainsi, les utilisateurs savent où ils se trouvent dans la hiérarchie à n’importe quelle étape de leur workflow.

Pour obtenir des informations générales sur les hiérarchies et les chemins de navigation, voir [&#x200B; Présentation des hiérarchies et des chemins de navigation &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Conditions d’accès

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

Vous pouvez créer jusqu’à 5 hiérarchies dans un espace de travail.

{#step1-to-planning}

1. Cliquez sur une carte d’espace de travail.
1. Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom de l’espace de travail, puis cliquez sur **Paramètres**.
La section **Hiérarchies** s’ouvre par défaut.
1. Cliquez sur **Nouvelle hiérarchie** dans le coin supérieur droit de la page **Hiérarchies**.
1. Cliquez sur **Ajouter un objet** et sélectionnez un type d’objet dans le menu déroulant. Il s&#39;agira du premier type d&#39;objet de votre hiérarchie. <!--logged bug to correct to "Add object type"-->

   Le premier type d&#39;objet ne peut être qu&#39;un type d&#39;enregistrement Planning.

   Les projets Workfront ne peuvent pas être sélectionnés en tant que parents d&#39;autres types d&#39;objets dans une hiérarchie.

1. Cliquez sur **Ajouter un objet** pour ajouter un second type d&#39;objet correspondant au premier enfant de votre hiérarchie, puis sélectionnez un autre type d&#39;objet dans le menu déroulant.
Chaque type d&#39;objet supplémentaire devient l&#39;enfant des types d&#39;objet précédents.

   ![Nouvelle zone de hiérarchie sans champ sélectionné](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. Cliquez sur **Sélectionner le champ connecté** pour indiquer quel champ connecte les deux objets.
1. (Conditionnel) S’il existe plusieurs champs de connexion, sélectionnez-en un dans la liste,

   Ou

   Cliquez sur **Ajouter une nouvelle connexion** pour ajouter un nouveau champ de connexion.

   Cela crée un champ de connexion à partir du type d’enregistrement que vous utilisez en tant que parent et un champ de connexion correspondant à celui-ci à partir du type d’enregistrement que vous utilisez en tant qu’enfant.

   Si vous créez une connexion à des projets Workfront, aucun champ n’est créé pour le projet.

1. (Conditionnel) Si aucun champ connecté n’est disponible, cliquez sur **Créer une connexion** et ajoutez une nouvelle connexion, puis cliquez sur **Enregistrer**.

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

      Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).

   1. Cliquer sur **Enregistrer**.

1. (Conditionnel) Si l’option **Créer le champ correspondant sur le type d’enregistrement lié** n’a pas été sélectionnée lors de la création du champ connecté, vous obtenez une erreur et devez d’abord effectuer les opérations suivantes : <!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. Cliquez sur **Annuler** dans la zone **Nouvelle hiérarchie**.
   1. Cliquez sur la flèche vers l’arrière à gauche du nom de l’espace de travail, puis cliquez sur la carte du type d’enregistrement que vous souhaitez choisir comme parent.
   1. Ouvrez la vue Tableau du type d’enregistrement que vous avez sélectionné à l’étape ci-dessus, puis accédez au champ de connexion avec le type d’objet que vous souhaitez utiliser comme enfant, passez la souris sur l’en-tête de colonne, puis cliquez sur le champ **Modifier**.
   1. Activez le paramètre **Créer le champ correspondant sur le type d’enregistrement lié** puis cliquez sur **Enregistrer**.
   1. Revenez à la zone **Paramètres** de l’espace de travail et cliquez de nouveau sur **Nouvelle hiérarchie**, puis suivez les étapes pour créer une hiérarchie.

1. (Facultatif) Continuez à ajouter jusqu’à 4 types d’objets à vos hiérarchies en suivant les étapes ci-dessus. Vous pouvez d’abord ajouter tous vos types d’objets, puis ajouter les champs de connexion entre eux.
1. (Facultatif) Cliquez sur l’icône **Supprimer** ![Icône Supprimer](assets/minus-icon.png) pour supprimer une connexion.
1. Cliquez sur **Enregistrer** pour enregistrer votre hiérarchie.

   >[!TIP]
   >
   >Le bouton **Enregistrer** est grisé si tous les champs connectés ne sont pas en place.

   Les événements suivants se produisent :

   * La hiérarchie est ajoutée à la section **Hiérarchies** de l’espace de travail.
   * Les enregistrements qui renseignent les champs de connexion affichent toutes les connexions dans leurs chemins de navigation, lorsque vous accédez à la page d&#39;un enregistrement.

   >[!NOTE]
   >
   >Vous pouvez connecter un enregistrement d&#39;un type d&#39;enregistrement enfant à un maximum de 10 enregistrements d&#39;un type d&#39;enregistrement parent.
   >
   >Pour plus d’informations, voir [&#x200B; Présentation de la hiérarchie et du chemin de navigation &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

1. (Facultatif) Passez la souris sur une hiérarchie, puis cliquez sur le menu **Plus**.

   ![Menu Hiérarchie plus développé](assets/hierarchy-more-menu-expanded.png)

1. Cliquez sur l’une des options suivantes :

   * **Modifier** : permet d’ouvrir la boîte de dialogue **Modifier la hiérarchie** dans laquelle vous pouvez apporter des modifications.
   * **Supprimer** : supprime définitivement la hiérarchie. Les hiérarchies supprimées ne peuvent pas être récupérées. Les champs de connexion ne sont pas supprimés.





