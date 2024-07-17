---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules SharePoint
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les processus qui utilisent SharePoint et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2850'
ht-degree: 13%

---

# Modules [!DNL SharePoint]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL SharePoint] et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser des modules [!DNL SharePoint], vous devez disposer d’un compte [!DNL SharePoint].

## Connecter [!DNL SharePoint] à [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connectez-vous  [!DNL SharePoint]  à  [!DNL Workfront Fusion] à l&#39;aide d&#39;un  [!DNL Microsoft] compte](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connectez-vous  [!DNL SharePoint] à  [!DNL Workfront Fusion] à l&#39;aide des paramètres avancés](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connectez [!DNL SharePoint] à [!DNL Workfront Fusion] à l’aide d’un compte [!DNL Microsoft]

Vous pouvez utiliser votre compte [!DNL Microsoft] pour créer une connexion à [!DNL SharePoint]. Pour plus d’informations sur la connexion de votre compte [!DNL Sharepoint] à [!DNL Workfront Fusion], voir [Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connecter [!DNL SharePoint] à [!DNL Workfront Fusion] à l’aide des paramètres avancés

Pour vous connecter [!DNL SharePoint] à [!DNL Workfront Fusion] sans compte [!DNL Microsoft], vous avez besoin d’un identifiant client, d’un secret client et d’un identifiant client.

1. Cliquez sur **[!UICONTROL Ajouter]** près du haut de la zone **[!DNL SharePoint]** pour ouvrir la zone **[!UICONTROL Créer une connexion]**.

1. (Facultatif) Modifiez le **[!UICONTROL nom de connexion]** par défaut.
1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.
1. Saisissez les [!DNL SharePoint] **[!UICONTROL ID client]** et **[!UICONTROL Secret client]**.

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre de connexion qui s’affiche, saisissez vos informations d’identification pour vous connecter à l’application si vous ne l’avez pas déjà fait.
1. (Conditionnel) Si un bouton **[!UICONTROL Autoriser]** s’affiche, cliquez sur le bouton pour connecter l’application à [!DNL Workfront Fusion].

## Modules [!DNL SharePoint] et leurs champs

Lorsque vous configurez des modules [!DNL SharePoint], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL SharePoint] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Élément de lecteur](#drive-item)
* [Élément](#item)
* [Liste](#list)
* [Page (Beta)](#page-beta)
* [Site](#site)
* [Autre](#other)

### Élément de lecteur

* [Création d’un fichier](#create-a-file)
* [Création d’un dossier](#create-a-folder)
* [Obtention d’un fichier](#get-a-file)
* [Éléments du dossier de contrôle](#watch-folder-items)

#### Obtenir les modifications

Ce module renvoie les modifications qui ont été apportées dans SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du dossier dans lequel vous souhaitez récupérer les modifications.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID de dossier]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez l’emplacement où vous souhaitez récupérer les modifications. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### Création d’un dossier

Ce module d’action crée un dossier dans SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du dossier que vous souhaitez créer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID de dossier]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez l’emplacement où vous souhaitez créer le dossier. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du dossier]</td> 
   <td>Saisissez ou mappez un nom pour le nouveau dossier.</td> 
  </tr>
  </tbody> 
</table>

#### Obtention d’un fichier

Ce module d’action récupère le fichier SharePoint spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du fichier que vous souhaitez obtenir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID de fichier]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez l’emplacement du fichier. </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### Éléments du dossier de contrôle

Ce module de déclenchement lance un scénario lorsqu’un élément est mis à jour dans un dossier que vous sélectionnez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du fichier que vous souhaitez obtenir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID de dossier]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez l’emplacement du dossier que vous souhaitez voir. </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Entrez le nombre maximal d’éléments que [!DNL Workfront Fusion] doit renvoyer au cours d’un cycle d’exécution de scénario.</td> 
  <tr>
  </tr>
</tbody> 
</table>

### Élément

* [[!UICONTROL Copier l’élément]](#copy-an-item)
* [[!UICONTROL Créer un élément]](#create-an-item)
* [[!UICONTROL Supprimer un élément]](#delete-an-item)
* [[!UICONTROL Obtenir un élément]](#get-an-item)
* [[!UICONTROL Eléments de liste]](#list-items)
* [[!UICONTROL Déplacer l’élément]](#move-an-item)
* [[!UICONTROL Mettre à jour un élément]](#update-an-item)
* [[!UICONTROL Watch Items] (Planifié)](#watch-items-scheduled)


#### [!UICONTROL Copier l’élément]

Ce module d’action copie un élément existant dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Saisie des ID de site, de lecteur et de dossier</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste qui contiennent l’élément que vous souhaitez copier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Dans le champ Type d’élément , choisissez si vous déplacez un champ ou un dossier.  Sélectionnez le site qui contient l’élément à copier, puis sélectionnez la liste et choisissez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destination]</td> 
   <td> Saisissez ou mappez l’identifiant du dossier dans lequel vous souhaitez copier l’élément. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouveau nom]</td> 
   <td>Saisissez ou mappez un nom pour la nouvelle copie de l’élément. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un élément]

Ce module d’action crée un élément dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Créer un élément]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et la liste dans laquelle vous souhaitez créer un élément.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>[!UICONTROL ID de liste]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la liste dans laquelle vous souhaitez créer un élément, puis sélectionnez la liste. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Pour chaque champ que vous souhaitez définir pour le nouvel élément, saisissez la clé du champ (identifie le champ) et la valeur que vous souhaitez que le nouvel élément ait pour ce champ.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un élément]

Ce module d’action supprime un élément existant dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mettre à jour un élément]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément à supprimer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site qui contient l’élément à supprimer, puis sélectionnez la liste et choisissez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un élément]

Ce module d’action renvoie les données d’un élément spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir un élément]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément que vous souhaitez obtenir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la liste à partir de laquelle vous souhaitez récupérer un élément, sélectionnez la liste, puis sélectionnez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eléments de liste]

Ce module d’action récupère une liste de tous les éléments d’une liste spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eléments de liste]</td> 
   <td> <p>Sélectionnez le mode d’identification de la liste à partir de laquelle vous souhaitez récupérer les éléments.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>[!UICONTROL ID de liste]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la liste à partir de laquelle vous souhaitez récupérer les éléments, puis sélectionnez la liste. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’éléments que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un élément]

Ce module d’action copie un élément existant dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Saisie des ID de site, de lecteur et de dossier</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément à déplacer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Dans le champ Type d’élément , choisissez si vous déplacez un champ ou un dossier. Sélectionnez le site qui contient l’élément à copier, puis sélectionnez la liste et choisissez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de destination]</td> 
   <td> Saisissez ou mappez l’identifiant du dossier dans lequel vous souhaitez déplacer l’élément. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouveau nom]</td> 
   <td>Saisissez ou mappez un nom pour l’élément déplacé. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un élément]

Ce module d’action met à jour un élément existant dans une liste SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mettre à jour un élément]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément que vous souhaitez mettre à jour.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de liste]</strong> et <strong>[!UICONTROL ID d’élément]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site qui contient l’élément que vous souhaitez mettre à jour, puis sélectionnez la liste et choisissez l’élément. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td>Pour chaque champ que vous souhaitez mettre à jour pour le nouvel élément, saisissez la clé du champ (identifie le champ) et la nouvelle valeur que vous souhaitez que l’élément ait pour ce champ.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Items] (Planifié)

Ce module de déclenchement lance un scénario lorsqu’un élément est créé ou modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listes de contrôle]</td> 
   <td>Choisissez si vous souhaitez regarder les listes par heure de création (nouveaux éléments) ou par heure de modification (éléments mis à jour).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrée dans le site et ID de liste]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste à regarder.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>[!UICONTROL ID de liste]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez le site que vous souhaitez voir, puis sélectionnez la liste. Ces listes déroulantes récupèrent uniquement les sites suivis.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’éléments que le module doit renvoyer au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Liste

* [[!UICONTROL Créer une liste]](#create-a-list)
* [[!UICONTROL Obtenir une liste]](#get-a-list)
* [[!UICONTROL Listes de liste]](#list-lists)
* [[!UICONTROL Listes de contrôle]](#watch-lists)

#### [!UICONTROL Créer une liste]

Ce module d’action crée une nouvelle liste dans SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrez un ID de site]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste dans lesquels vous souhaitez créer une liste.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez l’ <strong>[!UICONTROL ID de site]</strong> où vous souhaitez créer une liste.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site sur lequel vous souhaitez créer une liste. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display Name]</td> 
   <td>Saisissez ou mappez un nom pour la nouvelle liste.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description pour la nouvelle liste.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ajouter des colonnes]</td> 
   <td>Pour chaque colonne que vous souhaitez définir pour la nouvelle liste, saisissez un <strong>[!UICONTROL Name]</strong> pour le champ, puis sélectionnez la valeur <strong>[!UICONTROL Type]</strong> de la valeur que vous souhaitez que la nouvelle colonne ait.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une liste]

Ce module d’action renvoie les données d’une liste spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir une liste]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément que vous souhaitez obtenir.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>ID de liste</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la liste que vous souhaitez récupérer, puis sélectionnez la liste. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listes de liste]

Ce module d’action récupère une liste de tous les éléments d’une liste spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Liste]</td> 
   <td> <p>Sélectionnez le mode d’identification du site à partir duquel vous souhaitez récupérer les listes.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez l’ <strong>[!UICONTROL ID de site]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site qui contient les listes que vous souhaitez récupérer. La liste déroulante récupère uniquement les sites que vous suivez.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de listes que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listes de contrôle]

Ce module de déclenchement lance un scénario lorsqu’une liste est créée ou modifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listes de contrôle]</td> 
   <td>Choisissez si vous souhaitez regarder les listes par heure de création (nouveaux éléments) ou par heure de modification (éléments mis à jour).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrée dans le site et ID de liste]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste à regarder.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez l’ <strong>[!UICONTROL ID de site]</strong> où se trouve la liste à regarder.</p> </li> 
     <li> <p><strong>[!UICONTROL Effectuez une sélection dans la liste que vous suivez]</strong> </p> <p>Sélectionnez le site que vous souhaitez voir. Le menu déroulant récupère uniquement le site que vous suivez.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de listes que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Page (Beta)

>[!NOTE]
>
>Les API de la version `beta` de [!DNL Microsoft Graph] peuvent être modifiées. L’utilisation de ces API dans les applications de production n’est pas prise en charge.

#### [!UICONTROL Obtenir une page]

Ce module d’action renvoie les données d’une page spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir une page]</td> 
   <td> <p>Sélectionnez le mode d’identification de la page que vous souhaitez récupérer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong> et <strong>[!UICONTROL ID de page]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site qui contient la page que vous souhaitez récupérer, puis sélectionnez la page.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Site

* [[!UICONTROL Obtenir un site]](#get-a-site)
* [[!UICONTROL Rechercher dans les sites]](#search-sites)

#### [!UICONTROL Obtenir un site]

Ce module d’action renvoie les données d’un site spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtenir un site]</td> 
   <td> <p>Sélectionnez le mode d’identification de la page que vous souhaitez récupérer.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez l’ <strong>[!UICONTROL ID de site]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site que vous souhaitez récupérer.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher dans les sites]

Ce module d’action recherche des sites en fonction d’un paramètre que vous spécifiez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mot-clé du nom d’affichage]</td> 
   <td> <p>Saisissez ou mappez le terme de recherche que vous souhaitez rechercher sur les sites.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de sites que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

#### Obtenir les modifications

Ce module récupère les ajouts, les mises à jour et les suppressions effectués dans le dossier SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer les ID de site, de lecteur et de dossier]</td> 
   <td> <p>Sélectionnez le mode d’identification du site et de la liste contenant l’élément que vous souhaitez mettre à jour.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de site]</strong>, <strong>[!UICONTROL ID de lecteur]</strong> et <strong>[!UICONTROL ID de dossier]</strong> dans les champs qui s’affichent.</p> </li> 
     <li> <p><strong>[!UICONTROL Sélectionnez dans la liste]</strong> </p> <p>Sélectionnez le site contenant l’élément à mettre à jour, puis le lecteur, puis sélectionnez le dossier. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Token]</td> 
   <td> Le jeton identifie à partir de quel point le module doit commencer à récupérer les modifications.  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL SharePoint] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connexion [!DNL SharePoint] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à <code>https://graph.microsoft.com</code>. Exemple :<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Sélectionnez le type de données à envoyer dans l’appel API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Surveiller les événements

Ce module de déclenchement instantané démarre un scénario lorsqu’un élément est ajouté, mis à jour ou supprimé dans SharePoint.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez un webhook existant ou cliquez sur Ajouter pour créer un nouveau webhook.</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

