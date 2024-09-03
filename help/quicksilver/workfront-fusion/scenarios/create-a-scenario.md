---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Créer un scénario dans Adobe Workfront Fusion
description: Les tâches suivantes expliquent comment créer un scénario  [!DNL Adobe Workfront Fusion] .
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: ee2283ac159ca26ca473cac28ec4bed85d1dea04
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 96%

---

# Créer un scénario dans [!DNL Adobe Workfront Fusion]

Les tâches suivantes expliquent comment créer un scénario [!DNL Adobe Workfront Fusion].

Pour un exercice d’entraînement qui vous guide tout au long de la création d’un scénario d’automatisation, voir [Créer un scénario d’automatisation d’entraînement dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Pour un exercice d’entraînement qui vous guide tout au long de la création d’un scénario d’intégration à l’aide des données que nous fournissons, voir [Créer un scénario d’intégration d’entraînement dans Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Pour créer un scénario à partir d’un modèle, voir [Créer des scénarios avec les modèles  [!DNL Adobe Workfront Fusion] ](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Formule Adobe Workfront</td>  
      <td>Tous</td>  
    </tr>  
    <tr>  
      <td>Licence Adobe Workfront</td>  
      <td>
        Nouveau : Standard<br>
        Ou<br>
        Actuel : travail ou plus élevé
      </td>  
    </tr>  
    <tr>  
      <td>Licence Adobe Workfront Fusion</td>  
      <td> 
        Actuel : aucune exigence de licence Workfront Fusion.<br>
        Ou<br>
        Hérité : Tout
      </td>  
    </tr>  
    <tr>  
      <td>Produit</td>  
      <td> 
        Nouveau : sélectionnez ou forfait Workfront Prime : votre entreprise doit acheter Adobe Workfront Fusion.<br>
        Formule Workfront ultime : Workfront Fusion est incluse.<br>
        Ou<br>
        Actuel : votre entreprise doit acheter Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Commencer à créer un scénario

1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche.

1. Cliquez sur **[!UICONTROL Créer un scénario]** dans le coin supérieur droit de la page.
1. Dans l’écran qui s’affiche (dans l’éditeur de scénario), si vous créez un scénario, cliquez sur **[!UICONTROL Nouveau scénario]** dans le coin supérieur gauche et saisissez un nom pour le scénario.
1. Passez à [Ajouter un module dans un scénario](#add-a-module-in-a-scenario).

## Ajouter un module dans un scénario

1. Pour ajouter le premier module au scénario, cliquez sur l’icône de point d’interrogation ![](assets/question-mark-icon.gif).

   Ou

   Pour ajouter d’autres modules au scénario, cliquez sur la poignée à droite du module qu’il doit suivre.

1. Dans la zone qui s’affiche, recherchez et cliquez sur l’application ou le service avec lequel vous souhaitez commencer.

   Toutes les applications précédemment sélectionnées s’affichent dans la zone pour pouvoir y accéder facilement, ainsi que dans la section **[!UICONTROL Favoris]** au bas de l’écran.

   Si vous cliquez sur **[!UICONTROL Ajouter un autre module]**, les modules qui s’affichent dépendent de l’endroit où vous ajoutez le module dans le scénario. Certains modules ne peuvent être placés qu’entre d’autres modules, tandis que d’autres ne peuvent être placés qu’au début du scénario.

   >[!TIP]
   >
   >Les deux types de modules les plus courants sont les actions et les déclencheurs. Pour plus d’informations, voir [Types de modules](../../workfront-fusion/modules/module-types.md).

1. Dans la liste des modules qui s’affiche, cliquez sur le premier module que vous souhaitez ajouter au scénario.

   Les modules qui s’affichent dépendent de l’endroit où vous souhaitez ajouter un module dans votre scénario. Certains modules ne peuvent être placés qu’entre d’autres modules, tandis que d’autres ne peuvent être placés qu’au début du scénario.

   Les deux types de modules les plus courants sont les actions et les déclencheurs. Pour plus d’informations, voir [Types de modules](../../workfront-fusion/modules/module-types.md).

1. Passez à [Connecter l’application ou le service web du module à  [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Connecter l’application ou le service web du module à [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Les modules Workfront Fusion qui se connectent à une application (comme [!DNL Workfront], [!DNL Salesforce] ou [!DNL Jira)]) comprennent le champ [!UICONTROL Connexion]. Vous pouvez spécifier ici la connexion que ce module doit utiliser pour se connecter à l’application. Vous pouvez sélectionner une connexion existante dans la liste déroulante ou en créer une nouvelle.

Lorsque vous sélectionnez ou créez une connexion pour une application dans un scénario, les autres modules de cette application utilisent automatiquement la même connexion, sauf si vous en sélectionnez une autre lors de la configuration des modules ultérieurs.

Pour plus d’informations, consultez [Vue d’ensemble des connexions](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

Pour créer une connexion dans un module [!DNL Workfront Fusion], procédez comme suit :

1. Cliquez sur **[!UICONTROL Ajouter]** pour ouvrir la zone **[!UICONTROL Créer une connexion]**.
1. (Facultatif) Modifiez le **[!UICONTROL nom de la connexion]** par défaut.
1. (Le cas échéant) Si l’application nécessite des paramètres de connexion avancés, tels qu’un identifiant, une clé ou [!UICONTROL secret], saisissez ces informations.

   Il se peut que vous deviez cliquer sur **[!UICONTROL Afficher les paramètres avancés]** pour afficher les champs dans lesquels saisir ce type d’informations.

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre de connexion qui s’affiche, saisissez vos informations d’identification pour vous connecter à l’application si vous ne l’avez pas déjà fait.
1. (Le cas échéant) Si un bouton **[!UICONTROL Autoriser]** s’affiche, examinez les actions que le connecteur pourra effectuer, puis cliquez sur le bouton pour connecter l’application à [!DNL Workfront Fusion].
1. Passez à [Configurer le module](#configure-the-module).


## Configurer le module

1. Dans les champs situés sous le champ Connexion, configurez les paramètres du module, puis cliquez sur **[!UICONTROL OK]**.

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

1. Si vous ajoutez le premier module à votre scénario, sélectionnez une option pour indiquer où vous souhaitez que le scénario démarre à chaque exécution.

   ![](assets/choose-where-start-350x194.png)

1. Répétez les étapes des sections [Ajouter un module dans un scénario](#add-a-module-in-a-scenario) et [Configurer le module](#configure-the-module) pour ajouter d’autres modules au scénario.

1. (Facultatif) Copiez et collez un module ou un groupe de modules.

   Pour plus d’informations, voir [Copier des modules ou des scénarios dans Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Passez à [Configurer et travailler avec votre scénario](#configure-and-work-with-your-scenario).

## Configurer et travailler avec votre scénario

1. Pour configurer votre scénario, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Spécifiez quand et à quelle fréquence le scénario s’exécutera.</td> 
      <td> <p>Cliquez sur l’icône d’horloge. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Planifier un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurer une route</td> 
      <td> <p>Cliquez sur l’icône de clé à molette <img src="assets/wrench-icon.gif"> entre les deux modules et utilisez l’une des options suivantes. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajouter un filtre à un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Set up a filter]</strong> : contrôle les lots utilisés à certains moments dans le scénario.</li> 
        <li><strong>[!UICONTROL Unlink]</strong> : supprime une route.</li> 
        <li><strong>[!UICONTROL Add a router]</strong> : ajoute un routeur entre les modules. </li> 
        <li><strong>[!UICONTROL Add a module]</strong> : ajoute un nouveau module entre les modules.</li> 
        <li><strong>[!UICONTROL Add a note]</strong> : ajoute une note à la route.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurer les paramètres du scénario</td> 
      <td>Cliquez sur l’icône [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> Ces paramètres sont principalement destinés aux utilisateurs et utilisatrices avancés. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configurer des paramètres de contrôle de flux</td> 
      <td> <p>Cliquez sur l’icône [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Vous pouvez définir une tâche pour qu’elle se répète un certain nombre de fois, convertisse un tableau en une série de lots et fusionne plusieurs lots en un seul. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Contrôle des flux dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Améliorer le scénario à l’aide d’outils avancés</td> 
      <td>Cliquez sur l’icône [!DNL Tools]. <img src="assets/tools-icon.gif"> Vous pouvez créer des déclencheurs, des actions, des agrégateurs et des transformateurs. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Outils</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Outils d’analyse de texte utilisateur</td> 
      <td>Cliquez sur l’icône [!DNL Text parser] <img src="assets/text-parser-icon.gif">. Vous pouvez récupérer des éléments à partir d’un code HTML, rechercher et extraire des éléments de chaîne correspondant à un modèle de recherche, rechercher et remplacer du texte et « extraire » des données d’un site web. Pour plus d’informations, consultez <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Outils</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Effectuez l’une des opérations suivantes suivant votre scénario :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher un journal des événements qui se produisent lors de l’exécution du scénario.</td> 
      <td> <p>Cliquez sur la flèche <img src="assets/exit-editing-arrow.png"> [!UICONTROL Exit editing] dans l’éditeur de scénario pour afficher la page Détails du scénario. Le journal s’affiche au bas de la fenêtre ou dans le coin inférieur droit. Il contient des informations sur chaque phase et les erreurs rencontrées lors de l’exécution du scénario.</p> <p>Pour revenir à l’utilisation de votre scénario dans l’[!DNL scenario editor], cliquez n’importe où sur la page Détails du scénario.</p> <p>Pour plus d’informations sur la page Détails du scénario, consultez <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Détails du scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Accéder à vos applications et services les plus couramment utilisés</td> 
      <td> Cliquez sur une icône dans la section <strong>[!UICONTROL Favorites]</strong> au bas de l’écran. Les icônes s’affichent automatiquement dans cette section lorsque vous ajoutez des applications et des services à votre scénario. Vous pouvez également cliquer sur l’icône <img src="assets/add-icon.gif"> [!UICONTROL Add] pour ajouter manuellement des applications et des services à cette zone.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher une animation montrant comment les données circulent dans le scénario</td> 
      <td>Cliquez sur l’icône <img src="assets/explain-flow-airplane-icon.gif"> [!UICONTROL Explain flow].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aligner automatiquement la disposition des modules </td> 
      <td>Cliquez sur l’icône <img src="assets/auto-align-icon.gif"> [!UICONTROL Auto-align].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Saisir ou afficher des notes sur le scénario</td> 
      <td>Cliquez sur l’icône <img src="assets/notes-icon.gif"> [!UICONTROL Notes].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un module</td> 
      <td>Cliquez avec le bouton droit sur le module, puis cliquez sur <strong>[!UICONTROL Delete module]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Pour tester le scénario, cliquez sur **[!UICONTROL Exécuter une fois]**.

   Il est important de vérifier que le scénario s’exécute comme prévu avant de l’activer. Une fois activé, le scénario s’exécute selon son planning. Si tout ne fonctionne pas comme prévu, consultez [Gestion des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Lorsque vous avez terminé de modifier le scénario (ou à tout moment pendant la modification), cliquez sur l’icône [!UICONTROL Enregistrer] en bas de la fenêtre ![](assets/save-icon.gif).

Pour plus d’informations sur l’activation d’un scénario, consultez [Activer ou désactiver un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Raccourcis clavier du scénario Workfront Fusion

Vous pouvez utiliser les raccourcis clavier suivants lors de la création ou de la modification d’un scénario :

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
   <td role="rowheader">[!UICONTROL Save] </td> 
   <td>Ctrl+Maj+S</td> 
   <td><span style="font-weight: normal;">Cmd+Maj+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Run Once]</td> 
   <td>Ctrl+Maj+Entrée</td> 
   <td><span style="font-weight: normal;">Cmd+Maj+Entrée</span> </td> 
  </tr> 
 </tbody> 
</table>
