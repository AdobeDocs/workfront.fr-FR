---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules FTP
description: Les modules FTP vous permettent de surveiller les modifications de fichier dans un dossier sélectionné, de charger de nouveaux fichiers dans le dossier souhaité et de modifier ou supprimer des fichiers existants qui se trouvent déjà dans un dossier.
author: Becky
feature: Workfront Fusion
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---

# Modules FTP

Les modules FTP vous permettent de surveiller les modifications de fichier dans un dossier sélectionné, de charger de nouveaux fichiers dans le dossier souhaité et de modifier ou supprimer des fichiers existants qui se trouvent déjà dans un dossier.

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

## Conditions préalables

Pour utiliser [Application de fusion] avec [!DNL Workfront Fusion], vous devez disposer d’un compte FTP.

## Création d’une connexion dans un module FTP {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nom de la connexion]</td> 
   <td> <p> Saisissez le nom de votre connexion FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Host] </td> 
   <td> <p>Saisissez le nom d’hôte du serveur FTP. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Port] </td> 
   <td> <p>Saisissez le numéro de port du serveur FTP. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom d’utilisateur] </td> 
   <td> <p>Saisissez le nom d’utilisateur de votre compte FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Password] </td> 
   <td> <p>Saisissez le mot de passe de votre compte FTP.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utiliser une connexion sécurisée (TLS)</p> </td> 
   <td> <p>Indiquez si vous souhaitez utiliser une connexion sécurisée.</p> <p style="font-weight: bold;">[!UICONTROL No]</p> <p>La connexion n’est pas sécurisée.</p> <p style="font-weight: bold;">[!UICONTROL Cryptage explicite ou cryptage implicite]</p> <p>La connexion est sécurisée à l’aide de SSL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Rejeter les certificats non autorisés]</p> </td> 
   <td> <p>Activez cette option pour vérifier le certificat du serveur FTP. Si la vérification échoue, la connexion ne sera pas créée. Pour réussir la vérification, le certificat doit répondre à l’un des critères suivants :</p> 
    <ul> 
     <li>être signé par une racine <a href="https://en.wikipedia.org/wiki/Certificate_authority">Autorité de certification</a></li> 
     <li>être signé par une autorité de certification intermédiaire (voir par exemple <a href="https://knowledge.digicert.com/solution/SO16297.html">Fonctionnement des chaînes de certificats</a> pour plus d’informations). Dans ce cas, tous les certificats intermédiaires doivent être installés sur le serveur FTP.</li> 
     <li>être un certificat auto-signé fourni dans le champ [!UICONTROL Auto-signé certificate] (voir ci-dessous) ;</li> </ul>

Si cette option est désactivée, le certificat du serveur FTP n’est pas vérifié. Nous vous déconseillons vivement de désactiver cette option, car elle risque d&#39;insécurité de la connexion et de présenter un risque de sécurité élevé.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL Certificat auto-signé]</p> </td> 
   <td> <p>Cliquez sur le bouton <b>[!UICONTROL Extraction]</b> pour ouvrir la boîte de dialogue de téléchargement.</p> <p>Téléchargez le certificat pour utiliser le TLS avec votre certificat auto-signé. [!DNL Workfront Fusion] ne conserve ni ne stocke les données que vous fournissez, telles que les fichiers et les mots de passe. Le fichier et le mot de passe sont utilisés uniquement pour extraire le certificat.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modules FTP et leurs champs

* [Triggers](#triggers)
* [Actions](#actions)

### Triggers

#### [!UICONTROL Fichiers de contrôle]

[!UICONTROL Fichiers de contrôle] est le seul module de déclenchement pour FTP. Il contrôle le contenu du fichier du dossier sélectionné. Le déclencheur est exécuté lorsqu’un nouveau fichier est inséré dans le dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#create-a-connection" class="MCXref xref">[!UICONTROL Créer une connexion] dans un module FTP</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Sélectionnez le dossier que vous souhaitez voir.</p> <p><b>Remarque :</b> Un seul dossier par scénario est autorisé. Les sous-dossiers sont ignorés.</p> <p><b>Conseil :</b> Pour effectuer le suivi de plusieurs dossiers, créez un scénario indépendant pour chacun d’eux.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de fichiers renvoyés] </td> 
   <td> <p>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle. Si la valeur est définie sur une valeur trop élevée, la connexion peut être interrompue du côté du service tiers donné (délai d’expiration). [!DNL Workfront Fusion] n'a aucune influence sur cela. Nous vous recommandons de définir une valeur inférieure et de définir une valeur supérieure pour le nombre maximal de cycles ou d’exécuter le scénario plus fréquemment.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Modification des autorisations]](#change-permissions)
* [[!UICONTROL Création d’un dossier]](#create-a-folder)
* [[!UICONTROL Suppression d’un fichier]](#delete-a-file)
* [[!UICONTROL Suppression d’un dossier]](#delete-a-folder)
* [[!UICONTROL Obtention d’un fichier]](#get-a-file)
* [[!UICONTROL Liste des fichiers dans un dossier]](#list-of-files-in-a-folder)
* [[!UICONTROL Déplacer un fichier ou un dossier]](#move-a-file-or-folder)
* [[!UICONTROL Télécharger] un fichier](#upload-a-file)

#### [!UICONTROL Modification des autorisations]

Ce module d’action modifie les paramètres d’autorisation d’un fichier ou d’un dossier.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Créer une connexion] dans un module FTP</a> dans cet article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Modifier les paramètres d’autorisation de]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>Indiquez si vous souhaitez modifier les paramètres d’un fichier ou d’un dossier.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Chemin du fichier]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Entrez ou mappez le chemin d’accès au fichier avec le dossier ou le fichier.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Permissions]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Définissez les autorisations de fichier ou de dossier de votre choix. Utilisez les paramètres chmod . Par exemple : <code>777 </code>ou <code>-rwxrwxrwx</code>.</p>
               <p>Les autorisations doivent correspondre au modèle <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Création d’un dossier]

Ce module d’action crée un dossier.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Créer une connexion] dans un module FTP</a> dans cet article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Chemin du dossier]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Entrez ou mappez le chemin du fichier avec le nouveau dossier.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Nouveau nom du dossier]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>Saisissez ou mappez un nom pour le nouveau dossier.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Suppression d’un fichier]

Supprime un fichier du dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Créer une connexion] dans un module FTP</a> dans cet article.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier FTP dans lequel vous souhaitez supprimer un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom du fichier]</td> 
   <td> <p> Saisissez le nom du fichier, y compris son extension. Exemple: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un dossier]

Ce module d’action supprime définitivement le dossier spécifié.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Créer une connexion] dans un module FTP</a> dans cet article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Folder]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>Sélectionnez le dossier FTP dans lequel vous souhaitez supprimer un fichier.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Obtention d’un fichier]

Récupère un fichier du serveur FTP qui peut être traité ultérieurement, par exemple transféré vers le [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#creating-the-ftp-connection" class="MCXref xref">Création de la connexion FTP</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Chemin du fichier]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez obtenir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Liste des fichiers dans un dossier]

Récupère les informations sur le fichier et/ou le dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#creating-the-ftp-connection" class="MCXref xref">Création de la connexion FTP</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier FTP dans lequel vous souhaitez effectuer une recherche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Afficher] </td> 
   <td> <p>Indiquez si vous souhaitez récupérer des informations sur les fichiers ou les dossiers, ou les deux.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Saisissez le terme à rechercher. Si aucun terme de recherche n’est saisi, tous les fichiers et dossiers du dossier spécifié seront récupérés.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de fichiers renvoyés]</td> 
   <td> <p> Définissez le nombre maximal de fichiers récupérés par ce module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un fichier ou un dossier]

Ce module d’action déplace un fichier ou un dossier vers un autre emplacement.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Créer une connexion] dans un module FTP</a> dans cet article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Ancien chemin d’accès au fichier]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>Saisissez le chemin d’accès à partir duquel vous souhaitez déplacer le fichier. Exemple: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Nouveau chemin d’accès au fichier]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>Saisissez le chemin vers lequel vous souhaitez déplacer le fichier. Exemple: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL Chargement d’un fichier]

Télécharge un fichier sur le serveur FTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#creating-the-ftp-connection" class="MCXref xref">Création de la connexion FTP</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier FTP vers lequel vous souhaitez transférer le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fichier source] </td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ajouter à un fichier existant]</td> 
   <td> <p>Si cette option est activée et que le fichier existe déjà sur le serveur FTP, le contenu du fichier est ajouté au fichier existant. Si cette option n’est pas activée, le contenu du fichier est remplacé.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Créer des dossiers s’ils n’existent pas] </td> 
   <td> <p>Si cette option est activée et que le dossier que vous avez entré dans le champ Dossier n’existe pas sur le serveur FTP, le module crée le dossier.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dépannage {#troubleshooting}

Si vous rencontrez des problèmes avec l’application FTP pendant la création de la connexion ou le fonctionnement d’un module, essayez d’utiliser l’un des clients FTP les plus courants et essayez d’effectuer la même action (par exemple, créer une connexion ou lister des fichiers dans un dossier). avec le client FTP. Si vous rencontrez les mêmes problèmes avec le client FTP, la raison peut être une mauvaise configuration du serveur FTP.
