---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Choisir le point de départ d’un module de déclenchement dans Adobe Workfront Fusion
description: Certains modules de déclenchement vous permettent de sélectionner le premier lot à partir duquel vous souhaitez que la récupération des lots démarre.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 34%

---

# Choisir l’endroit où un module de déclenchement commence dans [!DNL Adobe Workfront Fusion]

Certains modules de déclenchement vous permettent de sélectionner le premier lot à partir duquel vous souhaitez que la récupération des lots démarre.

Vous pouvez également indiquer si vous souhaitez récupérer tous les lots ou uniquement les lots à partir d’une date spécifique.

Pour plus d’informations sur les modules de déclenchement, consultez la section [Déclencher des modules](../../workfront-fusion/modules/module-types.md#triggers) dans l’article [Types de modules](../../workfront-fusion/modules/module-types.md).

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
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## Choix de l’emplacement de démarrage d’un module de déclenchement

1. Enregistrez un module de déclenchement.

   Ou

   Modifiez les paramètres du module déclencheur comme décrit dans [Configurer les paramètres d’un module dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   Ou

   Cliquez avec le bouton droit de la souris sur l’icône du module de déclenchement dans l’ [!UICONTROL éditeur de scénario], comme décrit dans la section [Créer un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Sélectionnez une option dans la zone **[!UICONTROL Choisir où commencer]** qui s&#39;affiche.

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
