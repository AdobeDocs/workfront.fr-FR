---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ajouter un filtre à un scénario dans  [!DNL Adobe]  Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 87%

---

# Ajouter un filtre à un scénario dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Ajouter un filtre à un scénario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-filter-to-a-scenario.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans certains scénarios, vous devez travailler uniquement avec des lots qui répondent à des critères spécifiques. Les filtres vous permettent de sélectionner ces lots.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Vous pouvez ajouter un filtre entre deux modules et vérifier si les lots reçus des modules précédents remplissent des conditions de filtrage spécifiques :

* Si tel est le cas, les lots sont transmis au module suivant dans le scénario.
* Dans le cas contraire, le traitement des lots s’arrête.

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
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Vous devez ajouter les deux modules à un scénario avant de pouvoir ajouter un filtre entre eux.

## Ajoutez un filtre entre deux modules :

1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche, puis sélectionnez le scénario pour l’ouvrir.
1. Dans le coin supérieur droit de la fenêtre, cliquez sur **[!UICONTROL Modifier]**.
1. Cliquez sur la ligne reliant les modules.
1. Dans le champ qui s’affiche, saisissez un **[!UICONTROL Libellé]** pour le filtre.
1. Définissez une **[!UICONTROL Condition]** de filtre.

   Vous pouvez saisir un ou deux opérandes dans les deux champs. Si vous saisissez des opérandes dans les deux champs, vous pouvez sélectionner un opérateur dans le menu déroulant situé entre les deux champs afin de définir la relation entre les opérandes.

   >[!TIP]
   >
   >Dans les champs des opérandes, vous pouvez saisir des valeurs de la même manière que vous les mappez, comme décrit dans la section [Mappage des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Par exemple, si vous souhaitez que le filtre recherche des fichiers dans [!DNL Adobe Workfront] se terminant par XML et qu’il les transmette à [!DNL Dropbox], vous devez entrer le **[!UICONTROL Nom du fichier]** dans le premier champ et.**[!UICONTROL xml]** dans le second champ. Dans le menu déroulant qui sépare les champs, vous pouvez sélectionner **[!UICONTROL Se termine par (non sensible à la casse)]**. Ce filtre s’applique aux lots entrants du premier module (Workfront). Seuls les lots contenant des fichiers XML sont transmis au module suivant ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Cliquez sur **[!DNL OK]**.

## Copier un filtre

Actuellement, l’éditeur de scénario n’inclut pas de fonctionnalité permettant la copie d’un filtre.

>[!NOTE]
>
>Si vous copiez les modules de chaque côté du filtre, le filtre est également copié.
>
>Pour plus d’informations sur la copie de modules, voir [Copie de modules ou de scénarios dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Pour copier un filtre sans copier de modules, vous pouvez utiliser [!DNL Google] Chrome pour la solution suivante :

1. Installez l’extension Chrome [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool].
1. Dans [!DNL Workfront Fusion], ouvrez le scénario.
1. Cliquez sur le menu à trois points de Chrome, puis sur **[!UICONTROL Autres outils*]* > **[!UICONTROL Outils de développement]**.

1. Dans le panneau [!UICONTROL Outils de développement] qui s’affiche, dans la barre de menus située en haut, cliquez sur l’onglet [!UICONTROL Workfront Fusion].

   ![](assets/copy-a-filter-350x174.png)

1. Cliquez sur l’icône **[!UICONTROL Outils]** ![](assets/devtools-tools-icon.png) dans la barre latérale gauche.

1. Cliquez sur **[!UICONTROL Copier le filtre]**, puis configurez l’outil **[!UICONTROL Copier le filtre]** dans le panneau latéral droit :

   1. Définissez le **[!UICONTROL Module source]** comme module juste après le filtre que vous souhaitez copier.
   1. Définissez le **[!UICONTROL Module cible]** comme module juste avant le filtre que vous souhaitez copier.

1. Cliquez sur **[!UICONTROL Exécuter]**.
