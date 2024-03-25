---
title: Création de types d’enregistrement de taxonomie
description: Lorsque vous utilisez un modèle pour créer un espace de travail, les types d’enregistrements sont créés dans les sections Types d’enregistrements opérationnels et Taxonomies .
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 3%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Création de types d’enregistrement de taxonomie

{{maestro-important-intro}}

Lorsque vous utilisez un modèle pour créer un espace de travail, les types d’enregistrement sont créés dans les sections suivantes :

* Types d’enregistrements opérationnels
* Taxonomies

Les types d’enregistrement dans la section Taxonomies d’un espace de travail capturent des attributs sur les types d’enregistrement dans la section Types d’enregistrement opérationnels du même espace de travail.

Par exemple, Campaign peut être un type d’enregistrement opérationnel. Vous trouverez ci-dessous des taxonomies qui capturent des attributs sur le type d’enregistrement Campaign : Région, Audience, Pays.

Pour plus d’informations sur les types d’enregistrement, voir [Présentation des types d’enregistrement](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>Pour connecter des types d’enregistrement à Experience Manager Assets, vous devez disposer d’une licence Adobe Experience Manager Assets et l’instance de Workfront de votre entreprise doit être intégrée à Adobe Business Platform ou à Adobe Admin Console.</p> </td>
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
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour la planification Adobe Workfront.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Planning dans votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Gestion des autorisations d’un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Remarques concernant la création de taxonomies

* Vous devez créer un espace de travail à l’aide d’un modèle avant de pouvoir créer des types d’enregistrement dans la section Taxonomies de l’espace de travail.

  Pour plus d’informations sur les espaces de travail, voir [Créer des espaces de travail](../architecture/create-workspaces.md).
* Vous pouvez créer un type d&#39;enregistrement dans la section Taxonomies d&#39;un espace de travail en effectuant l&#39;une des opérations suivantes :
   * Créez-les automatiquement lorsque vous créez un espace de travail à l’aide d’un modèle. Pour plus d’informations, voir [Créer des espaces de travail](../architecture/create-workspaces.md).
   * Créez-les manuellement, à partir de zéro, dans la section Taxonomies d&#39;un espace de travail.

* Par défaut, toutes les taxonomies nouvellement créées comportent les champs suivants :

   * Nom
   * Description
   * Date de début
   * Date de fin
   * Statut

  De plus, vous pouvez ajouter des champs personnalisés aux taxonomies. Pour plus d’informations, voir [Créer des champs](../fields/create-fields.md).

  >[!NOTE]
  >
  >    Les types d&#39;enregistrements de taxonomie créés lors de l&#39;utilisation d&#39;un modèle d&#39;espace de travail comportent des champs supplémentaires.

## Création d’un type d’enregistrement de taxonomie

La création de types d’enregistrement de taxonomie est similaire à la création de types d’enregistrement.

Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).
