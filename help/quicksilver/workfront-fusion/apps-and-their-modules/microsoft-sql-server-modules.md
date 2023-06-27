---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules Microsoft SQL Server
description: Vous pouvez utiliser [!DNL Adobe Workfront Fusion] pour vous connecter à Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# [!DNL Microsoft SQL Server] modules

Vous pouvez utiliser [!DNL Adobe Workfront Fusion] pour se connecter à [!UICONTROL Microsoft SQL Server].

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

## Utilisation [!DNL Microsoft SQL Server] modules

Vous pouvez exécuter votre logique personnalisée directement sur votre serveur de base de données par le biais de procédures stockées. [!DNL Adobe Workfront Fusion] charge dynamiquement l’interface des paramètres d’entrée/de sortie et du jeu d’enregistrements afin que chaque paramètre ou valeur puisse être mappé individuellement. Avant de commencer à configurer votre scénario, assurez-vous que le compte que vous utilisez pour vous connecter à votre base de données dispose d’un accès en lecture à `INFORMATION_SCHEMA.ROUTINES` et `INFORMATION_SCHEMA.PARAMETERS` vues.

When [!DNL Fusion] établit la connexion à la variable [!DNL SQL server] destination, la variable [!DNL Fusion] L’utilisateur identifie l’hôte (le nom de domaine ou l’adresse IP où le serveur est hébergé) et le port. [!DNL Fusion] peut se connecter à n’importe quel hôte et port disponibles.

Pour plus d’informations sur les adresses IP spécifiques utilisées par [!DNL Workfront Fusion], voir [Adresses IP pour l’accès [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Pour en savoir plus sur la création d’une procédure stockée, reportez-vous à la section [!DNL Microsoft SQL Server] documentation.

>[!NOTE]
>
>[!DNL Workfront Fusion] ne prend pas en charge plusieurs jeux d’enregistrements. Seul le premier est traité.

## Erreur de dépannage [!UICONTROL ER_LOCK_WAIT_TIMEOUT : Dépassement du délai d’attente de verrouillage ; essayer de redémarrer la transaction]

Cette erreur se produit lorsque vous modifiez les mêmes données à l’aide de plusieurs modules. Il est dû à des transactions SQL.

Lorsqu&#39;un module SQL est exécuté, il lance une transaction. La transaction est terminée une fois le scénario entièrement exécuté.

Si un autre module tente d&#39;accéder aux mêmes données, il doit attendre que la transaction précédente soit terminée. Puisque la première transaction sera terminée une fois le scénario terminé, la seconde transaction ne pourra jamais commencer.

### Solution :

Activez la validation automatique. La validation automatique termine (valide) chaque transaction immédiatement après la fin de l’exécution du module.

1. Cliquez sur le bouton [!UICONTROL Paramètres du scénario] icon ![](assets/scenario-settings-icon.png)au bas de l’écran.
1. Cliquez sur le bouton **[!UICONTROL Validation automatique]** .
1. Cliquez sur **[!UICONTROL OK]** pour enregistrer les paramètres du scénario.
