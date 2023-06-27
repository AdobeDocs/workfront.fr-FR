---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive pour les modules métier
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft OneDrive for Business], ainsi que de la connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft OneDrive for Business], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Microsoft OneDrive for Business] avec [!DNL Adobe Workfront Fusion], vous aurez besoin d’un [!DNL Microsoft] compte .

Pour obtenir des instructions sur la connexion à [!DNL OneDrive for Business] compte à [!DNL Workfront Fusion], voir [Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] modules et leurs champs

Lorsque vous configurez [!DNL Microsoft OneDrive for Business] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Microsoft OneDrive for Business] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)

### Triggers

* [[!UICONTROL Fichiers de contrôle]](#watch-files)
* [[!UICONTROL Surveiller les dossiers]](#watch-folders)

#### [!UICONTROL Fichiers de contrôle]

Ce module de déclenchement s’active lorsqu’un nouveau fichier est ajouté ou mis à jour dans un dossier contrôlé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>Sélectionnez le lecteur à regarder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> Sélectionnez le dossier que vous souhaitez voir. Dans un scénario, vous ne pouvez surveiller qu’un seul dossier.</p> <p>Conseil : Pour effectuer le suivi de plusieurs dossiers, créez un scénario indépendant pour chacun d’eux.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Je veux regarder]</p> </td> 
   <td> <p>Indiquez si vous souhaitez regarder les nouveaux fichiers et toutes les modifications, ou les nouveaux fichiers uniquement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de lignes renvoyées]</td> 
   <td> <p> Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les dossiers]

Ce module de déclenchement s’active lorsqu’un nouveau dossier est ajouté au dossier contrôlé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>Sélectionnez le lecteur à regarder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> Sélectionnez le dossier que vous souhaitez voir. Dans un scénario, vous ne pouvez surveiller qu’un seul dossier.</p> <p>Conseil : Pour effectuer le suivi de plusieurs dossiers, créez un scénario indépendant pour chacun d’eux.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Je veux regarder]</p> </td> 
   <td> <p>Indiquez si vous souhaitez consulter les nouveaux dossiers et toutes les modifications, ou les nouveaux dossiers uniquement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de lignes renvoyées]</td> 
   <td> <p> Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Chargement d’un fichier]](#upload-a-file)
* [[!UICONTROL Suppression d’un fichier]](#delete-a-file)
* [[!UICONTROL Obtention d’un fichier]](#get-a-file)
* [[!UICONTROL Création d’un dossier]](#create-a-folder)
* [[!UICONTROL Suppression d’un dossier]](#delete-a-folder)
* [[!UICONTROL Obtention d’un lien de partage]](#get-a-sharing-link)

#### [!UICONTROL Chargement d’un fichier]

Ce module d’action charge un fichier binaire ou texte dans un dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur sur lequel vous souhaitez charger un fichier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier dans le lecteur.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Fichier source]</p> </td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Si le fichier portant le même nom existe]</td> 
   <td> <p> Sélectionnez ce que vous souhaitez faire si un fichier portant le même nom que le fichier que vous essayez de télécharger existe déjà.</p> 
    <ul> 
     <li>[!UICONTROL Remplacer le fichier existant]</li> 
     <li>[!UICONTROL Renommer le nouveau fichier]</li> 
     <li>[!UICONTROL Fin avec erreur]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un fichier]

Ce module d’action déplace le fichier spécifié vers la corbeille.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur sur lequel vous souhaitez supprimer un fichier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>Saisissez l’identifiant du fichier que vous souhaitez supprimer. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un fichier]

Ce module d’action récupère le fichier avec l’identifiant donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur à partir duquel vous souhaitez récupérer un fichier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>Saisissez l’identifiant du fichier que vous souhaitez récupérer. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un dossier]

Crée un dossier dans le dossier parent spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Connection]</strong> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Drive ID]</strong> </td> 
   <td> <p>Sélectionnez le lecteur sur lequel vous souhaitez créer un dossier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder]</strong> </td> 
   <td> <p>Sélectionnez le dossier dans lequel vous souhaitez créer un dossier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Nom du dossier]</strong> </td> 
   <td>Saisissez ou mappez un nom pour le nouveau dossier.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un dossier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur sur lequel vous souhaitez supprimer un fichier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de dossier]</td> 
   <td> <p>Saisissez ou mappez l’identifiant du dossier à supprimer. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un lien de partage]

Ce module récupère un lien que vous pouvez partager pour donner accès au fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]</a> dans l’article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Création d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur sur lequel vous souhaitez charger un fichier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entrée]</td> 
   <td> <p>Choisissez si vous souhaitez choisir un fichier à l’aide de l’identifiant de fichier ou du chemin d’accès au fichier. Saisissez l’identifiant du fichier ou le chemin d’accès dans le champ qui s’affiche.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type d’autorisation]</p> </td> 
   <td> <p>Indiquez si vous souhaitez que les personnes qui reçoivent le lien disposent d’autorisations de lecture/écriture ou de lecture seule.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope]</td> 
   <td> <p> Indiquez si vous souhaitez que le fichier soit accessible à toute personne disposant du lien ou accessible uniquement aux membres de votre organisation.</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
