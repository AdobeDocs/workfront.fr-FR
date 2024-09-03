---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Gérer des scénarios verrouillés dans  [!DNL Adobe Workfront Fusion]
description: Gérer des scénarios verrouillés dans  [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 5fccf336-d904-43fe-ad4a-c3ce76dbcad0
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 100%

---

# Gérer des scénarios verrouillés dans [!DNL Adobe Workfront Fusion]

Dans certains cas, un scénario peut être temporairement verrouillé dans [!DNL Workfront Fusion]. Les exécutions verrouillées seront automatiquement déverrouillées dans les 2 à 4 heures. Vous pouvez également déverrouiller les scénarios manuellement.

>[!IMPORTANT]
>
>Le déverrouillage manuel d’un scénario peut entraîner des erreurs d’exécution du scénario.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Présentation des scénarios verrouillés

Les scénarios peuvent être verrouillés pour plusieurs raisons.

Workfront Fusion ne prend pas en charge le traitement parallèle de scénarios planifiés. Ces scénarios sont verrouillés au début de l’exécution du scénario et déverrouillés à la fin. Si l’exécution est interrompue, le scénario peut ne pas se déverrouiller. Cela peut se produire lorsqu’un utilisateur ou une utilisatrice force manuellement l’arrêt du scénario ou en cas de problème du système.

En outre, l’équipe d’ingénierie de Workfront Fusion peut verrouiller un scénario, car il entraîne des problèmes de performances ou d’autres problèmes.

Quelle que soit la cause d’un scénario verrouillé, le scénario se déverrouille automatiquement 2 à 4 heures après son verrouillage.

## Déverrouiller un scénario verrouillé

Les scénarios verrouillés seront déverrouillés 2 à 4 heures après leur verrouillage. Vous pouvez déverrouiller un scénario manuellement avant qu’il ne soit automatiquement déverrouillé.

Le déverrouillage manuel d’un scénario peut entraîner des erreurs d’exécution du scénario. Nous vous recommandons de déverrouiller manuellement les scénarios uniquement lorsqu’un scénario est verrouillé en raison du démarrage et de l’arrêt des exécutions dans le cadre de la conception du scénario. Dans d’autres cas, nous vous recommandons d’attendre que le scénario soit déverrouillé automatiquement.

>[!IMPORTANT]
>
>Le déverrouillage manuel d’un scénario peut entraîner des erreurs d’exécution du scénario.

1. Accédez à la page Détails du scénario du scénario verrouillé.
1. Cliquez sur **[!UICONTROL Options]** dans le coin supérieur droit de l’écran.
1. Sélectionnez **[!UICONTROL Déverrouiller l’exécution]**.
1. Cliquez sur **[!UICONTROL Déverrouiller]**.
