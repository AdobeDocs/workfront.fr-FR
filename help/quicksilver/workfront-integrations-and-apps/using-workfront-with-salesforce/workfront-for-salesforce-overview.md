---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Vue d’ensemble d’Adobe Workfront pour Salesforce
description: Vous pouvez installer  [!DNL Adobe Workfront]  pour Salesforce afin de permettre aux personnes utilisant Salesforce de soumettre des requêtes  [!DNL Workfront]  et de créer automatiquement des projets sans jamais quitter Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 94%

---

# Vue d’ensemble d’[!DNL Adobe Workfront for Salesforce]

Une formule [!UICONTROL Pro] [!DNL Workfront] est nécessaire pour utiliser cette fonction. Pour plus d’informations sur les différentes formules disponibles, consultez la section [[!DNL Workfront] Formules.](https://www.workfront.com/plans?lang=fr)

Vous pouvez installer [!DNL Adobe Workfront for Salesforce] pour permettre aux personnes utilisant [!DNL Salesforce] de soumettre des requêtes [!DNL Workfront] et de créer automatiquement des projets sans jamais quitter [!DNL Salesforce].

En tant que personne membre de l’administration [!DNL Workfront], vous pouvez télécharger et configurer [!DNL Workfront for Salesforce]. Vous pouvez ensuite le partager avec l’ensemble des utilisateurs et des utilisatrices de [!DNL Salesforce].

Pour plus d’informations sur l’installation de [!DNL Workfront for Salesforce], consultez la section [Installer [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Pour plus d’informations sur la configuration de la section [!DNL Workfront] dans [!DNL Salesforce] pour l’ensemble des utilisateurs et des utilisatrices, consultez la section [Configurer  [!DNL Adobe Workfront]  pour les utilisateurs et les utilisatrices de  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des accès suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez l’administration [!DNL Workfront].

## [!DNL Workfront for Salesforce]

Vous pouvez effectuer les opérations suivantes en utilisant [!DNL Workfront for Salesforce] :

* Créez manuellement de nouvelles requêtes [!DNL Workfront] à partir de [!DNL Salesforce] au sein d’une opportunité ou d’un compte.

  Pour plus d’informations sur la création de requêtes [!DNL Workfront] à partir de [!DNL Salesforce], consultez la section [Soumettre des requêtes  [!DNL Adobe Workfront]  à partir d’objets  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Déclenchez automatiquement la création de projets dans [!DNL Workfront] lorsque certains critères sont remplis dans [!DNL Salesforce]. Votre équipe d’administration système [!DNL Salesforce] doit configurer les déclencheurs pour la création de projets à partir de [!DNL Salesforce].

  Pour plus d’informations sur la création de projets [!DNL Workfront] à partir de [!DNL Salesforce], consultez la section [Créer des projets  [!DNL Adobe Workfront]  à partir d’objets  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tenez compte des points suivants lorsque vous utilisez [!DNL Workfront] pour [!DNL Salesforce] :

* Nous prenons en charge les frameworks [!DNL Salesforce Classic] et [!DNL Lightning Experience].
* Les éléments ne peuvent être créés que de [!DNL Salesforce] vers [!DNL Workfront].
* Vous pouvez consulter des informations sur les éléments [!DNL Workfront] dans [!DNL Salesforce].

  Ces informations ne peuvent pas être personnalisées.

  Pour une liste des champs [!DNL Workfront] que vous pouvez afficher dans [!DNL Salesforce], consultez [Soumettre des requêtes  [!DNL Adobe Workfront]  à partir des objets  [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md) et [Créer des projets  [!DNL Adobe Workfront]  à partir d’objets [!DNL Salesforce] ](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Vous pouvez accéder directement aux éléments liés à [!DNL Salesforce] en cliquant sur le lien **[!UICONTROL Aller à Salesforce]** depuis Workfront.

  Vous ne pouvez pas afficher d’informations sur les éléments [!DNL Salesforce] dans [!DNL Workfront], mais vous disposez d’un lien vers l’élément [!UICONTROL Salesforce] à partir de [!DNL Workfront] pour les consulter dans [!DNL Salesforce].

  [!UICONTROL Le lien **Aller à Salesforce**] s’affiche dans les zones suivantes :

   * Section [!UICONTROL Détails] d’un projet ou d’un problème
   * En-tête d’un projet ou d’un problème.

     Votre équipe d’administration système ou de groupes doit ajouter le champ [!UICONTROL Intégrations] à votre modèle de mise en page pour afficher le lien [!UICONTROL Aller à Salesforce] dans l’en-tête du projet ou du problème.
   * Panneau [!DNL Summary] d’un événement lors de la sélection de l’événement dans une liste, après avoir cliqué sur l’icône [!UICONTROL Ouvrir le résumé] ![Icône du panneau Résumé](assets/summary-panel-icon.png) dans la barre d’outils de la liste.

     >[!NOTE]
     >
     >Le lien [!UICONTROL Aller à Salesforce] est visible par tous les utilisateurs et toutes les utilisatrices [!DNL Workfront] qui peuvent afficher le projet ou le problème. Vous devez avoir un compte [!DNL Salesforce] pour pouvoir accéder à l’opportunité ou au compte [!DNL Salesforce] où le problème a été enregistré.

* La mise à jour des champs d’un élément dans une application ne met pas à jour les informations sur les éléments liés dans l’autre application.
