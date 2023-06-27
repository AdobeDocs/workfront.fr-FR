---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Module de routeur dans Adobe Workfront Fusion
description: Le module Router vous permet de diviser votre flux en plusieurs itinéraires et de traiter les données de chaque itinéraire différemment. Une fois qu’un module de routeur reçoit un lot, il le transfère vers chaque itinéraire connecté dans l’ordre où les itinéraires ont été attachés au module de routeur.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!UICONTROL Routeur] module dans [!DNL Adobe Workfront Fusion]

Le [!UICONTROL Routeur] vous permet de diviser votre flux en plusieurs itinéraires et de traiter les données de chaque itinéraire différemment. Une fois un [!UICONTROL Routeur] module reçoit un lot, il le transfère vers chaque itinéraire connecté dans l’ordre où les itinéraires ont été associés à la variable [!UICONTROL Routeur] module .

>[!NOTE]
>
>* Pour vérifier l’ordre des itinéraires, vous pouvez cliquer sur le bouton [!UICONTROL Alignement automatique] qui organisera les itinéraires en fonction de l’ordre de haut en bas.
>
>  Pour modifier l’ordre, supprimez la variable [!UICONTROL Routeur] et reliez à nouveau les itinéraires dans l’ordre souhaité.
>
>* Les itinéraires sont traités de manière séquentielle, et non en parallèle. Un lot n’est pas envoyé vers l’itinéraire suivant tant qu’il n’a pas été complètement traité par l’itinéraire précédent.
>



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
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
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

## Ajouter un [!UICONTROL Routeur] vers un scénario

A [!UICONTROL Routeur] peut être ajouté à un scénario de l’une des manières suivantes :

* Si vous souhaitez connecter la variable [!UICONTROL Routeur] après un module, cliquez sur la poignée droite du module, puis commencez à saisir **[!UICONTROL routeur]** pour la rechercher, puis choisissez **[!UICONTROL Contrôle de flux]** > **[!UICONTROL Routeur]** dans la liste des modules qui s’affiche.

  ![](assets/connect-the-router-350x108.png)

* Si vous souhaitez insérer la variable [!UICONTROL Routeur] module entre deux modules, cliquez sur l&#39;icône en forme de clé à molette sous l&#39;itinéraire reliant les deux modules (ou cliquez avec le bouton droit de la souris sur l&#39;itinéraire) et choisissez **[!UICONTROL Ajouter un routeur]** dans le menu.

  ![](assets/insert-router-350x191.png)

* Vous pouvez insérer une [!UICONTROL Routeur] module automatiquement. Par exemple, dans l’image ci-dessous, pour connecter le module dans le coin inférieur droit à celui dans le coin supérieur gauche (qui est déjà connecté à celui dans le coin supérieur droit), faites glisser la poignée gauche du module inférieur droit et déposez-le dans le module supérieur gauche.

  ![](assets/insert-router-automatically-350x379.png)

## Filtres

Vous pouvez placer un filtre sur un itinéraire après l’événement [!UICONTROL Routeur] pour filtrer les lots comme sur tout autre itinéraire :

1. Cliquez sur l’un des points de l’itinéraire.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. Dans le **[!UICONTROL Configurer un filtre]** s’affiche, ajoutez des conditions, puis cliquez sur **[!UICONTROL OK]** pour enregistrer la configuration du filtre.

   ![](assets/set-up-a-filter-2-350x242.png)

Pour plus d’informations, voir [Ajoutez un filtre à un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Itinéraire de secours

La configuration du filtre sur un itinéraire après une [!UICONTROL Routeur] module contient une option spéciale : L’itinéraire de secours :

![](assets/fallback-route-350x260.png)

Lorsqu’il est activé, cet itinéraire est utilisé lorsqu’un lot ne peut pas continuer à partir de la variable [!UICONTROL Routeur] via tout autre itinéraire, car les filtres sur les autres itinéraires l’ont filtré.

L’itinéraire de secours se distingue par un autre signe fléché à l’intérieur du [!UICONTROL Routeur] module :

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Un cas d’utilisation type de l’itinéraire de secours consiste à poursuivre le flux avec un itinéraire si la condition est remplie et avec un autre itinéraire s’il ne l’est pas, comme dans les étapes suivantes :

1. Insérer une [!UICONTROL Routeur] dans votre scénario.
1. Connectez les deux itinéraires à [!UICONTROL Routeur] module .
1. Cliquez sur le premier itinéraire et spécifiez une condition :

   ![](assets/set-up-a-filter-2-350x242.png)

1. Cliquez sur le deuxième itinéraire et activez la variable [!UICONTROL itinéraire de secours] option :

   ![](assets/enable-fallback-route-option-350x238.png)
