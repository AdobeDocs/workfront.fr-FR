---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : permet d’afficher une image au lieu d’une chaîne dans une colonne'
description: Vous pouvez remplacer le nom d’un objet dans une vue par une image en mode texte. Vous pouvez également ajouter un lien vers l’image qui permet d’ouvrir l’objet qu’elle remplace.
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 85%

---

# Vue : afficher une image au lieu d’une chaîne dans une colonne

<!--Audited: 11/2024-->

Vous pouvez remplacer le nom d’un objet dans une vue par une image en mode texte. Vous pouvez également ajouter un lien vers l’image qui permet d’ouvrir l’objet qu’elle remplace.

>[!NOTE]
>
>Les images apparaissent dans leur résolution réelle, essayez donc d’utiliser de petites images.

![Remplacer le nom du projet par une image et un lien](assets/replace-project-name-with-image-and-link-350x125.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur pour modifier un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exemple : remplacez le nom d’un projet dans une vue de projet par une image :

1. Chargez une image sur un site web ou un serveur externe à Adobe Workfront. Vous devez pouvoir accéder à l’image à l’aide de votre navigateur web.

   >[!TIP]
   >
   >* Chaque type de navigateur est différent, mais tous peuvent afficher des URL.
   >* Évitez d’utiliser des images chargées sur Workfront. Comme les images stockées dans Workfront ne sont pas disponibles publiquement et possèdent une clé d’accès qui expire au bout d’un certain temps, ces images ne s’affichent plus dans la vue au fil du temps.
   >* Une image enregistrée sur votre ordinateur ne comporte pas d’URL inhérente. Trouvez un site d’hébergement d’images et hébergez-y votre image. Votre entreprise dispose peut-être déjà d’un tel site.

1. À l’aide de votre navigateur web, accédez à l’image que vous avez enregistrée.
1. Obtenez l’URL de l’image en procédant comme suit :

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Cliquez avec le bouton droit et sélectionnez **Copier l’emplacement de l’image**, ou **Obtenir le lien**, selon votre navigateur. Vous disposez maintenant de l’URL de cette image spécifique et pouvez la coller dans le presse-papiers.
   1. Assurez-vous que toutes les personnes disposant de ce lien sont autorisées à afficher l’image en accédant simplement au lien et qu’elles n’ont pas besoin de nom d’utilisateur ou d’utilisatrice pour y accéder.

1. Accédez à un projet, cliquez sur le menu **Plus** ![icône Plus](assets/more-icon-45x33.png) en regard du nom du projet, puis cliquez sur **Modifier**.

1. Dans le champ **URL**, ajoutez le lien à l’image.
1. Accédez à une vue de projet dans une liste de projets.
1. Cliquez sur le menu déroulant **Affichage**, puis sur **Nouvel affichage**.
1. Cliquez sur l’en-tête de la colonne pour le **Nom du projet**, puis cliquez sur **Passer en mode Texte**.

1. Ajoutez le code suivant à la colonne au code existant :

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. Cliquez sur **Terminé** > **Enregistrer la vue**.
L’image que vous avez sélectionnée remplace le nom du projet dans la vue du projet et l’image est un lien vers le projet.
