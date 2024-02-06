---
title: Modifier des enregistrements
description: Vous pouvez modifier les informations d’enregistrement dans Adobe Maestro. Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 08a7fa1f3871494c4c6b0c385a98a64735b7f7e4
workflow-type: tm+mt
source-wordcount: '1056'
ht-degree: 1%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Modifier des enregistrements

{{maestro-important-intro}}

Vous pouvez modifier les informations d’enregistrement dans Adobe Manager en modifiant les valeurs des champs associés aux enregistrements.

Vous devez créer des types d’enregistrement avant de pouvoir commencer à créer et modifier des enregistrements.

Pour plus d’informations, voir [Création de types d’enregistrement](../architecture/create-record-types.md).

Pour plus d’informations sur la création d’enregistrements, voir [Créer des enregistrements](/help/quicksilver/maestro/records/create-records.md).

&lt;!— mentionnez ici que les champs de la vue Détails sont identiques à ceux de la vue Tableau — cet article est lié à la vue Gestion des enregistrements pour faire référence à ces informations—>

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
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td>
   <td>
   <p>Nouveau : clair ou supérieur</p>
   Ou
   <p>Actuel : travail ou plus élevé</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Paramétrages du niveau d'accès</p></td>
   <td> <p>Il n’existe aucun contrôle d’accès pour Maestro </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Attribution ou autorisations supérieures à un espace de travail</a> </p>  
   <p>Les administrateurs système disposent d’autorisations pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>L’administrateur de Workfront ou de groupe doit ajouter la zone Maestro à votre modèle de mise en page. Pour plus d’informations, voir <a href="../access/access-overview.md">Présentation de l’accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Remarques concernant la modification d’enregistrements

* Vous pouvez modifier les enregistrements que vous avez créés ou créés par d’autres utilisateurs, si des autorisations vous ont été accordées à l’espace de travail.
* Vous pouvez modifier les champs d’enregistrement à partir de la page Détails d’un enregistrement ou de la vue tabulaire d’un type d’enregistrement.
* Vous ne pouvez pas modifier les informations d’enregistrement dans la vue de la chronologie.
* Les types de champs suivants sont automatiquement mis à jour et vous ne pouvez pas modifier leurs valeurs manuellement :
   * Champs liés à partir d’autres enregistrements
   * Champs de type Formule
   * Champs système (Créé par, Date de création, Dernière modification par, Date de dernière modification)
* Si les enregistrements que vous affichez sont liés à d&#39;autres enregistrements, les nouvelles informations des enregistrements que vous éditez se répercutent sur les enregistrements liés.
* Vous ne pouvez pas modifier les enregistrements en masse. <!--this will probably change-->
* Les URL sont reconnues comme des liens dans les types de champ de texte sur une seule ligne uniquement lorsqu’elles commencent par les éléments suivants : http://, https://, ftp:// ou www. .

## Modifier des enregistrements

Vous pouvez modifier un enregistrement à partir des zones suivantes :

* [Sur la page Détails d’un enregistrement](#edit-a-record-from-the-records-details-page)
* [En mode Tableau d’un type d’enregistrement](#edit-a-record-from-the-table-view-of-a-record-type)

### Modifier un enregistrement à partir de la page Détails de l’enregistrement

{{step1-to-maestro}}

L’espace de travail auquel vous accédez en dernier s’ouvre.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas située à droite du nom de l’espace de travail pour sélectionner l’espace de travail dont vous souhaitez mettre à jour les enregistrements.
1. Utilisez l’une des méthodes suivantes :

   * Depuis un **Tableau** cliquez sur le nom d’un enregistrement.
   * Dans la **Tableau** visionnez, survolez le nom d’un enregistrement avec la souris, puis cliquez sur le bouton **Plus** menu ![](assets/more-menu.png), puis cliquez sur **Affichage**

     ![](assets/contextual-menu-for-record-row.png)
   * Dans la vue Chronologie, cliquez sur une barre d’enregistrement.

   L&#39;enregistrement **Détails** s’ouvre.

1. Cliquez sur le bouton **Plus** menu ![](assets/more-menu.png) à droite du nom de l’enregistrement, puis cliquez sur **Modifier**

   Ou

   Cliquez dans n’importe quel champ modifiable de la page Détails pour modifier les informations.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Cliquez sur **Enregistrer les modifications**. <!--logged a bug for this - this needs to be "Save"-->

### Modification d’un enregistrement depuis la vue table d’un type d’enregistrement

{#step1-to-maestro}

L’espace de travail auquel vous avez accédé la dernière fois s’ouvre.

1. (Facultatif) Cliquez sur la flèche pointant vers le bas située à droite du nom de l’espace de travail pour sélectionner l’espace de travail dont vous souhaitez mettre à jour les enregistrements.
1. Cliquez sur une carte de type enregistrement.

   La page de type enregistrement s’ouvre.
1. (Conditionnel) Dans la variable **Affichage** sélectionnez un menu déroulant dans le coin supérieur droit du tableau **Tableau** vue. Il doit s’agir de la vue par défaut, sauf si vous avez visualisé le type d’enregistrement dans la vue chronologique lors de votre dernier accès.

   Les enregistrements associés au type d&#39;enregistrement sélectionné s&#39;affichent dans la vue Tableau.
1. Cliquez dans la ligne d’un enregistrement pour commencer à modifier les informations sur l’enregistrement intégré.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!NOTE]
   >
   >  Vous ne pouvez pas modifier les informations des champs suivants, car ils sont en lecture seule et Workfront les met automatiquement à jour :
   >  
   >  * Champs liés créés par la connexion des types d’enregistrement. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).
   >  * Champs des types suivants : Créé par, Date de création, Dernière modification par, Date de dernière modification .

1. (Facultatif et conditionnel) Lorsque vous modifiez un champ de type Paragraphe, utilisez ce qui suit : **Texte enrichi** options de formatage :

   * Gras
   * Italiques
   * Souligner
   * Ajouter un lien
   * Ajouter une liste à puces
   * Ajouter une liste numérotée

   ![](assets/rich-text-toolbar-on-paragraph-field.png)
1. Presse **Entrée** sur votre clavier ou cliquez en dehors d’une ligne pour enregistrer vos modifications. Les modifications sont enregistrées automatiquement. A **Enregistré** s’affiche brièvement dans le coin supérieur droit de la vue du tableau pour indiquer que les modifications ont été enregistrées.

1. (Facultatif) Pour copier et coller des informations d’un champ vers un autre, effectuez l’une des opérations suivantes :

   * Copiez une ou plusieurs valeurs existantes d’un champ, puis collez-les dans un champ du même type sur un autre enregistrement
   * Cliquez sur l’en-tête de colonne d’une colonne pour la sélectionner et la copier, puis cliquez sur l’en-tête de colonne d’une autre colonne et collez le contenu de la colonne copiée. Les colonnes doivent contenir des types de champ similaires.
   * Lorsque vous appuyez sur la touche Maj, cliquez pour sélectionner plusieurs lignes d’un tableau, copiez les informations des lignes sélectionnées, puis cliquez sur une autre ligne et collez les informations sélectionnées dans la nouvelle ligne, puis sur les lignes suivantes.

   >[!NOTE]
   >
   >Tenez compte des points suivants :
   >
   >* Utilisez les raccourcis clavier suivants pour copier et coller des informations :
   >   * Copier : Ctrl + C (⌘ + C pour Mac)
   >   * Coller : Ctrl + V ( ⌘ + V pour Mac)
   >* Vous ne pouvez pas copier des informations provenant d’une autre source, autre qu’un champ Maestro du même type que le champ dans lequel vous collez les informations.
   >
   >* Vous ne pouvez pas copier et coller de valeurs de champ dans la zone Détails d’un enregistrement. Cette fonctionnalité n’est prise en charge que dans le mode Tableau d’un type d’enregistrement.
   >* Vous ne pouvez pas copier et coller des valeurs de champ pour les types de champ suivants :
   >
   >
   >    * Champs liés créés par la connexion des types d’enregistrement. Vous pouvez copier et coller des champs d’enregistrement liés. Pour plus d’informations, voir [Connexion des types d’enregistrement](../architecture/connect-record-types.md).
   >    * Champs des types suivants : Créé par, Date de création, Dernière modification par, Date de dernière modification .

1. (Facultatif) Utilisez les raccourcis clavier suivants pour annuler ou rétablir la modification ou la copie et le collage des informations d’enregistrement :

   * Ctrl + Z (⌘ + Z pour Mac) pour annuler une modification.
   * Ctrl + Maj + Z (⌘ + Maj + Z pour Mac) pour rétablir la modification

   >[!TIP]
   >
   >    Vous pouvez utiliser les raccourcis clavier plusieurs fois de suite pour annuler plusieurs modifications.

1. (Facultatif) Ajoutez une miniature à un enregistrement. Pour plus d’informations, voir [Ajout d’une miniature à un enregistrement](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).
