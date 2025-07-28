---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 'Soumettre des demandes  [!DNL Adobe Workfront]  à partir d’objets  [!DNL Salesforce] '
description: Après avoir installé  [!DNL Adobe Workfront]  pour les demandes  [!DNL Salesforce], you can submit [!DNL Workfront]  à partir d’opportunités et de comptes  [!DNL Salesforce] . Cette fonctionnalité est disponible dans les frameworks d’expérience Classic et Lightning.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 83%

---

# Soumettre des demandes [!DNL Adobe Workfront] à partir d’objets [!DNL Salesforce]

>[!IMPORTANT]
>
>Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, l’intégration de Workfront for Salesforce ne sera plus disponible après le **28 février 2026**.
>
>Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre entreprise avec Salesforce.
>
>Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Salesforce, consultez [Modules Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Après avoir installé [!DNL Adobe Workfront for Salesforce], vous pouvez soumettre des demandes [!DNL Workfront] à partir d’opportunités et de comptes [!DNL Salesforce]. Cette fonctionnalité est disponible dans les frameworks [!DNL Classic] et [!DNL Lightning Experience].

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des accès suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] formule*</p></td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] licence*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Pour envoyer une demande [!DNL Workfront] à partir d’une opportunité ou d’un compte [!DNL Salesforce], vérifiez que vous disposez des éléments suivants dans votre environnement :

* Votre équipe d’administration [!DNL Workfront] a installé [!DNL Workfront for Salesforce].\
   Pour plus d’informations sur l’installation de [!DNL Workfront for Salesforce], voir [Installer [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Votre équipe d’administration [!DNL Workfront] a ajouté la section [!DNL Workfront] à vos dispositions de page [!UICONTROL Opportunité] et [!UICONTROL Compte].\
   Pour plus d’informations sur l’ajout de la section [!DNL Workfront] à une disposition de page, voir [Configurer la section  [!DNL Adobe Workfront]  pour les utilisateurs et utilisatrices  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Vous avez un compte [!DNL Workfront] et vous pouvez vous y connecter à partir de la section [!DNL Workfront] dans votre opportunité ou votre compte.\
   Après la connexion, vous pouvez voir l’onglet [!UICONTROL Nouvelles demandes] dans lequel vous pouvez commencer à saisir des demandes.

## Soumettre des demandes [!DNL Workfront] à partir de [!DNL Salesforce]

1. Accédez à une opportunité ou à un compte dans Salesforce.
1. Accédez à la section [!DNL Workfront].
1. Dans l’onglet **[!UICONTROL Nouvelles demandes]**, sélectionnez un type de demande dans le menu déroulant **[!UICONTROL Sélectionner un type de demande]**.

   Vous pouvez voir les mêmes files d’attente de demandes que celles auxquelles vous avez accès dans Workfront.

1. Renseignez tout d’abord les champs disponibles de votre demande.

   Soumettre une demande à partir de [!DNL Salesforce] revient à soumettre une demande dans l’application web [!DNL Workfront].

   >[!NOTE]
   >
   >Le chargement d’un document à l’aide du plug-in [!DNL Workfront] dans [!DNL Salesforce] est temporairement indisponible.

   Continuez à suivre les étapes décrites dans [Créer et soumettre des demandes  [!DNL Adobe Workfront] ](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Cliquez sur **[!UICONTROL Soumettre]**.

## Afficher les demandes [!DNL Workfront]

1. Accédez à une opportunité ou à un compte dans [!DNL Salesforce].
1. Accédez à la section **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Selon la manière dont votre équipe d’administration [!DNL Workfront] a configuré cette section, elle peut porter un nom différent.

1. Sélectionnez l’onglet **[!UICONTROL Demandes envoyées]**.

   Vous pouvez afficher toutes les demandes que vous ou d’autres personnes avez envoyées depuis cette opportunité ou ce compte dans cet onglet. Les demandes envoyées vers cette file d’attente des demandes dans l’application web ne s’affichent pas dans cette liste dans [!DNL Salesforce].

   >[!NOTE]
   >
   >Les demandes envoyées vers cette file d’attente des demandes dans l’application web ne s’affichent pas dans cette liste dans Salesforce.

   ![salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Vous pouvez afficher les informations suivantes sur les demandes envoyées :

   * Nom de la requête (dans la colonne [!UICONTROL Objet])
   * Numéro de référence
   * Type de demande
   * Statut
   * Date d’envoi
   * Nom de la personne ayant effectué la demande
   * Nom de la personne à laquelle la demande est attribuée

     Lorsque vous mettez à jour ces informations dans [!DNL Workfront], elles sont également mises à jour dans cette liste.

1. (Facultatif) Cliquez sur le nom de la demande pour l’ouvrir dans [!DNL Workfront].

1. (Facultatif) Cliquez sur **[!UICONTROL Accéder à[!DNL Salesforce]]** pour accéder à l’opportunité ou au compte d’où provient le problème dans les zones suivantes de Workfront :

   * Dans la section [!UICONTROL Détails] du problème
   * Dans le panneau Résumé, lorsque vous sélectionnez l’événement dans une liste, après avoir cliqué sur [!UICONTROL Ouvrir le résumé] ![Icône du panneau Résumé](assets/summary-panel-icon.png) dans la barre d’outils de la liste.
   * Dans l’en-tête du problème, lorsque le champ [!UICONTROL Intégrations] est disponible. Votre administrateur ou administratrice système ou groupe doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de mise en page pour afficher le lien Accéder à Salesforce dans l’en-tête du problème. Pour plus d’informations, consultez [Personnaliser les en-têtes d’objet à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >Le lien [!UICONTROL Accéder à Salesforce] est visible pour tous les utilisateurs et utilisatrices [!DNL Workfront] qui peuvent afficher le problème. Vous devez disposer d’un compte [!DNL Salesforce] pour pouvoir accéder à l’opportunité ou au compte [!DNL Salesforce] où le problème a été consigné.
