---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Contrôle du flux dans Adobe Workfront Fusion
description: Lorsque vous créez ou modifiez un scénario, vous pouvez configurer des paramètres pour contrôler la manière dont les données transitent dans celui-ci.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 100%

---

# Contrôle du flux dans Adobe Workfront Fusion

Lorsque vous créez ou modifiez un scénario, vous pouvez configurer des paramètres pour contrôler la manière dont les données transitent dans celui-ci.

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
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Répéteur

Vous pouvez utiliser un module [!UICONTROL Répéteur] pour répéter une tâche un nombre de fois défini. Une module [!UICONTROL Répéteur] génère des lots l’un après l’autre.

Par exemple, vous pouvez utiliser un module [!UICONTROL Répéteur] pour envoyer cinq e-mails avec les objets « Bonjour 1 », « Bonjour 2 », et ainsi de suite, en connectant le module **[!UICONTROL E-mail] > [!UICONTROL M’envoyer un e-mail]** au module [!UICONTROL Répéteur].

Pour utiliser un module [!UICONTROL Répéteur], procédez comme suit :

1. Cliquez sur l’icône [!UICONTROL Contrôle du flux] ![](assets/flow-control-icon.gif) au bas de l’écran, puis sur **[!UICONTROL Répéteur]** dans le menu qui s’affiche.
1. Cliquez sur le lot [!UICONTROL Répéteur], puis sur **[!UICONTROL Se connecter automatiquement]** dans la zone qui s’affiche.
1. Dans la zone [!UICONTROL Contrôle du flux] qui s’affiche, saisissez le nombre de répétitions (lots sortants) souhaité dans la zone **[!UICONTROL Répétitions]**.

   Dans notre exemple d’e-mail, vous devez saisir 5.

   ![](assets/repeater-2-350x207.png)

   La valeur de l’élément augmente à chaque répétition selon la valeur spécifiée dans le champ **[!UICONTROL Étape]** que vous pouvez afficher en sélectionnant **[!UICONTROL Afficher les paramètres avancés]**. Ce nombre est 1 par défaut.

1. Cliquez sur **[!UICONTROL OK]** pour fermer la zone **[!UICONTROL Contrôle du flux]**.

1. Cliquez sur l’application ou le module de service connecté au module [!UICONTROL Répéteur].
1. Dans la zone qui s’affiche, saisissez les informations que vous souhaitez répéter.

   Dans notre exemple d’e-mail, vous devez saisir Bonjour dans le champ [!UICONTROL Objet], puis mapper `i` à partir du module répéteur.

   ![](assets/repeater-3-350x207.png)

| Élément | Description |
|---|---|
| [!UICONTROL Valeur initiale] | Saisissez ou mappez le nombre que le module doit définir comme `i` dans la première itération. La valeur par défaut est 1. |
| [!UICONTROL Répétitions] | Saisissez ou mappez le nombre de répétitions du module. Ce nombre doit être supérieur ou égal à 0 et inférieur ou égal à 10 000. |
| [!UICONTROL Étape] | Il s’agit du nombre selon lequel le module augmente la valeur de `i`. La valeur par défaut est 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>Le nombre de répétitions n’est pas déterminé par la valeur de `i`, comme c’est le cas dans une boucle de programmation. Le module effectue autant de répétitions que le nombre indiqué dans le champ [!UICONTROL Répétitions]. La valeur `i` change à chaque itération du module [!DNL repeater] et peut être mappée à des modules ultérieurs. L’exemple ci-dessus mappe la valeur de `i` au message Bonjour, ce qui entraîne la création des messages « Bonjour 1 », « Bonjour 2 », et ainsi de suite.

## [!UICONTROL Itérateur]

Un [!UICONTROL Itérateur] est un type spécial de module qui convertit un tableau en une série de lots. Chaque élément du tableau constitue un lot distinct dans la sortie du module [!UICONTROL Itérateur]. Pour plus d’informations, voir module [[!UICONTROL Itérateur] dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Agrégateur de tableaux

Un agrégateur de tableaux est un type spécial de module qui permet de fusionner plusieurs lots en un seul lot. Pour plus d’informations, voir module [[!UICONTROL Agrégateur] dans Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Routeur]

Le module [!UICONTROL Routeur] vous permet de diviser votre flux en plusieurs itinéraires et de traiter les données de chaque itinéraire de manière différente. Dès qu’un module [!UICONTROL Routeur] reçoit un lot, il le transfère vers chaque itinéraire connecté dans l’ordre dans lequel les itinéraires ont été associés au module [!UICONTROL Routeur]. Pour plus d’informations, voir [Module Routeur dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
