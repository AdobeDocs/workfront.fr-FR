---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: connections-annd-webhooks
title: Créer une connexion à  [!DNL Adobe Workfront Fusion]  - Instructions de base
description: De nombreux connecteurs  [!DNL Adobe Workfront Fusion]  ne nécessitent pas de configuration personnalisée lors de la création d’une connexion. Cet article décrit le processus de création de connexion par défaut.
author: Becky
feature: Workfront Fusion
exl-id: 6576a515-a1a1-4613-8d04-3c9d36bb1ed9
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 100%

---

# Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Créer une connexion

Pour créer une connexion dans un module [!DNL Workfront Fusion], procédez comme suit :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la case [!UICONTROL Connexion] pour ouvrir le panneau **[!UICONTROL Créer une connexion]**.
1. (Facultatif) Modifiez le **[!UICONTROL nom de la connexion]** par défaut.
1. (Le cas échéant) Si l’application nécessite des paramètres de connexion avancés, tels qu’un identifiant, une clé ou [!UICONTROL secret], saisissez ces informations.

   Il se peut que vous deviez cliquer sur **[!UICONTROL Afficher les paramètres avancés]** pour afficher les champs dans lesquels saisir ce type d’informations.

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre de connexion qui s’affiche, saisissez vos informations d’identification pour vous connecter à l’application si vous ne l’avez pas déjà fait.
1. (Le cas échéant) Si un bouton **[!UICONTROL Autoriser]** s’affiche, examinez les actions que le connecteur pourra effectuer, puis cliquez sur le bouton pour connecter l’application à [!DNL Workfront Fusion].

   >[!NOTE]
   >
   >Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations d’utilisateur ou d’utilisatrice. Ainsi, lors de la création d’une connexion, l’écran de consentement aux autorisations affiche les autorisations précédemment accordées à la connexion de cet utilisateur ou de cette utilisatrice, en plus des nouvelles autorisations nécessaires à l’application actuelle.
   >
   >Par exemple, si un utilisateur ou une utilisatrice dispose d’autorisations « Lire le tableau » accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les e-mails, l’écran de consentement aux autorisations affiche à la fois l’autorisation « Lire le tableau » déjà accordée et l’autorisation « Écrire des e-mails » nouvellement requise.