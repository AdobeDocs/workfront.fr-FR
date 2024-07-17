---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ajout d’un filtre à un scénario dans  [!DNL Adobe] Workfront Fusion
description: Dans certains scénarios, vous devez travailler uniquement avec des lots qui répondent à des critères spécifiques. Les filtres vous permettent de sélectionner ces lots.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 21%

---

# Ajout d’un filtre à un scénario dans [!DNL Adobe Workfront Fusion]

Dans certains scénarios, vous devez travailler uniquement avec des lots qui répondent à des critères spécifiques. Les filtres vous permettent de sélectionner ces lots.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Vous pouvez ajouter un filtre entre deux modules et vérifier si les lots reçus des modules précédents remplissent des conditions de filtrage spécifiques :

* Si tel est le cas, les lots sont transmis au module suivant dans le scénario.
* Dans le cas contraire, le traitement des lots s’arrête.

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
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

## Conditions préalables

Vous devez ajouter les deux modules à un scénario avant de pouvoir ajouter un filtre entre eux.

## Ajoutez un filtre entre deux modules :

1. Cliquez sur **[!UICONTROL Scénarios]** ![](assets/scenarios-icon.png) dans le panneau de gauche, puis sélectionnez le scénario pour l’ouvrir.
1. Dans le coin supérieur droit de la fenêtre, cliquez sur **[!UICONTROL Modifier]**.
1. Cliquez sur la ligne de connexion entre les modules.
1. Dans la zone qui s’affiche, saisissez un **[!UICONTROL Libellé]** pour le filtre.
1. Définissez un filtre **[!UICONTROL Condition]**.

   Vous pouvez saisir un ou deux opérandes dans les deux zones. Si vous saisissez des opérandes dans les deux zones, vous pouvez sélectionner un opérateur dans le menu déroulant situé entre les deux afin de définir la relation entre eux.

   >[!TIP]
   >
   >Dans les champs de l’opérande, vous pouvez saisir des valeurs de la même manière que vous les mappez, comme décrit dans la section [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Par exemple, si vous souhaitez que le filtre trouve des fichiers dans [!DNL Adobe Workfront] se terminant par XML et les transmettant à [!DNL Dropbox], saisissez **[!UICONTROL Nom de fichier]** dans la première zone et .**[!UICONTROL xml]** dans la seconde zone. Dans le menu déroulant qui les sépare, vous sélectionnez **[!UICONTROL Se termine par (non-respect de la casse)]**. Ce filtre s’appliquerait aux lots entrants du premier module (Workfront). Seuls les lots contenant des fichiers XML passeraient au module suivant ([!DNL Dropbox]).

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

1. Installez l’extension [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome].
1. Dans [!DNL Workfront Fusion], ouvrez le scénario.
1. Cliquez sur le menu à trois points Chrome, puis sur **[!UICONTROL Autres outils*]* > **[!UICONTROL Outils de développement]**.

1. Dans le panneau [!UICONTROL Outils de développement] qui s’affiche, dans la barre de menus en haut, cliquez sur l’onglet [!UICONTROL Workfront Fusion].

   ![](assets/copy-a-filter-350x174.png)

1. Cliquez sur l’icône **[!UICONTROL Outils]** ![](assets/devtools-tools-icon.png) dans la barre de gauche.

1. Cliquez sur **[!UICONTROL Copier le filtre]**, puis configurez l’outil **[!UICONTROL Copier le filtre]** dans le panneau de droite :

   1. Définissez le **[!UICONTROL module Source]** comme module juste après le filtre que vous souhaitez copier.
   1. Définissez le **[!UICONTROL module Target]** comme module juste avant le filtre que vous souhaitez copier.

1. Cliquez sur **[!UICONTROL Exécuter]**.
