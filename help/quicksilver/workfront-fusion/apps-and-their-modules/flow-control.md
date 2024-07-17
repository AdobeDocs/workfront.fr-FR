---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Contrôle des flux dans Adobe Workfront Fusion
description: Lorsque vous créez ou modifiez un scénario, vous pouvez configurer des paramètres pour contrôler le flux de données à travers celui-ci.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 20%

---

# Contrôle des flux dans Adobe Workfront Fusion

Lorsque vous créez ou modifiez un scénario, vous pouvez configurer des paramètres pour contrôler le flux de données à travers celui-ci.

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
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Répéteur

Vous pouvez utiliser un module [!UICONTROL Répéteur] pour répéter une tâche un nombre donné de fois. Un module [!UICONTROL Répéteur] génère des lots, l’un après l’autre.

Par exemple, vous pouvez utiliser un module [!UICONTROL Répéteur] pour envoyer cinq emails avec les sujets &quot;Bonjour 1&quot;, &quot;Bonjour 2&quot;, etc., en connectant le module **[!UICONTROL Email] >[!UICONTROL M’envoyer un email]** au module [!UICONTROL Répéteur].

Pour utiliser un module [!UICONTROL Répéteur] :

1. Cliquez sur l’icône [!UICONTROL Contrôle de flux] ![](assets/flow-control-icon.gif) en bas de l’écran, puis cliquez sur **[!UICONTROL Répéteur]** dans le menu qui s’affiche.
1. Cliquez sur le lot [!UICONTROL Répéteur], puis sur **[!UICONTROL Se connecter automatiquement]** dans la zone qui s’affiche.
1. Dans la zone [!UICONTROL Contrôle de flux] qui s’affiche, saisissez le nombre de répétitions (regroupements sortants) souhaité dans la zone **[!UICONTROL Répétition]**.

   Dans notre exemple d’email, saisissez 5.

   ![](assets/repeater-2-350x207.png)

   La valeur de l’élément augmente à chaque répétition de cette valeur spécifiée dans le champ **[!UICONTROL Étape]**, que vous pouvez afficher en sélectionnant **[!UICONTROL Afficher les paramètres avancés]**. Ce nombre est 1 par défaut.

1. Cliquez sur **[!UICONTROL OK]** pour fermer la zone **[!UICONTROL Flux Control]**.

1. Cliquez sur l’application ou le module de service connecté au module [!UICONTROL Répéteur].
1. Dans la zone qui s’affiche, saisissez les informations que vous souhaitez répéter.

   Dans notre exemple de courrier électronique, vous devez saisir Hello dans la zone [!UICONTROL Subject], puis mapper `i` à partir du module de répéteur.

   ![](assets/repeater-3-350x207.png)

| Élément | Description |
|---|---|
| [!UICONTROL Valeur initiale] | Saisissez ou mappez le nombre que le module doit définir comme `i` dans la première itération. La valeur par défaut est 1. |
| [!UICONTROL Répétition] | Saisissez ou mappez le nombre de répétitions du module. Ce nombre doit être supérieur ou égal à 0, inférieur ou égal à 10 000. |
| [!UICONTROL Étape] | Il s’agit du nombre par lequel le module augmente la valeur de `i`. La valeur par défaut est 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>Le nombre de répétitions n’est pas déterminé par la valeur de `i`, car il serait dans une boucle de programmation. Le module répète le nombre de répétitions indiqué dans le champ [!UICONTROL Répéter] . La valeur `i` change à chaque itération du module [!DNL repeater] et peut être mappée à des modules ultérieurs. L’exemple ci-dessus mappe la valeur de `i` dans le message Hello, ce qui entraîne la lecture de messages &quot;Hello 1&quot;, &quot;Hello 2&quot;, etc.

## [!UICONTROL Itérateur]

Un [!UICONTROL itérateur] est un type spécial de module qui convertit un tableau en une série de lots. Chaque élément de tableau sera un lot distinct dans la sortie du module [!UICONTROL Itérateur]. Pour plus d’informations, voir le module [[!UICONTROL Itérateur] dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Agrégateur de tableau

Un agrégateur de tableaux est un type spécial de module qui permet de fusionner plusieurs lots en un seul lot. Pour plus d’informations, voir le module [[!UICONTROL Agrégateur] dans Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Router]

Le module [!UICONTROL Router] vous permet de diviser votre flux en plusieurs itinéraires et de traiter les données de chaque itinéraire différemment. Une fois qu’un module [!UICONTROL Router] reçoit un lot, il le transfère vers chaque itinéraire connecté dans l’ordre dans lequel les itinéraires ont été associés au module [!UICONTROL Router]. Pour plus d’informations, voir [Module de routeur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
