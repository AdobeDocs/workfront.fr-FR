---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: connections-annd-webhooks
title: Création d’une connexion à [!DNL Adobe Workfront Fusion]  - Instructions de base
description: De nombreux connecteurs  [!DNL Adobe Workfront Fusion] ne nécessitent pas de configuration personnalisée lors de la création d’une connexion. Cet article décrit le processus de création de connexion par défaut.
author: Becky
feature: Workfront Fusion
exl-id: 6576a515-a1a1-4613-8d04-3c9d36bb1ed9
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 32%

---

# Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base

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

## Création d’une connexion

Pour créer une connexion dans un module [!DNL Workfront Fusion] :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone [!UICONTROL Connexion] pour ouvrir le panneau **[!UICONTROL Créer une connexion]**.
1. (Facultatif) Modifiez le **[!UICONTROL nom de connexion]** par défaut.
1. (Conditionnel) Si l’application nécessite des paramètres de connexion avancés, tels qu’un identifiant, une clé ou [!UICONTROL secret], saisissez ces informations.

   Vous devrez peut-être cliquer sur **[!UICONTROL Afficher les paramètres avancés]** pour afficher les champs où vous pouvez saisir ce type d’informations.

1. Cliquez sur **[!UICONTROL Continuer]**.
1. Dans la fenêtre de connexion qui s’affiche, saisissez vos informations d’identification pour vous connecter à l’application si vous ne l’avez pas déjà fait.
1. (Conditionnel) Si un bouton **[!UICONTROL Autoriser]** s’affiche, examinez les actions que le connecteur pourra entreprendre, puis cliquez sur le bouton pour connecter l’application à [!DNL Workfront Fusion].

   >[!NOTE]
   >
   >Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations utilisateur individuelles. Par conséquent, lors de la création d’une connexion, l’écran de consentement des autorisations affiche les autorisations qui ont été accordées à la connexion de cet utilisateur, en plus des nouvelles autorisations nécessaires à l’application actuelle.
   >
   >Par exemple, si un utilisateur dispose d’autorisations &quot;Lecture de tableau&quot; accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les emails, l’écran de consentement des autorisations affiche à la fois l’autorisation &quot;Lecture de tableau&quot; déjà accordée et l’autorisation &quot;Ecriture d’email&quot; nouvellement requise.