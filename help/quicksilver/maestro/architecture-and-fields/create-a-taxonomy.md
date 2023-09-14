---
title: Création de types d’enregistrement de taxonomie
description: Les taxonomies sont un type de types d'enregistrements réutilisables qui capture les attributs d'un type d'enregistrement opérationnel dans Adobe Workfront Maestro.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Création de types d’enregistrement de taxonomie

>[!IMPORTANT]
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Les taxonomies sont des types d&#39;enregistrements qui capturent des attributs sur les types d&#39;enregistrements opérationnels dans Adobe Maestro.

Par exemple, Campaign peut être un type d’enregistrement opérationnel. Vous trouverez ci-dessous des taxonomies qui capturent des attributs sur le type d’enregistrement Campaign : Région, Audience, Pays.

Pour plus d’informations sur les types d’enregistrement Maestro, voir [Présentation des types d’enregistrement et des taxonomies](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
<td>
   <p> Adobe de produit</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite au programme bêta fermé Adobe Maestro. Contactez le représentant de votre compte pour en savoir plus sur cette nouvelle offre. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Formule Adobe Workfront</p></td>
   <td>
<p>Tous</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>Tous</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Niveau d’accès</td>
   <td> <p>Tous</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Modèle de mise en page</td>
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/grant-access.md">Accorder l’accès à Adobe Maestro</a>. </p>  
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

* Vous devez créer un espace de travail avant de pouvoir créer des taxonomies dans l’espace de travail.

  Pour plus d’informations sur les espaces de travail, voir [Créer des espaces de travail](../architecture-and-fields/create-workspaces.md).
* Vous pouvez créer un type d’enregistrement de taxonomie en effectuant l’une des opérations suivantes :
   * Créez-les automatiquement lorsque vous créez un espace de travail à l’aide d’un modèle. Pour plus d’informations, voir [Créer des espaces de travail](../architecture-and-fields/create-workspaces.md).
   * Créez-les manuellement, à partir de zéro.
   * Créez-les manuellement en collant des informations à partir d’une liste externe.

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* Toutes les taxonomies nouvellement créées sont fournies avec les champs suivants :

   * Nom <!--if there won't be any more fields, consider rephrasing this-->

  De plus, vous pouvez ajouter des champs personnalisés aux taxonomies. Pour plus d’informations, voir [Créer des champs](../architecture-and-fields/create-fields.md).

  >[!NOTE]
  >
  >    Les taxonomies créées lors de l&#39;utilisation d&#39;un modèle d&#39;espace de travail comportent des champs supplémentaires.

## Création d’une taxonomie

La création de taxonomies est similaire à la création d&#39;un type d&#39;enregistrement opérationnel à partir de zéro ou d&#39;un modèle d&#39;espace de travail.

Pour plus d’informations, reportez-vous à la section &quot;Création d’un type d’enregistrement à partir de zéro&quot; dans l’article . [Création de types d’enregistrement](../architecture-and-fields/create-record-types.md).

Pour plus d’informations sur la création automatique de taxonomies lors de la création d’un espace de travail à partir d’un modèle, voir [Créer des espaces de travail](../architecture-and-fields/create-workspaces.md).
