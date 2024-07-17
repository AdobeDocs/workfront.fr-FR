---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Adobe Experience Manager Forms
description: Avec le connecteur  [!DNL Adobe Experience Manager Forms] pour le compte  [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Forms] , créez, téléchargez et mettez à jour des ressources, et copiez ou déplacez des dossiers et des ressources.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 107d81f7-ca41-4d76-a6dd-e579886dc2ad
source-git-commit: 6c7d22bea669586c56acfc23d328d7cc815b04be
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 41%

---

# Modules [!DNL Adobe Experience Manager Forms]

Avec le connecteur [!DNL Adobe Experience Manager Forms] pour [!DNL Adobe Workfront Fusion], vous pouvez démarrer un scénario basé sur les événements de votre compte [!DNL Adobe Experience Manager Forms] en créant un webhook.

Vous pouvez configurer un formulaire dans [!DNL Adobe Experience Manager Forms] pour envoyer des envois de formulaire à ce webhook.

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

## Conditions préalables

* Vous devez disposer d’un compte [!DNL Adobe Experience Manager Forms] pour utiliser ce module.

## Création d’une connexion à Adobe Experience Manager Forms

Pour créer une connexion pour vos modules [!DNL Adobe Experience Manager Forms] :

1. Cliquez sur **[!UICONTROL Ajouter]** en regard de la zone Connexion.

1. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Nommez cette connexion.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>
          <p>Indiquez si cette connexion se connecte à un environnement de production ou hors production.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>
          <p>Indiquez si ce compte est un compte de service ou un compte personnel.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL URL de l’instance sans barre oblique]</td>
        <td>
          <p>Saisissez l’URL d’accès au compte, sans la barre oblique.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Point d’entrée IMS]</td>
        <td>
          <p><code>https://ims-na1.adobelogin.com</code></p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Saisissez votre ID client [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Saisissez votre secret client [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID d’organisation]</td>
        <td>Saisissez votre ID d’organisation [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID du compte technique]</td>
        <td>Saisissez votre ID de compte technique [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] de l’[!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Portées des métadonnées]</td>
        <td>Saisissez les portées méta appropriées.       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Clé privée]</td>
        <td>
          <p>Entrez la clé privée qui a été générée lors de la création de vos informations d’identification dans le [!DNL Adobe Developer Console]. </p>
          <p>Pour extraire votre clé privée ou votre certificat :</p>
          <ol>
            <li value="1">
              <p>Cliquez sur <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Sélectionnez le type de fichier que vous extrayez.</p>
            </li>
            <li value="3">
              <p>Sélectionnez le fichier contenant la clé privée ou le certificat.</p>
            </li>
            <li value="4">
              <p>Saisissez le mot de passe du fichier.</p>
            </li>
            <li value="5">
              <p>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour extraire le fichier et revenir à la configuration de la connexion.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.

## Module Adobe Experience Manager Forms et ses champs

Actuellement, il n’existe qu’un seul module dans le connecteur Adobe Experience Manager Forms.

### Surveillance des événements de formulaire

Ce déclencheur instantané (webhook) vous permet de lancer un scénario lorsqu’une action Envoyer se produit sur un formulaire Adobe Experience Manager.

>[!IMPORTANT]
>
>Ce module nécessite également une configuration dans Adobe Experience Manager. Après avoir configuré ce webhook, vous devez ouvrir Adobe Experience Manager et configurer votre formulaire pour envoyer des envois au webhook.
>
><!--For instructions on the required form configuration, see insert url here-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p>Saisissez le nom du webhook.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL Adobe Experience Manager] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">Créer une connexion à [!DNL Adobe Experience Manager Forms]</a></p> </td> 
  </tr>

Le module crée un webhook et vous donne l’adresse webhook, que vous pouvez saisir dans la boîte de dialogue d’envoi du formulaire dans [!DNL Adobe Experience Manager Forms].
