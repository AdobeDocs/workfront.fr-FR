---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: 'Scénario de Kickstart : importation de champs personnalisés à options multiples dans Workfront'
description: Vous pouvez importer des champs personnalisés avec plusieurs options dans Adobe Workfront à l’aide de la fonctionnalité de lancement.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 70f3dac7-f449-4dc8-9d7d-a5284b37f9ec
source-git-commit: aa2bef064df3ff7dd9e4fd896ac7482df3c55e32
workflow-type: tm+mt
source-wordcount: '2163'
ht-degree: 88%

---

# Scénario de lancement : importer des champs personnalisés à plusieurs options dans Workfront

Vous pouvez importer des champs personnalisés avec plusieurs options dans Adobe Workfront à l’aide de la fonctionnalité de lancement.

Exemples de champs personnalisés avec plusieurs options :

* Menu déroulant multi-sélection
* Menu déroulant
* Cases à cocher
* Cases d’option

Ces champs peuvent parfois comporter de nombreuses options (parfois des centaines). Les importer à l’aide de la fonctionnalité de lancement peut vous faire gagner beaucoup de temps, en tant qu’administrateur ou administratrice Workfront, et vous permettre d’éviter les erreurs.

>[!IMPORTANT]
>
>Vous devez suivre les étapes décrites dans les sections ci-dessous, dans cet ordre, pour importer des champs personnalisés avec plusieurs options à l’aide d’un lancement :
>
>1. Exporter des données personnalisées existantes à partir de Workfront (étape facultative)
>1. Exporter le modèle de lancement pour les données personnalisées
>1. Renseigner la feuille de calcul Excel de lancement
>1. Charger la feuille de calcul Excel vers Workfront

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p> Nouveau : Standard</p>
   ou
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exporter des données personnalisées existantes à partir de Workfront (étape facultative)

Si vous ne connaissez pas la structure de la base de données Workfront ou si vous ne connaissez pas le fichier de lancement requis par Workfront pour importer des informations d’import, nous vous recommandons d’exporter d’abord un fichier de lancement à partir de Workfront avec des informations existantes, semblables à celles des champs que vous souhaitez importer.

Par exemple, si vous souhaitez importer des formulaires personnalisés ou des champs personnalisés, vous devez d’abord exporter un fichier de lancement avec des données personnalisées existantes.

L’export initial de vos données existantes vous permet de les analyser et de voir comment vos nouvelles données doivent être formatées.

Si vous maîtrisez bien les objets et la structure de la base de données Workfront, vous pouvez continuer avec la section ci-dessous.

Pour exporter des données existantes à partir de Workfront :

{{step-1-to-setup}}

1. Développez **Système** dans le menu de gauche, puis cliquez sur **Exporter les données (Kick-Starts)**.

1. Sélectionnez **Données personnalisées** dans la section **Éléments à inclure**.

   ![Sélectionner les données personnalisées](assets/kickstarts-select-existing-data.png)

1. Choisissez **fichier .xlsx** dans la section **Format de téléchargement**.

   >[!TIP]
   >
   >Selon le volume de données personnalisées de votre système, cette opération peut prendre un certain temps.

1. Cliquez sur **Télécharger**. Un fichier .xlsx est téléchargé sur votre ordinateur. Accédez-y et ouvrez-la.

   ![Données exportées dans Excel](assets/existing-data-excel-parameter-sheet.png)

1. Examinez le fichier téléchargé et notez les détails suivants :

   * Le fichier contient plusieurs feuilles. Vous n’aurez peut-être pas besoin de connaître les informations contenues dans chaque feuille, mais vous utiliserez certaines feuilles pour importer vos informations. Prenez le temps de vous familiariser avec leur contenu, et en particulier avec le format du contenu dans chaque feuille.
   * Accordez une attention particulière aux noms des colonnes et au format d’affichage des données de chaque colonne.
   * Vous ne devez pas modifier les noms ou l’ordre des colonnes dans aucune des feuilles. Les en-têtes de colonne indiquent les champs que vous devez remplir avec vos informations, dans chaque ligne. Si l’en-tête de colonne s’affiche en gras, il s’agit d’un champ obligatoire. Vous devez donc y inclure des informations.

   >[!IMPORTANT]
   >
   >Certains en-têtes de colonne peuvent ne pas s’afficher en gras, mais ils peuvent toujours être obligatoires.

   * Conservez le fichier téléchargé à des fins de référence ultérieure et passez à la section suivante.

## Exporter le modèle de lancement pour les données personnalisées

Après avoir analysé les informations sur les champs personnalisés existants de votre système, vous pouvez télécharger un nouveau modèle de lancement pour votre import.

{{step-1-to-setup}}

1. Développez **Système** dans le menu de gauche.

1. Cliquez sur **Importer des données (lancement)**.

1. Dans la zone **Télécharger une feuille de calcul Kickstart vierge**, cochez la case **Données personnalisées**, puis cliquez sur **Télécharger**.

   ![Sélectionner les données personnalisées](assets/kickstarts-blank-spreadsheet-options.png)

   Un fichier de lancement vierge est téléchargé sur votre ordinateur.

   >[!NOTE]
   >
   >Le nombre de feuilles dans le fichier, leur nom, ainsi que le nombre et le nom des colonnes de chaque feuille doivent être identiques à ceux du lancement téléchargé dans la section ci-dessus, qui contenait vos données personnalisées existantes.

## Renseigner la feuille de calcul Excel de lancement

Avant de remplir la feuille de calcul Excel, téléchargez le modèle Kickstart comme décrit dans la section ci-dessus.

>[!IMPORTANT]
>
>N’essayez pas d’importer des informations à l’aide d’une feuille de calcul Excel ad hoc. Toutes les feuilles de calcul pour importer des informations dans Workfront à l’aide de la fonctionnalité de lancement doivent correspondre au contenu des fichiers que vous téléchargez à partir de Workfront et décrits dans cet article.

Pour remplir la feuille de calcul Excel avec des informations sur les nouveaux champs personnalisés :

1. Ouvrez la feuille de calcul Excel que vous avez téléchargée à la section précédente, puis passez en revue les feuilles. Chaque feuille représente un objet dans l’application.

   Par exemple : **Paramètre** (qui fait référence à un champ personnalisé), **Option de paramètre**(qui fait référence à l’option Champ personnalisé), **Catégorie** (qui fait référence à un formulaire personnalisé).

   Vous devez écrire les noms des objets et leurs attributs au format pris en charge par la base de données Workfront.

   Pour plus d’informations sur la signification de ces objets, voir [Glossaire de la terminologie  [!DNL Adobe Workfront] &#x200B;](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   Pour plus d’informations sur les noms des objets dans la base de données Workfront, voir [Explorateur d’API](../../../wf-api/general/api-explorer.md).

   ![Feuilles incluses dans l&#39;export de données](assets/sheets-included-in-custom-data-export-kick-start-file.png)

1. Assurez-vous que les informations suivantes sont correctement formatées :

   * La première ligne de chaque feuille doit rester vide, sinon l’import génère une erreur.
   * Les en-têtes de colonne de chaque feuille représentent les attributs des objets qui peuvent être définis lors d’un import. Tous les en-têtes de colonne doivent rester dans l’ordre où ils se trouvent lorsque vous exportez la feuille. Ils ne peuvent pas être renommés.
   * Les en-têtes de colonne en gras sont des champs obligatoires qui doivent avoir une valeur.

     >[!TIP]
     >
     >Certaines colonnes sont obligatoires, bien qu’elles ne soient pas en gras. Par exemple, les colonnes `isNew` et `ID` ne sont pas en gras, mais il s’agit de champs obligatoires.

1. Sélectionnez la feuille `**PARAM Parameter`** et ajoutez des informations sur les nouveaux champs personnalisés dans les colonnes obligatoires suivantes :

   * **`isNew`** = saisissez **`TRUE`** dans cette colonne pour chaque ligne qui représente un nouveau champ personnalisé. Cela indique que le champ est nouveau et qu’il n’existe pas dans Workfront.

     >[!TIP]
     >
     >Si une ligne représente un champ existant déjà dans Workfront, vous devez saisir **`isNew`** = **`FALSE`**.

   * **`ID`** = doit être un nombre unique pour chaque ligne qui représente un nouveau champ. Vous pouvez utiliser n’importe quel nombre commençant par 1, à condition que chaque nouveau champ ait un numéro unique.
   * **`setDataType`** = pour chaque ligne représentant un nouveau champ, saisissez le type de données pris en charge par le champ. Le type de données doit être renseigné tel qu’il apparaîtrait dans la base de données. Sélectionnez l’un des types de données suivants :

      * **`NMBR`** pour un nombre
      * **`CURC`** pour une devise
      * **`TEXT`** pour du texte

   * `**setDisplaySize**`= la taille d’affichage (« **setDisplaySize** ») pour les champs personnalisés de plusieurs options est toujours 0.
   * **`setDisplayType`** = pour chaque ligne représentant un nouveau champ, saisissez le type d’affichage du champ. Le type d’affichage doit être renseigné tel qu’il apparaîtrait dans la base de données.

     Pour les champs personnalisés à plusieurs options, sélectionnez l’une des options suivantes :

      * **`MULT`** pour une liste déroulante à sélection multiple
      * **`SLCT`** pour une liste déroulante
      * **`RDIO`** pour des cases d’option
      * **`CHCK`** pour des cases à cocher

     >[!TIP]
     >
     >Pour connaître le type de données et le type d’affichage, reportez-vous à la section [Explorateur d’API](../../../wf-api/general/api-explorer.md), développez l’objet **Paramètre** et recherchez ces attributs sous l’onglet **champs**.

   * **`setName`** = saisissez le nom des champs personnalisés tel que vous souhaitez qu’il s’affiche dans Workfront.

     >[!INFO]
     >
     >Par exemple, nous pouvons importer deux champs personnalisés, appelés _Marque_, un champ de case à cocher et _Médias_, un champ de case d’option.

   * Les colonnes **`setName`** et **`setValue`** contiennent généralement les mêmes informations et doivent refléter les noms souhaités dans l’interface Workfront pour votre nouveau champ.

   La valeur d’un champ est le nom qui apparaît dans les rapports, par exemple, tandis que le nom s’affiche dans les formulaires personnalisés associés aux objets.

   Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   ![Feuille de paramètres remplie](assets/parameter-sheet-filled-out-kick-starts.png)

1. Sélectionnez la feuille **`POPT Parameter Options`** et ajoutez des informations sur les options de chaque champ personnalisé dans les colonnes obligatoires suivantes :

   * **`isNew`** = saisissez **`TRUE`** dans cette colonne pour chaque ligne qui représente une nouvelle option de champ.

     >[!TIP]
     >
     >    Si une ligne représente une option existante, vous devez saisir **`isNew`** = **`FALSE`**.

   * **`ID`** = doit être un nombre unique pour chaque ligne qui représente une nouvelle option. Vous pouvez utiliser n’importe quel nombre commençant par 1, à condition que chaque nouvelle option ait un numéro unique.
   * **`setIsDefault`** = saisissez `TRUE` pour les options que vous souhaitez afficher par défaut, et `FALSE` pour toutes les autres options, pour chaque champ.  Par exemple, nous voulons que _Nike_ soit l’option par défaut pour _Marque_ et _Impression_ l’option par défaut pour _Médias_.

     >[!TIP]
     >
     >Vous ne pouvez avoir qu’une seule option par défaut pour chaque champ.

   * **`setParameterID`** = les options correspondant au champ personnalisé _Marque_ comportent un **`setParameterID`** de 1 et les options correspondant au _Média_ ont un **`setParameterID`**&#x200B;de 2. Les feuilles `PARAM` et `POPT` se croisent pour indiquer quelles options appartiennent à quel champ personnalisé.
   * **`setDisplayOrder`**= la colonne d’ordre d’affichage indique l’ordre dans lequel les options s’afficheront dans votre champ personnalisé. Vous pouvez commencer par 1 et continuer par ordre croissant pour toutes les options, quels que soient les champs auxquels elles appartiennent. L’important ici est d’avoir des nombres uniques pour chaque option.
   * Les colonnes **`setLabel`** et `**setValue`** contiennent généralement les mêmes informations et doivent refléter les noms souhaités dans l’interface d’utilisation de Workfront. La valeur d’une option est le nom qui s’affiche dans les rapports, par exemple, tandis que le libellé s’affiche dans les formulaires personnalisés lorsqu’il est associé à un objet. Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
   * **`setIsHidden`** = saisissez `TRUE` si vous souhaitez que l’une des options soit masquée.

   ![Feuille de paramètres remplie](assets/parameter-option-sheet-filled-out-kick-starts.png)

1. (Facultatif) Si vous souhaitez également créer un formulaire personnalisé dans lequel vous pourrez ajouter les nouveaux champs ultérieurement, sélectionnez la feuille **`CTGY Category`** et mettez à jour les colonnes requises suivantes pour les informations de formulaire personnalisées :

   * **`isNew`** = saisissez **`TRUE`** dans cette colonne pour chaque ligne qui représente un nouveau formulaire personnalisé.
   * **`ID`** = saisissez un nombre unique pour chaque ligne représentant un nouveau formulaire. Vous pouvez utiliser n’importe quel nombre commençant par 1, à condition que chaque nouvelle option ou ligne ait un numéro unique.
   * **`setGroupID`** = ajoutez l’ID de groupe de votre groupe interne, ou tout autre groupe du système dont vous souhaitez que les membres aient accès à ce formulaire. Champ obligatoire.

   Pour découvrir l’`ID` d’un groupe, vous pouvez créer un rapport Groupe et ajouter l’`ID` dans la vue ou accédez à un groupe et recherchez l’URL du groupe. L’identifiant de groupe se trouve dans l’URL de la page du groupe. Par exemple, si l’URL du groupe est `https://companyName.my.workfront.com/group/575b000800467a6f66e747932c807464/members`, l’identifiant de groupe est `575b000800467a6f66e747932c807464`.

   * **`setCatObjCode`**= il s’agit du code objet du type d’objet pour lequel vous souhaitez que le formulaire soit créé. Saisissez un code parmi les options suivantes :
      * **`CMPY`** pour l‘entreprise
      * **`TASK`** pour la tâche
      * **`PROJ`** pour le projet
      * **`PORT`** pour le portfolio
      * **`PRGM`** pour le programme
      * **`USER`** pour l’utilisateur ou utilisatrice
      * **`DOCU`** pour le document
      * **`OPTASK`** pour le problème
      * **`EXPNS`** pour les frais
      * **`ITRN`** pour l’itération
      * **`BILL`** pour les enregistrements de facturation
      * **`GROUP`** pour le groupe

     >[!NOTE]
     >
     >Dans le cas des formulaires à plusieurs objets, saisissez le premier objet que vous sélectionnez lors de la création d’un formulaire dans l’interface d’utilisation. Par exemple, définissez `setCatObjCode` sur `TASK`, si vous voulez sélectionner Tâche dans l’interface de Workfront, puis Problème, Portfolio, etc., mais que vous ne souhaitez pas que le formulaire soit disponible pour les projets.

   * **`setName`** = nom du formulaire personnalisé tel que vous souhaitez le voir apparaître dans l’interface de Workfront.

     ![Feuille de catégorie remplie](assets/category-sheet-filled-out-kick-starts.png)

1. Enregistrez la feuille de calcul au format .xls ou .xlsx sur votre ordinateur. Votre feuille de calcul Excel est remplie et prête à être importée dans Workfront.

## Charger la feuille de calcul Excel vers Workfront

Après avoir suivi les étapes décrites dans les sections précédentes, procédez comme suit pour charger les nouveaux champs et formulaires dans Workfront :

{{step-1-to-setup}}

1. Cliquez sur **Système > Importer des données (Kick-Starts)**.

1. Cliquez sur **Choisir un fichier** dans la section **Charger des données avec feuille de calcul Kickstart**.

1. Recherchez la feuille de calcul Excel que vous avez préparée, sur votre ordinateur, et sélectionnez-la lorsque vous la trouvez.

   Le fichier se charge automatiquement et une notification indiquant que l’importation a réussi s’affiche. Selon le volume d’informations que vous importez, cette étape peut prendre quelques secondes à une minute.

   Les nouveaux champs et formulaires personnalisés se trouvent désormais dans votre système Workfront. Vous pouvez les trouver dans la zone Formulaires personnalisés de Configuration.

   >[!NOTE]
   >
   >Les nouveaux formulaires et les champs que vous avez importés ne sont pas encore connectés. Le formulaire est importé sans champ personnalisé. Vous devez ajouter manuellement les champs au nouveau formulaire personnalisé ou à un autre formulaire personnalisé existant.

   Pour plus d’informations sur l’ajout de champs aux formulaires personnalisés, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Conditionnel) Si l’importation a échoué, vous recevez un message d’erreur indiquant l’origine du problème. Essayez d&#39;identifier le champ, la feuille et le numéro de ligne dans lequel le problème a été rencontré et corrigez les informations dans le fichier Excel. Réessayez ensuite d’importer le fichier.

1. (Le cas échéant) Selon le problème, comme indiqué dans le message d’erreur, certaines informations ont peut-être déjà été importées. Vous devez effectuer l’une des opérations suivantes avant de pouvoir réimporter la feuille :

   * Supprimez les informations importées de Workfront à partir de la zone Formulaires personnalisés, puis apportez la correction indiquée par le message d’erreur.
   * Indiquez qu’un champ ou un formulaire se trouve déjà dans le système pour les champs ou formulaires déjà importés, puis apportez la correction.
Pour indiquer qu’un champ ou un formulaire personnalisé se trouve déjà dans Workfront, vous devez vous assurer que le champ `inNew` est marqué comme `FALSE` dans les feuilles contenant des informations sur le formulaire (`CTGY`) ou le champ (`PARAM`) dans la feuille de démarrage de l’import.
