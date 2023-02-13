---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Présentation d’Adobe Workfront for Salesforce
description: Vous pouvez installer [!DNL Adobe Workfront] pour Salesforce afin d’autoriser vos utilisateurs Salesforce à envoyer des [!DNL Workfront] demande et crée automatiquement des projets sans quitter Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] aperçu

A [!UICONTROL Pro] [!DNL Workfront] Planifiez l’utilisation de cette fonctionnalité. Pour plus d’informations sur les différents plans disponibles, voir [[!DNL Workfront] Formules.](https://www.workfront.com/plans)

Vous pouvez installer [!DNL Adobe Workfront for Salesforce] pour autoriser votre [!DNL Salesforce] utilisateurs à envoyer [!DNL Workfront] requêtes et créer automatiquement des projets sans jamais quitter [!DNL Salesforce].

Comme [!DNL Workfront] administrateur, vous pouvez télécharger et configurer [!DNL Workfront for Salesforce]. Ensuite, vous pouvez le partager et tous les autres [!DNL Salesforce] utilisateurs.

Pour plus d’informations sur l’installation [!DNL Workfront for Salesforce], voir [Installer [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
Pour plus d’informations sur la configuration de la variable [!DNL Workfront] dans [!DNL Salesforce] pour tous les utilisateurs, voir [Configurez la variable [!DNL Adobe Workfront] section pour [!DNL Salesforce] utilisateurs](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## [!DNL Workfront for Salesforce]

Vous pouvez effectuer les opérations suivantes lors de l’utilisation de [!DNL Workfront for Salesforce]:

* Créer manuellement [!DNL Workfront] de [!DNL Salesforce] dans une opportunité ou un compte.

   Pour plus d’informations sur la création [!DNL Workfront] de [!DNL Salesforce], voir [Envoyer [!DNL Adobe Workfront] de [!DNL Salesforce] objet](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* Déclenchement automatique de la création de projets dans [!DNL Workfront] lorsque certains critères sont satisfaits dans [!DNL Salesforce]. Votre [!DNL Salesforce] l’administrateur système doit configurer des déclencheurs pour créer des projets à partir de [!DNL Salesforce].

   Pour plus d’informations sur la création [!DNL Workfront] projets à partir de [!DNL Salesforce], voir [Créer [!DNL Adobe Workfront] projets à partir de [!DNL Salesforce] objet](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

Tenez compte des points suivants lorsque vous utilisez [!DNL Workfront] pour [!DNL Salesforce]:

* Nous soutenons les deux [!DNL Salesforce Classic] et [!DNL Lightning Experience] frameworks.
* Les éléments ne peuvent être créés qu’à partir de [!DNL Salesforce] en [!DNL Workfront].
* Vous pouvez afficher quelques informations sur la variable [!DNL Workfront] éléments dans [!DNL Salesforce].

   Ces informations ne peuvent pas être personnalisées.

   Pour une liste de [!DNL Workfront] champs que vous pouvez afficher à partir de [!DNL Salesforce], voir  [Envoyer [!DNL Adobe Workfront] de [!DNL Salesforce] objet](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  et [Créer [!DNL Adobe Workfront] projets à partir de [!DNL Salesforce] objet](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* Vous pouvez accéder directement aux éléments liés à [!DNL Salesforce] en cliquant sur le bouton **[!UICONTROL Accéder à Salesforce]** à partir de Workfront.

   Vous ne pouvez pas afficher d’informations sur la variable [!DNL Salesforce] éléments dans [!DNL Workfront], mais vous disposez d’un lien vers le [!UICONTROL Salesforce] item from [!DNL Workfront] pour la consulter dans [!DNL Salesforce].

   [!UICONTROL Le **Accéder à Salesforce**] s’affiche dans les zones suivantes :

   * Le [!UICONTROL Détails] section d’un projet ou d’un problème
   * En-tête d’un projet ou d’un problème.

      Votre administrateur système ou groupe doit ajouter la variable [!UICONTROL Intégrations] à votre modèle de mise en page pour afficher la variable [!UICONTROL Accéder à Salesforce] lien dans l’en-tête du projet ou du problème.
   * Le [!DNL Summary] d’un problème lors de la sélection du problème dans une liste, après avoir cliqué sur [!UICONTROL Résumé ouvert] ![](assets/summary-panel-icon.png) dans la barre d’outils de la liste.

      >[!NOTE]
      >
      >Le [!UICONTROL Accéder à Salesforce] Le lien est visible pour tous [!DNL Workfront] utilisateurs qui peuvent afficher le projet ou le problème. Vous devez disposer d’un [!DNL Salesforce] pour pouvoir accéder à la variable [!DNL Salesforce] Opportunité ou compte où le problème a été consigné.

* La mise à jour des champs d’un élément dans une application ne met à jour aucune information sur les éléments liés dans l’autre application.
