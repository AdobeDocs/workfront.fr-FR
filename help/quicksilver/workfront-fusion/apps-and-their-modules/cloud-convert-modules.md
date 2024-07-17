---
title: Modules CloudConvert
description: Modules CloudConvert
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3008'
ht-degree: 16%

---

# Modules [!DNL CloudConvert]

Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent CloudConvert et les connecter à plusieurs applications et services tiers. Les modules [!DNL CloudConvert] vous permettent de surveiller et de gérer des tâches, des tâches, ainsi que d’importer et d’exporter des fichiers dans votre compte [!DNL CloudConvert].

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

## Connecter [!DNL CloudConvert] à [!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

Pour connecter votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], vous devez obtenir la clé API de votre compte [!DNL CloudConvert].

1. Connectez-vous à votre compte [!DNL CloudConvert] et ouvrez votre [!UICONTROL tableau de bord].
1. Ouvrez la section **[!UICONTROL Authorization] > [!UICONTROL API Keys]** .
1. Cliquez sur **[!UICONTROL Créer une clé d’API]**.
1. Saisissez le nom de la clé API, activez les portées que vous souhaitez utiliser, puis cliquez sur **[!UICONTROL Créer]**.
1. Copiez le jeton fourni et stockez-le dans un endroit sûr.
1. Dans [!DNL Workfront Fusion], commencez à créer un scénario et ouvrez la boîte de dialogue **[!UICONTROL Créer une connexion]** du module [!DNL CloudConvert].

   Pour obtenir des instructions, voir [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Saisissez le jeton que vous avez enregistré à l’étape 5, puis cliquez sur **[!UICONTROL Continuer]** pour établir la connexion.

## Modules [!DNL CloudConvert] et leurs champs {#cloudconvert-modules-and-their-fields}

Lorsque vous configurez des modules [!DNL CloudConvert], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL CloudConvert] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Tâches courantes](#common-tasks)
* [Tâches](#jobs)
* [Tâches](#tasks)
* [Autre](#other)

### Tâches courantes

* [Capture d’un site Web](#capture-a-website)
* [[!UICONTROL Convertir un fichier]](#convert-a-file)
* [Créer une archive](#create-an-archive)
* [Fusionner les fichiers](#merge-files)
* [Optimisation d’un fichier](#optimize-a-file)

#### [!UICONTROL Capture d’un site Web]

Ce module d’action capture un site web spécifié et l’enregistre au format PDF, JPG ou PNG.

Vous spécifiez l’URL du site web et d’autres informations, telles que l’emplacement où vous souhaitez stocker les informations.

Le module renvoie l’ID du fichier et tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Saisissez l’URL du site web que vous souhaitez capturer. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format] </td> 
   <td>Indiquez si vous souhaitez enregistrer le site web capturé au format PNG, JPG ou PDF. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File Name] </td> 
   <td>Saisissez un nom de fichier (extension incluse) pour le fichier de sortie cible.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>(Facultatif) Définissez des en-têtes de requête. </p> <p>Cela s’avère utile, par exemple, lorsque l’URL spécifiée nécessite une autorisation. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Options de conversion et spécifiques au moteur] </p> </td> 
   <td>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, consultez la documentation <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> pour <code>input_format</code> et <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier] </td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertir un fichier]

Convertit un fichier dans le format de sortie sélectionné.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fichier d’entrée]</td> 
   <td>Indiquez si vous souhaitez télécharger un fichier à l’aide de [!DNL Workfront Fusion] ou fournissez l’URL à partir de laquelle le fichier sera chargé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importer un fichier à partir d’une URL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Saisissez l’URL du fichier que vous souhaitez convertir.</p> </li> 
     <li> <p><strong>[!UICONTROL Headers]</strong></p> <p>Définissez des en-têtes de requête (facultatif). Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert l’autorisation.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Format]</td> 
   <td>Indiquez si vous souhaitez spécifier le format d’entrée du fichier à convertir. Si elle n’est pas spécifiée, l’extension du fichier d’entrée est utilisée comme format d’entrée.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>Sélectionnez le format actuel du fichier.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td>Sélectionnez le format de fichier cible vers lequel vous souhaitez convertir le fichier.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL File Name]</td> 
   <td>Choisissez un nom de fichier (extension comprise) pour le fichier de sortie cible.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Options de conversion et spécifiques au moteur] </p> </td> 
   <td>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, consultez la documentation <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> pour <code>input_format</code> et <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier] </td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une archive]

Permet d’ajouter un ou plusieurs fichiers à l’archive ZIP, RAR, 7Z, TAR, TAR.GZ ou TAR.BZ2.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Input Files]</p> </td> 
   <td> <p>Spécifiez les fichiers à ajouter à l’archive.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importer un fichier à partir d’une URL]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>Saisissez l’URL du fichier que vous souhaitez archiver.</p> <p><strong>[!UICONTROL Headers]</strong> </p> <p>Définissez des en-têtes de requête (facultatif). Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert l’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p> Sélectionnez le format cible du fichier archivé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p> Saisissez le nom du fichier (extension comprise) pour le fichier de sortie cible.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Options de conversion et spécifiques au moteur] </td> 
   <td> <p>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, consultez la documentation <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> pour <code>input_format</code> et <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier]</td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fusionner les fichiers]

Fusionne au moins deux fichiers dans un PDF. Si les fichiers d’entrée ne sont pas PDF, ils sont automatiquement convertis en PDF.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Input Files]</p> </td> 
   <td> <p>Spécifiez les fichiers à fusionner.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importer un fichier à partir d’une URL]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>Saisissez l’URL du fichier que vous souhaitez archiver.</p> <p><strong>[!UICONTROL Headers]</strong> </p> <p>Définissez des en-têtes de requête (facultatif). Cela s’avère utile, par exemple, lorsque l’URL spécifiée requiert l’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format]</td> 
   <td> <p> Sélectionnez le format cible du fichier fusionné.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p> Saisissez le nom du fichier (extension comprise) pour le fichier de sortie cible.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Options de conversion et spécifiques au moteur] </td> 
   <td> <p>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, consultez la documentation <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> pour <code>input_format</code> et <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier]</td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Optimiser un fichier]

Ce module d’action optimise et compresse un fichier au format PDF, PNG ou JPG.

Vous spécifiez le fichier et les paramètres d’optimisation et de stockage.

Le module renvoie l’ID du fichier et tous les champs associés, ainsi que les valeurs et les champs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input File]</td> 
   <td>Indiquez si vous souhaitez charger un fichier à l’aide de Workfront Fusion ou fournissez l’URL à partir de laquelle le fichier sera chargé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Télécharger un fichier]</p> </td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importer un fichier à partir d’une URL] </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong> : saisissez l’URL du fichier que vous souhaitez convertir.</li> 
     <li><strong>[!UICONTROL Headers]</strong> : (facultatif) définissez des en-têtes de requête. Cela s’avère utile, par exemple, lorsque l’URL spécifiée nécessite une autorisation.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optimisation pour] </td> 
   <td> <p>Sélectionnez le profil d’optimisation en fonction des besoins spécifiques de la cible.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Web]</strong> : optimisation pour le Web (par défaut)</p> 
      <ul> 
       <li>Suppression des données redondantes et inutiles pour le web</li> 
       <li>Sous-échantillonnage, clip et compression intelligente des images</li> 
       <li>Fusion et jeux partiels de polices</li> 
       <li>Convertir les couleurs en RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Print]</strong> : optimisation pour l’impression</p> 
      <ul> 
       <li> <p>Suppression des données redondantes et inutiles pour l’impression</p> </li> 
       <li> <p>Sous-échantillonnage, clip et compression intelligente des images</p> </li> 
       <li> <p>Fusion et jeux partiels de polices</p> </li> 
       <li> <p>Convertir les couleurs en CMJN</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Archive]</strong> : optimisation à des fins d’archivage</p> 
      <ul> 
       <li> <p>Suppression des données redondantes et inutiles pour l’archivage</p> </li> 
       <li> <p>Compression intelligente des images</p> </li> 
       <li> <p>Fusion et jeux partiels de polices</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Images numérisées]</strong> : optimisation des images numérisées</p> 
      <ul> 
       <li> <p>Profil optimisé pour les PDF principalement composés d’images pixellisées</p> </li> 
       <li> <p>Compresser les images sans réduire significativement la qualité visuelle</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL réduction de taille maximale]</strong> : optimisation pour une réduction de taille maximale</p> 
      <ul> 
       <li> <p>Utiliser la compression maximale possible</p> </li> 
       <li> <p>Peut réduire la qualité visuelle</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Format d’entrée] </td> 
   <td>Sélectionnez le format du fichier d’entrée à optimiser. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td> <p>Saisissez un nom de fichier (extension incluse) pour le fichier de sortie cible.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Options de conversion et spécifiques au moteur]</td> 
   <td> <p>Spécifiez les options de conversion et spécifiques au moteur. Pour afficher les options disponibles, consultez la documentation <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> pour <code>input_format</code> et <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier]</td> 
   <td> <p>Activez cette option si vous souhaitez également inclure des données de fichier dans la sortie du module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Travaux

* [[!UICONTROL Créer une tâche (avancée)]](#create-a-job-advanced)
* [[!UICONTROL Nouvel événement de tâche]](#new-job-event)
* [[!UICONTROL Tâches de liste]](#list-jobs)
* [[!UICONTROL Obtenir une tâche]](#get-a-job)
* [[!UICONTROL Supprimer une tâche]](#delete-a-job)

#### [!UICONTROL Créer une tâche (avancée)]

Ce module crée une tâche. Une tâche peut être une ou plusieurs tâches qui sont identifiées dans le champ [!UICONTROL Nom] et liées entre elles à l’aide du champ [!UICONTROL Entrée].

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input Files]</td> 
   <td> <p>Indiquez si vous souhaitez télécharger un fichier à l’aide de [!DNL Workfront Fusion] ou fournissez l’URL à partir de laquelle le fichier sera chargé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Télécharger un fichier]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importer un fichier à partir d’une URL]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong> : saisissez l’URL du fichier que vous souhaitez traiter.</li> 
     <li><strong>[!UICONTROL Headers]</strong> : (facultatif) définissez des en-têtes de requête. Cela s’avère utile, par exemple, lorsque l’URL spécifiée nécessite une autorisation.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tasks]</p> </td> 
   <td> <p>Ajoutez les tâches qui seront exécutées dans la tâche.</p> <p>Retrouvez la description des champs des opérations dans la section correspondante.</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[!UICONTROL Convertir un fichier]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[!UICONTROL Capture d’un site web]e</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[!UICONTROL Optimiser un fichier]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[!UICONTROL Créer une archive]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[!UICONTROL Fusionner les fichiers]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Exécuter une commande]</strong> </p> <p>Pour plus d’informations sur l’exécution d’une commande, consultez la <a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert] documentation de l’API</a>.</p> </li> 
     <li> <p><strong>[!UICONTROL Exporter un fichier vers une URL temporaire]</strong> </p> <p> Indiquez le nom de la tâche et le nom de la tâche d’entrée (par exemple, Conversion).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag] </td> 
   <td> <p>Saisissez une balise . Les balises sont des chaînes arbitraires permettant d’identifier la tâche. Ils n’ont aucun effet et peuvent être utilisés pour associer la tâche à un identifiant.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une tâche]

Ce module supprime une tâche, y compris toutes les tâches et données.

>[!NOTE]
>
>Les tâches sont automatiquement supprimées 24 heures après leur fin.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de tâche]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la tâche à supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une tâche]

Ce module récupère les détails de la tâche.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de tâche]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la tâche dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tâches de liste]

Ce module récupère toutes les tâches qui ont été exécutées dans votre compte.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status] </td> 
   <td> <p>Sélectionnez l’état de la tâche en fonction de laquelle filtrer les tâches renvoyées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Définissez le nombre de tâches que Workfront Fusion 2.0 renverra au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nouvel événement de tâche]

Déclenche lorsqu’une tâche dans votre compte ou tâche est créée, terminée ou échoue.

>[!NOTE]
>
>* La tâche créée par le module [!UICONTROL Créer une tâche (avancé)] se compose de *tâches*.
>* Le déclencheur [!UICONTROL New Job Event] est également déclenché lorsqu’une tâche *individuelle* est créée, s’est terminée ou a échoué.
>

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td>Saisissez le nom du webhook. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Format] </td> 
   <td>Indiquez si vous souhaitez enregistrer le site web capturé au format PNG, JPG ou PDF. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event]</td> 
   <td>Indiquez si le module est déclenché lorsque la tâche est créée, terminée ou échouée.</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Si vous utilisez l’agrégateur de tableaux (par exemple, vous avez de nombreux fichiers dans différents formats à convertir), utilisez l’option **[!UICONTROL Je ne connais pas le format d’entrée]** dans la boîte de dialogue [!UICONTROL Ajouter une tâche]. Sinon, l’erreur est renvoyée.
>* Liaison de tâches dans la tâche (nom > entrée, nom > entrée, etc.) :
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### Tâches

* [[!UICONTROL Obtenir une tâche]](#get-a-task)
* [[!UICONTROL Télécharger un fichier]](#download-a-file)
* [[!UICONTROL Tâches de liste]](#list-tasks)
* [[!UICONTROL Réessayer une tâche]](#retry-a-task)
* [[!UICONTROL Annuler une tâche]](#cancel-a-task)
* [[!UICONTROL Supprimer une tâche]](#delete-a-task)

#### [!UICONTROL Annuler une tâche]

Ce module annule une tâche dont l’état est en attente ou en traitement.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de la tâche que vous souhaitez annuler.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une tâche]

Supprimez une tâche, y compris toutes les données.

>[!NOTE]
>
>Les tâches sont automatiquement supprimées 24 heures après leur fin.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p> Saisissez (map) l’identifiant de la tâche que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger un fichier]

Ce module récupère le nom de fichier et les données de fichier de la tâche spécifiée.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de la tâche à partir de laquelle vous souhaitez télécharger le fichier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une tâche]

Ce module récupère les détails de la tâche.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de la tâche dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tâches de liste]

Ce module récupère toutes les tâches de votre compte en fonction des paramètres de filtre.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status] </td> 
   <td> <p>Sélectionnez l’état de la tâche par laquelle filtrer les tâches renvoyées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de tâche] </td> 
   <td> <p>Saisissez ou mappez l’identifiant de tâche pour renvoyer uniquement les tâches de la tâche spécifiée.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Saisissez le type d’opération pour renvoyer uniquement les tâches avec l’opération spécifiée. </p> <p>Remarque : Utilisez le module [!UICONTROL Liste des opérations possibles] pour récupérer les opérations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Réessayer une tâche]

Ce module crée une nouvelle tâche, en fonction des paramètres (charge utile) d’une autre tâche.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Task ID]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de la tâche à partir de laquelle vous souhaitez créer une tâche.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Autre

* [[!UICONTROL Obtenir Mes Informations]](#get-my-info)
* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)

#### [!UICONTROL Obtenir Mes Informations]

Récupère les détails du compte authentifié de l’utilisateur actuel.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL CloudConvert] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Connexion [!DNL CloudConvert] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effectuer un appel API]

Permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [Fusion App] à Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à Adobe Workfront Fusion - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Saisissez un chemin relatif à <code>https://api.cloudconvert.com/</code>. Par exemple : <code>/v2/tasks</code></p> <p>Pour obtenir la liste des points de terminaison disponibles, consultez la <a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert] documentation de l’API v2</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0 ajoute les en-têtes d’autorisation pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard. Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** Tâches de liste

L’appel API suivant renvoie toutes les tâches de votre compte CloudFront :

URL : `/v2/tasks`

Méthode : `GET`

![](assets/cloudconvert-api-example-input.png)

Les correspondances de la recherche se trouvent dans la sortie du module sous [!UICONTROL Bundle] > [!UICONTROL Body] > [!UICONTROL data].

Dans notre exemple, 6 tâches ont été renvoyées :

![](assets/cloudconvert-api-example-output.png)

## Dépannage {#troubleshooting}

Consultez le tableau suivant pour connaître les erreurs possibles et leurs solutions :

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Erreur</p> </th> 
   <th>Étapes suivantes</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL La taille du fichier de sortie dépasse la limite autorisée pour votre scénario.]</span> </p> </td> 
   <td> <p>Reportez-vous aux limites de taille de fichier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL Vous avez dépassé la durée de conversion maximale.]</span> </p> </td> 
   <td> <p>Le forfait gratuit [!DNL CloudConvert] offre 25 minutes de conversion par jour. Si votre utilisation dépasse la limite du forfait gratuit, vous pouvez passer à un package (prépayé) ou à un abonnement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL Échec de lecture de la taille d’image : impossible de rechercher jusqu’à 1508. � /output/JLIADSA00137P0.mp3 : argument non valide.]</span> </p> </td> 
   <td> <p>Cette erreur est générée, par exemple lors de la conversion de fichiers du format MP3 au format WAV. Assurez-vous d’avoir sélectionné la région appropriée, car elle contient des références à des fichiers, mais pas seulement au fichier approprié.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL RuntimeError:] </p> <p><span style="font-weight: normal;">[!UICONTROL Nombre maximal de répétitions dépassé.]</span> </p> </td> 
   <td> <p>Recherchez la tâche [!DNL CloudConvert] correspondante dans la liste des tâches de votre tableau de bord [!DNL CloudConvert] et vérifiez la durée de la tâche :</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>Le délai d’expiration du module [!DNL CloudConvert] &gt; [!UICONTROL Convertir un fichier] est défini sur 3 minutes. Si la durée de la tâche dépasse 3 minutes (probablement en raison d’une surcharge temporaire du service [!DNL CloudConvert]), le module renvoie l’erreur mentionnée ci-dessus.</p> <p>Dans ce cas, envisagez l’une des options suivantes :</p> 
    <ul> 
     <li>Activez l’option <strong>[!UICONTROL Autoriser le stockage des exécutions incomplètes]</strong> dans les paramètres du scénario pour stocker les exécutions incomplètes pour une résolution manuelle ultérieure. Vous pouvez éventuellement joindre un itinéraire de gestion des erreurs au module [!DNL CloudConvert] avec la directive [!UICONTROL Break] pour résoudre automatiquement les exécutions incomplètes.</li> 
     <li>Désactivez l’option <strong>[!UICONTROL Télécharger un fichier]</strong> dans le module [!DNL CloudConvert] &gt; [!UICONTROL Convertir un fichier] . Dans ce cas, le module n’attend pas le résultat de la conversion. Pour obtenir le résultat de la conversion, créez un scénario et utilisez le déclencheur [!DNL CloudConvert] &gt; [!UICONTROL Nouvel événement de tâche].</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Exemple de workflow pour le connecteur [!DNL CloudConvert]

>[!INFO]
>
>**Exemple :** Conversion d’une vidéo au format MOV au format MP4
>
>1. Visite [https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter)
>1. Cliquez sur **[!UICONTROL Sélectionner un fichier]** et choisissez votre fichier MOV d’exemple.
>1. Cliquez sur la liste déroulante en regard de **[!UICONTROL Convertir en]** et sélectionnez **[!UICONTROL MP4]**.
>
>1. Cliquez sur l’icône **[!UICONTROL clé à molette]** .
>1. Configurez les paramètres de compression MP4 à votre convenance.
>1. Cliquez sur **[!UICONTROL Convert]**.
>1. Une fois la conversion terminée, cliquez sur **[!UICONTROL Télécharger]**.
>1. Passez en revue la vidéo convertie.
>1. Répétez les étapes 1 à 8 jusqu’à ce que vous ayez trouvé les paramètres de conversion optimaux pour l’étape 5.
>1. Visite [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
>1. Sélectionnez **[!UICONTROL mov]** pour le champ **[!UICONTROL input_format]**.
>
>1. Sélectionnez **[!UICONTROL mp4]** pour le champ **[!UICONTROL output_format]** .
>
>1. Liste de tous les paramètres possibles, tels que video_codec, crf, etc. s’affiche.
>1. Dans Workfront Fusion 2.0, insérez le module **[!UICONTROL CloudConvert]** > **[!UICONTROL Convert a File]** dans votre scénario.
>
>1. Ouvrez les paramètres du module.
>1. Configurez le module comme illustré ci-dessous :
>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. Veillez à inclure tous les paramètres dans le champ Options de conversion et spécifiques au moteur : pour chaque paramètre de l&#39;étape 5, localisez le paramètre correspondant de l&#39;étape 13 et sa valeur correspondante.
