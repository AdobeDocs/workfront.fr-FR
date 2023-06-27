---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Choix de l’endroit où commence un module de déclenchement dans Adobe Workfront Fusion
description: Certains modules de déclenchement vous permettent de sélectionner le premier lot à partir duquel vous souhaitez que la récupération des lots démarre.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Sélectionnez l’endroit où commence un module de déclenchement dans [!DNL Adobe Workfront Fusion]

Certains modules de déclenchement vous permettent de sélectionner le premier lot à partir duquel vous souhaitez que la récupération des lots démarre.

Vous pouvez également indiquer si vous souhaitez récupérer tous les lots ou uniquement les lots à partir d’une date spécifique.

Pour plus d’informations sur les modules de déclenchement, voir la section [Déclencher des modules](../../workfront-fusion/modules/module-types.md#triggers) dans l’article [Types de modules](../../workfront-fusion/modules/module-types.md).

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

## Choix de l’emplacement de démarrage d’un module de déclenchement

1. Enregistrez un module de déclenchement.

   Ou

   Modifiez les paramètres du module de déclencheur comme décrit dans la section [Configurez les paramètres d’un module dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Ou

   Cliquez avec le bouton droit de la souris sur l’icône correspondant au module de déclenchement dans le [!UICONTROL Éditeur de scénario], comme décrit dans [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Sélectionnez une option dans le **[!UICONTROL Choisir où commencer]** qui s’affiche.

   ![](assets/choose-where-to-start-350x346.jpg)

   Les options affichées dépendent des possibilités d&#39;un service donné. Ils peuvent inclure les éléments suivants :

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL À partir de maintenant] (par défaut)</td>
            <td>Récupère désormais tous les lots ajoutés ou mis à jour (en fonction des paramètres).</td>
        </tr>
        <tr>
            <td>[!UICONTROL À partir d’une date spécifique]</td>
            <td>Récupère tous les lots ajoutés ou mis à jour (en fonction des paramètres) après une date/heure spécifiée</td>
        </tr>
        <tr>
            <td>[!UICONTROL Avec un ID supérieur ou égal à une valeur spécifique]</td>
            <td>Récupère tous les lots avec un ID supérieur ou égal à un ID spécifié</td> 
        </tr>
        <tr>
            <td>[!UICONTROL Tous les lots]</td>
            <td>Récupère tous les lots disponibles</td>
        </tr>
        <tr>
            <td>[!UICONTROL Sélectionner le premier lot]</td>
            <td>Permet de sélectionner le premier lot à partir duquel la récupération des lots doit commencer.</td>
        </tr>
   </table>
