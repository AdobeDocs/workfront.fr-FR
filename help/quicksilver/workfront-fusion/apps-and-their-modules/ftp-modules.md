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
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 97%

---

# Modules FTP

Les modules FTP vous permettent de surveiller les modifications de fichier dans un dossier sélectionné, de charger de nouveaux fichiers dans le dossier souhaité et de modifier ou supprimer des fichiers existants qui se trouvent déjà dans un dossier.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [Application de fusion] avec [!DNL Workfront Fusion], vous devez disposer d’un compte FTP.

## Créer une connexion dans un module FTP {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection name]</td> 
   <td> <p> Saisissez le nom de votre connexion FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Host] </td> 
   <td> <p>Saisissez le nom d’hôte du serveur FTP. Par exemple : <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Port] </td> 
   <td> <p>Saisissez le numéro de port du serveur FTP. Par exemple : <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User name] </td> 
   <td> <p>Saisissez le nom d’utilisateur ou d’utilisatrice de votre compte FTP.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Password] </td> 
   <td> <p>Saisissez le mot de passe de votre compte FTP.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Utiliser une connexion sécurisée (TLS)</p> </td> 
   <td> <p>Indiquez si vous souhaitez utiliser une connexion sécurisée.</p> <p style="font-weight: bold;">[!UICONTROL No]</p> <p>La connexion n’est pas sécurisée.</p> <p style="font-weight: bold;">[!UICONTROL Explicit encryption or Implicit encryption]</p> <p>La connexion est sécurisée à l’aide de SSL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Reject unauthorized certificates]</p> </td> 
   <td> <p>Activez cette option pour vérifier le certificat du serveur FTP. Si la vérification échoue, la connexion ne sera pas créée. Pour réussir la vérification, le certificat doit répondre à l’un des critères suivants :</p> 
    <ul> 
     <li>être signé par une <a href="https://fr.wikipedia.org/wiki/Autorité_de_certification">Autorité de certification émettant des certificats racines</a></li> 
     <li>être signé par une autorité de certification intermédiaire (voir par exemple <a href="https://knowledge.digicert.com/solution/SO16297.html">Fonctionnement des chaînes de certification</a> pour plus d’informations). Dans ce cas, tous les certificats intermédiaires doivent être installés sur le serveur FTP.</li> 
     <li>être un certificat auto-signé fourni dans le champ [!UICONTROL Self-signed certificate] (voir ci-dessous)</li> </ul>

Si cette option est désactivée, le certificat du serveur FTP n’est pas vérifié. Nous vous déconseillons vivement de désactiver cette option, car elle rend la connexion non sécurisée et pose un risque sérieux pour la sécurité.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL Self-signed certificate]</p> </td> 
   <td> <p>Cliquez sur le bouton <b>[!UICONTROL Extract]</b> pour ouvrir la boîte de dialogue de chargement.</p> <p>Chargez le certificat pour utiliser le TLS avec votre certificat auto-signé. [!DNL Workfront Fusion] ne conserve ni ne stocke les données que vous fournissez, telles que les fichiers et les mots de passe. Le fichier et le mot de passe sont utilisés uniquement pour extraire le certificat.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Modules FTP et leurs champs

* [Déclencheurs](#triggers)
* [Actions](#actions)

### Déclencheurs

#### [!UICONTROL Contrôle des fichiers]

[!UICONTROL Contrôle des fichiers] est le seul module déclencheur pour FTP. Il contrôle le contenu du fichier du dossier sélectionné. Le déclencheur est exécuté lorsqu’un nouveau fichier est inséré dans le dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#create-a-connection" class="MCXref xref">[!UICONTROL Create a connection] dans un module FTP</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Sélectionnez le dossier que vous souhaitez consulter.</p> <p><b>Remarque :</b> un seul dossier est autorisé par scénario. Les sous-dossiers sont ignorés.</p> <p><b>Conseil :</b> pour effectuer le suivi de plusieurs dossiers, créez un scénario indépendant pour chacun d’eux.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned files] </td> 
   <td> <p>Définissez le nombre maximal de résultats avec lesquels [!DNL Workfront Fusion] fonctionnera pendant un cycle. Si la valeur est définie sur une valeur trop élevée, la connexion peut être interrompue du côté du service tiers donné (délai d’expiration). [!DNL Workfront Fusion] n’a aucune influence sur cela. Nous vous recommandons de définir une valeur inférieure et de définir une valeur supérieure pour le nombre maximal de cycles ou d’exécuter le scénario plus fréquemment.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Modifier les autorisations]](#change-permissions)
* [[!UICONTROL Créer un dossier]](#create-a-folder)
* [[!UICONTROL Supprimer un fichier]](#delete-a-file)
* [[!UICONTROL Supprimer un dossier]](#delete-a-folder)
* [[!UICONTROL Obtenir un fichier]](#get-a-file)
* [[!UICONTROL Liste des fichiers dans un dossier]](#list-of-files-in-a-folder)
* [[!UICONTROL Déplacer un fichier ou un dossier]](#move-a-file-or-folder)
* [[!UICONTROL Charger] un fichier](#upload-a-file)

#### [!UICONTROL Modifier des autorisations]

Ce module d’action modifie les paramètres d’autorisation d’un fichier ou d’un dossier.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] dans un module FTP</a> dans cet article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Change permission settings of]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>Indiquez si vous souhaitez modifier les paramètres d’un fichier ou d’un dossier.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL File path]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Entrez ou mappez le chemin d’accès au fichier sur le dossier ou le fichier.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Permissions]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Définissez les autorisations de fichier ou de dossier de votre choix. Utilisez les paramètres chmod. Par exemple, saisissez <code>777 </code> ou <code>-rwxrwxrwx</code>.</p>
               <p>Les autorisations doivent correspondre au motif <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Créer un dossier]

Ce module d’action crée un dossier.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] dans un module FTP</a> dans cet article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Folder path]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Entrez ou mappez le chemin du fichier sur le nouveau dossier.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL New folder name]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>Saisissez ou mappez un nom pour le nouveau dossier.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Supprimer un fichier]

Supprime un fichier du dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] dans un module FTP</a> dans cet article.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier FTP dans lequel vous souhaitez supprimer un fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td> <p> Saisissez le nom du fichier, y compris son extension de nom de fichier. Exemple : <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un dossier]

Ce module d’action supprime définitivement le dossier spécifié.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] dans un module FTP</a> dans cet article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Folder]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>Sélectionnez le dossier FTP dans lequel vous souhaitez supprimer un fichier.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Obtenir un fichier]

Récupère un fichier du serveur FTP qui peut être traité ultérieurement, par exemple transféré vers [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#creating-the-ftp-connection" class="MCXref xref">Créer la connexion FTP</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File path]</td> 
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
   <td> <p>Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#creating-the-ftp-connection" class="MCXref xref">Créer la connexion FTP</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier FTP dans lequel vous souhaitez effectuer une recherche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Indiquez si vous souhaitez récupérer des informations sur les fichiers ou les dossiers, ou les deux.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Saisissez le terme de recherche. Si aucun terme de recherche n’est saisi, tous les fichiers et dossiers du dossier spécifié seront récupérés.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned files]</td> 
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
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] dans un module FTP</a> dans cet article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Old file path]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>Saisissez le chemin d’accès à partir duquel vous souhaitez déplacer le fichier. Exemple : <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL New file path]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>Saisissez le chemin vers lequel vous souhaitez déplacer le fichier. Exemple : <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL Charger un fichier]

Charge un fichier sur le serveur FTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Pour plus d’informations sur l’établissement d’une connexion au compte FTP, voir <a href="#creating-the-ftp-connection" class="MCXref xref">Créer la connexion FTP</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Sélectionnez le dossier FTP dans lequel vous souhaitez charger le fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file] </td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Append to an already existing file]</td> 
   <td> <p>Si cette option est activée et que le fichier existe déjà sur le serveur FTP, le contenu du fichier est ajouté au fichier existant. Si cette option n’est pas activée, le contenu du fichier est remplacé.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create folders if don't exist] </td> 
   <td> <p>Si cette option est activée et que le dossier que vous avez entré dans le champ Dossier n’existe pas sur le serveur FTP, le module crée ce dossier.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dépannage {#troubleshooting}

Si vous rencontrez des problèmes avec l’application FTP pendant la création de la connexion ou l’opération d’un module, essayez d’utiliser l’un des clients FTP les plus courants et d’effectuer la même action (par exemple, créer une connexion ou répertorier des fichiers dans un dossier). avec le client FTP. Si vous rencontrez les mêmes problèmes avec le client FTP, la cause peut être une mauvaise configuration du serveur FTP.
