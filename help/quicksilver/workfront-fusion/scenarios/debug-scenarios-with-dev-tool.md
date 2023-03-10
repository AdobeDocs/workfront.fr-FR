---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Débogage des scénarios avec l’outil de développement de fusion Adobe Workfront
description: Adobe Workfront Fusion DevTool vous permet de comprendre et de résoudre les problèmes liés aux scénarios. DevTool ajoute un panneau supplémentaire aux outils de développement Chrome. Grâce à ce panneau du débogueur, vous pouvez vérifier toutes les exécutions manuelles de votre scénario, passer en revue toutes les opérations effectuées et afficher les détails de chaque appel API effectué. Vous pouvez voir quel module, opération ou réponse unique a provoqué l’erreur et utiliser ces connaissances pour affiner votre scénario.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 3d5b9e178cc3222523b558e3c6717ce54f322ff9
workflow-type: tm+mt
source-wordcount: '1659'
ht-degree: 0%

---

# Déboguer les scénarios à l’aide de la méthode [!DNL Adobe Workfront Fusion] DevTool

Le [!DNL Adobe Workfront Fusion] DevTool vous permet de comprendre et de résoudre les problèmes liés aux scénarios. DevTool ajoute un panneau supplémentaire à la variable [!DNL Chrome Developer Tools]. Grâce à ce panneau du débogueur, vous pouvez vérifier toutes les exécutions manuelles de votre scénario, passer en revue toutes les opérations effectuées et afficher les détails de chaque appel API effectué. Vous pouvez voir quel module, opération ou réponse unique a provoqué l’erreur et utiliser ces connaissances pour affiner votre scénario.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Installez le [!DNL Chrome] Extension DevTool

Pour utiliser la variable [!DNL Workfront Fusion] DevTool, vous devez d’abord l’installer.

1. Cliquez sur [ce lien](assets/workfront-fusion-devtool-2023-feb.zip) pour télécharger l’extension.
1. Une fois les fichiers téléchargés, extrayez-les dans un dossier de votre choix.
1. Ouvrir un onglet dans [!DNL Chrome]
1. Dans la barre de recherche de l’onglet, saisissez `chrome://extensions`.
1. Cliquez sur le bouton **[!UICONTROL Mode Développeur]** Activez le mode Développeur dans le coin supérieur droit de l’écran. Si le bouton bascule vers la droite, le mode Développeur est activé.
1. Cliquez sur **[!UICONTROL Chargement non compressé]**.
1. Sélectionnez le dossier contenant l’outil de développement (dans lequel vous avez extrait les fichiers à l’étape 2).

   Une fois décompressé, DevTool apparaît parmi vos autres extensions Chrome.

## Recherchez la variable [!DNL Workfront Fusion] DevTool

Pour utiliser la variable [!DNL Workfront Fusion] DevTool, vous devez ajouter la variable [!DNL Workfront Fusion] Extension DevTool à votre [!DNL Chrome] , comme décrit dans la section [Installation de l’extension Chrome DevTool](#install-the-chrome-devtool-extension).

1. Ouvrez votre [!DNL Workfront Fusion] .
1. Ouvrir [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Commande + Option + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Ctrl + Maj + I</p> <p> Ou </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Il est recommandé d’ancrer la variable [!DNL Chrome Developer Console] en bas pour une meilleure vue de vos modules.

1. Cliquez sur le bouton **[!DNL Workfront Fusion]** dans [!DNL Chrome Dev Tools].

## Utilisez la variable [!DNL Workfront Fusion] DevTool

Workfront Fusion DevTool est divisé en 3 sections principales. Vous pouvez les trouver dans le panneau de gauche de votre fenêtre DevTool.

* [Flux en direct](#live-stream)
* [Débogueur de scénario](#scenario-debugger)
* [Outils](#tools)

### Flux en direct

Live Stream affiche ce qui se passe en arrière-plan lorsque vous cliquez sur Exécuter une fois dans votre scénario.

1. Cliquez sur le bouton **[!UICONTROL Flux en direct]** icon ![](assets/live-stream-icon.png) pour ouvrir la section Live Stream .
1. Effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Action</th> 
      <th>Instructions</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Affichage des informations sur la requête</td> 
      <td> <p>Vous pouvez afficher les informations suivantes pour chaque module dans votre scénario.</p> 
       <ul> 
        <li> <p>En-têtes de requête (URL du point de terminaison de l’API, méthode http, heure et date d’appel de la requête, en-têtes de requête et chaîne de requête)</p> </li> 
        <li> <p>Corps de requête</p> </li> 
        <li> <p>En-têtes de réponse</p> </li> 
        <li> <p>Corps de réponse</p> </li> 
       </ul> <p>Pour afficher ces informations, cliquez sur l’onglet approprié dans le panneau de droite du [!DNL Workfront Fusion] DevTool.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Requêtes de recherche et réponses</p> </td> 
      <td> <p>Saisissez le terme recherché dans le champ de recherche du panneau de gauche de la variable [!DNL Workfront Fusion] DevTool affiche uniquement les requêtes qui contiennent le terme de recherche.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Supprimer la liste des requêtes </p> </td> 
      <td> <p>Cliquez sur l’icône de corbeille dans le coin supérieur droit du panneau de gauche de DevTool pour effacer la liste des requêtes enregistrées par la variable [!DNL Workfront Fusion] DevTool. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Activation de la journalisation de la console</p> </td> 
      <td> <p>Cliquez sur l’icône de l’ordinateur. <img src="assets/console-computer-icon.png"> dans le coin supérieur droit du panneau de gauche de DevTool.</p> <p>La journalisation dans la console est activée lorsque l’icône de l’ordinateur est verte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Récupération de la requête au format JSON brut ou cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>JSON brut</strong> </p> <p>Cliquez sur <strong>[!UICONTROL Copier RAW]</strong> dans le coin supérieur droit du volet de droite de DevTool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Cliquez sur <strong>[!UICONTROL Copier cURL]</strong> dans le coin supérieur droit du volet de droite de DevTool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Débogueur de scénario

Le débogueur de scénario est utile pour les scénarios plus complexes. Il affiche l’historique du scénario qui s’exécute et vous permet de rechercher les modules par leur nom ou identifiant.

1. Cliquez sur le bouton **[!UICONTROL Débogueur de scénario]** icon ![](assets/scenario-debugger-icon.png) pour ouvrir le débogueur de scénario.
1. (Facultatif) Saisissez le terme à rechercher (nom ou identifiant de module) dans le champ de recherche du volet de gauche de la variable [!DNL Workfront Fusion] DevTool dans la [!UICONTROL Débogueur de scénario] .
1. Double-cliquez sur le nom du module pour ouvrir ses paramètres dans l’éditeur de scénarios.
1. Affichez les détails de la requête en cliquant sur l’opération souhaitée.

### Outils

Le [!DNL Workfront Fusion] DevTool contient des outils qui facilitent la configuration de votre scénario.

1. Cliquez sur le bouton **[!UICONTROL Outils]** icon ![](assets/console-tools-icon.png) pour ouvrir les outils.
1. Sélectionnez l’outil à utiliser.
1. Configurez les champs comme décrit ci-dessous.
1. Cliquez sur **[!UICONTROL Exécuter]**.

Outils et leurs champs :

* [Mise au point d’un module](#focus-a-module)
* [Recherche de modules par mappage](#find-modules-by-mapping)
* [Obtenir les métadonnées d’application](#get-app-metadata)
* [Copier le mappage](#copy-mapping)
* [Copier le filtre](#copy-filter)
* [Permutation de la connexion](#swap-connection)
* [Variable Swap](#swap-variable)
* [Permutation d’application](#swap-app)
* [Base 64](#base-64)
* [Copier le nom du module](#copy-module-name)
* [Remap Source](#remap-source)
* [Mettre l’application en surbrillance](#highlight-app)
* [Migration des GS](#migrate-gs)

#### [!UICONTROL Mise au point d’un module]

Ouvre les paramètres du module spécifié par son identifiant.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL ID de module]</td>
        <td>Saisissez l’identifiant du module pour lequel vous souhaitez ouvrir les paramètres.</td>
    </tr>
</table>

#### [!UICONTROL Recherche de modules par mappage]

Permet de rechercher les valeurs des modules pour un terme spécifié. La sortie contient les identifiants des modules qui contiennent le terme que vous avez recherché.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mot-clé]</td> 
   <td> <p> Saisissez le terme à rechercher. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Utiliser uniquement les valeurs]</p> </td> 
   <td> <p>Activez cette option pour ne rechercher que dans les valeurs des champs du module.</p> <p>Désactivez cette option pour effectuer également une recherche dans les noms des champs du module.</p> <p>La recherche est effectuée par le biais des paramètres de nom et de libellé.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir les métadonnées d’application]

Récupère les métadonnées de l’application par le nom ou l’identifiant du module de l’application. Cela s’avère utile, par exemple, lorsque vous devez connaître la version de l’application utilisée dans votre scénario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module source]</td>
        <td>Sélectionnez le module pour lequel vous souhaitez récupérer les métadonnées.</td>
    </tr>
</table>

#### [!UICONTROL Copier le mappage]

Copie les valeurs du module source vers le module cible.

>[!CAUTION]
>
>Assurez-vous de définir les modules source et cible corrects. Si vous sélectionnez un autre type de module, les valeurs du module cible seront supprimées.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module source]</td> 
   <td> <p> Sélectionnez le module ou saisissez l’identifiant du module à partir duquel vous souhaitez copier les valeurs de champ.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module Target]</p> </td> 
   <td> <p>Sélectionnez le module ou saisissez l'identifiant du module dans lequel vous souhaitez insérer les valeurs du module source.</p> <p>Important : Les valeurs du module cible seront écrasées.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier le filtre]

Copie les paramètres de filtre du module source vers le module cible.

>[!NOTE]
>
>L’action de copie est effectuée sur le filtre placé sur le côté gauche du module sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module source]</td> 
   <td> <p> Sélectionnez le module ou saisissez l’identifiant du module à partir duquel vous souhaitez copier les valeurs de filtre.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module Target]</p> </td> 
   <td> <p>Sélectionnez le module ou saisissez l'identifiant du module dans lequel vous souhaitez insérer les valeurs de filtre du module source.</p> <p>Important : Les valeurs du module cible seront écrasées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conserver le paramètre d’itinéraire de secours]</p> </td> 
   <td> <p>Le filtre source est défini comme itinéraire de secours. Activez cette option pour définir également le filtre cible comme itinéraire de secours.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Permutation de la connexion]

Duplique une connexion du module source à chaque module dans le scénario d’une même application.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module source]</td>
        <td>Sélectionnez le module ou saisissez l'identifiant du module à partir duquel vous souhaitez dupliquer la connexion.</td>
    </tr>
</table>

#### [!UICONTROL Variable Swap]

Recherche les variables spécifiées dans le scénario et les remplace par une nouvelle variable.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable à rechercher]</td> 
   <td> <p> Localisez la pilule de variable que vous souhaitez remplacer à partir du module dans votre scénario et copiez-la dans ce champ ([!UICONTROL Variable à rechercher]). Dans le champ, il apparaît avec des accolades doubles. Exemple: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Remplacer par]</p> </td> 
   <td> <p>Localisez la pilule de variables que vous souhaitez remplacer la variable par à partir du module dans votre scénario et copiez-la dans ce champ ([!UICONTROL Variable à rechercher]). Dans le champ, il apparaît avec des accolades doubles. Exemple: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Sélectionnez le module dans lequel vous souhaitez remplacer la variable. Si aucun module n’est sélectionné, la variable sera remplacée dans l’ensemble du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Permutation d’application]

Remplace la version sélectionnée de l’application dans votre scénario par une autre version de l’application.

Cela peut être utilisé, par exemple, pour mettre à niveau les modules des applications Gmail et Email vers la dernière version.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Application à remplacer]</td> 
   <td> <p> Sélectionnez l’application à remplacer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Remplacer par]</p> </td> 
   <td> <p>Sélectionnez l’application par laquelle vous souhaitez la remplacer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Permet de coder les données saisies dans Base64 ou de décoder Base64. Certaines requêtes sont codées en Base64. Cet outil peut s’avérer utile lorsque vous souhaitez rechercher des données spécifiques dans la requête codée.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Indiquez si vous souhaitez coder les données du champ [!UICONTROL Données brutes] en Base64 ou décoder Base64 en Données brutes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> Saisissez les données que vous souhaitez coder en Base64 ou Base64 si vous souhaitez les décoder en données brutes, selon l’option sélectionnée dans le champ [!UICONTROL Opération] ci-dessus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copier le nom du module]

Copie le nom du module sélectionné dans le presse-papiers.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>Sélectionnez le module dont vous souhaitez copier le nom.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remap Source]

Permet de changer la source de mapping d&#39;un module vers un autre.

Vous devez d’abord ajouter le module que vous souhaitez utiliser comme module source à l’itinéraire dans votre scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module source] </td> 
   <td> <p> Sélectionnez le module que vous souhaitez remplacer en tant que source de mappage pour les autres modules de votre scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module Target]</p> </td> 
   <td> <p>Sélectionnez le module à utiliser comme nouvelle source de mappage.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module à modifier]</p> </td> 
   <td> <p>Sélectionnez le module pour lequel vous souhaitez modifier le mappage si vous ne souhaitez pas modifier le mappage dans l’ensemble du scénario. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre l’application en surbrillance]

Met en surbrillance les modules de l’application spécifiée dans votre scénario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Application à mettre en surbrillance] </td> 
   <td> <p> Sélectionnez l’application que vous souhaitez mettre en surbrillance dans votre scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>Sélectionnez la version de l’application que vous souhaitez mettre en surbrillance.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Couleur de surbrillance]</p> </td> 
   <td> <p> Saisissez l’hexadécimal de couleur à utiliser pour la mise en surbrillance des modules.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migration des GS]

Cet outil est spécialement mis à niveau. [!DNL Google Sheets] modules (hérités) vers la dernière version [!DNL Google Sheets] version. Il ajoute une nouvelle version du module juste après la version héritée du module dans l’itinéraire du scénario.

Ce module ne nécessite la définition d’aucun paramètre.
