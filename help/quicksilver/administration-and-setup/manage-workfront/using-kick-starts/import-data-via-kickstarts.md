---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Importer des données dans Workfront à l’aide d’un modèle Kickstart
description: Les Kickstarts sont des classeurs Excel spécialement formatés que vous pouvez renseigner avec les données à importer dans Workfront. Adobe Workfront fournit un modèle Kickstart que vous pouvez utiliser pour ce faire, comme expliqué dans la rubrique Importateur de données Kickstart.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 69cd1eafd7798861a4868fe0d68707ab5ba9106c
workflow-type: tm+mt
source-wordcount: '2776'
ht-degree: 97%

---

# Importer des données dans Workfront à l’aide d’un modèle Kickstart

<!--Audited: 12/2023-->

Les Kickstarts sont des classeurs Excel spécialement formatés que vous pouvez renseigner avec les données à importer dans Workfront. Adobe Workfront fournit un modèle Kickstart que vous pouvez utiliser pour ce faire, comme expliqué dans la section [Importateur de données Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Ce processus est divisé en trois tâches principales :

* Premièrement, vous exportez un modèle Kickstart sous forme de fichier de feuille de calcul.
* Deuxièmement, vous remplissez la feuille de calcul avec vos données.
* Enfin, vous importez la feuille de calcul renseignée dans Workfront.

Chacune de ces procédures est décrite dans l’ordre approprié dans le présent article.

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

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limites

Vous pouvez importer un grand nombre d’objets dans Workfront à l’aide d’un modèle Kickstart. Toutefois, tenez compte des restrictions suivantes :

* L’import de données de cette manière ne met pas à jour les informations sur les enregistrements déjà présents dans Workfront.
* Vous ne pouvez importer que les nouveaux enregistrements et leurs informations.
* N’importez pas plus de 2 000 enregistrements à la fois pour vous assurer que l’import n’expire pas.

## Exporter un modèle Kickstart sous la forme d’un fichier de feuille de calcul

Lorsque vous exportez un modèle Kickstart, vous recevez un classeur de feuille de calcul Excel vierge. Une fois la feuille de calcul téléchargée sur votre ordinateur, vous pouvez l’utiliser pour remplir vos informations, puis les réimporter dans Workfront.

Pour exporter un modèle Kickstart, procédez comme suit :

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  -->

1. Cliquez sur **Système** > **Importer des données (Kickstarts)**.

1. Sélectionnez les types d’information à inclure.

   Chaque option sélectionnée représente un ensemble de plusieurs onglets dans la feuille de calcul exportée. Par exemple, si vous sélectionnez l’option **Rapport**, tous les objets nécessaires à la création d’un rapport seront inclus dans la feuille de calcul (vues, filtres, regroupements, rapports).

   Vous pouvez utiliser tous les types d’objets répertoriés ci-dessous pour importer des données dans Workfront. (La seule exception concerne l’option Niveaux d’accès. La feuille de données des niveaux d’accès d’un export est fournie à titre de référence ; elle vous permet d’attribuer un niveau d’accès à un nouveau compte d’utilisateur ou d’utilisatrice par son ID.)

   Le modèle de chacun des types d’objet peut être exporté dans les formats de fichiers suivants et contient les feuilles suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objet</strong> </p> </th> 
      <th> <p><strong>Exporte en tant que</strong> </p> </th> 
      <th> <p><strong>Feuilles dans la feuille de calcul exportée</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Tableau de bord</p> <p>Tous les tableaux de bord du système peuvent être exportés. Vous pouvez sélectionner jusqu’à 100 tableaux de bord spécifiques dans un seul export.</p> </td> 
      <td scope="col">Exporte sous forme de fichier ZIP.</td> 
      <td scope="col"> <p>Paramètre</p> <p>Texte descriptif</p><p>Option de paramètre</p> <p>Groupe de paramètres</p> <p>Paramètre de catégorie</p> <p>Catégorie</p> <p>Rapport</p> <p>Section d'onglet de portail</p> <p>Tableau de bord</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Rapport</p> <p>Tous les rapports du système peuvent être exportés. Vous pouvez sélectionner jusqu’à 100 rapports spécifiques au sein d’une seule exportation.</p> <p>Kick-Starts ne prend pas en charge les filtres ou les regroupements en mode texte. Pour une exportation réussie, les filtres et les regroupements de rapports doivent passer en mode standard.</p> </td> 
      <td scope="col">Exporte sous forme de fichier ZIP. </td> 
      <td scope="col"> <p scope="col">Paramètre</p> <p scope="col">Texte descriptif</p> <p scope="col">Option de paramètre</p> <p scope="col">Groupe de paramètres</p> <p scope="col">Paramètre de catégorie</p> <p scope="col">Catégorie</p> <p scope="col">Rapport</p> <p scope="col">Préférences</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Approbation</p> </td> 
      <td scope="col"> <p>Exporte sous forme de fichier Excel.</p> </td> 
      <td scope="col"> <p>Approbateur d'étape</p> <p>Étape d’approbation</p> <p>Approbation</p> <p>Processus d’approbation</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Données personnalisées</p> </td> 
      <td scope="col"> <p>Exporte sous forme de fichier Excel.</p> </td> 
      <td scope="col"> <p>Paramètre</p> <p>Texte descriptif</p>  <p>Option de paramètre</p> <p>Groupe de paramètres</p> <p>Paramètre de catégorie</p> <p>Catégorie</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Type de frais</p> </td> 
      <td scope="col"> <p>Exporte sous forme de fichier Excel.</p> </td> 
      <td> <p>Type de frais</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Type d’heure</p> </td> 
      <td scope="col"> <p>Exporte sous forme de fichier Excel.</p> </td> 
      <td> <p>Type d’heure</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Equipe</p> </td> 
      <td scope="col"> <p>Exporte sous forme de fichier Excel.</p> </td> 
      <td> <p> Membre d'équipe</p> <p>Equipe</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
      <td> <p>Exporte sous forme de fichier Excel. Pour afficher la liste complète des options, cliquez sur <strong>Plus d’options</strong>.</p> </td> 
      <td> <p>l’utilisateur ou de l’utilisatrice</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td>Niveau d’accès</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p>Niveau d’accès</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td>Affectation</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p>Affectation</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td>Entreprise</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Entreprise</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Modèle d'e-mail</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p>Modèle d'e-mail</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Frais</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Dépense</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Page externe</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Page externe</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Filtre</td> 
      <td>Exporte sous forme de fichier ZIP.</td> 
      <td> <p> Filtre</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Groupe</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Groupe</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Regroupement </td> 
      <td>Exporte sous forme de fichier ZIP.</td> 
      <td> <p> Regroupement </p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Heure</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Heure</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Problème</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Problème</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Fonction</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Fonction</p> <p>Préférences </p> </td> 
     </tr>

   <tr> 
      <td>Chemin jalonné</td> 
      <td> Exporte sous forme de fichier Excel.</td> 
      <td> <p> Jalon</p> <p>Chemin jalonné</p> <p>Préférences </p> </td> 
     </tr>

   <tr> 
      <td>Note</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Note</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Portfolio</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Portfolio</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Projet</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> File d'attente</p> <p>Projet</p> <p>Règle de transmission</p> <p>Rubrique de file d'attente</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Estimation de ressources</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Estimation de ressources</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Risque</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Risque</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Type de risque</td> 
      <td> Exporte sous forme de fichier Excel.</td> 
      <td> <p> Type de risque</p> <p>Préférences</p> </td> 
     </tr> 
     <tr> 
      <td>Carte de score</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p>Question sur la carte de score</p> <p>Option de la carte de résultats</p> <p>Carte de score</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Tâche</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Tâche</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Modèle</td> 
      <td> Exporte sous forme de fichier Excel.</td> 
      <td> <p> File d'attente</p> <p>Modèle</p> <p>Règle de transmission</p> <p>Rubrique de file d'attente</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Modèle d'affectation</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Modèle d'affectation</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Tâche de modèle</td> 
      <td>Exporte sous forme de fichier Excel.</td> 
      <td> <p> Tâche de modèle</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Feuille de temps</td> 
      <td> Exporte sous forme de fichier Excel.</td> 
      <td> <p> Profil de feuille de temps</p> <p>Feuille de temps</p> <p>Préférences </p> </td> 
     </tr> 
     <tr> 
      <td>Afficher </td> 
      <td> <p>Exporte sous forme de fichier ZIP.</p> </td> 
      <td> <p> Afficher</p> <p>Préférences </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Télécharger**.
1. Continuez avec [Remplir le modèle de feuille de calcul avec vos données](#populate-the-spreadsheet-template-with-your-data) pour remplir la feuille de calcul de modèle vierge avec vos informations.

## Remplir le modèle de feuille de calcul avec vos données {#populate-the-spreadsheet-template-with-your-data}

* [Vue d’ensemble des onglets (feuilles de données) inclus dans la feuille de calcul](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importer un enregistrement](#import-a-record)
* [Inclure des dates](#include-dates)
* [Utiliser des caractères génériques](#use-wildcards)
* [Substitution des noms d’attribut pour les identifiants](#attribute-name-substitution-for-ids)

### Vue d’ensemble des onglets (feuilles de données) inclus dans la feuille de calcul

>[!TIP]
>
>Pour mieux comprendre comment vous devrez formater les informations dans chaque colonne lorsque vous renseignez le modèle Kickstart, envisagez d’effectuer une exécution pratique en exportant un Kickstart avec des données Workfront existantes sur les objets que vous essayez d’importer. Pour obtenir des instructions, voir [Exporter des données d’Adobe Workfront par le biais de Kickstarts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Lorsque vous ouvrez un modèle Kickstart vierge, plusieurs onglets (feuilles de données) sont disponibles. Ils dépendent des objets que vous avez sélectionnés pour le téléchargement. Chacun représente un objet dans l’application, tel que le projet, les tâches, les heures, le tableau de bord et les personnes :

Lorsque vous ouvrez l’un de ces onglets, la ligne 2 affiche les champs de chaque objet pouvant être défini au cours d’une importation. Dans un en-tête de colonne, après le mot « set », le nom du champ s’affiche tel qu’il apparaît dans la base de données. Ces champs se comportent comme des en-têtes de colonne.

>[!IMPORTANT]
>
>Pour éviter les erreurs, vérifiez les points suivants :
>
>* Ne supprimez pas la première ligne vide d’une feuille de calcul Kickstart.
>* Ne supprimez, ne modifiez pas et ne réorganisez pas ces champs (en-têtes de colonne) de quelque manière que ce soit. Par exemple, ne modifiez pas leur ordre ou leur nom.
>* Ajoutez des valeurs à chaque champ qui s’affiche en gras dans l’en-tête de colonne. Il s’agit des champs obligatoires.
>
>     Toutefois, si un champ obligatoire contient une valeur par défaut définie dans les préférences du système, il n’est pas nécessaire de le renseigner.
>
>     Par exemple, sur l’onglet **Projet PROJ**, les champs **setCondition** et **setConditionType** peuvent être laissés vides, mais les colonnes **setGroupID** et **setName** ne le peuvent pas.
>
>* Certains champs, y compris **setResourceRevenue** et **setEnteredByID**, sont générés automatiquement par le système. Si vous saisissez des données pour ces champs dans la feuille de calcul, le processus Kickstart l’emportera lors du chargement de la feuille de calcul.

### Importer un enregistrement  {#import-a-record}

Chaque ligne de la feuille correspond à un objet unique.

1. Ajoutez des informations dans la colonne **isNew** :

   * Si l’objet que vous importez est nouveau, saisissez **TRUE** pour importer les données dans la ligne. Cette valeur est sensible à la casse et doit toujours être saisie en majuscules.
   * Si l’objet se trouve déjà dans Workfront, saisissez **FALSE** dans la colonne **isNew** pour ignorer la ligne. Cette valeur est sensible à la casse et doit toujours être saisie en majuscules.

      * Les enregistrements qui existent déjà dans Workfront ne sont pas mis à jour.
      * Si vous avez téléchargé un modèle contenant des données provenant de Workfront, la valeur **FALSE** est déjà indiquée pour les objets existants.
      * Si vous avez téléchargé un modèle vierge, il n’est pas nécessaire d’ajouter de nouvelles lignes pour les objets existants.

1. Ajoutez des informations dans la colonne **ID** de l’une des manières suivantes :

   * Si l’objet que vous importez est nouveau (et que vous avez saisi **TRUE** dans la colonne **isNew**), saisissez n’importe quel numéro pour l’ID. Ce nombre doit être unique dans la feuille de calcul. Par exemple, si vous importez trois objets, vous pouvez leur attribuer respectivement les identifiants 1, 2 et 3.

   * Si l’objet existe déjà dans Workfront (et que la valeur **FALSE** est indiquée dans la colonne **isNew**) et que vous importez de nouvelles informations sur les objets existants, l’ID doit être le GUID alphanumérique existant dans Workfront pour cet objet.

   >[!TIP]
   >
   > Pour découvrir le GUID unique d’un objet dans Workfront, vous pouvez créer un rapport pour cet objet et ajouter la colonne ID au rapport. La valeur de chaque objet de cette colonne correspond au GUID de l’objet.

   * Les enregistrements qui existent déjà dans Workfront ne sont pas mis à jour.
   * Si vous avez téléchargé un modèle avec des données, les objets existants contiennent déjà le GUID en tant qu’ID.
   * Vous pouvez importer un nouvel objet en fonction d’un objet existant en remplaçant **FALSE** par **TRUE** dans la colonne **isNew**, en modifiant l’ID et en ajustant les données avant l’import.

   ![Exemple d’ID pour un groupe](assets/kick-start-group-example.png)

   * Lorsque vous importez un projet, vous devez indiquer un ID de groupe.

      * Si le groupe existe déjà dans Workfront, vous devez ajouter son ID unique au champ **setGroupID** pour le projet.
      * Si le groupe n’existe pas dans Workfront, vous pouvez ajouter la feuille de **groupe GROUP** dans votre fichier d’import, définir le champ **isNew** sur **TRUE** dans la feuille de groupe, puis indiquer un ID numérique pour le nouveau groupe dans la colonne **ID**. Le champ **setGroupID** pour le nouveau projet doit correspondre à l’**ID** numérique pour le nouveau groupe.

     **Exemple :** pour un projet, la valeur affichée dans la colonne **setGroupID** doit correspondre à l’un des éléments suivants :

      * GUID d’un groupe existant dans votre instance Workfront.
      * Valeur (nombre) dans la colonne ID de la feuille de **groupe GROUP** si vous créez un groupe au cours de l’import.

1. Saisissez des valeurs pour les champs obligatoires et pour les autres champs que vous souhaitez renseigner lors de l’import.
1. (Facultatif) Pour ajouter des données personnalisées, procédez comme suit :

   * Créez une colonne pour chaque champ personnalisé que vous souhaitez inclure dans le processus d’import.
   * Nommez chaque nouvelle colonne en fonction de son champ personnalisé correspondant comme suit : **DE:[Nom du champ personnalisé tel qu’il apparaît dans Workfront]**. Par exemple, vous pouvez créer le champ personnalisé suivant : « DE:Departments » (Services).
   * Dans la colonne **setCategoryID**, saisissez le GUID du formulaire personnalisé existant sur lequel réside ce champ personnalisé. Ce champ est obligatoire lors de l’import de données personnalisées.
   * Si vous devez ajouter plusieurs valeurs de données dans un champ personnalisé (comme des cases d’option, des cases à cocher ou des listes), utilisez le délimiteur de données personnalisées à barre verticale « | » répertorié dans l’onglet Préférences pour séparer les valeurs.

     **Exemple :** saisissez A|D sous la colonne DE:Departments pour renseigner les services A et D dans votre formulaire personnalisé.

     >[!NOTE]
     >
     >Utilisez uniquement le délimiteur « | » pour séparer les valeurs de champ personnalisé. Vous ne pouvez pas l&#39;utiliser dans les autres colonnes de la feuille de calcul, y compris **setCategoryID**.

### Inclure des dates  {#include-dates}

Workfront peut traiter la plupart des formats de date. Cependant, vous devez vous assurer que la colonne de date de la feuille de calcul est formatée en tant que date. L’import échoue si la colonne est formatée en tant que général, nombre ou texte.

>[!TIP]
>
>Le format le plus populaire aux États-Unis est le format MM/JJ/AAAA.
>
>Par exemple : 07/10/2023 (10 juillet 2023).

Workfront accepte également que l’heure soit incluse avec la date.

Par exemple : 07/10/2022 01:30 ou 07/10/2022 1:00 PM (au format 12 heures).

Si vous ne mettez pas d’heure avec la date, Workfront effectue l’une des opérations suivantes :

* Workfront suppose que l’heure est 12:00 AM (minuit). Pour que le résultat de la date soit visible, le fuseau horaire du système doit correspondre à votre fuseau horaire.
* S’il se trouve sur un objet associé à un planning, l’heure est décalée au premier moment autorisé par le planning.

>[!NOTE]
>
>Lorsque vous utilisez un horodatage UNIX, vous devez inclure trois zéros supplémentaires à la fin de la valeur.
>
>Par exemple, si votre horodatage est 7336899000, vous devez saisir 7336899000000 dans la cellule.

### Utiliser des caractères génériques {#use-wildcards}

Vous pouvez utiliser les caractères génériques suivants lorsque vous renseignez votre feuille de calcul de modèle Kickstart :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Caractère générique</strong> </p> </th> 
   <th> <p><strong>Comportement</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$TODAY</p> </td> 
   <td> <p>Lorsqu’il est utilisé dans un champ <strong>setDate</strong>, ce caractère générique fixe la date à minuit le jour de l’import du Kickstart.</p> <p>Vous pouvez modifier le caractère générique en utilisant la syntaxe standard autorisée avec le caractère générique sur un filtre.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>si vous souhaitez qu’un projet commence le lundi de la semaine où il est importé, quel que soit le jour où vous effectuez l’import, vous pouvez utiliser <strong>$$TODAYbw</strong>. La date de début prévue de votre projet est alors fixée au dimanche à 00h00. Comme le planning du projet n’autorise probablement pas le travail à ce moment-là, il commencera lundi matin à 9h00.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Lorsqu’il est utilisé dans un champ <strong>setDate</strong>, ce caractère générique définit la date en fonction du moment où vous créez l’enregistrement lors de l’import du Kickstart.</p> <p>Vous pouvez modifier le caractère générique en utilisant la syntaxe standard autorisée avec le caractère générique sur un filtre.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span>si vous souhaitez qu’un projet démarre 3 heures après son import, vous pouvez utiliser <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Lorsqu’il est utilisé dans un champ <strong>setAssignedToID</strong> ou dans un autre champ basé sur l’ID de l’utilisateur ou de l’utilisatrice, ce caractère générique affecte le travail ou associe l’enregistrement à la personne qui effectue l’import.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Ce caractère générique a été ajouté spécifiquement pour les imports des utilisateurs et utilisatrices Kickstart. La création d’un compte Workfront génère la création d’un utilisateur ou d’une utilisatrice disposant d’un niveau d’accès à l’administration du système. Le nom d’utilisateur ou d’utilisatrice attribué à l’administration par défaut peut être utilisé comme préfixe lors de la création d’autres utilisateurs et d’autres utilisatrices dans le compte.</p> <p>Les noms d’utilisateur ou d’utilisatrice doivent être uniques pour toute la clientèle. Cette option est très utile lorsque vous avez plusieurs personnes avec des noms d’utilisateur ou d’utilisatrice très courants, tels que John Smith, dont le nom d’utilisateur peut être « jsmith ». En ajoutant l’affectation du nom d’utilisateur ou d’utilisatrice en préfixe au nom par défaut affecté à l’administration, vous garantissez que chaque nom d’utilisateur ou d’utilisatrice est unique (par exemple : <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Conseil : pour vous assurer que les noms d’utilisateur ou d’utilisatrice sont uniques à l’échelle du système, saisissez l’adresse e-mail de la personne dans le champ <strong>setUsername</strong>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Substitution des noms d’attribut pour les identifiants  {#attribute-name-substitution-for-ids}

Même si l’usage des identifiants est préférable lorsque cela est possible, il n’est pas toujours pratique de les transférer d’une feuille à l’autre lors de la configuration de la valeur d’un **setAttributeID**. Vous pouvez référencer des valeurs par nom en modifiant simplement l’en-tête de colonne.

**Exemples :**

* **Import de projet**

  Lors de l’import de projets, définissez les **setGroupID** des projets en allant sur la feuille de **groupe GROUP**, en notant les ID de groupe respectifs et en les collant dans les cellules correctes (colonne **setGroupID**) sur la feuille de **projet PROJ**.

  Cette méthode fonctionne bien avec quelques groupes et projets ; cependant, elle devient impraticable lorsque le nombre de projets et de groupes augmente.

  Pour substituer le nom de l’attribut dans l’exemple décrit ci-dessus, vous devez remplacer l’en-tête de colonne **setGroupID** par le **nom #setGroupID GROUP**. Vous pouvez ensuite référencer le groupe de chaque projet par nom.

  >[!NOTE]
  >
  >L’option permettant d’utiliser la substitution du nom d’attribut est limitée aux références pour les enregistrements existants uniquement. Vous ne pouvez pas utiliser la substitution de nom pour les objets que vous créez dans le même import.

* **Import d’utilisateur ou d’utilisatrice**

  Lors de l’import d’utilisateurs et d’utilisatrices, renseignez le **setRoleID** à partir de la liste de rôles de l’onglet de **rôle ROLE**.

  Certains ID de rôle concernent des enregistrements déjà présents dans le compte, tandis que d’autres sont créés lors de l’import.

  Pour les nouveaux enregistrements d’utilisateurs et d’utilisatrices affectés aux rôles existants, vous pouvez utiliser la substitution de nom. Pour les nouveaux enregistrements d’utilisateurs et d’utilisatrices affectés aux rôles nouvellement importés, il est impossible d’utiliser la substitution de nom.

  Voici comment utiliser les deux méthodes sur le même fichier d’import :

   * Ajoutez une colonne dans la feuille de calcul située à gauche de la colonne **setRoleID**.
   * Donnez à la nouvelle colonne le **nom #setRoleID ROLE**.
   * Pour les affectations de rôle aux enregistrements existants, saisissez les noms de rôle dans la colonne au **nom #setRoleID ROLE**.

     Pour les affectations de rôles aux nouveaux enregistrements de rôle, saisissez l’ID que vous avez affecté dans la feuille de « rôle ROLE » dans « setRoleID ».

     ![Identifiant de rôle pour les utilisateurs et les utilisatrices](assets/set-role-id.png)

## Importer des données de feuille de calcul dans Workfront

Une fois que vous avez renseigné les données du modèle Excel, vous pouvez les charger dans Workfront.

L’import rapide prend en charge les types de fichiers suivants :

* Excel (.xls ou .xlsx)
* Fichier compressé (.ZIP) (contenant uniquement des fichiers .xlsx ou .xls)

  >[!NOTE]
  >
  >Vous devez utiliser un fichier .ZIP lors de l’import de feuilles de calcul Excel qui référencent les objets suivants :
  >
  >* Rapports
  >* Documents
  >* Avatars
  >* Afficher, filtrer ou regrouper des fichiers de propriétés
  >
  >Lors de l’utilisation d’un fichier d’import compressé, le fichier .ZIP doit porter le même nom que le fichier .xlsx ou .xls, et tous les fichiers doivent être au même niveau de structure (pas de dossiers).

Pour importer les données de feuille de calcul du modèle dans Workfront, procédez comme suit :

<!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Importer des données (Kickstarts)**.

1. Dans la section **Charger des données avec la feuille de calcul Kickstart**, cliquez sur **Choisir un fichier**, puis parcourez et sélectionnez la feuille de calcul renseignée.

1. Cliquez sur **Charger**.

   Si le chargement du fichier Excel prend plus de 5 minutes dans Workfront, l’application expire et Workfront ne peut pas charger le fichier.

   Essayez d’importer vos données en lots d’objets plus petits.

1. (Le cas échéant) Si vous utilisez Workfront Fusion, vous pouvez désormais activer vos FLO ou scénarios.
