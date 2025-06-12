---
product-area: projects;templates
navigation-topic: manage-projects
title: Enregistrer un projet en tant que modèle
description: Enregistrer un projet en tant que modèle Enregistrer en tant que modèle au niveau du projet, afin que les utilisateurs et utilisatrices puissent le voir dans l’IU. Il existe un autre article que vous pouvez consulter pour plus de détails (étape par étape). Cette fonctionnalité doit rester dans les zones de projets ET de modèles.
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 63%

---

# Enregistrer un projet en tant que modèle

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<div class="preview">

Les informations surlignées sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Les mêmes fonctionnalités seront également disponibles dans l’environnement de production pour tous les clients après une semaine à compter de la version préliminaire.

Pour plus d’informations, voir [Modernisation des interfaces](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Si vous décidez qu’un projet va être reproduit à l’avenir, vous pouvez créer un modèle à partir de ce projet existant. Vous pouvez ensuite réutiliser le modèle pour créer des projets futurs qui contiennent des informations similaires ou qui partagent la même chronologie ou les mêmes affectations que le projet existant.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard </p>
   Ou 
   <p>Actuel : formule </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur sur un projet </p> <p>Vous obtenez les autorisations de gestion sur le modèle après avoir enregistré le projet en tant que modèle.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Enregistrer un projet en tant que modèle

L’enregistrement d’un projet en tant que modèle diffère dans les environnements de production et de prévisualisation.

### Enregistrement d’un projet en tant que modèle dans l’environnement de production

1. Accédez au projet que vous souhaitez enregistrer en tant que modèle.
1. Cliquez sur le menu **Plus** ![icône Plus](assets/qs-more-icon-on-an-object.png), puis sur **Enregistrer en tant que modèle**.
1. Indiquez les informations suivantes pour le modèle :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td>Attribuez un nom au modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Fournissez une description du modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est active</td> 
      <td> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Oui</strong> : d’autres utilisateurs et utilisatrices peuvent trouver le modèle et le joindre à des projets.</p> </li> 
        <li><strong>Non</strong> : les autres utilisateurs et utilisatrices ne peuvent pas trouver le modèle et ne peuvent pas le joindre aux projets.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td>Utilisez la liste déroulante pour sélectionner les formulaires personnalisés à joindre au modèle. Si des formulaires personnalisés ont déjà été associés au projet, tous les champs de données de ces formulaires personnalisés s’affichent.<br>Vous pouvez inclure jusqu’à 10 formulaires personnalisés sur un seul modèle.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Géer les formulaires** pour supprimer ou réorganiser les formulaires. Pour plus d’informations sur la suppression et la réorganisation des formulaires personnalisés sur le modèle, voir [Formulaires personnalisés](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. Cliquez sur **Étape suivante.**
1. Dans la section **Options**, cochez la case en regard des informations que vous souhaitez effacer du modèle.

   ![](assets/save-as-template-options-step-350x109.png)

1. Cliquez sur **Étape suivante.**
1. Dans la section **Exclure**, sélectionnez les tâches à exclure du projet.

   ![](assets/save-as-template-exclude-350x205.png)

1. Cliquez sur **Terminer et enregistrer le modèle**.

   Votre modèle apparaît désormais dans la liste des modèles disponibles et peut être joint à un projet existant ou utilisé pour en créer un nouveau.


<div class="preview">

### Enregistrement d’un projet en tant que modèle dans l’environnement de prévisualisation

1. Accédez au projet que vous souhaitez enregistrer en tant que modèle.
1. Cliquez sur le menu **Plus** ![icône Plus](assets/qs-more-icon-on-an-object.png), puis sur **Enregistrer en tant que modèle**.
1. Dans la section **Enregistrer en tant que modèle**, spécifiez les informations suivantes pour le modèle :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom de modèle</td> 
      <td>Attribuez un nom au modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Fournissez une description du modèle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Est active</td> 
      <td> <p>Sélectionnez l’une des options suivantes :</p> 
       <ul> 
        <li> <p><strong>Oui</strong> : d’autres utilisateurs et utilisatrices peuvent trouver le modèle et le joindre à des projets.</p> </li> 
        <li><strong>Non</strong> : les autres utilisateurs et utilisatrices ne peuvent pas trouver le modèle et ne peuvent pas le joindre aux projets.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td>Utilisez la liste déroulante pour sélectionner les formulaires personnalisés à joindre au modèle. Si des formulaires personnalisés ont déjà été associés au projet, tous les champs de données de ces formulaires personnalisés s’affichent.<br>Vous pouvez inclure jusqu’à 10 formulaires personnalisés sur un seul modèle.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Forms personnalisé** dans le panneau de gauche pour supprimer ou réorganiser les formulaires.

   Pour réorganiser les formulaires, faites-les glisser et déposez-les dans l’ordre approprié.
Pour supprimer un formulaire, sélectionnez-le, puis cliquez sur **Supprimer**. Cliquez sur **Annuler** pour supprimer les formulaires sélectionnés.

   ![Zone des formulaires personnalisés dans la zone enregistrer en tant que modèle](assets/custom-forms-ara-in-save-as-template-box.png)

1. Mettez à jour les informations dans les formulaires personnalisés joints, si nécessaire. Les informations sont transférées vers le modèle.

1. Cliquez sur **Options** dans la section du panneau de gauche, puis cochez la case en regard des informations à transférer au modèle. Les éléments désélectionnés ne sont pas transférés vers le modèle. Par défaut, toutes les options sont désélectionnées.

   ![Zone Options de la zone Enregistrer en tant que modèle](assets/options-area-in-save-as-template-box.png)

1. Cliquez sur **Exclure** dans le panneau de gauche, puis sélectionnez les tâches à exclure du projet. Par défaut, toutes les tâches sont désélectionnées.

   ![Exclure la zone dans la zone Enregistrer comme modèle](assets/exclude-area-save-as-template-box.png)

1. Cliquez sur **Terminer et enregistrer le modèle**.

   Votre modèle apparaît désormais dans la liste des modèles disponibles et peut être joint à un projet existant ou utilisé pour en créer un nouveau.

</span>