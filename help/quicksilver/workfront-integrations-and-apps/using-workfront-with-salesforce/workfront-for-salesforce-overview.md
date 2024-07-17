---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Vue d’ensemble d’Adobe Workfront pour Salesforce
description: Vous pouvez installer  [!DNL Adobe Workfront] pour Salesforce pour permettre à vos utilisateurs Salesforce d’envoyer des requêtes  [!DNL Workfront]  et de créer automatiquement des projets sans quitter Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 7%

---

# Vue d’ensemble d’[!DNL Adobe Workfront for Salesforce]

Un abonnement [!UICONTROL Pro] [!DNL Workfront] est requis pour utiliser cette fonctionnalité. Pour plus d’informations sur les différents plans disponibles, voir [[!DNL Workfront] Plans.](https://www.workfront.com/plans?lang=fr)

Vous pouvez installer [!DNL Adobe Workfront for Salesforce] pour permettre à vos utilisateurs [!DNL Salesforce] d&#39;envoyer des requêtes [!DNL Workfront] et de créer automatiquement des projets sans jamais quitter [!DNL Salesforce].

En tant qu&#39;administrateur [!DNL Workfront], vous pouvez télécharger et configurer [!DNL Workfront for Salesforce]. Ensuite, vous pouvez le partager avec tous les autres utilisateurs [!DNL Salesforce].

Pour plus d&#39;informations sur l&#39;installation de [!DNL Workfront for Salesforce], voir [Installation [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Pour plus d’informations sur la configuration de la section [!DNL Workfront] dans [!DNL Salesforce] pour tous les utilisateurs, voir [Configuration de la section  [!DNL Adobe Workfront] pour les  [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## [!DNL Workfront for Salesforce]

Vous pouvez effectuer les opérations suivantes lors de l’utilisation de [!DNL Workfront for Salesforce] :

* Créez manuellement de nouvelles requêtes [!DNL Workfront] à partir de [!DNL Salesforce] dans une opportunité ou un compte.

  Pour plus d’informations sur la création de [!DNL Workfront] requêtes à partir de [!DNL Salesforce], voir [Soumettre [!DNL Adobe Workfront] demandes à partir de [!DNL Salesforce] objets](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* déclencher automatiquement la création de projets dans [!DNL Workfront] lorsque certains critères sont satisfaits dans [!DNL Salesforce]. Votre administrateur système [!DNL Salesforce] doit configurer des déclencheurs pour créer des projets à partir de [!DNL Salesforce].

  Pour plus d’informations sur la création de [!DNL Workfront] projets à partir de [!DNL Salesforce], voir [Créer [!DNL Adobe Workfront] projets à partir de [!DNL Salesforce] objets](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tenez compte des points suivants lorsque vous utilisez [!DNL Workfront] pour [!DNL Salesforce] :

* Nous prenons en charge les structures [!DNL Salesforce Classic] et [!DNL Lightning Experience].
* Les éléments ne peuvent être créés que de [!DNL Salesforce] à [!DNL Workfront].
* Vous pouvez afficher des informations sur les éléments [!DNL Workfront] dans [!DNL Salesforce].

  Ces informations ne peuvent pas être personnalisées.

  Pour obtenir la liste des champs [!DNL Workfront] que vous pouvez afficher à partir de [!DNL Salesforce], voir [Soumettre [!DNL Adobe Workfront] les demandes à partir de [!DNL Salesforce] objets](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) et [Créer [!DNL Adobe Workfront] des projets à partir de [!DNL Salesforce] objets](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Vous pouvez accéder directement aux éléments liés à [!DNL Salesforce] en cliquant sur le lien **[!UICONTROL Aller à Salesforce]** à partir de Workfront.

  Vous ne pouvez pas afficher d’informations sur les éléments [!DNL Salesforce] dans [!DNL Workfront], mais vous disposez d’un lien vers l’élément [!UICONTROL Salesforce] de [!DNL Workfront] pour le consulter dans [!DNL Salesforce].

  [!UICONTROL Le lien **Aller à Salesforce**] s’affiche dans les zones suivantes :

   * La section [!UICONTROL Détails] d’un projet ou d’un problème
   * En-tête d’un projet ou d’un problème.

     L’administrateur du système ou du groupe doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de mise en page pour afficher le lien [!UICONTROL Aller à Salesforce] dans l’en-tête du projet ou du problème.
   * Panneau [!DNL Summary] d’un problème lors de la sélection du problème dans une liste, après avoir cliqué sur [!UICONTROL Ouvrir le résumé] ![](assets/summary-panel-icon.png) dans la barre d’outils de la liste.

     >[!NOTE]
     >
     >Le lien [!UICONTROL Aller à Salesforce] est visible par tous les utilisateurs de [!DNL Workfront] qui peuvent afficher le projet ou le problème. Vous devez disposer d’un compte [!DNL Salesforce] pour pouvoir accéder à l’opportunité ou au compte [!DNL Salesforce] où le problème a été consigné.

* La mise à jour des champs d’un élément dans une application ne met à jour aucune information sur les éléments liés dans l’autre application.
