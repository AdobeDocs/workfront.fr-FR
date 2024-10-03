---
title: Création et gestion d’un formulaire de requête dans Adobe Workfront Planning
description: Après avoir sélectionné un type d’enregistrement dans la zone de planification Adobe Workfront, vous pouvez créer un formulaire de demande et l’associer à ce type d’enregistrement. Vous pouvez ensuite partager un lien vers ce lien avec d’autres utilisateurs internes ou externes. Les utilisateurs disposant d’un lien vers le formulaire peuvent renseigner les valeurs de champ qu’il contient et en l’envoyant, ils peuvent ajouter un nouvel enregistrement pour le type d’enregistrement qui lui est associé.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 7c2fa065045f434b3a761f4742ca496670bfd6b2
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 15%

---

# Création et gestion d’un formulaire de requête dans Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Vous pouvez créer un formulaire de demande et l’associer à un type d’enregistrement dans Adobe Workfront Planning. Vous pouvez ensuite partager un lien vers ce lien avec d’autres utilisateurs internes ou externes.

Les utilisateurs disposant d’un lien vers le formulaire peuvent y mettre à jour les valeurs de champ et ajouter de nouveaux enregistrements en les envoyant.

Cet article décrit comment un gestionnaire d’espace de travail peut créer un formulaire de demande associé à un type d’enregistrement.

Pour plus d’informations sur l’envoi d’une demande à un type d’enregistrement pour créer un enregistrement, voir [Soumettre des demandes de planification Adobe Workfront pour créer des enregistrements](/help/quicksilver/planning/requests/submit-requests.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Pour pouvoir accéder à Workfront Planning, vous devez disposer des éléments suivants :

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
   <td role="rowheader"><p>Formule de planification Adobe Workfront*</p></td>
   <td>
<p>Tous </p>  
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </td>

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
   <td>
   <p>Standard</p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations d’objet</p></td>
   <td>
   <ul>
   <li><p>Gérer les autorisations d’un espace de travail</p></li>
    <li><p>L’administration système peut gérer les espaces de travail qu’elle n’a pas créés. </p></li>
    </ul>
   <p>Pour plus d’informations sur les autorisations de partage pour les objets Workfront Planning, voir <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Vue d’ensemble des autorisations de partage dans Adobe Workfront Planning</a>. 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p>  
</td>
  </tr>
 </tbody>
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un formulaire de demande pour un type d’enregistrement

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail dans lequel vous souhaitez ajouter des enregistrements.

   L’espace de travail s’ouvre et les types d’enregistrement s’affichent sous forme de cartes.

1. Cliquez sur la vignette d’un type d’enregistrement pour plus de détails. Pour plus d’informations sur la création d’un type d’enregistrement, consultez la section [Créer des types d’enregistrement](/help/quicksilver/planning/architecture/create-record-types.md).

   La page du type d’enregistrement s’ouvre dans la dernière vue à laquelle vous avez accédé. Par défaut, une page de type enregistrement s’ouvre dans la vue de tableau.

1. Cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du nom du type d’enregistrement dans l’en-tête de la page, puis cliquez sur **Créer un formulaire de demande**.
1. Mettez à jour le nom du formulaire de requête. Par défaut, le nom du formulaire est **Formulaire de demande sans titre**. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (Facultatif) Ajoutez une **description** pour le formulaire de demande.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Cliquez sur **Créer**. Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre.

   ![](assets/campaigns-request-form-edit-mode.png)

   Le formulaire de demande contient les informations suivantes, par défaut :

   * Champs d’enregistrement disponibles dans la vue de tableau du type d’enregistrement sélectionné. <!--they are working on removing the limitation below-->

     >[!IMPORTANT]
     >
     >   Les champs des types suivants ne s’affichent pas dans le formulaire de requête :
     >
     >    * Personnes
     >    * Champs connectés (y compris les connexions avec des ressources Experience Manager)
     >    * Champs de recherche connectés
     >    * Formule

   * **Section par défaut** : il s’agit du saut de section par défaut appliqué par Workfront au formulaire de demande. La section Par défaut ne peut pas être renommée ni supprimée.
   * **Objet** : champ qui identifie la demande dans Workfront. Cette fonctionnalité n’est pas encore disponible.
   * Tous les champs associés au type d&#39;enregistrement.

     Les champs contenus dans le formulaire de demande seront visibles par tous ceux qui envoient une demande à ce type d’enregistrement.

1. (Facultatif) Pointez sur les champs du formulaire que vous souhaitez supprimer, puis cliquez sur l’icône **x** pour les supprimer. Ils sont ajoutés à l’onglet **Champs** situé à gauche du formulaire.

   Par exemple, supprimez le champ **Objet**, car celui-ci n’est pas visible dans la planification Workfront. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Cliquez sur n’importe quel champ, puis utilisez les commandes du panneau de droite du formulaire pour définir leur taille ou l’une des informations suivantes :

   * **Libellé** : il s’agit du nom du champ tel qu’il apparaîtra sur le formulaire de demande. Cela ne modifie pas le nom du champ d’enregistrement.
   * **Instructions** : ajoutez des informations supplémentaires sur le champ.
   * **Créer un champ obligatoire** : lorsque cette option est sélectionnée, le champ doit avoir une valeur. Sinon, le formulaire ne peut pas être envoyé.
   * **Ajouter une logique** : définissez les conditions qui doivent être remplies pour que le champ s’affiche ou soit masqué.

   Le type de champ de chaque champ s’affiche en haut du panneau de droite, une fois le champ sélectionné dans le formulaire. Les noms des types de champ sur le formulaire de requête diffèrent de ceux de la vue de tableau. Le tableau suivant décrit les différences entre les noms des types de champ dans la vue de tableau et les noms des mêmes champs dans le formulaire de requête du type d’enregistrement :

   | Type de champ Planification Workfront | Type de champ de formulaire de requête |
   |-------------------------------|-------------------------|
   | Texte à une ligne | Texte sur une seule ligne |
   | Paragraphe | Texte avec formatage |
   | Devise, Nombre, Pourcentage | Texte sur une seule ligne |
   | Sélection unique | Liste déroulante à sélection unique |
   | Sélection multiple | Menu déroulant multi-sélection |
   | Case à cocher | Groupe Case à cocher |

   >[!NOTE]
   >
   >   Les formats des champs sont conservés. Par exemple, bien que les champs Devise et Pourcentage s’affichent sous forme de champs de texte Ligne unique , les informations contenues dans les champs s’affichent sous forme de devise et de valeur en pourcentage.


1. (Facultatif) Cliquez sur l’onglet **Eléments de contenu** sur le côté gauche du formulaire, puis ajoutez l’un des éléments suivants :

   * **Texte descriptif**
   * **Saut de section**

   Pour plus d’informations sur la création d’un formulaire personnalisé, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Facultatif) Cliquez sur **Aperçu** pour afficher comment le formulaire s’affichera pour les autres utilisateurs lorsqu’ils l’utiliseront pour envoyer un nouvel enregistrement.
1. Cliquez sur **Publish** pour publier le formulaire et obtenir un lien unique.

   Les événements suivants se produisent :

   * Le bouton Publish est supprimé.
   * Le bouton **Annuler la publication** est ajouté au formulaire. Si vous cliquez dessus, le formulaire n’est pas accessible.
   * Un bouton **Partager** est ajouté au formulaire.

1. Cliquez sur **Partager** pour partager le formulaire avec d’autres personnes.

   ![](assets/share-box-for-request-form.png)

1. Sélectionnez l’une des options suivantes pour indiquer quels types d’utilisateurs peuvent accéder à ce formulaire :

   * Toute personne disposant d’un accès en affichage ou supérieur à l’espace de travail
   * Toute personne disposant d’un accès en contribution ou supérieur à l’espace de travail
   * Toute personne disposant du lien

   >[!IMPORTANT]
   >
   >Lorsque vous sélectionnez **Toute personne disposant du lien**, tout le monde peut accéder au formulaire et envoyer un nouvel enregistrement, même les personnes en dehors de votre organisation qui n’ont pas de compte Workfront.

1. (Conditionnel) Si vous avez sélectionné **Toute personne ayant le lien** à l’étape précédente, sélectionnez la **date d’expiration du lien** dans le calendrier disponible. Une erreur s’affichera lorsque le lien arrivera à expiration. Vous devrez mettre à jour la date du lien pour pouvoir accéder à nouveau au formulaire.

   Vous pouvez sélectionner des dates futures dans les 180 jours à partir de la date actuelle.

1. Cliquez sur **Enregistrer et copier le lien** pour enregistrer les détails de partage pour le formulaire.

   Les options de partage de formulaire sont enregistrées et le lien est copié dans le presse-papiers. Vous pouvez maintenant le partager avec d’autres personnes.

   Pour plus d’informations sur la création d’enregistrements à l’aide d’un lien vers un formulaire de demande, voir [Soumettre des demandes de planification Adobe Workfront](/help/quicksilver/planning/requests/submit-requests.md).

1. Cliquez sur **Enregistrer** dans le coin inférieur droit de l’écran pour enregistrer le formulaire.
1. Cliquez sur la flèche pointant vers la gauche située à gauche du nom du formulaire dans l’en-tête pour fermer le formulaire.

   La page de type d’enregistrement s’ouvre.
1. (Facultatif) Cliquez sur le menu **Plus** ![](assets/more-menu.png) situé à droite du nom du type d’enregistrement dans l’en-tête, puis effectuez l’une des opérations suivantes :
   * Cliquez sur **Mettre à jour le formulaire de demande** pour apporter des modifications au formulaire de demande.
   * Cliquez sur **Copier le lien vers le formulaire de demande** pour partager le lien vers le formulaire avec d’autres personnes.

   >[!TIP]
   >
   >Il y a une indication que le lien est partagé publiquement lorsque c&#39;est le cas.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
