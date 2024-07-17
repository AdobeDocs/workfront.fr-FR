---
title: Créer des champs
description: Dans Adobe Workfront Planning, vous pouvez créer des champs personnalisés pour chaque type d’enregistrement. Vous pouvez ensuite associer le champ à des enregistrements Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '3384'
ht-degree: 82%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Create fields
description: In Adobe Workfront Planning, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with records.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# Créer des champs

{{planning-important-intro}}

Dans Adobe Workfront Planning, vous pouvez créer des champs personnalisés pour des types d’enregistrements. Vous pouvez ensuite associer les champs à des enregistrements Workfront Planning afin d’améliorer les informations d’enregistrement.

Vous devez créer des types d’enregistrements avant de pouvoir créer des champs à associer à ceux-ci. Pour plus d’informations, voir [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

Vous pouvez créer des champs de la manière suivante dans la planification Workfront :

* À partir de zéro
* En connectant des types d’enregistrements
* En important des types d’enregistrement à l’aide d’un fichier Excel ou CSV
* En créant un type d’enregistrement
* En créant un espace de travail à partir d’un modèle

Pour plus d’informations sur les champs de planification Workfront, voir [Présentation des champs](/help/quicksilver/planning/fields/fields-overview.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Accord Adobe Workfront</p></td>
   <td>
<p>Votre entreprise doit être inscrite à l’étape d’accès anticipé pour la planification Workfront </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Forfait Adobe Workfront</p></td>
   <td>
<p>N’importe quelle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licence Adobe Workfront</p></td>
   <td>
   <p>N’importe quelle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurations du niveau d’accès</p></td>
   <td> <p>Il n’existe pas de contrôle sur le niveau d’accès pour Adobe Planning.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Autorisations</p></td>
   <td> <p>Autorisations de gestion d’un espace de travail</a> </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’elles n’ont pas créés.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Votre administrateur ou administratrice Workfront ou de groupes doit ajouter la zone Planning dans votre modèle de disposition. Pour plus d’informations, voir <a href="/help/quicksilver/planning/access/access-overview.md">Vue d’ensemble des accès</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Créer des champs à partir de zéro {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

{{step1-to-planning}}

1. Cliquez sur l&#39;espace de travail pour lequel vous souhaitez créer des champs.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur la carte d’un type d’enregistrement.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue du tableau.

   >[!TIP]
   >
   >    Si aucun enregistrement ne s’affiche, il se peut que vous n’ayez encore aucun enregistrement ou qu’un filtre soit appliqué pour limiter ce que vous voyez à l’écran.

   Tous les champs existants associés au type d&#39;enregistrement s&#39;affichent dans les colonnes de la vue de tableau.

   >[!TIP]
   >
   >    Certains champs peuvent être masqués. Cliquez sur Champs et activez le bouton d’activation/désactivation des champs à afficher en tant que colonnes dans la vue Tableau.

1. Cliquez sur l’icône **+** dans le coin supérieur droit de la vue de tableau.

   Ou

   Pointez sur l’en-tête d’une colonne, cliquez sur la flèche pointant vers le bas située après le nom du champ, puis cliquez sur **Insérer à gauche** ou **Insérer à droite** pour ajouter le nouveau champ.
1. Dans l’onglet **Nouveau champ**, recherchez un type de champ dans la zone **Type de champ** ou sélectionnez parmi les types de champs suivants :

   * [Texte à une ligne](#single-line-text)
   * [Paragraphe](#paragraph)
   * [Sélection multiple](#multi-select)
   * [Sélection unique](#single-select)
   * [Date](#date)
   * [Nombre](#number)
   * [Pourcentage](#percentage)
   * [Devise](#currency)
   * [Case à cocher](#checkbox)
   * [Formule](#formula)
   * [Personnes](#people)
   * [Créé par](#created-by)
   * [Date de création](#created-date)
   * [Dernière modification par](#last-modified-by)
   * [Date de dernière modification](#last-modified-date)

   >[!IMPORTANT]
   >
   >    Une fois enregistré, vous ne pouvez pas modifier le type de champ du champ.

1. Poursuivez en ajoutant chaque champ, comme décrit dans les sections ci-dessous.

### Texte à une ligne {#single-line-text}

Les champs de texte à une ligne capturent des informations alphanumériques limitées. Vous pouvez, par exemple, capturer les informations du ou de la propriétaire, partie prenante, équipe ou entité organisationnelle dans un champ de texte à une ligne. Le contenu d’un champ de texte à une ligne peut contenir jusqu’à 250 caractères. <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Texte à une ligne**.

   ![](assets/single-line-text-field-type.png)

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom** : nom du type de champ, tel qu’il apparaît dans un tableau ou la page Détails de l’enregistrement. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez l’en-tête de colonne du champ dans un tableau.
1. Cliquez sur **Créer**.

   Le nouveau champ d&#39;une seule ligne est ajouté en colonne au type d&#39;enregistrement et ses valeurs peuvent être associées à des enregistrements.


### Paragraphe {#paragraph}

Les champs de paragraphe capturent des informations alphanumériques supplémentaires sur un enregistrement, semblables au champ Description.

>[!TIP]
>
>* Le contenu d’un champ de paragraphe peut contenir jusqu’à 1 000 caractères.
>
>* Vous pouvez utiliser la mise en forme Texte enrichi pour améliorer le contenu des champs de paragraphe lorsqu’ils s’affichent dans la vue du tableau ou la page Détails d’un enregistrement. Pour plus d’informations, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Paragraphe**.

   ![](assets/paragraph-field-type.png)


1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom** : nom du type de champ, tel qu’il apparaît dans un tableau ou la page Détails de l’enregistrement. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
1. Cliquez sur **Créer**.

   Le nouveau champ de paragraphe est ajouté en tant que colonne au type d’enregistrement et ses valeurs peuvent être associées à des enregistrements.


### Sélection multiple {#multi-select}

Vous pouvez utiliser un champ à sélection multiple pour capturer des informations supplémentaires dans n’importe quel format en sélectionnant plusieurs options dans un menu déroulant.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Sélection multiple**.

   ![](assets/multi-select-field-type.png)


1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom** : nom du type de champ, tel qu’il apparaît dans un tableau ou la page Détails de l’enregistrement. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Choix** : options disponibles pour sélection dans le menu déroulant après l’enregistrement du champ. Vous pouvez avoir des nombres et des lettres pour le nom de chaque choix.
1. Cliquez sur **Ajouter un choix** pour ajouter autant de choix que nécessaire. Le nombre de choix que vous pouvez ajouter à un champ à sélection multiple n’est pas limité.
1. (Facultatif) Faites glisser et déposez manuellement chaque choix dans l’ordre souhaité, ou sélectionnez l’option
   **Trier les choix dans l’ordre alphabétique** si vous souhaitez que les choix soient automatiquement répertoriés dans l’ordre alphabétique. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Facultatif) Pour supprimer un choix, cliquez sur l’icône **x** située à droite.
1. Cliquez sur l’échantillon de couleur à gauche d’un choix pour développer le sélecteur de couleur et personnaliser la couleur de chaque option.
1. Cliquez sur **Créer**.

   Le nouveau champ à sélection multiple est ajouté en tant que colonne au type d&#39;enregistrement et ses valeurs peuvent être associées à des enregistrements.

### Sélection unique {#single-select}

Les champs à sélection unique capturent des informations supplémentaires dans n’importe quel format en sélectionnant une option dans un menu déroulant.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Sélection unique**.

   ![](assets/single-select-field-type.png)


1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom** : nom du type de champ, tel qu’il apparaît dans un tableau ou la page Détails de l’enregistrement. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Choix** : options disponibles pour sélection dans le menu déroulant après l’enregistrement du champ. Vous pouvez avoir des nombres et des lettres pour le nom de chaque choix.

1. Cliquez sur **Ajouter un choix** pour ajouter autant de choix que nécessaire. Le nombre de choix que vous pouvez ajouter à un champ à sélection unique n’est pas limité.
1. (Facultatif) Faites glisser et déposez manuellement chaque choix dans l’ordre souhaité, ou sélectionnez l’option **Trier les choix dans l’ordre alphabétique** si vous souhaitez que les choix soient automatiquement répertoriés dans l’ordre alphabétique. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Facultatif) Pour supprimer un choix, cliquez sur l’icône **x** située à droite.
1. Cliquez sur l’échantillon de couleur à gauche d’un choix pour développer le sélecteur de couleur et personnaliser la couleur de chaque option.
1. Cliquez sur **Créer**.

   Le nouveau champ à sélection unique est ajouté en tant que colonne au type d&#39;enregistrement et ses valeurs peuvent être associées à des enregistrements.

### Date {#date}

Vous pouvez utiliser un champ date pour capturer des informations supplémentaires au format de date et d’heure.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Date**.

   ![](assets/date-field-type.png)


1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom**: nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Format de date** : type de format de date à afficher dans ce champ. <!--update this casing - submitted bug for it-->

     Sélectionnez l’un des formats suivants :
      * **Paramètre local** : correspond aux paramètre local de votre navigateur.
      * **Standard** : 05/16/2023
      * **Long** : 16 mai 2023
      * **Européen** : 16/05/2023
      * **ISO** : 2023-05-16
   * **Inclure un champ horaire** : sélectionnez cette option si vous souhaitez inclure un horodatage. Cette option est désélectionnée par défaut. <!--update this setting name - submitted bug for it to be changed-->

     Sélectionnez l’une des options suivantes :

      * **24 h** : par exemple : 18:00
      * **12 h** : par exemple : 6:00 PM

1. Cliquez sur **Créer**.

   Le nouveau champ date est ajouté en tant que colonne au type d&#39;enregistrement et ses valeurs peuvent être associées à des enregistrements.

### Nombre {#number}

Les types de champs Nombre capturent des informations au format numérique.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Nombre**.

   ![](assets/number-field-type.png)
1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :

   * **Nom** : nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement.
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Précision** : nombre de décimales que vous souhaitez enregistrer pour le champ. Vous pouvez afficher jusqu’à 6 décimales.
   * **Autoriser les nombres négatifs** : sélectionnez cette option si vous souhaitez autoriser les nombres négatifs dans ce champ. Cette option est désélectionnée par défaut.

   >[!NOTE]
   >
   >    Si vous sélectionnez Autoriser les nombres négatifs et que les valeurs négatives sont stockées sur les enregistrements auxquels le champ est associé, vous ne pouvez plus désélectionner ce paramètre à l’avenir.

1. Cliquez sur **Créer**.

   Le nouveau champ numérique est ajouté en tant que colonne au type d&#39;enregistrement et ses valeurs peuvent être associées à des enregistrements.

### Pourcentage {#percentage}

Les types de champs Pourcentage capturent des informations au format numérique, suivies d’un signe de pourcentage.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Pourcentage**.

   ![](assets/percentage-field-type.png)

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom** : nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement.
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Précision** : nombre de décimales que vous souhaitez enregistrer pour le champ. Vous pouvez afficher jusqu’à 6 décimales.
   * **Autoriser les nombres négatifs** : sélectionnez cette option si vous souhaitez autoriser les valeurs en pourcentage négatives dans ce champ. Cette option est désélectionnée par défaut.

   >[!NOTE]
   >
   >    Si vous sélectionnez Autoriser les nombres négatifs et que les valeurs négatives sont stockées sur les enregistrements auxquels le champ est associé, vous ne pouvez plus désélectionner ce paramètre à l’avenir.

1. Cliquez sur **Créer**.

   Le nouveau champ de pourcentage est ajouté en tant que colonne au type d&#39;enregistrement et ses valeurs peuvent être associées à des enregistrements.

### Devise {#currency}

Les types de champs Devise capturent des informations au format numérique, précédées d’un symbole de devise.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Devise**.

   ![](assets/currency-field-type.png)

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom**: nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Devise** : type de devise que vous souhaitez afficher dans ce champ. Il s’agit d’une liste de devises selon l’Organisation internationale de normalisation (ISO).
   * **Précision** : nombre de décimales que vous souhaitez enregistrer pour le champ. Vous pouvez afficher jusqu’à 6 décimales.
   * **Autoriser les nombres négatifs** : sélectionnez cette option si vous souhaitez autoriser les valeurs de devise négatives dans ce champ. Cette option est désélectionnée par défaut.

   >[!NOTE]
   >
   >    Si vous sélectionnez Autoriser les nombres négatifs et que les valeurs négatives sont stockées sur les enregistrements auxquels le champ est associé, vous ne pouvez plus désélectionner ce paramètre à l’avenir.

1. Cliquez sur **Créer**.

   Le nouveau champ de devise est ajouté en tant que colonne au type d’enregistrement et ses valeurs peuvent être associées à des enregistrements.

### Case à cocher

Vous pouvez utiliser le type de champ Case à cocher pour ajouter une option à case à cocher unique à un enregistrement. Vous pouvez utiliser ce champ pour indiquer un attribut ou un statut spécifique pour cet enregistrement. Par exemple, vous pouvez l’utiliser en tant qu’indicateur pour le suivi de l’achèvement, de l’approbation ou de tout autre attribut binaire pour chaque enregistrement.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Case à cocher**.

   ![](assets/checkbox-field-type.png)

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom**: nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
1. Cliquez sur **Créer**.

   Le nouveau champ de case à cocher est ajouté en tant que colonne au type d’enregistrement et ses valeurs peuvent être associées à des enregistrements.

### Formule

Les champs Formule génèrent une nouvelle valeur en utilisant les valeurs existantes d’autres champs d’un type d’enregistrement et une fonction qui indique comment les valeurs existantes doivent être calculées.

Pour plus d’informations, voir [Vue d’ensemble des champs Formule](/help/quicksilver/planning/fields/formula-fields.md).

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Formule**.

   ![](assets/new-formula-field-with-list-of-expressions.png)

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :

   * **Nom** : saisissez un nom pour le nouveau champ.
   * **Description** : ajoutez des informations sur le nouveau champ.
   * **Formule** : commencez à saisir au moins un caractère pour accéder à une expression, puis sélectionnez-la lorsqu’elle s’affiche dans la liste.

1. Cliquez sur l’expression sélectionnée pour montrer la définition et afficher sa mise en forme.

   ![](assets/description-of-formula-expression.png)

   Pour plus d’informations sur les expressions prises en charge, voir [Présentation des champs de formule](/help/quicksilver/planning/fields/formula-fields.md).

1. Ajoutez les noms des champs tels qu’ils s’affichent dans la Planification Workfront pour les référencer dans une formule.

   >[!NOTE]
   >
   >* Vous ne pouvez pas ajouter de champs de type multi-sélection dans une formule.
   >
   >* Vous pouvez référencer un champ situé à 4 niveaux au maximum du type d’enregistrement actif. Par exemple, si vous créez un champ de formule pour un type d’enregistrement Activité et que l’activité est connectée au type d’enregistrement Produit connecté au type d’enregistrement Campagne connecté à un projet Workfront, vous pouvez référencer le budget du projet dans la formule que vous créez pour le type d’enregistrement Activité .

1. Cliquez sur **Créer**.

   Le nouveau champ de formule est ajouté en tant que colonne au type d&#39;enregistrement et ses valeurs peuvent être associées à des enregistrements.


### Personnes

Vous pouvez utiliser le type de champ Personnes pour ajouter une <!--, job role, or team--> d’un utilisateur ou d’une utilisatrice à un enregistrement. Il s’agit d’un champ de type anticipé, et vous pouvez ajouter uniquement les utilisateurs<!--, roles, or teams--> qui existent déjà dans votre instance Workfront.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Personnes**.

   ![](assets/people-field-type.png)

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :
   * **Nom** : nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement.
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Autoriser plusieurs valeurs** : sélectionnez cette option si vous souhaitez permettre aux utilisateurs et utilisatrices d’ajouter plusieurs personnes dans ce champ. Cette option est désélectionnée par défaut.

   >[!NOTE]
   >
   >    Si vous sélectionnez Autoriser plusieurs valeurs et que plusieurs personnes sont stockées dans les enregistrements auxquels le champ est associé, vous ne pouvez plus désélectionner le paramètre à l’avenir lors de la modification de ce champ.

1. Cliquez sur **Créer**.

   Le nouveau champ Type de personne est ajouté en tant que colonne au type d’enregistrement et ses valeurs peuvent être associées à des enregistrements.

### Créé par

Vous pouvez utiliser le type de champ Créé par pour ajouter à un enregistrement la personne qui a créé l’enregistrement. Il s’agit d’un champ en lecture seule qui s’affiche automatiquement avec le nom de la personne connectée lors de la création de l’enregistrement.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Créé par**.

   ![](assets/created-by-field-type.png)

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :

   * **Nom**: nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement. <!--this might change and they might prepopulate it with "Created by"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.

1. Cliquez sur **Créer**.

   Le nouveau champ « Créé par » est ajouté en tant que colonne au type d’enregistrement et ses valeurs sont préremplies avec le nom de la personne qui a créé chaque enregistrement.


### Date de création

Vous pouvez utiliser le type de champ Date de création pour ajouter à un enregistrement la date à laquelle l’enregistrement a été créé. Il s’agit d’un champ en lecture seule qui est automatiquement renseigné avec la date (et éventuellement l’heure) de création de l’enregistrement.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Date de création**.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :

   * **Nom**: nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement. <!--this might change and they might prepopulate it with "Created date"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Format de date** : sélectionnez l’un des formats suivants :

      * **Paramètres régionaux** : correspond aux paramètres régionaux de votre navigateur.
      * **Standard** : 05/16/2023
      * **Long** : 16 mai 2023
      * **Européen** : 16/05/2023
      * **ISO** : 2023-05-16
   * **Inclure un champ horaire** : sélectionnez cette option si vous souhaitez inclure un horodatage. Cette option est désélectionnée par défaut. <!--submitted a UI text change for this - check the UI-->

     Sélectionnez l’une des options suivantes :

      * **24 h** : par exemple : 18:00
      * **12 h** : par exemple : 6:00 PM

1. Cliquez sur **Créer**.

   Le nouveau champ de type Date de création est ajouté en tant que colonne au type d’enregistrement et ses valeurs sont préremplies avec la date (ou la date et l’heure) de création de l’enregistrement.


### Dernière modification par

Vous pouvez utiliser le type de champ Dernière modification par pour ajouter à un enregistrement la personne qui a modifié l’enregistrement pour la dernière fois. Il s’agit d’un champ en lecture seule qui s’affiche automatiquement avec le nom de la personne connectée lors de la dernière mise à jour de l’enregistrement.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Dernière modification par**.

   ![](assets/last-modified-by-field-type.png)

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :

   * **Nom**: nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement. <!--this might change and they might prepopulate it with "Created by"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.

1. Cliquez sur **Créer**.

   Le nouveau champ de type Dernière modification par est ajouté en tant que colonne au type d’enregistrement et ses valeurs sont préremplies avec le nom de la personne qui a modifié chaque enregistrement pour la dernière fois.


### Date de dernière modification

Vous pouvez utiliser le type de champ Date de dernière modification pour ajouter à un enregistrement la date de dernière modification d’un enregistrement. Il s’agit d’un champ en lecture seule qui s’affiche automatiquement avec la date (et éventuellement l’heure) de la dernière modification de l’enregistrement.

1. Commencez à créer un champ comme décrit dans la section [Créer des champs à partir de zéro](#create-fields-from-scratch) de cet article, puis sélectionnez le type de champ **Date de création**.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Ajoutez les informations suivantes dans l’onglet **Nouveau champ** :

   * **Nom**: nom du type de champ, tel qu’il apparaît dans un tableau ou la page de l’enregistrement. <!--this might change and they might prepopulate it with "Created date"-->
   * **Description** : informations complémentaires sur le champ. La description d’un champ s’affiche lorsque vous survolez la colonne du champ dans un tableau.
   * **Format de date** : sélectionnez l’un des formats suivants :

      * **Paramètres régionaux** : correspond aux paramètres régionaux de votre navigateur.
      * **Standard** : 05/16/2023
      * **Long** : 16 mai 2023
      * **Européen** : 16/05/2023
      * **ISO** : 2023-05-16
   * **Inclure un champ horaire** : sélectionnez cette option si vous souhaitez inclure un horodatage. Cette option est désélectionnée par défaut. <!--submitted a UI text change for this - check the UI-->

     Sélectionnez l’une des options suivantes :

      * **24 h** : par exemple : 18:00
      * **12 h** : par exemple : 6:00 PM

1. Cliquez sur **Créer**.

   Le nouveau champ de type Date de dernière modification est ajouté en tant que colonne au type d’enregistrement et ses valeurs sont préremplies avec la date (ou la date et l’heure) de la dernière modification de l’enregistrement.

## Créer des champs en connectant des types d’enregistrement

Vous pouvez créer des champs d’enregistrement liés lorsque vous ajoutez une nouvelle connexion entre deux types d’enregistrement ou un type d’enregistrement et des types d’objet à partir d’autres applications.

Pour plus d’informations sur la connexion des types d’enregistrement Workfront Planning, consultez la section [Connecter des types d’enregistrement](/help/quicksilver/planning/architecture/connect-record-types.md).

## Créer des champs en important des types d’enregistrement à l’aide d’un fichier Excel ou CSV

Pour plus d’informations, consultez la section [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

## Créer des champs en créant un type d’enregistrement

Lorsque vous créez un type d’enregistrement, plusieurs champs associés au nouveau type d’enregistrement sont également créés par défaut. Pour plus d’informations, consultez la section [Créer des types d’enregistrements](/help/quicksilver/planning/architecture/create-record-types.md).

## Créer des champs en créant un espace de travail à partir d’un modèle

Adobe Workfront Planning crée des champs pour les types d’enregistrement lorsque vous créez un espace de travail à partir d’un modèle.

Pour plus d’informations, consultez la section [Créer des espaces de travail](/help/quicksilver/planning/architecture/create-workspaces.md).