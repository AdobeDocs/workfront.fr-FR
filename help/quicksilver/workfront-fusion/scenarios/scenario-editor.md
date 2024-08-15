---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Éditeur de scénario dans  [!DNL Adobe] Workfront Fusion
description: L’éditeur de scénarios vous permet de créer et de modifier des scénarios dans une interface visuelle.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: cb4edb02aad8a0738ea80f058fcc2bc016832ce1
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 12%

---

# L’éditeur de scénario dans [!DNL Adobe Workfront Fusion]

L’éditeur de scénarios vous permet de créer et de modifier des scénarios dans une interface visuelle.

![](assets/scenario-editor.jpg)

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
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

## Ouvrez l’éditeur de scénarios :

1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche.

1. Si vous souhaitez créer un scénario, cliquez sur **[!UICONTROL Créer un scénario]** dans le coin supérieur droit de la page.

   Ou

   Si vous souhaitez modifier un scénario existant, cliquez sur le scénario.

   Dans l’éditeur de scénario qui s’affiche, vous pouvez effectuer toutes les opérations répertoriées dans le tableau ci-dessous. Pour plus d’informations, voir [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Lorsque vous avez terminé de modifier un scénario (ou à tout moment pendant que vous le modifiez), cliquez sur l’icône [!UICONTROL Enregistrer] . ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Après avoir enregistré votre scénario, une nouvelle version sera disponible sous le menu à trois points si vous devez y accéder ultérieurement. Les versions de scénario précédemment enregistrées ne sont disponibles que pendant 60 jours.

## Actions de l’éditeur de scénarios disponibles

Les actions suivantes sont disponibles dans l’éditeur de scénario :

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Ajouter le premier module</td>
     <td> <p>Cliquez sur l’icône Point d’interrogation. <img src="assets/question-mark-full-size.png"></p> <p> Recherchez et cliquez ensuite sur l’application ou le service avec lequel vous souhaitez commencer. Si vous avez sélectionné des applications à l’étape 2, elles s’affichent ici pour un accès facile (et dans la section <strong>[!UICONTROL Favoris]</strong> au bas de l’écran).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Ajouter un module</td>
     <td>Pointez sur un module, cliquez sur l’icône plus située à droite, puis cliquez sur le module souhaité dans le menu qui s’affiche.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Spécifiez quand et à quelle fréquence le scénario s’exécutera.</td>  
      <td> <p>Cliquez sur l’icône de l’horloge. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Planification d’un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Configuration d’un itinéraire</td>   
     <td> <p>Cliquez sur l’icône [!UICONTROL clé <img src="assets/wrench-icon.gif"> entre les deux modules et utilisez l’une des options suivantes :</p>    
       <ul>
         <li><strong>[!UICONTROL Configurer un filtre]</strong> : contrôlez les lots utilisés à certains moments dans le scénario. Pour plus d'informations, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajout d'un filtre à un scénario dans [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Dissocier]</strong> : supprime un itinéraire.</li>     
         <li><strong>[!UICONTROL Ajouter un routeur]</strong> : ajoute un routeur entre les modules. </li>     
         <li><strong>[!UICONTROL Ajouter un module]</strong> : ajoute un nouveau module entre les modules.</li>     
         <li><strong>[!UICONTROL Ajouter une note]</strong> : ajoute une note à l’itinéraire.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Suppression d’un module</td>   
     <td>Cliquez avec le bouton droit sur le module, puis cliquez sur <strong>[!UICONTROL Supprimer le module]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Afficher un journal des événements qui se produit est un scénario</td>     
     <td> 
       <p>Exécutez un scénario. Lorsque l’exécution du scénario est terminée, le journal s’affiche dans le coin inférieur droit de l’[!UICONTROL Éditeur de scénario]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Selon le scénario, le journal peut contenir des informations sur la difficulté de chaque phase et les erreurs rencontrées lors de l’exécution du scénario.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Configuration des paramètres du scénario</td>   
     <td>Cliquez sur l’icône [!UICONTROL Paramètres du scénario] . <img src="assets/gear-icon-settings.png"> Ces paramètres sont principalement destinés aux utilisateurs avancés.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Type ou affichage des notes sur le scénario</td>   
     <td>Cliquez sur l’icône [!UICONTROL Notes] . <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Alignement automatique de la mise en page des modules </td>   
     <td>Cliquez sur l’icône [!UICONTROL Alignement automatique] . <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Afficher une animation montrant comment les données circulent dans le scénario</td>   <td>Cliquez sur l’icône [!UICONTROL Expliquer le flux] . <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exporter le scénario sur votre ordinateur en tant que plan directeur</td>   
     <td>Cliquez sur le menu [!UICONTROL Plus] <img src="assets/more-icon.png">, puis sur [!UICONTROL Exporter le plan directeur].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importation d’un plan directeur de scénario à partir de votre ordinateur</td>   
     <td>Cliquez sur le menu [!UICONTROL Plus] <img src="assets/more-icon.png">, puis sur [!UICONTROL Importer le plan directeur].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Restaurer une version précédente du scénario</td>   
     <td>Consultez l’article <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Restaurer une version de scénario dans [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Configuration des paramètres de [!UICONTROL Contrôle de flux]</td>   
     <td> <p>Cliquez sur l’icône [!UICONTROL Contrôle de flux] . <img src="assets/flow-control-icon.gif"> Vous pouvez définir une tâche pour répéter un nombre donné de fois, convertir un tableau en une série de lots et fusionner plusieurs lots en un seul lot. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Contrôle de flux dans [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Amélioration du scénario à l’aide d’outils avancés</td>   
     <td>Cliquez sur l’icône [!UICONTROL Outils] . <img src="assets/tools-icon.gif"> Vous pouvez créer des déclencheurs, des actions, des agrégateurs et des transformateurs. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Outils</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Utilisation des outils d’analyse de texte</td>   
     <td>Cliquez sur l’icône [!UICONTROL Analyseur de texte] . <img src="assets/text-parser-icon.gif"> Vous pouvez récupérer des éléments à partir du code de l’HTML, rechercher et extraire des éléments de chaîne correspondant à un modèle de recherche, rechercher et remplacer du texte et "récupérer" des données d’un site web. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Outils</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Accès à vos applications et services les plus couramment utilisés</td>   
     <td> Cliquez sur une icône dans la section <strong>[!UICONTROL Favoris]</strong> au bas de l’écran. Les icônes s’affichent automatiquement dans cette section lorsque vous ajoutez des applications et des services à votre scénario. Vous pouvez également cliquer sur l’icône Ajouter <img src="assets/add-icon.gif"> pour ajouter manuellement des applications et des services à cette zone.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Test du scénario</td>   
     <td>Cliquez sur <strong>[!UICONTROL Exécuter une fois]</strong> pour vérifier que le scénario s’exécute comme prévu avant de l’activer. Une fois activé, le scénario s’exécute selon son planning. Si tout ne fonctionne pas comme prévu, vous pouvez consulter notre section de gestion des erreurs pour savoir comment gérer les erreurs.</td> 
   </tr> 
   <tr> 
     <td role="rowheader">Utilisez l’outil Devtool pour déboguer le scénario</td>   
     <td>Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">Débogage de scénarios avec l’ [!DNL Adobe Workfront Fusion] Devtool</a> .
</td> 
   </tr> 
<tr>
<td>Vérification de l’état du scénario</td>
<td>Les scénarios peuvent être actifs ou inactifs. Vous pouvez modifier l’état du scénario en cliquant sur le bouton Activé/Désactivé dans le détail du scénario.

Pour plus d’informations, consultez les articles suivants :
<ul>
<li><a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md">Activer ou désactiver un scénario dans Adobe Workfront Fusion</a></li>
<li><a href="../../workfront-fusion/scenarios/scenario-detail.md">Détails du scénario dans Adobe Workfront Fusion</a></li>
</ul>
</td>
</tr>
<tr>
<td>Modification de la planification du scénario</td>
<td>Les scénarios actifs sont exécutés conformément à une planification. Par défaut, un scénario s’exécute toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution d’un scénario activé. Les scénarios de fusion peuvent être planifiés pour s’exécuter aussi souvent que toutes les 5 minutes.

Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md">Planification d’un scénario dans Adobe Workfront Fusion</a>.
</td>
</tr>
<tr>
<td>Renommer le scénario</td>
<td>Pour renommer un scénario, ouvrez-le, cliquez sur son nom dans le coin supérieur gauche et modifiez-le. Appuyez sur Entrée ou cliquez en dehors du champ modifié pour enregistrer le nom du scénario.</td>
</tr>
<tr>
<td>Sélectionner le premier lot</td>
<td>Certains modules de déclenchement vous permettent de sélectionner le premier lot à partir duquel vous souhaitez que la récupération des lots démarre.

Pour plus d’informations, voir <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md">Choix de l’endroit où un module de déclenchement commence dans Adobe Workfront Fusion</a>.</td>
</tr>
<tr>
<td>Définir le nombre de lots renvoyés</td>
<td>Par défaut, les modules renvoient toujours deux lots uniquement. Cela peut être modifié dans les paramètres du module dans le champ [!UICONTROL Nombre maximum de bundles renvoyés].</td>
</tr>
<tr>
<td>Configuration des paramètres avancés du scénario</td>
<td>[!DNL Adobe Workfront Fusion] vous donne la possibilité de configurer un certain nombre d’autres paramètres avancés.

Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md">Panneau des paramètres de scénario dans Adobe Workfront Fusion</a>.</td>
</tr>
</tbody>
</table>
