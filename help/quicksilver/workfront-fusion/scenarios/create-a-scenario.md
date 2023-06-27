---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Création d’un scénario dans Adobe Workfront Fusion
description: Les tâches suivantes expliquent comment créer une [!DNL Adobe Workfront Fusion] .
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# Création d’un scénario dans [!DNL Adobe Workfront Fusion]

Les tâches suivantes expliquent comment créer une [!DNL Adobe Workfront Fusion] .

Pour un exercice d’entraînement qui vous guide tout au long de la création d’un scénario d’automatisation, voir [Créez un scénario d’automatisation des pratiques dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Pour un exercice d’entraînement qui vous guide tout au long de la création d’un scénario d’intégration à l’aide des données que nous fournissons, voir [Création d’un scénario d’intégration d’une pratique dans Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Pour créer un scénario à partir d’un modèle, voir [Création de scénarios avec [!DNL Adobe Workfront Fusion] templates](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>    </td> 
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

## Commencer à créer un scénario

1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche.

1. Cliquez sur **[!UICONTROL Création d’un scénario]** dans le coin supérieur droit de la page.
1. Dans l’écran qui s’affiche (dans l’éditeur de scénarios), si vous créez un scénario, cliquez sur **[!UICONTROL Nouveau scénario]** dans le coin supérieur gauche, saisissez le nom du scénario.
1. Passez à la [Ajouter un module dans un scénario](#add-a-module-in-a-scenario).

## Ajouter un module dans un scénario

1. Pour ajouter le premier module au scénario, cliquez sur l’icône de point d’interrogation. ![](assets/question-mark-icon.gif)

   Ou

   Pour ajouter d’autres modules au scénario, cliquez sur la poignée située sur le côté droit du module à suivre.

1. Dans la zone qui s’affiche, recherchez et cliquez sur l’application ou le service avec lequel vous souhaitez commencer.

   Toutes les applications sélectionnées précédemment s’affichent dans la zone pour un accès facile, et dans la variable **[!UICONTROL Favoris]** au bas de l’écran.

   Si vous cliquez sur **[!UICONTROL Ajouter un autre module]**, les modules qui s’affichent dépendent de l’endroit où vous ajoutez le module dans le scénario. Certains modules ne peuvent être placés qu’entre d’autres modules, tandis que d’autres ne peuvent être placés qu’au début du scénario.

   >[!TIP]
   >
   >Les deux types de modules les plus courants sont les actions et les déclencheurs. Pour plus d’informations, voir [Types de modules](../../workfront-fusion/modules/module-types.md).

1. Dans la liste des modules qui s’affiche, cliquez sur le premier module à ajouter au scénario.

   Les modules qui s’affichent dépendent de l’endroit où vous souhaitez ajouter un module dans votre scénario. Certains modules ne peuvent être placés qu’entre d’autres modules, tandis que d’autres ne peuvent être placés qu’au début du scénario.

   Les deux types de modules les plus courants sont les actions et les déclencheurs. Pour plus d’informations, voir [Types de modules](../../workfront-fusion/modules/module-types.md).

1. Passez à la [Connectez l’application ou le service Web du module à [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Connectez l’application ou le service Web du module à [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Modules Workfront Fusion se connectant à une application (tels que [!DNL Workfront], [!DNL Salesforce]ou [!DNL Jira)] de la fonction [!UICONTROL Connexion] champ . Ici, vous pouvez spécifier la connexion que ce module doit utiliser pour se connecter à l’application. Vous pouvez sélectionner une connexion existante dans la liste déroulante ou créer une connexion.

Lorsque vous sélectionnez ou créez une connexion pour une application dans un scénario, les autres modules de cette application utilisent automatiquement la même connexion, sauf si vous en sélectionnez une autre lors de la configuration des modules ultérieurs.

Pour plus d’informations, voir [A propos de la connexion [!DNL Adobe Workfront Fusion] vers une application ou un service](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Pour créer une connexion dans un [!DNL Workfront Fusion] module :

1. Cliquez sur **[!UICONTROL Ajouter]** pour ouvrir le **[!UICONTROL Création d’une connexion]** de la boîte.
1. (Facultatif) Modifiez la valeur par défaut **[!UICONTROL Nom de la connexion]**.
1. (Conditionnel) Si l’application nécessite des paramètres de connexion avancés, tels qu’un identifiant, une clé ou [!UICONTROL secret], saisissez ces informations.

   Vous devrez peut-être cliquer sur **[!UICONTROL Afficher les paramètres avancés]** pour afficher les champs où vous pouvez saisir ce type d&#39;informations.

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre de connexion qui s’affiche, saisissez vos informations d’identification pour vous connecter à l’application si vous ne l’avez pas déjà fait.
1. (Conditionnel) Si un événement **[!UICONTROL Autoriser]** s’affiche, examinez les actions que le connecteur pourra effectuer, puis cliquez sur le bouton pour connecter l’application à [!DNL Workfront Fusion].
1. Passez à la [Configuration du module](#configure-the-module).


## Configuration du module

1. Dans les champs situés sous le champ Connexion , configurez les paramètres du module, puis cliquez sur **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Ces paramètres sont différents pour chaque module. Un titre en gras indique un paramètre requis.

   >[!TIP]
   >
   >Au fur et à mesure que vous travaillez sur votre scénario, vous pouvez cliquer sur le module pour afficher à tout moment cette boîte de paramètres.
   >
   >
   >Si un cercle noir s’affiche sur un module, vous n’avez pas fini de configurer ses paramètres. Cliquez sur le module pour l’ouvrir et poursuivre la configuration.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Si vous ajoutez le premier module à votre scénario, sélectionnez une option pour indiquer où vous souhaitez que le scénario démarre chaque fois qu’il s’exécute.

   ![](assets/choose-where-start-350x194.png)

1. Répétez les étapes des sections [Ajouter un module dans un scénario](#add-a-module-in-a-scenario) et [Configuration du module](#configure-the-module) pour ajouter d’autres modules au scénario.

1. (Facultatif) Copiez et collez un module ou un groupe de modules.

   Pour plus d’informations, voir [Copie de modules ou de scénarios dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Passez à la [Configuration et utilisation de votre scénario](#configure-and-work-with-your-scenario).

## Configuration et utilisation de votre scénario

1. Pour configurer votre scénario, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Spécifiez quand et à quelle fréquence le scénario s’exécutera.</td> 
      <td> <p>Cliquez sur l’icône de l’horloge. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Planification d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuration d’un itinéraire</td> 
      <td> <p>Cliquez sur l’icône de clé à molette <img src="assets/wrench-icon.gif"> entre les deux modules et utilisez l’une des options suivantes. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajoutez un filtre à un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Configurer un filtre]</strong>: Contrôlez les lots utilisés à certains moments dans le scénario.</li> 
        <li><strong>[!UICONTROL Dissocier]</strong>: Supprime un itinéraire.</li> 
        <li><strong>[!UICONTROL Ajouter un routeur]</strong>: Ajoute un routeur entre les modules. </li> 
        <li><strong>[!UICONTROL Ajouter un module]</strong>: Ajoute un nouveau module entre les modules.</li> 
        <li><strong>[!UICONTROL Ajouter une note]</strong>: Ajoute une note à l’itinéraire.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuration des paramètres du scénario</td> 
      <td>Cliquez sur l’icône [!UICONTROL Paramètres du scénario] . <img src="assets/gear-icon-settings.png"> Ces paramètres sont principalement destinés aux utilisateurs avancés. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Le panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuration des paramètres de contrôle de flux</td> 
      <td> <p>Cliquez sur l’icône [!UICONTROL Contrôle de flux] . <img src="assets/flow-control-icon.gif"> Vous pouvez définir une tâche pour répéter un nombre donné de fois, convertir un tableau en une série de lots et fusionner plusieurs lots en un seul lot. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Contrôle de flux dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Amélioration du scénario à l’aide d’outils avancés</td> 
      <td>Cliquez sur le bouton [!DNL Tools] icône . <img src="assets/tools-icon.gif"> Vous pouvez créer des déclencheurs, des actions, des agrégateurs et des transformateurs. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Outils</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Outils d’analyse de texte utilisateur</td> 
      <td>Cliquez sur le bouton [!DNL Text parser] icon <img src="assets/text-parser-icon.gif">. Vous pouvez récupérer des éléments à partir du code de HTML, rechercher et extraire des éléments de chaîne correspondant à un modèle de recherche, rechercher et remplacer du texte et "récupérer" des données d’un site web. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Outils</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Pour utiliser votre scénario, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher un journal des événements qui se produisent lors de l’exécution du scénario</td> 
      <td> <p>Cliquez sur la flèche [!UICONTROL Quitter l’édition] . <img src="assets/exit-editing-arrow.png"> dans l’éditeur de scénario pour afficher la page Détails du scénario. Le journal s’affiche au bas de la fenêtre ou dans le coin inférieur droit. Elle contient des informations sur chaque phase et les erreurs rencontrées lors de l’exécution du scénario.</p> <p>Pour revenir à l’utilisation de votre scénario dans le [!DNL scenario editor], cliquez n’importe où sur la page Détails du scénario .</p> <p>Pour plus d’informations sur la page Détails du scénario, voir <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Détails du scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accès à vos applications et services les plus couramment utilisés</td> 
      <td> Cliquez sur une icône dans le <strong>[!UICONTROL Favoris]</strong> au bas de l’écran. Les icônes s’affichent automatiquement dans cette section lorsque vous ajoutez des applications et des services à votre scénario. Vous pouvez également cliquer sur l’icône [!UICONTROL Ajouter] <img src="assets/add-icon.gif"> pour ajouter manuellement des applications et des services à cette zone.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher une animation montrant comment les données circulent dans le scénario</td> 
      <td>Cliquez sur l’icône [!UICONTROL Expliquer le flux] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alignement automatique de la mise en page des modules </td> 
      <td>Cliquez sur l’icône [!UICONTROL Alignement automatique] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type ou affichage des notes sur le scénario</td> 
      <td>Cliquez sur l’icône [!UICONTROL Notes] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suppression d’un module</td> 
      <td>Cliquez avec le bouton droit sur le module, puis cliquez sur <strong>[!UICONTROL Supprimer le module]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Pour tester l’exécution du scénario, cliquez sur **[!UICONTROL Exécuter une seule fois]**.

   Il est important de vérifier que le scénario s’exécute comme prévu avant de l’activer. Une fois activé, le scénario s’exécute selon son planning. Si tout ne fonctionne pas comme prévu, reportez-vous à la section [Gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Lorsque vous avez terminé de modifier le scénario (ou à tout moment pendant la modification), cliquez sur le bouton [!UICONTROL Enregistrer] icône en bas de la fenêtre ![](assets/save-icon.gif).

Pour plus d’informations sur l’activation d’un scénario, voir [Activez ou désactivez un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Raccourcis clavier du scénario Workfront Fusion

Vous pouvez utiliser les raccourcis clavier suivants lors de la création ou de la modification d’un scénario :

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enregistrer] </td> 
   <td>Ctrl+Maj+S</td> 
   <td><span style="font-weight: normal;">Cmd+Maj+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Exécuter une fois]</td> 
   <td>Ctrl+Maj+Entrée</td> 
   <td><span style="font-weight: normal;">Cmd+Maj+Entrée</span> </td> 
  </tr> 
 </tbody> 
</table>
