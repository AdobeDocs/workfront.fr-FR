---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Microsoft OneDrive
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent OneDrive et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '4073'
ht-degree: 9%

---

# Modules [!DNL Microsoft OneDrive]

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL OneDrive], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créez un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
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

Pour utiliser [!DNL OneDrive] modules, vous devez disposer d’un [!DNL Microsoft OneDrive] compte .




## Connexion de la variable [!DNL OneDrive] service à [!DNL Workfront Fusion]

Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!UICONTROL Workfront Fusion], voir [Créer une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations utilisateur individuelles. Par conséquent, lors de la création d’une connexion, l’écran de consentement des autorisations affiche les autorisations qui ont été accordées à la connexion de cet utilisateur, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur dispose d’autorisations &quot;Lecture de tableau&quot; accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les emails, l’écran de consentement des autorisations affiche à la fois l’autorisation &quot;Lecture de tableau&quot; déjà accordée et l’autorisation &quot;Ecriture d’email&quot; nouvellement requise.

## Modules [!DNL Microsoft OneDrive] et leurs champs

Lorsque vous configurez des modules [!DNL OneDrive], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL OneDrive] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Fichier/Dossier](#filefolder)
* [Autre](#other)

### Fichier/Dossier

* [[!UICONTROL Fichiers/dossiers de contrôle]](#watch-filesfolders)
* [[!UICONTROL Fichiers/dossiers de recherche]](#search-filesfolders)
* [[!UICONTROL Obtention d’un fichier]](#get-a-file)
* [[!UICONTROL Téléchargement d’un fichier]](#download-a-file)
* [[!UICONTROL Chargement d’un fichier]](#upload-a-file)
* [[!UICONTROL Création d’un dossier]](#create-a-folder)
* [[!UICONTROL Obtention d’un lien de partage]](#get-a-share-link)
* [[!UICONTROL Déplacer un fichier/dossier]](#move-a-filefolder)
* [[!UICONTROL Copier un fichier]](#copy-a-file)
* [[!UICONTROL Suppression d’un fichier/dossier]](#delete-a-filefolder)

#### [!UICONTROL Fichiers/dossiers de contrôle]

Ce module de déclenchement lance un scénario lorsqu’un fichier ou un dossier est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fichiers/dossiers de contrôle]</td> 
   <td> <p>Sélectionnez le mode de contrôle des fichiers ou des dossiers :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Par Heure De Création]</b> </p> <p>Recherchez de nouveaux fichiers ou dossiers.</p> </li> 
     <li> <p><b>[!UICONTROL Par Heure De Mise À Jour]</b> </p> <p>Surveillez les fichiers ou dossiers existants mis à jour.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement à surveiller :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur que le module doit surveiller.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Accédez au dossier que le module doit surveiller. Vous pouvez également saisir une requête pour filtrer les résultats renvoyés.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Partagé Avec Moi]</b> </p> <p>Le module surveille les fichiers qui ont été partagés avec le propriétaire du lecteur.</p> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez le site SharePoint que vous souhaitez que le module regarde. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont vous souhaitez que le module regarde le lecteur.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un type d’élément]</td> 
   <td> <p>Indiquez si vous souhaitez surveiller les fichiers, les dossiers ou les deux.</p> <p>Remarque : Vous ne pouvez pas rechercher des dossiers dans un lecteur [!UICONTROL Partagé avec moi].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL Fichiers/dossiers de recherche]

Ce module de recherche renvoie les fichiers et les dossiers en fonction des critères que vous avez définis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement à rechercher :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur que le module doit rechercher.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Accédez au dossier dans lequel vous souhaitez que le module recherche. Vous pouvez également saisir une requête pour filtrer les résultats renvoyés.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Partagé Avec Moi]</b> </p> <p>Le module recherche les fichiers qui ont été partagés avec le propriétaire du lecteur.</p> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez la variable [!DNL SharePoint] Site sur lequel vous souhaitez que le module effectue une recherche. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont vous souhaitez que le module effectue la recherche.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisir un type d’élément]</td> 
   <td> <p>Indiquez si vous souhaitez rechercher des fichiers, des dossiers ou les deux.</p> <p>Remarque : Vous ne pouvez pas rechercher des dossiers dans un lecteur [!UICONTROL Partagé avec moi].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un fichier]

Ce module d’action récupère les métadonnées d’un fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrée (ID du fichier et chemin du fichier)]</td> 
   <td>Indiquez si vous souhaitez identifier le fichier par identifiant de fichier ou par chemin d’accès au fichier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrez un ID de fichier] / [!UICONTROL Chemin du fichier]</td> 
   <td> <p>Sélectionnez le mode de saisie de l’identifiant de fichier ou du chemin d’accès au fichier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrée Manuelle]</b> </p> <p>Sélectionnez cette option si vous souhaitez saisir directement l’identifiant ou le chemin d’accès, ou le mapper à partir d’un module précédent.</p> </li> 
     <li> <p><b>[!UICONTROL Effectuer une sélection dans une liste]</b> </p> <p>Sélectionnez cette option si vous souhaitez effectuer une sélection dans une liste de fichiers ou chemins disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement à rechercher :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur contenant le fichier que vous souhaitez obtenir.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez le site SharePoint qui contient le fichier que vous souhaitez obtenir. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont le lecteur contient le fichier que vous souhaitez obtenir.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez ou mappez le lecteur contenant le fichier que vous souhaitez obtenir. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Si vous avez sélectionné [!UICONTROL Entrer manuellement], saisissez ou mappez l’identifiant ou le chemin d’accès du fichier que vous souhaitez obtenir.</p> <p>Si vous avez sélectionné [!UICONTROL Sélectionner dans la liste], sélectionnez le fichier que vous souhaitez obtenir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Téléchargement d’un fichier]

Ce module d’action télécharge le fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrée (ID du fichier et chemin du fichier)]</td> 
   <td>Indiquez si vous souhaitez identifier le fichier par identifiant de fichier ou par chemin d’accès au fichier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Saisissez un ID de fichier/un chemin d’accès au fichier.</td> 
   <td> <p>Sélectionnez le mode de saisie de l’identifiant de fichier ou du chemin d’accès au fichier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrée Manuelle]</b> </p> <p>Sélectionnez cette option si vous souhaitez saisir directement l’identifiant ou le chemin d’accès, ou le mapper à partir d’un module précédent.</p> </li> 
     <li> <p><b>[!UICONTROL Effectuer une sélection dans une liste]</b> </p> <p>Sélectionnez cette option si vous souhaitez effectuer une sélection dans une liste de fichiers ou chemins disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement contenant le fichier à télécharger :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur contenant le fichier que vous souhaitez télécharger.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez le site SharePoint qui contient le fichier que vous souhaitez télécharger. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont le lecteur contient le fichier que vous souhaitez télécharger.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez ou mappez le lecteur contenant le fichier que vous souhaitez télécharger. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Si vous avez sélectionné [!UICONTROL Entrer manuellement], saisissez ou mappez l’identifiant ou le chemin du fichier à télécharger.</p> <p>Si vous avez sélectionné [!UICONTROL Sélectionner dans la liste], sélectionnez le fichier à télécharger.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Convertir en PDF]</td> 
   <td> <p>Activez cette option pour convertir le fichier en fichier de PDF. Vous pouvez effectuer une conversion à partir des types de fichiers suivants :</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>POT</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chargement d’un fichier]

Ce module d’action charge un fichier dans le dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Entrée (ID et chemin d’accès de l’emplacement du dossier)</td> 
   <td>Indiquez si vous souhaitez identifier le dossier cible par identifiant ou par chemin d’accès.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement où vous souhaitez charger un fichier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Sélectionnez le lecteur contenant le fichier que vous souhaitez obtenir.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez la variable [!DNL SharePoint] Site contenant le dossier dans lequel vous souhaitez charger un fichier. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont le lecteur contient le dossier dans lequel vous souhaitez charger un fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur contenant le dossier dans lequel vous souhaitez charger un fichier. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Si le fichier portant le même nom existe]</td> 
   <td>Sélectionnez le mode de traitement si un fichier portant le même nom existe déjà.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Ajoutez une description au fichier téléchargé.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un dossier]

Ce module d’action crée un dossier dans le lecteur spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement où vous souhaitez créer un dossier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Sélectionnez le lecteur sur lequel vous souhaitez créer un dossier.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez la variable [!DNL SharePoint] Emplacement où vous souhaitez créer un dossier. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe propriétaire du lecteur dans lequel vous souhaitez créer un dossier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez le lecteur sur lequel vous souhaitez créer un dossier. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Si vous souhaitez que le nouveau dossier soit un sous-dossier, accédez au dossier dans lequel vous souhaitez qu’il soit un sous-dossier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New Folder Name]</td> 
   <td> <p>Saisissez ou mappez un nom pour le nouveau dossier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Si le dossier portant le même nom existe]</td> 
   <td>Sélectionnez le mode de traitement si un fichier portant le même nom existe déjà.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un lien de partage]

Ce module d’action renvoie un lien de partage pour le fichier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrée (ID du fichier et chemin du fichier)]</td> 
   <td>Indiquez si vous souhaitez identifier le fichier par identifiant de fichier ou par chemin d’accès au fichier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrez un ID de fichier] / [!UICONTROL Chemin du fichier]</td> 
   <td> <p>Sélectionnez le mode de saisie de l’identifiant de fichier ou du chemin d’accès au fichier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrée Manuelle]</b> </p> <p>Sélectionnez cette option si vous souhaitez saisir directement l’identifiant ou le chemin d’accès, ou le mapper à partir d’un module précédent.</p> </li> 
     <li> <p><b>[!UICONTROL Effectuer une sélection dans une liste]</b> </p> <p>Sélectionnez cette option si vous souhaitez effectuer une sélection dans une liste de fichiers ou chemins disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement pour lequel vous souhaitez récupérer un lien de partage :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur contenant le fichier pour lequel vous souhaitez récupérer un lien de partage.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez le site SharePoint contenant le fichier pour lequel vous souhaitez récupérer un lien de partage. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont le lecteur contient le fichier pour lequel vous souhaitez récupérer un lien de partage.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez ou mappez le lecteur contenant le fichier pour lequel vous souhaitez récupérer un lien de partage. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Si vous avez sélectionné [!UICONTROL Entrer manuellement], saisissez ou mappez l’identifiant ou le chemin du fichier pour lequel vous souhaitez récupérer un lien de partage.</p> <p>Si vous avez sélectionné [!UICONTROL Sélectionner] dans la liste, sélectionnez le fichier pour lequel vous souhaitez récupérer un lien de partage.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’autorisation]</td> 
   <td> <p>Indiquez si vous souhaitez que les personnes disposant du lien puissent lire et écrire dans le fichier, ou pour lire uniquement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scope]</td> 
   <td>Indiquez si vous souhaitez que le fichier soit disponible pour toute personne disposant du lien ou uniquement pour les membres de votre organisation disposant du lien.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un fichier/dossier]

Ce module d’action déplace un fichier ou un dossier vers un nouvel emplacement de dossier

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrée (ID du fichier et chemin du fichier)]</td> 
   <td>Indiquez si vous souhaitez identifier le fichier par identifiant de fichier ou par chemin d’accès au fichier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrez un ID de fichier/chemin d’accès au fichier]</td> 
   <td> <p>Sélectionnez le mode de saisie de l’identifiant de fichier ou du chemin d’accès au fichier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrée Manuelle]</b> </p> <p>Sélectionnez cette option si vous souhaitez saisir directement l’identifiant ou le chemin d’accès, ou le mapper à partir d’un module précédent.</p> </li> 
     <li> <p><b>[!UICONTROL Effectuer une sélection dans une liste]</b> </p> <p>Sélectionnez cette option si vous souhaitez effectuer une sélection dans une liste de fichiers ou chemins disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement contenant le fichier ou le dossier à déplacer :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur contenant le fichier ou le dossier à déplacer.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez la variable [!DNL SharePoint] Site contenant le fichier ou le dossier à déplacer. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont le lecteur contient le fichier ou le dossier que vous souhaitez déplacer.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez ou mappez le lecteur contenant le fichier ou le dossier à déplacer. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sélectionnez [!UICONTROL File/Folder]</td> 
   <td>Indiquez si vous souhaitez déplacer un fichier ou un dossier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> <p role="rowheader">[!UICONTROL Folder] / [!UICONTROL Folder ID] / [!UICONTROL Folder Path]</p> </td> 
   <td> <p>Si vous avez sélectionné [!UICONTROL Entrer manuellement], saisissez ou mappez l’identifiant ou le chemin d’accès du fichier ou du dossier que vous souhaitez déplacer.</p> <p>Si vous avez sélectionné [!UICONTROL Sélectionner] dans la liste, sélectionnez le fichier ou le dossier à déplacer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer un nouvel emplacement de dossier]</td> 
   <td> <p>Sélectionnez le mode de saisie de l’emplacement vers lequel vous souhaitez déplacer le fichier ou le dossier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrée Manuelle]</b> </p> <p>Sélectionnez cette option si vous souhaitez saisir directement l’identifiant ou le chemin d’accès, ou le mapper à partir d’un module précédent.</p> </li> 
     <li> <p><b>[!UICONTROL Effectuer une sélection dans une liste]</b> </p> <p>Sélectionnez cette option si vous souhaitez effectuer une sélection dans une liste de fichiers ou chemins disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement où déplacer le fichier ou le dossier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur sur lequel vous souhaitez déplacer le fichier ou le dossier.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez la variable [!DNL SharePoint] Emplacement où vous souhaitez déplacer le fichier ou le dossier. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe sur lequel vous souhaitez déplacer le fichier ou le dossier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez ou mappez le lecteur contenant le dossier vers lequel vous souhaitez déplacer le fichier ou le dossier. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> <p>Si vous laissez ce champ vide, le fichier ou le dossier ne peut être déplacé que dans le même [!DNL OneDrive].</p> <p>Vous pouvez déplacer des fichiers et des dossiers de [!UICONTROL Mon lecteur] vers un [!UICONTROL Lecteur du site] ou un [!UICONTROL Lecteur du groupe]. </p> <p>Vous pouvez déplacer des fichiers d’un [!UICONTROL Site's Drive] uniquement vers le même lecteur du même site.</p> <p>Vous pouvez déplacer des fichiers d’un [!UICONTROL Group] uniquement vers le même lecteur du même groupe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Saisissez ou mappez le dossier dans lequel vous souhaitez déplacer le fichier ou le dossier.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier un fichier]

Ce module d’action copie un fichier dans un nouvel emplacement de dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrée (ID du fichier et chemin du fichier)]</td> 
   <td>Indiquez si vous souhaitez identifier le fichier par identifiant de fichier ou par chemin d’accès au fichier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrez un ID de fichier] / [!UICONTROL Chemin du fichier]</td> 
   <td> <p>Sélectionnez le mode de saisie de l’identifiant de fichier ou du chemin d’accès au fichier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrée Manuelle]</b> </p> <p>Sélectionnez cette option si vous souhaitez saisir directement l’identifiant ou le chemin d’accès, ou le mapper à partir d’un module précédent.</p> </li> 
     <li> <p><b>[!UICONTROL Effectuer une sélection dans une liste]</b> </p> <p>Sélectionnez cette option si vous souhaitez effectuer une sélection dans une liste de fichiers ou chemins disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement contenant le fichier à copier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur contenant le fichier ou le dossier à copier.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez le site SharePoint qui contient le fichier à déplacer. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont le lecteur contient le fichier que vous souhaitez copier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez ou mappez le lecteur contenant le fichier à copier. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> </td> 
   <td> <p>Si vous avez sélectionné [!UICONTROL Entrer manuellement], saisissez ou mappez l’identifiant ou le chemin d’accès du fichier à copier.</p> <p>Si vous avez sélectionné [!UICONTROL Sélectionner] dans la liste, sélectionnez le fichier à copier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer un nouvel emplacement de dossier]</td> 
   <td> <p>Sélectionnez le mode de saisie de l’emplacement où vous souhaitez copier le fichier ou dans :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrée Manuelle]</b> </p> <p>Sélectionnez cette option si vous souhaitez saisir directement l’identifiant ou le chemin d’accès, ou le mapper à partir d’un module précédent.</p> </li> 
     <li> <p><b>[!UICONTROL Effectuer une sélection dans une liste]</b> </p> <p>Sélectionnez cette option si vous souhaitez effectuer une sélection dans une liste de dossiers disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouvel emplacement OneDrive]</td> 
   <td> <p>Sélectionnez l’emplacement où vous souhaitez copier le filtre. Cette option est disponible si vous choisissez de sélectionner le nouvel emplacement du dossier dans une liste.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur sur lequel vous souhaitez copier le fichier.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez la variable [!DNL SharePoint] Emplacement où vous souhaitez copier le fichier. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe sur lequel vous souhaitez copier le fichier.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez ou mappez le lecteur contenant le dossier dans lequel vous souhaitez copier le fichier. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> <p>Si vous laissez ce champ vide, le fichier ou le dossier ne peut être copié que dans le même [!UICONTROL OneDrive].</p> <p>Vous pouvez copier des fichiers et des dossiers de [!UICONTROL Mon lecteur] vers un [!UICONTROL Lecteur du site] ou un [!UICONTROL Lecteur du groupe]. </p> <p>Vous pouvez copier des fichiers d’un [!UICONTROL Site's Drive] uniquement vers le même lecteur du même site.</p> <p>Vous pouvez copier des fichiers d’un [!UICONTROL Group] uniquement vers le même lecteur du même groupe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Saisissez ou mappez le dossier dans lequel vous souhaitez déplacer la copie ou le dossier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouveau nom de fichier copié]</td> 
   <td> <p>Saisissez ou mappez un nom pour la nouvelle copie du fichier. Vous pouvez laisser ce champ vide si vous ne souhaitez pas modifier le nom de fichier d’origine.</p> <p>Le nom doit inclure l’extension du fichier. Exemple :<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un fichier/dossier]

Ce module d&#39;action supprime le fichier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrée (File/Folder ID &amp; Path)]</td> 
   <td>Indiquez si vous souhaitez identifier le fichier par identifiant de fichier ou par chemin d’accès au fichier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrez un ID de fichier/dossier /Saisissez un Chemin de fichier/dossier]</td> 
   <td> <p>Sélectionnez le mode de saisie de l’identifiant de fichier ou du chemin d’accès au fichier :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrée Manuelle]</b> </p> <p>Sélectionnez cette option si vous souhaitez saisir directement l’identifiant ou le chemin d’accès, ou le mapper à partir d’un module précédent.</p> </li> 
     <li> <p><b>[!UICONTROL Effectuer une sélection dans une liste]</b> </p> <p>Sélectionnez cette option si vous souhaitez effectuer une sélection dans une liste de fichiers ou chemins disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choisissez votre [!DNL OneDrive] location]</td> 
   <td> <p>Sélectionnez l’emplacement à rechercher :</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mon lecteur]</b> </p> <p>Indiquez si le module doit entrer un identifiant de lecteur.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Oui]</b> </p> <p>Saisissez l’identifiant du lecteur qui contient le fichier ou le dossier que vous souhaitez supprimer.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Lecteur du site]</b> </p> <p>Sélectionnez la variable [!DNL SharePoint] Site contenant le fichier ou le dossier à supprimer. Les sites disponibles sont Sites, suivis par l’utilisateur connecté.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Sélectionnez le groupe dont le lecteur contient le fichier ou le dossier que vous souhaitez supprimer.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Sélectionnez ou mappez le lecteur qui contient le fichier ou le dossier à supprimer. Ce champ n’est pas disponible si vous avez sélectionné [!UICONTROL Non] dans le champ [!UICONTROL Activer pour entrer un identifiant de lecteur] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sélectionnez [!UICONTROL File/Folder]</td> 
   <td>Indiquez si vous souhaitez supprimer un fichier ou un dossier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Si vous avez sélectionné [!UICONTROL Entrer manuellement], saisissez ou mappez l’identifiant ou le chemin d’accès du fichier à supprimer.</p> <p>Si vous avez sélectionné [!UICONTROL Sélectionner] dans la liste, sélectionnez le fichier à supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

#### [!UICONTROL Lancer un appel API]

Ce module effectue un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL OneDrive] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez un chemin relatif à <code>https://graph.microsoft.com</code>. Exemple :<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute les en-têtes d’autorisation à votre place.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
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



## Si vous ne parvenez pas à charger ou mettre à jour un fichier

Plusieurs problèmes peuvent se produire lors de l’échec du téléchargement ou de la mise à jour d’un fichier :

* Le fichier téléchargé est trop volumineux et dépasse la taille maximale autorisée pour votre [!DNL OneDrive] planifiez ou vous avez utilisé l’ensemble de vos [!DNL OneDrive] quota de stockage du compte. Pour obtenir plus d’espace de stockage, supprimez les fichiers existants de [!DNL OneDrive] ou mettez à niveau votre [!DNL OneDrive] compte .
* OneDrive ne permet pas de charger deux fichiers portant le même nom dans un seul dossier. Si le dossier cible contient un fichier portant le même nom que le fichier téléchargé, l’exécution du scénario s’arrête avec une erreur. La solution consiste à simplement renommer le fichier en cours de chargement. Si vous souhaitez mettre à jour un fichier, utilisez la variable [!UICONTROL Mettre à jour un fichier] action.
* Le dossier précédemment sélectionné, vers lequel le fichier est chargé, n’existe plus. Le scénario s’arrête et vous devrez sélectionner à nouveau le dossier cible.
