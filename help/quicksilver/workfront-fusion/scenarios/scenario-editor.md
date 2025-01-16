---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Éditeur de scénario dans [!DNL Adobe] Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1172'
ht-degree: 84%

---

# Éditeur de scénario dans [!DNL Adobe Workfront Fusion]

L’éditeur de scénario vous permet de créer et de modifier des scénarios dans une interface visuelle.

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Éditeur de scénarios dans Adobe Workfront Fusion](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/navigate-workfront-fusion/scenario-editor.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

![](assets/scenario-editor.jpg)

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ouvrez l’éditeur de scénario :

1. Cliquez sur **[!UICONTROL Scénarios]**![](assets/scenarios-icon.png)dans le panneau de gauche.

1. Si vous souhaitez créer un scénario, cliquez sur **[!UICONTROL Créer un nouveau scénario]** dans le coin supérieur droit de la page.

   Ou

   Si vous souhaitez modifier un scénario existant, cliquez sur le scénario.

   Dans l’éditeur de scénario qui s’affiche, vous pouvez effectuer toutes les opérations énumérées dans le tableau ci-dessous. Pour plus d’informations, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Lorsque vous avez terminé la modification d’un scénario (ou à tout moment pendant la modification), cliquez sur l’icône [!UICONTROL Enregistrer]. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Après avoir enregistré votre scénario, une nouvelle version est disponible dans le menu à trois points si vous avez besoin d’y accéder ultérieurement. Les versions de scénario précédemment enregistrées ne sont disponibles que pendant 60 jours.

## Actions disponibles dans l’éditeur de scénario

Les actions suivantes sont disponibles dans l’éditeur de scénario :

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Ajouter le premier module</td>
     <td> <p>Cliquez sur l’icône représentant un point d’interrogation. <img src="assets/question-mark-full-size.png"></p> <p> Ensuite, recherchez l’application ou le service avec lequel vous voulez commencer et cliquez dessus. Si vous avez sélectionné des applications à l’étape 2, elles apparaissent ici pour un accès facile (et dans la section <strong>[!UICONTROL Favorites]</strong> au bas de l’écran).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Ajouter un module</td>
     <td>Pointez sur un module, cliquez sur l’icône plus qui apparaît à droite, puis sur le module de votre choix dans le menu qui s’affiche.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Spécifiez quand et à quelle fréquence le scénario s’exécutera.</td>  
      <td> <p>Cliquez sur l’icône d’horloge. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Planifier un scénario dans [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Configurer une route</td>   
     <td> <p>Cliquez sur l’icône [!UICONTROL wrench] <img src="assets/wrench-icon.gif"> entre les deux modules et utilisez l’une des options suivantes :</p>    
       <ul>
         <li><strong>[!UICONTROL Set up a filter]</strong> : contrôlez quels lots sont utilisés à certains points du scénario. Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Ajouter un filtre à un scénario dans [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Unlink]</strong> : supprime un itinéraire.</li>     
         <li><strong>[!UICONTROL Add a router]</strong> : ajoute un routeur entre les modules. </li>     
         <li><strong>[!UICONTROL Add a module]</strong> : ajoute un nouveau module entre les modules.</li>     
         <li><strong>[!UICONTROL Add a note]</strong> : ajoute une note à l’itinéraire.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Supprimer un module</td>   
     <td>Cliquez avec le bouton droit sur le module, puis sur <strong>[!UICONTROL Delete module]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Afficher un journal des événements qui se produisent dans un scénario</td>     
     <td> 
       <p>Exécutez un scénario. Lorsque l’exécution du scénario se termine, le journal apparaît dans le coin inférieur droit de l’[!UICONTROL Scenario Editor]. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>En fonction du scénario, le journal peut contenir des informations sur la difficulté de chaque phase et sur les éventuelles erreurs rencontrées lors de l’exécution du scénario.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Configurer les paramètres du scénario</td>   
     <td>Cliquez sur l’icône [!UICONTROL Scenario settings]. <img src="assets/gear-icon-settings.png"> Ces paramètres sont principalement destinés aux utilisateurs et utilisatrices expérimentés.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Saisir ou afficher des notes sur le scénario</td>   
     <td>Cliquez sur l’icône [!UICONTROL Notes]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Aligner automatiquement la disposition des modules </td>   
     <td>Cliquez sur l’icône [!UICONTROL Auto-align]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Afficher une animation montrant comment les données circulent dans le scénario</td>   <td>Cliquez sur l’icône [!UICONTROL Explain Flow]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exporter le scénario sur votre ordinateur sous la forme d’un plan directeur</td>   
     <td>Cliquez sur le menu [!UICONTROL More] <img src="assets/more-icon.png">, puis sur [!UICONTROL Export Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importer un plan directeur de scénario depuis votre ordinateur</td>   
     <td>Cliquez sur le menu [!UICONTROL More] <img src="assets/more-icon.png">, puis sur [!UICONTROL Import Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Restaurer une version précédente du scénario</td>   
     <td>Voir l’article <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Restaurer une version de scénario dans [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Configurer les paramètres de [!UICONTROL Flow Control]</td>   
     <td> <p>Cliquez sur l’icône [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Vous pouvez définir une tâche pour qu’elle se répète un certain nombre de fois, convertisse un tableau en une série de lots et fusionne plusieurs lots en un seul. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Contrôle des flux dans [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Améliorer le scénario à l’aide d’outils avancés</td>   
     <td>Cliquez sur l’icône [!UICONTROL Tools]. <img src="assets/tools-icon.gif"> Vous pouvez créer des déclencheurs, des actions, des agrégateurs et des transformateurs. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Outils</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Utiliser des outils d’analyse de texte</td>   
     <td>Cliquez sur l’icône [!UICONTROL Text parser]. <img src="assets/text-parser-icon.gif"> Vous pouvez extraire des éléments du code HTML, trouver et extraire des chaînes de caractères correspondant à un modèle de recherche, rechercher et remplacer du texte et « récupérer » les données d’un site web. Pour plus d’informations, voir <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Outils</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Accéder à vos applications et services les plus couramment utilisés</td>   
     <td> Cliquez sur une icône dans la section <strong>[!UICONTROL Favorites]</strong> au bas de l’écran. Les icônes s’affichent automatiquement dans cette section lorsque vous ajoutez des applications et des services à votre scénario. Vous pouvez également cliquer sur l’icône Ajouter <img src="assets/add-icon.gif"> pour ajouter manuellement des applications et des services à cette zone.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Tester le scénario</td>   
     <td>Cliquez sur <strong>[!UICONTROL Run once]</strong> pour vérifier que le scénario s’exécute comme prévu avant de l’activer. Une fois activé, le scénario s’exécute selon son planning. Si tout ne se passe pas comme prévu, vous pouvez consulter notre section sur la gestion des erreurs pour savoir comment y remédier.</td> 
   </tr> 
   <tr> 
     <td role="rowheader">Utiliser l’outil Devtool pour déboguer le scénario</td>   
     <td>Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">Déboguer des scénarios avec l’outil Devtool [!DNL Adobe Workfront Fusion]</a>.
</td> 
   </tr> 
<tr>
<td>Vérifier le statut du scénario</td>
<td>Les scénarios peuvent être actifs ou inactifs. Vous pouvez modifier le statut du scénario en cliquant sur le bouton « Activé/Désactivé » dans les détails du scénario.

Consultez les articles suivants pour plus d’informations :
<ul>
<li><a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md">Activer ou désactiver un scénario dans Adobe Workfront Fusion</a></li>
<li><a href="../../workfront-fusion/scenarios/scenario-detail.md">Détails du scénario dans Adobe Workfront Fusion</a></li>
</ul>
</td>
</tr>
<tr>
<td>Modifier le planning du scénario</td>
<td>Les scénarios actifs sont exécutés selon un planning. Par défaut, un scénario s’exécute toutes les 15 minutes. Vous pouvez modifier ce paramètre en définissant le moment et la fréquence d’exécution d’un scénario activé. Vous pouvez planifier les scénarios Fusion pour qu’ils s’exécutent toutes les 5 minutes.

Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md">Planification d’un scénario dans Adobe Workfront Fusion</a>.
</td>
</tr>
<tr>
<td>Renommer le scénario</td>
<td>Pour renommer un scénario, ouvrez-le scénario, cliquez sur son nom dans le coin supérieur gauche et modifiez-le. Appuyez sur « Entrée » ou cliquez en dehors du champ édité pour enregistrer le nom du scénario.</td>
</tr>
<tr>
<td>Sélectionner le premier lot</td>
<td>Certains modules déclencheur vous permettent de sélectionner le premier lot à partir duquel vous souhaitez que la récupération des lots démarre.

Pour plus d’informations, voir <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md">Choisir le début d’un module de déclenchement dans Adobe Workfront Fusion</a>.</td>
</tr>
<tr>
<td>Définissez le nombre de lots renvoyés</td>
<td>Par défaut, les modules renvoient toujours deux lots seulement. Cette valeur peut être modifiée dans les paramètres du module dans le champ [!UICONTROL Nombre maximal de lots renvoyés].</td>
</tr>
<tr>
<td>Configurer les paramètres avancés du scénario</td>
<td>[!DNL Adobe Workfront Fusion] vous donne la possibilité de configurer un certain nombre d’autres paramètres avancés.

Pour plus d’informations, voir <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md">Panneau des paramètres de scénario dans Adobe Workfront Fusion</a>.</td>
</tr>
</tbody>
</table>
