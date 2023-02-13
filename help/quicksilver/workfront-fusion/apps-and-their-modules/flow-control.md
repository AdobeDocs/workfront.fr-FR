---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Contrôle de flux dans Adobe Workfront Fusion
description: Lorsque vous créez ou modifiez un scénario, vous pouvez configurer des paramètres pour contrôler le flux de données à travers celui-ci.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 1%

---

# Contrôle de flux dans Adobe Workfront Fusion

Lorsque vous créez ou modifiez un scénario, vous pouvez configurer des paramètres pour contrôler le flux de données à travers celui-ci.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Répéteur

Vous pouvez utiliser une [!UICONTROL Répéteur] pour répéter une tâche un nombre donné de fois. A [!UICONTROL Répéteur] génère des lots, l’un après l’autre.

Par exemple, vous pouvez utiliser une [!UICONTROL Répéteur] module pour envoyer cinq emails avec les sujets &quot;Hello 1&quot;, &quot;Hello 2&quot;, etc, en connectant la variable **[!UICONTROL Email] >[!UICONTROL M&#39;envoyer un email]** au module [!UICONTROL Répéteur] module .

Pour utiliser une [!UICONTROL Répéteur] module :

1. Cliquez sur le bouton [!UICONTROL Contrôle de flux] icon ![](assets/flow-control-icon.gif) au bas de l’écran, puis cliquez sur **[!UICONTROL Répéteur]** dans le menu qui s’affiche.
1. Cliquez sur le bouton [!UICONTROL Répéteur] bundle, puis cliquez sur **[!UICONTROL Se connecter automatiquement]** dans la zone qui s’affiche.
1. Dans le [!UICONTROL Contrôle de flux] qui s’affiche, saisissez le nombre de répétitions (regroupements sortants) souhaité dans le champ **[!UICONTROL Répéter]** de la boîte.

   Dans notre exemple d’email, saisissez 5.

   ![](assets/repeater-2-350x207.png)

   La valeur de l’élément augmente à chaque répétition de cette valeur spécifiée dans la variable **[!UICONTROL Étape]** que vous pouvez afficher en sélectionnant **[!UICONTROL Afficher les paramètres avancés]**. Ce nombre est 1 par défaut.

1. Cliquez sur **[!UICONTROL OK]** pour fermer la **[!UICONTROL Contrôle de flux]** de la boîte.

1. Cliquez sur l’application ou le module de service connecté à [!UICONTROL Répéteur] module .
1. Dans la zone qui s’affiche, saisissez les informations que vous souhaitez répéter.

   Dans notre exemple de courrier électronique, vous devez saisir Hello dans la variable [!UICONTROL Objet] box, puis map `i` à partir du module de répéteur.

   ![](assets/repeater-3-350x207.png)

| Élément | Description |
|---|---|
| [!UICONTROL Valeur initiale] | Saisissez ou mappez le nombre que le module doit définir comme `i` dans la première itération. La valeur par défaut est 1. |
| [!UICONTROL Se répète] | Saisissez ou mappez le nombre de répétitions du module. Ce nombre doit être supérieur ou égal à 0, inférieur ou égal à 10 000. |
| [!UICONTROL Étape] | Il s’agit du nombre par lequel le module augmente la valeur de `i`. La valeur par défaut est 1. |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>Le nombre de répétitions n’est pas déterminé par la valeur de `i`, comme dans une boucle de programmation. Le module répète le nombre de fois indiqué dans la variable [!UICONTROL Répéter] champ . La valeur `i` change à chaque itération de la fonction [!DNL repeater] et peut être mappé à des modules ultérieurs. L’exemple ci-dessus mappe la valeur de `i` dans le message Hello, ce qui entraîne la lecture de messages &quot;Hello 1&quot;, &quot;Hello 2&quot;, etc.

## [!UICONTROL Itérateur]

Un [!UICONTROL Itérateur] est un type spécial de module qui convertit un tableau en une série de lots. Chaque élément du tableau sera un lot distinct dans la variable [!UICONTROL Itérateur] sortie du module. Pour plus d’informations, voir [[!UICONTROL Itérateur] module dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Agrégateur de tableau

Un agrégateur de tableaux est un type spécial de module qui permet de fusionner plusieurs lots en un seul lot. Pour plus d’informations, voir [[!UICONTROL Agrégateur] module dans Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Routeur]

Le [!UICONTROL Routeur] vous permet de diviser votre flux en plusieurs itinéraires et de traiter les données de chaque itinéraire différemment. Une fois un [!UICONTROL Routeur] module reçoit un lot, il le transfère vers chaque itinéraire connecté dans l’ordre où les itinéraires ont été associés à la variable [!UICONTROL Routeur] module . Pour plus d’informations, voir [Module de routeur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
