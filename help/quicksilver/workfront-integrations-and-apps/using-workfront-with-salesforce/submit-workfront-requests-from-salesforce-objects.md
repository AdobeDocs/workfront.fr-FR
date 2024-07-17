---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Envoi de  [!DNL Adobe Workfront]  demandes provenant d'objets  [!DNL Salesforce]
description: Après l’installation de  [!DNL Adobe Workfront] pour [!DNL Salesforce], you can submit [!DNL Workfront] demandes provenant de [!DNL Salesforce] Opportunités et comptes. Cette fonctionnalité existe dans les frameworks d’expérience classique et d’éclair.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 7%

---

# Envoi de [!DNL Adobe Workfront] demandes provenant d&#39;objets [!DNL Salesforce]

Après avoir installé [!DNL Adobe Workfront for Salesforce], vous pouvez envoyer des requêtes [!DNL Workfront] provenant de [!DNL Salesforce] opportunités et comptes. Cette fonctionnalité existe dans les structures [!DNL Classic] et [!DNL Lightning Experience].

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] forfait*</p></td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] licence*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Pour envoyer une requête [!DNL Workfront] d&#39;une opportunité ou d&#39;un compte [!DNL Salesforce], vérifiez que vous disposez des éléments suivants dans votre environnement :

* Votre administrateur [!DNL Workfront] a installé [!DNL Workfront for Salesforce].\
   Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Salesforce], voir [Installation [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Votre administrateur [!DNL Workfront] a ajouté la section [!DNL Workfront] à vos mises en page [!UICONTROL Opportunity] et [!UICONTROL Account].\
   Pour plus d’informations sur l’ajout de la section [!DNL Workfront] à une mise en page, voir [Configuration de la section  [!DNL Adobe Workfront] pour les  [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Vous disposez d&#39;un compte [!DNL Workfront] et vous pouvez vous y connecter à partir de la section [!DNL Workfront] de votre opportunité ou compte.\
   Une fois connecté, vous pouvez voir l’onglet [!UICONTROL Nouvelles requêtes] où vous pouvez commencer à saisir des requêtes.

## Envoyer [!DNL Workfront] demandes de [!DNL Salesforce]

1. Accédez à une opportunité ou à un compte dans Salesforce.
1. Accédez à la section [!DNL Workfront] .
1. Dans l’onglet **[!UICONTROL Nouvelles requêtes]** , sélectionnez un type de requête dans le menu déroulant **[!UICONTROL Sélectionner un type de requête]** .

   Vous pouvez voir les mêmes files d’attente de requête que celles que vous avez accès à voir dans Workfront.

1. Renseignez tout d’abord les champs disponibles pour votre requête.

   L&#39;envoi d&#39;une demande de [!DNL Salesforce] est identique à l&#39;envoi d&#39;une demande dans l&#39;application web [!DNL Workfront].

   >[!NOTE]
   >
   >Le téléchargement d’un document à l’aide du module externe [!DNL Workfront] dans [!DNL Salesforce] est temporairement indisponible.

   Continuez à suivre les étapes décrites dans [Créer et envoyer [!DNL Adobe Workfront] requêtes](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Cliquez sur **[!UICONTROL Soumettre]**.

## Affichage de [!DNL Workfront] requêtes

1. Accédez à une opportunité ou à un compte dans [!DNL Salesforce].
1. Accédez à la section **[!DNL Workfront]** .

   >[!NOTE]
   >
   >Selon la façon dont votre administrateur [!DNL Workfront] a configuré cette section, elle peut porter un nom différent.

1. Sélectionnez l’onglet **[!UICONTROL Demandes envoyées]** .

   Vous pouvez afficher toutes les requêtes que vous ou d’autres avez envoyées à partir de cette opportunité ou de ce compte dans cet onglet. Les requêtes envoyées à cette file d’attente de requêtes dans l’application web ne s’affichent pas dans cette liste dans [!DNL Salesforce].

   >[!NOTE]
   >
   >Les requêtes envoyées à cette file d’attente de requêtes dans l’application web ne s’affichent pas dans cette liste dans Salesforce.

   ![salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Vous pouvez afficher les informations suivantes sur les demandes envoyées :

   * Nom des requêtes (dans la colonne [!UICONTROL Objet])
   * Numéro de référence
   * Type de demande
   * Statut
   * Envoyé à la date
   * Demandé par nom
   * Attribué à Nom\

     Lorsque ces informations sont mises à jour dans [!DNL Workfront], elles sont également mises à jour dans cette liste.

1. (Facultatif) Cliquez sur le nom de la requête pour l’ouvrir dans [!DNL Workfront].

1. (Facultatif) Cliquez sur **[!UICONTROL Aller à[!DNL Salesforce]]** pour accéder à l’opportunité ou au compte où le problème provient des zones suivantes de Workfront :

   * Dans la section [!UICONTROL Details] du problème
   * Dans le panneau Résumé lors de la sélection du problème dans une liste, après avoir cliqué sur [!UICONTROL Ouvrir le résumé] ![](assets/summary-panel-icon.png) dans la barre d’outils de la liste.
   * Dans l’en-tête du problème, lorsque le champ [!UICONTROL Intégrations] est disponible. L’administrateur du système ou du groupe doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de mise en page pour afficher le lien Atteindre Salesforce dans l’en-tête du problème. Pour plus d’informations, consultez la section [Personnaliser les en-têtes d’objet à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >Le lien [!UICONTROL Aller à Salesforce] est visible par tous les utilisateurs de [!DNL Workfront] qui peuvent afficher le problème. Vous devez disposer d’un compte [!DNL Salesforce] pour pouvoir accéder à l’opportunité ou au compte [!DNL Salesforce] où le problème a été consigné.
