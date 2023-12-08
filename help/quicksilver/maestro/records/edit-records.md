---
title: Modifier des enregistrements
description: Vous pouvez modifier les informations d’enregistrement dans Adobe Maestro. Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 3e1e651662f9ff695d475ffcbdc77f0802d108f1
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Modifier des enregistrements

>[!IMPORTANT]
>
>Les informations de cet article se rapportent à Adobe Maestro, une nouvelle offre d’Adobe Workfront.
>
>Actuellement, Adobe Maestro fait partie d’un programme bêta ouvert à un nombre limité de clients. Vous devez être un client Workfront pour utiliser les fonctionnalités de Maestro.
>
>Pour plus d’informations sur l’inscription au programme bêta de Maestro, contactez le représentant de votre compte.
>
>Pour plus d’informations, voir [Présentation d’Adobe Maestro](../maestro-overview.md).

Vous pouvez modifier les informations d’enregistrement dans Adobe Maestro. Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

&lt;!— mentionnez ici que les champs de la vue Détails sont identiques à ceux de la vue Tableau — cet article est lié à la vue Gestion des enregistrements pour faire référence à ces informations—>

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 <tbody>
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
   <td role="rowheader">Niveau d’accès</td>
   <td> <p>Quelconque</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modèle de mise en page</td>
   <td> <p>L’administrateur système doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/grant-access.md">Accorder l’accès à Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Remarques concernant la modification d’enregistrements

* Vous pouvez modifier les enregistrements que vous ou un autre utilisateur avez créés. <!--will change with access levels-->
* Vous ne pouvez pas modifier les champs liés à d’autres enregistrements ou champs contenant des calculs.
* Si les enregistrements que vous affichez sont liés à d&#39;autres enregistrements, les nouvelles informations des enregistrements que vous éditez se répercutent sur les enregistrements liés.
* Vous ne pouvez pas modifier les enregistrements en masse. <!--this will probably change-->
* Les URL sont reconnues comme des liens dans les types de champ de texte sur une seule ligne uniquement lorsqu’elles commencent par les éléments suivants : http://, https://, ftp:// ou www. .
* Vous pouvez utiliser les options de mise en forme de texte enrichi suivantes lors de la modification d’un champ de type Paragraphe :

   * Gras
   * Italiques
   * Souligner
   * Ajouter un lien
   * Ajouter une liste à puces
   * Ajouter une liste numérotée

## Modifier des enregistrements

Vous pouvez modifier un enregistrement à partir des zones suivantes :

* [Sur la page Détails d’un enregistrement](#edit-a-record-from-the-records-details-page)
* [En mode Tableau d’un type d’enregistrement](#edit-a-record-from-the-record-type-table-view)

### Modifier un enregistrement à partir de la page Détails de l’enregistrement

1. Cliquez sur le bouton **Menu Principal** ![](assets/main-menu-workfront.png) dans le coin supérieur droit, ou le **Menu Principal** ![](assets/main-menu-shell.png) dans le coin supérieur gauche, le cas échéant, cliquez sur **Maestro**.

   L’espace de travail auquel vous accédez en dernier s’ouvre.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas située à droite du nom de l’espace de travail pour sélectionner l’espace de travail dont vous souhaitez mettre à jour les enregistrements.
1. Utilisez l’une des méthodes suivantes :

   * Dans une vue Tableau, cliquez sur le nom d’un enregistrement.
   * Dans la vue Tableau, passez la souris sur le nom d’un enregistrement, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Affichage**

     ![](assets/contextual-menu-for-record-row.png)
   * Dans la vue Chronologie, cliquez sur une barre d’enregistrement.

   L&#39;enregistrement **Détails** s’ouvre.

1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez sur **Modifier**

   Ou

   Cliquez dans n’importe quel champ modifiable de la page Détails pour modifier les informations.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Cliquez sur **Enregistrer les modifications**. <!--logged a bug for this - this needs to be "Save"-->

### Modification d’un enregistrement depuis la vue table d’un type d’enregistrement

1. Cliquez sur le bouton **Menu Principal** ![](assets/main-menu-workfront.png) dans le coin supérieur droit, ou le **Menu Principal** ![](assets/main-menu-shell.png) dans le coin supérieur gauche, le cas échéant, cliquez sur **Maestro** ![](assets/maestro-icon.png).

   L’espace de travail auquel vous avez accédé la dernière fois s’ouvre.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas située à droite du nom de l’espace de travail pour sélectionner l’espace de travail dont vous souhaitez mettre à jour les enregistrements.
1. Cliquez sur une carte de type enregistrement.

   La page de type enregistrement s’ouvre.
1. (Conditionnel) Dans la variable **Affichage** sélectionnez un menu déroulant dans le coin supérieur droit du tableau **Tableau** vue. Il doit s’agir de la vue par défaut, sauf si vous avez visualisé le type d’enregistrement dans la vue chronologique lors de votre dernier accès.

   Les enregistrements associés au type d&#39;enregistrement sélectionné s&#39;affichent dans la vue Tableau.
1. Cliquez dans la ligne d’un enregistrement pour commencer à modifier les informations sur l’enregistrement intégré.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Presse **Entrée** sur votre clavier ou cliquez en dehors d’une ligne pour enregistrer vos modifications. Les modifications sont enregistrées automatiquement. Un indicateur Enregistré s’affiche brièvement dans le coin supérieur droit du tableau pour indiquer que les modifications ont été enregistrées.

   >[!NOTE]
   >
   >  Vous ne pouvez pas modifier les informations des champs suivants, car ils sont en lecture seule et Workfront les met automatiquement à jour :
   >  
   >  * Champs liés créés par la connexion des types d’enregistrement. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).
   >  * Champs des types suivants : Créé par, Date de création, Dernière modification par, Date de dernière modification .


1. (Facultatif) Copiez une ou plusieurs valeurs existantes d’un champ, collez-les dans un champ du même type sur un autre enregistrement, puis cliquez sur **Entrée** sur votre clavier pour enregistrer vos modifications.

   >[!NOTE]
   >
   >Tenez compte des points suivants :
   >
   >* Vous ne pouvez pas copier des informations provenant d’une autre source, autre qu’un champ Maestro du même type que le champ dans lequel vous collez les informations.
   >
   >* Vous ne pouvez pas copier et coller de valeurs de champ dans la zone Détails d’un enregistrement. Cette fonctionnalité n’est prise en charge que dans le mode Tableau d’un type d’enregistrement.
   >* Vous ne pouvez pas copier et coller des valeurs de champ pour les types de champ suivants :
   >
   >
   >    * Champs liés créés par la connexion des types d’enregistrement. Vous pouvez copier et coller des champs d’enregistrement liés. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).
   >    * Champs des types suivants : Créé par, Date de création, Dernière modification par, Date de dernière modification .


   <!--take People out of the list above when they release this - this might be coming later-->
