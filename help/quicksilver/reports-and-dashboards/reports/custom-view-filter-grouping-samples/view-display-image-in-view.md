---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : afficher une image au lieu d’une chaîne dans une colonne »'
description: Vous pouvez remplacer le nom d’un objet dans une vue par une image en mode texte. Vous pouvez également ajouter un lien vers l’image qui permet d’ouvrir l’objet qu’elle remplace.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 100%

---

# Vue : afficher une image au lieu d’une chaîne dans une colonne

Vous pouvez remplacer le nom d’un objet dans une vue par une image en mode texte. Vous pouvez également ajouter un lien vers l’image qui permet d’ouvrir l’objet qu’elle remplace.

>[!NOTE]
>
>Les images apparaissent dans leur résolution réelle, essayez donc d’utiliser de petites images.

![](assets/replace-project-name-with-image-and-link-350x125.png)

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demander la modification d’un affichage </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

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

1. Accédez à un projet, cliquez sur le menu **Plus** ![](assets/more-icon-45x33.png) en regard du nom du projet, puis sur **Modifier**.

1. Dans le champ **URL**, ajoutez le lien à l’image.
1. Accédez à la vue d’un projet dans une liste ou un rapport et personnalisez-la.
1. Cliquez sur l’en-tête de la colonne pour le **Nom du projet**, puis cliquez sur **Passer en mode Texte**.

1. Ajoutez le code suivant à la colonne au code existant :

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   L’image que vous avez sélectionnée remplace le nom du projet dans la vue du projet et l’image est un lien vers le projet.

1. Cliquez sur **Enregistrer la vue**.
