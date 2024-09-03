---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Choisir le point de départ d’un module de déclenchement dans Adobe Workfront Fusion
description: Certains modules déclencheur vous permettent de sélectionner le premier lot à partir duquel vous souhaitez que la récupération des lots démarre.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 489ed23fe0d7945753b59810ff9da084bd3e92e4
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 100%

---

# Sélectionnez l’endroit où démarrer un module déclencheur dans [!DNL Adobe Workfront Fusion].

Certains modules déclencheur vous permettent de sélectionner le premier lot à partir duquel vous souhaitez que la récupération des lots démarre.

Vous pouvez également indiquer si vous souhaitez récupérer tous les lots ou uniquement les lots à partir d’une date spécifique.

Pour plus d’informations sur les modules déclencheur, voir la section [Déclencher des modules](../../workfront-fusion/modules/module-types.md#triggers) dans l’article [Types de modules](../../workfront-fusion/modules/module-types.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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

+++

## Choisir l’emplacement de démarrage d’un module déclencheur

1. Enregistrez un module déclencheur.

   Ou

   Modifiez les paramètres du module déclencheur comme décrit dans la section [Configurer les paramètres d’un module dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Ou

   Cliquez avec le bouton droit de la souris sur l’icône correspondant au module déclencheur dans l’[!UICONTROL éditeur de scénario], comme décrit dans [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Sélectionnez une option dans la zone **[!UICONTROL Choisir l’emplacement de démarrage]** qui s’affiche.

   ![](assets/choose-where-to-start-350x346.jpg)

   Les options affichées dépendent des possibilités d’un service donné. Elles peuvent inclure les éléments suivants :

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL From now on] (par défaut)</td>
            <td>Récupère désormais tous les lots ajoutés ou mis à jour (en fonction des paramètres).</td>
        </tr>
        <tr>
            <td>[!UICONTROL From after a specific date]</td>
            <td>Récupère tous les lots ajoutés ou mis à jour (en fonction des paramètres) après une date/heure spécifiée</td>
        </tr>
        <tr>
            <td>[!UICONTROL With ID greater than or equal to a specific value]</td>
            <td>Récupère tous les lots avec un ID supérieur ou égal à un ID spécifié</td> 
        </tr>
        <tr>
            <td>[!UICONTROL All bundles]</td>
            <td>Récupère tous les lots disponibles</td>
        </tr>
        <tr>
            <td>[!UICONTROL Select the first bundle]</td>
            <td>Permet de sélectionner le premier lot à partir duquel la récupération des lots doit démarrer.</td>
        </tr>
   </table>
