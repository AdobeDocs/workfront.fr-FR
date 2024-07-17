---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive pour les modules métier
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL Microsoft OneDrive for Business] et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1201'
ht-degree: 21%

---

# Modules [!DNL Microsoft OneDrive for Business]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft OneDrive for Business] et les connecter à plusieurs applications et services tiers.

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

Pour utiliser [!DNL Microsoft OneDrive for Business] avec [!DNL Adobe Workfront Fusion], vous aurez besoin d&#39;un compte [!DNL Microsoft].

Pour plus d’informations sur la connexion de votre compte [!DNL OneDrive for Business] à [!DNL Workfront Fusion], voir [Création d’une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)



## Connexion du service [!DNL Microsoft OneDrive for Business] à [!DNL Workfront Fusion]

Pour plus d’informations sur la connexion de votre compte [!DNL Microsoft OneDrive for Business] à [!UICONTROL Workfront Fusion], voir [Création d’une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations utilisateur individuelles. Par conséquent, lors de la création d’une connexion, l’écran de consentement des autorisations affiche les autorisations qui ont été accordées à la connexion de cet utilisateur, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur dispose d’autorisations &quot;Lecture de tableau&quot; accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les emails, l’écran de consentement des autorisations affiche à la fois l’autorisation &quot;Lecture de tableau&quot; déjà accordée et l’autorisation &quot;Ecriture d’email&quot; nouvellement requise.

## Modules [!DNL Microsoft OneDrive for Business] et leurs champs

Lorsque vous configurez des modules [!DNL Microsoft OneDrive for Business], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Microsoft OneDrive for Business] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)

### Déclencheurs

* [[!UICONTROL Fichiers de contrôle]](#watch-files)
* [[!UICONTROL Dossiers de contrôle]](#watch-folders)

#### [!UICONTROL Fichiers de contrôle]

Ce module de déclenchement s’active lorsqu’un nouveau fichier est ajouté ou mis à jour dans un dossier contrôlé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p> Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dossiers de contrôle]

Ce module de déclenchement s’active lorsqu’un nouveau dossier est ajouté au dossier contrôlé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p> Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Télécharger un fichier]](#upload-a-file)
* [[!UICONTROL Supprimer un fichier]](#delete-a-file)
* [[!UICONTROL Obtenir un fichier]](#get-a-file)
* [[!UICONTROL Créer un dossier]](#create-a-folder)
* [[!UICONTROL Supprimer un dossier]](#delete-a-folder)
* [[!UICONTROL Obtenir un lien de partage]](#get-a-sharing-link)

#### [!UICONTROL Télécharger un fichier]

Ce module d’action charge un fichier binaire ou texte dans un dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>[!UICONTROL Source File]</p> </td> 
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

#### [!UICONTROL Supprimer un fichier]

Ce module d’action déplace le fichier spécifié vers la corbeille.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur sur lequel vous souhaitez supprimer un fichier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td> <p>Saisissez l’identifiant du fichier que vous souhaitez supprimer. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un fichier]

Ce module d’action récupère le fichier avec l’identifiant donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur à partir duquel vous souhaitez récupérer un fichier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de fichier]</td> 
   <td> <p>Saisissez l’identifiant du fichier que vous souhaitez récupérer. </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un dossier]

Crée un dossier à l’intérieur du dossier parent spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Connection]</strong> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL ID de lecteur]</strong> </td> 
   <td> <p>Sélectionnez le lecteur sur lequel vous souhaitez créer un dossier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder]</strong> </td> 
   <td> <p>Sélectionnez le dossier dans lequel vous souhaitez créer un dossier.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Nom de dossier]</strong> </td> 
   <td>Saisissez ou mappez un nom pour le nouveau dossier.</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un dossier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL Obtenir un lien de partage]

Ce module récupère un lien que vous pouvez partager pour donner accès au fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connexion de l'application du module ou du service Web à [!DNL Workfront Fusion]</a> dans l'article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Créer un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
