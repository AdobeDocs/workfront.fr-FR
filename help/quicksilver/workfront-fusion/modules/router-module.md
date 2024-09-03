---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Module de routage dans Adobe Workfront Fusion
description: Le module routeur vous permet de diviser votre flux en plusieurs itinéraires et de traiter les données de chaque itinéraire différemment. Une fois qu’un module routeur reçoit un lot, il le transfère vers chaque itinéraire connecté dans l’ordre où les itinéraires ont été joints au module routeur.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 100%

---

# Module [!UICONTROL routeur] dans [!DNL Adobe Workfront Fusion]

Le module [!UICONTROL routeur] vous permet de diviser votre flux en plusieurs itinéraires et de traiter les données de chaque itinéraire différemment. Une fois qu’un module [!UICONTROL routeur] reçoit un lot, il le transfère vers chaque itinéraire connecté dans l’ordre où les itinéraires ont été joints au module [!UICONTROL routeur].

>[!NOTE]
>
>* Pour vérifier l’ordre des itinéraires, vous pouvez cliquer sur l’icône [!UICONTROL Alignement automatique] qui organisera les itinéraires en fonction de l’ordre de haut en bas.
>
>  Pour modifier l’ordre, supprimez le module [!UICONTROL routeur] et reconnectez les itinéraires dans l’ordre souhaité.
>
>* Les itinéraires sont traités de manière séquentielle, et non en parallèle. Un lot n’est pas envoyé vers l’itinéraire suivant tant qu’il n’a pas été complètement traité par l’itinéraire précédent.
>



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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ajouter un module [!UICONTROL routeur] à un scénario

Vous pouvez ajouter un module [!UICONTROL routeur] à un scénario de l’une des manières suivantes :

* Si vous souhaitez connecter le module [!UICONTROL routeur] après un module, cliquez sur la poignée droite du module, puis commencez à saisir **[!UICONTROL routeur]** pour le rechercher, puis choisissez **[!UICONTROL Contrôle de flux]** > **[!UICONTROL Routeur]** dans la liste des modules qui s’affiche.

  ![](assets/connect-the-router-350x108.png)

* Si vous souhaitez insérer le module [!UICONTROL routeur] entre deux modules, cliquez sur l’icône en forme de clé à molette sous l’itinéraire qui relie les deux modules (ou cliquez avec le bouton droit de la souris sur l’itinéraire) et choisissez **[!UICONTROL Ajouter un routeur]** dans le menu.

  ![](assets/insert-router-350x191.png)

* Vous pouvez insérer un module [!UICONTROL routeur] automatiquement. Par exemple, dans l’image ci-dessous, pour connecter le module dans le coin inférieur droit à celui du le coin supérieur gauche (qui est déjà connecté à celui du le coin supérieur droit), faites glisser la poignée gauche du module inférieur droit et déposez-le dans le module supérieur gauche.

  ![](assets/insert-router-automatically-350x379.png)

## Filtres

Vous pouvez placer un filtre sur un itinéraire après le module [!UICONTROL routeur] pour filtrer les lots comme sur tout autre itinéraire :

1. Cliquez sur l’un des points de l’itinéraire.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. Dans la zone **[!UICONTROL Configurer un filtre]** qui s’affiche, ajoutez des conditions, puis cliquez sur **[!UICONTROL OK]** pour enregistrer la configuration du filtre.

   ![](assets/set-up-a-filter-2-350x242.png)

Pour plus d’informations, voir [Ajouter un filtre à un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Itinéraire de secours

La configuration du filtre sur un itinéraire après un module [!UICONTROL routeur] contient une option spéciale : l’itinéraire de secours :

![](assets/fallback-route-350x260.png)

Lorsqu’il est activé, cet itinéraire est utilisé lorsqu’un lot ne peut pas continuer à partir du module [!UICONTROL routeur] via tout autre itinéraire, car les filtres sur les autres itinéraires l’ont filtré.

L’itinéraire de secours se distingue par un autre signe de flèche à l’intérieur du module [!UICONTROL routeur] :

![](assets/arrow-sign-in-router-module-350x361.png)

## Si/Dans le cas contraire

L’itinéraire de secours est habituellement utilisé pour poursuivre le flux avec un itinéraire si la condition est remplie et avec un autre itinéraire si elle ne l’est pas, comme dans les étapes suivantes :

1. Insérez un module [!UICONTROL routeur] dans votre scénario.
1. Connectez les deux itinéraires au module [!UICONTROL routeur].
1. Cliquez sur le premier itinéraire et spécifiez une condition :

   ![](assets/set-up-a-filter-2-350x242.png)

1. Cliquez sur le deuxième itinéraire et activez l’option [!UICONTROL Itinéraire de secours] :

   ![](assets/enable-fallback-route-option-350x238.png)
