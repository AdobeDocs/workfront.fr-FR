---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Entrepôts de données dans [!DNL Adobe Workfront Fusion]
description: Un entrepôt de données, similaire à une base de données ou à un tableau simple, peut stocker des données de scénarios, ce qui permet de transférer des données entre des scénarios individuels ou des exécutions de scénarios. Vous pouvez utiliser un entrepôt de données pour stocker de nouvelles données provenant de différents systèmes lors de la synchronisation.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# Entrepôts de données dans [!DNL Adobe Workfront Fusion]

Un entrepôt de données, similaire à une base de données ou à un tableau simple, peut stocker des données de scénarios, ce qui permet de transférer des données entre des scénarios individuels ou des exécutions de scénarios. Vous pouvez utiliser un entrepôt de données pour stocker de nouvelles données provenant de différents systèmes lors de la synchronisation.

Les modules d’entrepôt de données vous permettent d’effectuer les actions suivantes sur les enregistrements de votre [!DNL Adobe Workfront Fusion] entrepôt de données :

* Ajouter
* Remplacer
* Mettre à jour
* Récupération
* Supprimer
* Recherche
* Nombre

Pour plus d’informations sur l’utilisation des modules de l’entrepôt de données, voir [[!UICONTROL Entrepôt de données] modules](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

Pour une vidéo d’introduction aux entrepôts de données dans Workfront Fusion, voir :

* [Entrepôts de données](https://video.tv.adobe.com/v/3427029/){target=_blank}

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelles : non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de l’[!UICONTROL Select] ou de l’[!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Création d’un magasin de données dans [!DNL Workfront Fusion]

* [Configuration de l’entrepôt de données](#set-up-the-data-store)
* [Configuration de la structure de données](#set-up-the-data-structure)

### Configuration de l’entrepôt de données

Avant de pouvoir utiliser un entrepôt de données dans un module, vous devez créer l’entrepôt de données dans [!DNL Workfront Fusion].

>[!NOTE]
>
>Votre entreprise dispose d’un nombre limité de entrepôts de données disponibles. Si vous tentez de créer plus de entrepôts de données que vous n’en disposez, [!DNL Workfront] renvoie une [!UICONTROL Nombre maximum de magasins atteints] erreur.
>
>Pour plus d’informations, voir [Erreur maximum des magasins atteints](#maximum-stores-reached-error) dans cet article.

1. Connectez-vous à [!DNL Workfront Fusion] compte .
1. Cliquez sur **[!UICONTROL Entrepôts de données]** dans le panneau de navigation de gauche.
1. Cliquez sur **[!UICONTROL Ajouter un entrepôt de données]** dans le coin supérieur droit de l’écran.
1. Saisissez les paramètres du nouvel entrepôt de données.

   Titre en gras sur un champ d’un [!DNL Workfront Fusion] indique un paramètre requis.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nom de l’entrepôt de données] </td> 
      <td> <p>Saisissez le nom de l’entrepôt de données. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Structure de données]</p> </td> 
      <td> <p>Une structure de données est une liste des colonnes d’un tableau. Cette liste indique le nom de la colonne et le type de données.</p> <p>Utilisez l’une des méthodes suivantes :</p> 
       <ul> 
        <li style="font-weight: bold;">Sélectionner une structure de données déjà créée</li> 
        <li> <p style="font-weight: bold;">Ajouter une nouvelle structure de données</p> <p>Cliquez sur <strong>[!UICONTROL Ajouter]</strong> pour créer une structure de données.</p> <p>Pour plus d’informations, voir <a href="#set-up-the-data-structure" class="MCXref xref">Configuration de la structure de données</a> dans cet article.</p> </li> 
        <li style="font-weight: bold;"> <p>Laissez le champ vide</p> <p style="font-weight: normal;">Si vous ne sélectionnez ni n'ajoutez de structure de données, la base de données ne contiendra que la clé primaire. Un tel type de base de données est utile si vous souhaitez enregistrer des clés uniquement et que vous souhaitez uniquement savoir s’il existe ou non une clé spécifique dans la base de données.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Taille de stockage des données en Mo]</p> </td> 
      <td> <p>Allouez la taille de l’entrepôt de données à partir de votre stockage de données interne total.</p> <p> La valeur par défaut est de 10 Mo. Si vous disposez de moins de 10 Mo d’espace de stockage de données non alloué à partir de votre allocation de 500 Mo, la taille par défaut correspond à la quantité de stockage non alloué.  <p>Remarque : Le montant réservé peut être modifié à tout moment.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Configuration de la structure de données

1. Lors de la création ou de la modification d’un entrepôt de données, cliquez sur **[!UICONTROL Ajouter]**.
1. Dans le **[!UICONTROL Ajouter une structure de données]** qui s’affiche, configurez les champs suivants :

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nom de la structure de données]</td> 
      <td> <p> Saisissez un nom pour la nouvelle structure de données.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Specification]</p> </td> 
      <td> <p>Pour configurer les colonnes de votre entrepôt de données, effectuez l’une des opérations suivantes.</p> 
       <ul> 
        <li> <p>Cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong> pour spécifier manuellement les propriétés d’une colonne.</p> <p>Saisissez le <strong>[!UICONTROL Name]</strong> et <strong>[!UICONTROL Type]</strong> pour la colonne data store et définissez les propriétés correspondantes.</p> </li> 
        <li> <p>Cliquez sur <strong>[!UICONTROL Generator]</strong> pour déterminer les colonnes des exemples de données que vous fournissez.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Exemple : </b></span></span> 
          <p>Par exemple, les exemples de données JSON suivants créent trois colonnes : nom, âge et numéro de téléphone. Le numéro de téléphone est un ensemble de numéros de téléphone mobile et fixe.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>Les colonnes vides dans la vue d’entrepôt de données :</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>Vous pouvez ensuite ajouter des valeurs à l’entrepôt de données manuellement ou à l’aide de la variable [!DNL Workfront Fusion] modules d’entrepôt de données.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Strict] </td> 
      <td> <p>Activez cette option pour vous assurer que la payload correspond aux structures de données. Les payloads qui contiennent des éléments supplémentaires non spécifiés dans la structure de données sont rejetées.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Modifier un entrepôt de données existant

Vous pouvez modifier les propriétés et le contenu d’un entrepôt de données existant dans le [!UICONTROL Entrepôt de données] area of [!DNL Workfront Fusion].

* [Modification des propriétés d’un entrepôt de données](#edit-the-properties-of-a-data-store)
* [Modification du contenu d’un entrepôt de données](#edit-the-contents-of-a-data-store)

### Modification des propriétés d’un entrepôt de données

Les propriétés d’un entrepôt de données incluent la structure de données utilisée par l’entrepôt de données, ainsi que la taille de l’entrepôt de données.

1. Cliquez sur **[!UICONTROL Entrepôt de données]** ![](assets/data-store-icon.png) dans le panneau de navigation de gauche pour ouvrir la [!UICONTROL Entrepôt de données] zone.
1. Cliquez sur **[!UICONTROL Modifier]** ![](assets/data-store-edit.png) en regard de l’entrepôt de données que vous souhaitez modifier.
1. (Facultatif) Si vous souhaitez remplacer la structure de données utilisée par cet entrepôt de données par une autre structure de données existante, sélectionnez-la dans la liste **[!UICONTROL Structure des données]** menu déroulant.

   Ou

   (Facultatif) Si vous souhaitez modifier la structure de données utilisée par cet entrepôt de données en une structure de données entièrement nouvelle, reportez-vous à la section [Configuration de la structure de données](#set-up-the-data-structure) dans cet article.

1. (Facultatif) Modifiez la taille de l’entrepôt de données en saisissant la nouvelle taille dans la variable **[!UICONTROL Taille de stockage des données en Mo]** champ .
1. Cliquer sur **[!UICONTROL Enregistrer]**.

### Modification du contenu d’un entrepôt de données

1. Cliquez sur le bouton **[!UICONTROL Entrepôt de données]** icon ![](assets/data-store-icon.png) dans le panneau de navigation de gauche pour ouvrir la [!UICONTROL Entrepôt de données] zone.
1. Cliquez sur **[!UICONTROL Parcourir]**  en regard de l’entrepôt de données que vous souhaitez modifier.
1. (Facultatif) Réorganisez les colonnes en les faisant glisser à l’emplacement souhaité.
1. (Facultatif) [!UICONTROL Modifier] une seule cellule en cliquant sur la fonction **[!UICONTROL Modifier]** dans cette cellule, puis saisissez la valeur souhaitée.
1. (Facultatif) Ajoutez un nouvel élément au magasin de données en cliquant sur **[!UICONTROL Ajouter]**, puis saisissez les informations du nouvel élément.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Dépannage

* [Restauration des données perdues à partir d’un entrepôt de données](#restoring-lost-data-from-a-data-store)
* [Erreur de manque d’espace](#out-of-space-error)
* [Erreur maximum des magasins atteints](#maximum-stores-reached-error)

### Restauration des données perdues à partir d’un entrepôt de données

Il n’existe actuellement aucun outil capable d’automatiser la restauration des données perdues.

#### Solution

1. Examinez tous les journaux d’exécution des scénarios dans lesquels des éléments ont été insérés dans l’entrepôt de données.

   Pour plus d’informations sur l’examen des logs d’exécution, voir [Afficher l’historique d’exécution d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copiez les données.
1. Insérez à nouveau les données dans votre entrepôt de données.

   Pour plus d’informations sur l’insertion de données dans un entrepôt de données, voir [Modification du contenu d’un entrepôt de données](#edit-the-contents-of-a-data-store) dans cet article.

### [!UICONTROL Espace insuffisant] error

Un [!UICONTROL Espace insuffisant] s’affiche, car les entrepôts de données que vous avez créés précédemment ont déjà été attribués à votre stockage de données alloué.

#### Solution

1. Modifiez l’un de vos entrepôts de données existants pour utiliser moins d’espace. Cela libère de l’espace pour votre nouvel entrepôt de données.

   Pour plus d’informations, voir [Modification des propriétés d’un entrepôt de données](#edit-the-properties-of-a-data-store) dans cet article.

>[!NOTE]
>
>Nous vous recommandons de ne pas affecter tout votre espace à un seul entrepôt de données, sauf si vous êtes certain que vous n’aurez pas besoin d’autres entrepôts de données.

### [!UICONTROL Nombre maximum de magasins atteints] error

A [!UICONTROL Nombre maximum de magasins atteints] se produit car votre entreprise a utilisé tous ses entrepôts de données disponibles. Une organisation dispose d’un nombre de entrepôts de données égal au double du nombre de scénarios disponibles. Par conséquent, le nombre total de banques de données disponibles dépend du plan que vous avez acheté.

Par exemple, si votre entreprise a acheté un plan comportant 15 scénarios, elle peut avoir jusqu’à 30 entrepôts de données.

#### Solution

Pour réduire le nombre de entrepôts de données existants, envisagez d’effectuer l’une des opérations suivantes :

* Combiner des entrepôts de données existants
* Suppression des entrepôts de données inutilisés
