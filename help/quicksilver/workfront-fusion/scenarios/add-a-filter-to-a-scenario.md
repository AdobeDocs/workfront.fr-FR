---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ajoutez un filtre à un scénario dans [!DNL Adobe] Workfront Fusion
description: Dans certains scénarios, vous devez travailler uniquement avec des lots qui répondent à des critères spécifiques. Les filtres vous permettent de sélectionner ces lots.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Ajoutez un filtre à un scénario dans [!DNL Adobe Workfront Fusion]

Dans certains scénarios, vous devez travailler uniquement avec des lots qui répondent à des critères spécifiques. Les filtres vous permettent de sélectionner ces lots.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Vous pouvez ajouter un filtre entre deux modules et vérifier si les lots reçus des modules précédents remplissent des conditions de filtrage spécifiques :

* Si tel est le cas, les lots sont transmis au module suivant dans le scénario.
* Dans le cas contraire, le traitement des lots s’arrête.

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

## Conditions préalables

Vous devez ajouter les deux modules à un scénario avant de pouvoir ajouter un filtre entre eux.

## Ajoutez un filtre entre deux modules :

1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche, sélectionnez le scénario à ouvrir.
1. Dans le coin supérieur droit de la fenêtre, cliquez sur **[!UICONTROL Modifier]**.
1. Cliquez sur la ligne de connexion entre les modules.
1. Dans la zone qui s’affiche, saisissez une **[!UICONTROL Libellé]** pour le filtre.
1. Définir un filtre **[!UICONTROL Condition]**.

   Vous pouvez saisir un ou deux opérandes dans les deux zones. Si vous saisissez des opérandes dans les deux zones, vous pouvez sélectionner un opérateur dans le menu déroulant situé entre les deux afin de définir la relation entre eux.

   >[!TIP]
   >
   >Dans les champs de l’opérande, vous pouvez saisir des valeurs de la même manière que vous les mappez, comme décrit dans la section [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Par exemple, si vous souhaitez que le filtre recherche des fichiers dans [!DNL Adobe Workfront] se terminant par XML et les transmettant à [!DNL Dropbox], vous devez entrer **[!UICONTROL Nom du fichier]** dans la première zone et .**[!UICONTROL xml]** dans la seconde zone. Dans le menu déroulant qui les sépare, vous pouvez sélectionner **[!UICONTROL Se termine par (non-respect de la casse)]**. Ce filtre s’appliquerait aux lots entrants du premier module (Workfront). Seuls les lots contenant des fichiers XML sont transmis au module suivant ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Cliquez sur **[!DNL OK]**.

## Copier un filtre

Actuellement, l’éditeur de scénario n’inclut pas de fonctionnalité de copie d’un filtre.

>[!NOTE]
>
>Si vous copiez les modules de chaque côté du filtre, le filtre est également copié.
>
>Pour plus d’informations sur la copie de modules, voir [Copie de modules ou de scénarios dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Pour copier un filtre sans copier de modules, vous pouvez utiliser [!DNL Google] Chrome pour la solution de contournement suivante :

1. Installez le [!UICONTROL [!DNL Adobe Workfront Fusion] Chrome DevTool] extension .
1. Dans [!DNL Workfront Fusion], ouvrez le scénario.
1. Cliquez sur le menu à trois points de Chrome, puis sur **[!UICONTROL Autres outils*]* > **[!UICONTROL Outils de développement]**.

1. Dans le [!UICONTROL Outils de développement] qui s’affiche, dans la barre de menus située en haut, cliquez sur l’icône [!UICONTROL Workfront Fusion] .

   ![](assets/copy-a-filter-350x174.png)

1. Cliquez sur le bouton **[!UICONTROL Outils]** icon ![](assets/devtools-tools-icon.png) dans la barre de gauche.

1. Cliquez sur **[!UICONTROL Copier le filtre]**, puis configurez la variable **[!UICONTROL Copier le filtre]** dans le panneau latéral droit :

   1. Définissez la variable **[!UICONTROL Module source]** comme module juste après le filtre que vous souhaitez copier.
   1. Définissez la variable **[!UICONTROL Module Target]** comme module juste avant le filtre que vous souhaitez copier.

1. Cliquez sur **[!UICONTROL Exécuter]**.
