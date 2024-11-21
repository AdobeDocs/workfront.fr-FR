---
title: Création d’objets Workfront à l’aide des automatisations d’enregistrements de planification Adobe Workfront
description: Vous pouvez configurer des automatisations dans la planification Workfront qui, lorsqu’elles sont activées, créent des objets dans Workfront.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 03eedb00ab45b95e87670872cf015c0f6840658e
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 12%

---

# Création d’objets à l’aide d’automatismes d’enregistrement Adobe Workfront Planning

<!--add screen shots when UI is finalized-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

Vous pouvez configurer des automatisations dans la planification Adobe Workfront qui, lorsqu’elles sont activées, créent des objets dans la planification Workfront ou Workfront.

Vous pouvez configurer et activer l’automatisation dans la page de l’enregistrement. L&#39;objet qui est créé est connecté à l&#39;enregistrement Planning et placé dans le champ que vous indiquez dans l&#39;automatisation.

Par exemple, vous pouvez créer une automatisation qui prend une campagne de planification Workfront et crée un projet dans Workfront pour suivre la progression de cette campagne. Le projet sera connecté à la campagne de planification Workfront.

Pour plus d&#39;informations sur les enregistrements connectés, consultez la [présentation des enregistrements connectés](/help/quicksilver/planning/records/connected-records-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
<p>L’un des projets Workfront suivants est prévu :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package de planification Adobe Workfront*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td> Standard
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p> 
   <p>Modifiez l’accès dans Workfront pour les types d’objets que vous souhaitez créer (projets, portefeuilles, programmes). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Gérez les autorisations de l’espace de travail auquel vous souhaitez ajouter des enregistrements. </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>
   <p>Gérez les autorisations d’accès aux objets Workfront (portfolios) pour ajouter des objets enfants (projets).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Tous les utilisateurs, y compris les administrateurs Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planification dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Observations relatives à la création d’objets et d’enregistrements à l’aide d’une automatisation

* Le nouveau nom d’objet ou d’enregistrement est identique au nom d’enregistrement à partir duquel vous le créez.
* Si l&#39;enregistrement pour lequel vous utilisez l&#39;automatisation a déjà des objets du même type connectés dans le champ que vous choisissez d&#39;ajouter de nouveaux objets, les nouveaux objets sont ajoutés au champ de connexion et les objets existants restent également connectés.


## Configuration d’une automatisation dans la planification Workfront

Vous devez configurer une automatisation dans la planification Workfront avant de pouvoir l’utiliser pour créer des objets.

{{step1-to-planning}}

1. Cliquez sur une carte de type enregistrement, puis sur le nom d’un enregistrement.

   La page de type d’enregistrement s’ouvre.
1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du nom du type d’enregistrement, puis cliquez sur **Gérer les automatisations**.

   La liste des automatisations disponibles s’ouvre.

1. Cliquez sur **Nouvelle automatisation** dans le coin supérieur droit de l’écran.
1. Mettez à jour les champs suivants :

   * **Texte du bouton** : saisissez le texte que vous souhaitez afficher sur le bouton d’automatisation. Les utilisateurs cliqueront sur ce bouton lors de l’utilisation de l’automatisation pour créer un objet Workfront.
   * **Icône Bouton** : sélectionnez une icône pour le bouton. Une icône est sélectionnée par défaut.
   * **Type d’objet** : sélectionnez l’objet que vous souhaitez que l’automatisation crée. Champ obligatoire.

     Vous pouvez créer les objets suivants à partir des enregistrements de planification Workfront :

      * Projet
      * Portfolio
      * Programme
      * Groupe
      * Enregistrement
1. (Conditionnel) Selon le type d’objet que vous souhaitez créer, mettez à jour les champs suivants :

   * **Projet** :
      * **Champ connecté où l’objet est créé** : il s’agit du champ connecté où le nouveau projet s’affichera. Champ obligatoire
      * **Modèle à partir duquel créer le projet** : sélectionnez un modèle de projet que Workfront utilisera pour créer le projet.
   * **Portfolio** :
      * **Champ connecté où l’objet est créé** : il s’agit du champ connecté où le nouveau portfolio s’affichera. Champ obligatoire.
      * **Formulaire personnalisé à joindre au nouveau portfolio** : sélectionnez un formulaire personnalisé à joindre au nouveau portfolio. Vous devez créer un formulaire personnalisé de portefeuille avant de pouvoir le sélectionner.
   * **Program** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où le nouveau programme s&#39;affichera. Champ obligatoire.
      * **portefeuille de programmes** : sélectionnez un portefeuille où le nouveau programme sera ajouté. Champ obligatoire.
      * 
         * **Formulaire personnalisé à joindre au nouveau programme** : sélectionnez un formulaire personnalisé à joindre au nouveau programme. Vous devez créer un formulaire personnalisé de programme avant de pouvoir le sélectionner.
   * **Group** :
      * **Champ connecté où l&#39;objet est créé** : il s&#39;agit du champ connecté où le nouveau groupe s&#39;affichera. Champ obligatoire.
      * **Formulaire personnalisé à joindre au nouveau groupe** : sélectionnez un formulaire personnalisé à joindre au nouveau programme. Vous devez créer un formulaire personnalisé de programme avant de pouvoir le sélectionner.
   * **Record** :
      * **Type d’enregistrement connecté** : sélectionnez le type d’enregistrement à créer.
      * **Champ connecté où l&#39;enregistrement est créé** : il s&#39;agit du champ connecté où le nouvel enregistrement s&#39;affichera. Champ obligatoire.
      * **Champ de carte** : sélectionnez des champs à partir du type d’enregistrement pour lequel l’automatisation est créée afin de les mapper aux champs du type d’enregistrement connecté.
      * **Pour le champ d’enregistrement connecté** : sélectionnez des champs de l’enregistrement connecté qui correspondront aux champs du type d’enregistrement pour lequel vous créez l’automatisation.
1. (Facultatif et conditionnel) Si vous ne disposez pas d’un champ de connexion pour un type d’objet Workfront, cliquez sur l’icône **Créer un champ de connexion** ![](assets/create-a-connection-field-icon.png) pour ajouter un champ.
1. (Facultatif et conditionnel) Si vous avez choisi d’ajouter un enregistrement, cliquez sur **Ajouter** dans la zone **Associer les champs connectés** pour ajouter et mapper des champs supplémentaires.
1. Cliquez sur **Créer**

L’automatisation apparaît dans la liste des automatisations et peut être utilisée dans les enregistrements.

## Utilisation d’une automatisation de planification Workfront pour créer un objet

1. Dans Workfront Planning, ouvrez la page de type d’enregistrement contenant les enregistrements que vous souhaitez utiliser pour créer des objets Workfront.
1. Ouvrez le mode Tableau.
1. Sélectionnez un ou plusieurs enregistrements.

   Une barre bleue s’affiche au bas du tableau avec des boutons supplémentaires, notamment des boutons d’automatisation.
1. Cliquez sur le bouton d’automatisation près du coin inférieur droit de l’écran.

   ![Bouton Automatisation](assets/automation-custom-button.png)

   Le nouvel objet s’affiche dans le champ connecté que vous avez indiqué dans la configuration du bouton d’automatisation.

   >[!NOTE]
   >
   >Nous vous recommandons de vérifier que l’objet a été créé et connecté comme prévu.

1. (Facultatif) Cliquez sur le nouvel objet dans le champ connecté. La page d’objet s’ouvre et vous pouvez apporter des modifications supplémentaires au nouvel objet.

<!--you might need to add something about notifications and emails?!-->
