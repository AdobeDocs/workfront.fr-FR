---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Microsoft SQL Server
description: Vous pouvez utiliser [!DNL Adobe Workfront Fusion] pour vous connecter à Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 22%

---

# Modules [!DNL Microsoft SQL Server]

Vous pouvez utiliser [!DNL Adobe Workfront Fusion] pour se connecter à [!UICONTROL Microsoft SQL Server].

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
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



## Connexion de la variable [!DNL Microsoft SQL Server] service à [!DNL Workfront Fusion]

Pour obtenir des instructions sur la connexion à [!DNL Microsoft SQL Server] compte à [!UICONTROL Workfront Fusion], voir [Créer une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations utilisateur individuelles. Par conséquent, lors de la création d’une connexion, l’écran de consentement des autorisations affiche les autorisations qui ont été accordées à la connexion de cet utilisateur, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur dispose d’autorisations &quot;Lecture de tableau&quot; accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les emails, l’écran de consentement des autorisations affiche à la fois l’autorisation &quot;Lecture de tableau&quot; déjà accordée et l’autorisation &quot;Ecriture d’email&quot; nouvellement requise.

## Utilisation [!DNL Microsoft SQL Server] modules

Vous pouvez exécuter votre logique personnalisée directement sur votre serveur de base de données par le biais de procédures stockées. [!DNL Adobe Workfront Fusion] charge dynamiquement l’interface des paramètres d’entrée/de sortie et du jeu d’enregistrements afin que chaque paramètre ou valeur puisse être mappé individuellement. Avant de commencer à configurer votre scénario, assurez-vous que le compte que vous utilisez pour vous connecter à votre base de données dispose d’un accès en lecture à `INFORMATION_SCHEMA.ROUTINES` et `INFORMATION_SCHEMA.PARAMETERS` vues.

When [!DNL Fusion] établit la connexion à la variable [!DNL SQL server] destination, la variable [!DNL Fusion] L’utilisateur identifie l’hôte (le nom de domaine ou l’adresse IP où le serveur est hébergé) et le port. [!DNL Fusion] peut se connecter à n’importe quel hôte et port disponibles.

Pour plus d’informations sur les adresses IP spécifiques utilisées par [!DNL Workfront Fusion], voir [Adresses IP pour l’accès [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Pour en savoir plus sur la création d’une procédure stockée, voir la section [!DNL Microsoft SQL Server] la documentation.

>[!NOTE]
>
>[!DNL Workfront Fusion] ne prend pas en charge plusieurs jeux d’enregistrements. Seul le premier est traité.

## Erreur de dépannage [!UICONTROL ER_LOCK_WAIT_TIMEOUT : le délai d’attente de verrouillage a été dépassé ; essayez de redémarrer la transaction.]

Cette erreur se produit lorsque vous modifiez les mêmes données à l’aide de plusieurs modules. Il est dû à des transactions SQL.

Lorsqu&#39;un module SQL est exécuté, il lance une transaction. La transaction est terminée une fois le scénario entièrement exécuté.

Si un autre module tente d&#39;accéder aux mêmes données, il doit attendre que la transaction précédente soit terminée. Puisque la première transaction sera terminée une fois le scénario terminé, la seconde transaction ne pourra jamais commencer.

### Solution :

Activez la validation automatique. La validation automatique termine (valide) chaque transaction immédiatement après la fin de l’exécution du module.

1. Cliquez sur le bouton [!UICONTROL Paramètres du scénario] icon ![](assets/scenario-settings-icon.png)au bas de l’écran.
1. Cliquez sur le bouton **[!UICONTROL Validation automatique]** .
1. Cliquez sur **[!UICONTROL OK]** pour enregistrer les paramètres du scénario.
