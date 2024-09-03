---
product-area: projects;templates
navigation-topic: manage-projects
title: Enregistrer un projet en tant que modèle
description: Enregistrer un projet en tant que modèle Enregistrer en tant que modèle au niveau du projet, afin que les utilisateurs et utilisatrices puissent le voir dans l’IU. Il existe un autre article que vous pouvez consulter pour plus de détails (étape par étape). Cette fonctionnalité doit rester dans les zones de projets ET de modèles.
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 100%

---

# Enregistrer un projet en tant que modèle

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

Si vous décidez qu’un projet va être reproduit à l’avenir, vous pouvez créer un modèle à partir de ce projet existant. Vous pouvez ensuite réutiliser le modèle pour créer des projets futurs qui contiennent des informations similaires ou qui partagent la même chronologie ou les mêmes affectations que le projet existant.

## Conditions d’accès

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux modèles</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur sur un projet </p> <p>Vous obtenez les autorisations de gestion sur le modèle après avoir enregistré le projet en tant que modèle.</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Enregistrer un projet en tant que modèle

1. Accédez au projet que vous souhaitez enregistrer en tant que modèle.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png), puis sur **Enregistrer en tant que modèle**.
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
1. Dans la section **Options**, cochez la case en regard des informations à effacer du modèle.

   ![](assets/save-as-template-options-step-350x109.png)

1. Cliquez sur **Étape suivante.**
1. Dans la section **Exclure**, sélectionnez les tâches à exclure du projet.

   ![](assets/save-as-template-exclude-350x205.png)

1. Cliquez sur **Terminer et enregistrer le modèle**.

   Votre modèle apparaît désormais dans la liste des modèles disponibles et peut être joint à un projet existant ou utilisé pour en créer un nouveau.
