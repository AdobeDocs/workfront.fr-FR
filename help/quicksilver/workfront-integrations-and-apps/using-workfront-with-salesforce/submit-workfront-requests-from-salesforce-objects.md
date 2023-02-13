---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Envoyer [!DNL Adobe Workfront] de [!DNL Salesforce] objet
description: Après installation [!DNL Adobe Workfront] pour [!DNL Salesforce], you can submit [!DNL Workfront] de [!DNL Salesforce] Opportunités et comptes. Cette fonctionnalité existe dans les frameworks d’expérience classique et d’éclair.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# Envoyer [!DNL Adobe Workfront] de [!DNL Salesforce] objet

Après installation [!DNL Adobe Workfront for Salesforce], vous pouvez envoyer des [!DNL Workfront] de [!DNL Salesforce] Opportunités et comptes. Cette fonctionnalité existe dans les deux [!DNL Classic] et [!DNL Lightning Experience] frameworks.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan*</p></td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] license*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Pour envoyer une [!DNL Workfront] d’une [!DNL Salesforce] Une opportunité ou un compte vérifiez que vous disposez des éléments suivants dans votre environnement :

* Votre [!DNL Workfront] L’administrateur a installé [!DNL Workfront for Salesforce].\
   Pour plus d’informations sur l’installation [!DNL Workfront for Salesforce], voir [Installer [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Votre [!DNL Workfront] L’administrateur a ajouté la variable [!DNL Workfront] à votre [!UICONTROL Opportunité] et [!UICONTROL Compte] mises en page.\
   Pour plus d’informations sur l’ajout de la variable [!DNL Workfront] à une mise en page, voir [Configurez la variable [!DNL Adobe Workfront] section pour [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Vous avez une [!DNL Workfront] et vous pouvez vous y connecter à partir du [!DNL Workfront] dans votre opportunité ou votre compte.\
   Une fois connecté, vous pouvez voir le [!UICONTROL Nouvelles requêtes] où vous pouvez commencer à saisir des requêtes.

## Envoyer [!DNL Workfront] de [!DNL Salesforce]

1. Accédez à une opportunité ou à un compte dans Salesforce.
1. Accédez au [!DNL Workfront] .
1. Dans le **[!UICONTROL Nouvelles requêtes]** , sélectionnez un type de requête dans la **[!UICONTROL Sélection d’un type de requête]** menu déroulant.

   Vous pouvez voir les mêmes files d’attente de requête que celles que vous avez accès à voir dans Workfront.

1. Commencez à remplir les champs disponibles pour votre requête.

   Envoi d’une demande depuis [!DNL Salesforce] est identique à l’envoi d’une requête dans la variable [!DNL Workfront] application web.

   >[!NOTE]
   >
   >Téléchargement d’un document à l’aide du [!DNL Workfront] plug-in [!DNL Salesforce] est temporairement indisponible.

   Suivez les étapes décrites dans la section [Créer et envoyer [!DNL Adobe Workfront] requests](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Cliquez sur **[!UICONTROL Envoyer]**.

## Affichage [!DNL Workfront] requests

1. Accédez à une opportunité ou à un compte dans [!DNL Salesforce].
1. Accédez au **[!DNL Workfront]** .

   >[!NOTE]
   >
   >Selon la manière dont votre [!DNL Workfront] l’administrateur a configuré cette section. elle peut porter un nom différent.

1. Sélectionnez la **[!UICONTROL Demandes envoyées]** .

   Vous pouvez afficher toutes les requêtes que vous ou d’autres avez envoyées depuis cette opportunité ou ce compte dans cet onglet. Les requêtes envoyées vers cette file d’attente de demandes dans l’application web ne s’affichent pas dans cette liste dans [!DNL Salesforce].

   >[!NOTE]
   >
   >Les requêtes envoyées à cette file d’attente de requêtes dans l’application web ne s’affichent pas dans cette liste dans Salesforce.

   ![salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Vous pouvez afficher les informations suivantes sur les demandes envoyées :

   * Nom de la requête (dans la variable [!UICONTROL Objet] column)
   * Numéro de référence
   * Type de demande
   * Statut
   * Envoyé à la date
   * Demandé par nom
   * Attribué à Nom\

      Lorsque ces informations sont mises à jour dans [!DNL Workfront], il est également mis à jour dans cette liste.

1. (Facultatif) Cliquez sur le nom de la requête pour l’ouvrir dans [!DNL Workfront].

1. (Facultatif) Cliquez sur **[!UICONTROL Accédez à[!DNL Salesforce]]** pour accéder à l’ opportunité ou au compte où le problème provient des zones suivantes de Workfront :

   * Dans le [!UICONTROL Détails] section du problème
   * Dans le panneau Résumé lors de la sélection du problème dans une liste, après avoir cliqué sur [!UICONTROL Résumé ouvert] ![](assets/summary-panel-icon.png) dans la barre d’outils de la liste.
   * Dans l’en-tête du problème, lorsque la variable [!UICONTROL Intégrations] est disponible. Votre administrateur système ou groupe doit ajouter la variable [!UICONTROL Intégrations] à votre modèle de mise en page pour afficher le lien Atteindre Salesforce dans l’en-tête du problème. Pour plus d’informations, voir [Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >Le [!UICONTROL Accéder à Salesforce] Le lien est visible pour tous [!DNL Workfront] utilisateurs qui peuvent afficher le problème. Vous devez disposer d’un [!DNL Salesforce] pour pouvoir accéder à la variable [!DNL Salesforce] Opportunité ou compte où le problème a été consigné.
