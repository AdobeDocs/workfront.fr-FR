---
title: Modification des types d’enregistrement
description: Vous pouvez modifier les types d’enregistrement après leur enregistrement. Les types d’enregistrement sont les types d’objet de la planification Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Modification des types d’enregistrement

{{maestro-important-intro}}

Les types d’enregistrement sont les types d’objet de la planification Adobe Workfront. Vous pouvez modifier l’aspect des types d’enregistrement que vous ou toute autre personne avez créés. Pour plus d’informations sur la création de types d’enregistrement de planification Workfront, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produit</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Pour connecter les types d’enregistrements de planification Adobe Workfront à Experience Manager Assets, vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance de Workfront de votre entreprise doit être intégrée à Adobe Business Platform ou à Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite dans le programme bêta fermé de planification d’Adobe Workfront. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Quelconque</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Quelconque</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Paramétrages du niveau d'accès</p></td>
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour la planification Workfront.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Planning dans votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Modification des types d’enregistrement

{{step1-to-maestro}}

L’espace de travail du dernier accès doit s’ouvrir par défaut.

1. (Facultatif) Développez la flèche pointant vers le bas située à droite du nom d’un espace de travail existant, puis sélectionnez l’espace de travail pour lequel vous souhaitez modifier les types d’enregistrement.
1. Pointez sur la carte d’un type d’enregistrement, puis cliquez sur le **Plus** menu ![](assets/more-menu.png) dans le coin supérieur droit de la carte de type enregistrement, puis cliquez sur **Mettre à jour l&#39;aspect**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. Dans le **Mettre à jour le type d’enregistrement** , mettez à jour les informations suivantes :

   * **Nom de l’enregistrement**: modifiez le nom du type d’enregistrement, si nécessaire. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **Apparence**: modifiez la couleur et la forme de l’icône associée au type d’enregistrement. Procédez comme suit :
      * Sélectionnez une couleur pour identifier le type d’enregistrement. Il s’agit de la couleur de l’icône de type d’enregistrement. L’option Gris est sélectionnée par défaut.
      * Sélectionnez une icône dans la liste ou commencez à saisir le nom d’une icône pour décrire ce qu’elle représente, puis sélectionnez-la lorsqu’elle s’affiche. Il s’agit de l’icône du type d’enregistrement. Une icône de fichier est sélectionnée par défaut.

     ![](assets/update-record-type-box.png)

1. Cliquez en dehors du **Mettre à jour le type d’enregistrement** pour enregistrer vos modifications.
1. (Facultatif) Cliquez sur la carte de type d’enregistrement dans la zone de l’espace de travail pour ouvrir la page du type d’enregistrement.
1. Cliquez sur le bouton **Plus** à droite du nom du type d’enregistrement, puis cliquez sur **Renommer** pour renommer le type d’enregistrement

   Ou

   Renommez le type d’enregistrement dans l’en-tête .  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   Vous pouvez également renommer un type d’enregistrement dans l’en-tête de la page du type d’enregistrement.
1. (Facultatif) Développez la flèche vers le bas située à droite d’un nom de type d’enregistrement et sélectionnez un autre type d’enregistrement à modifier.
