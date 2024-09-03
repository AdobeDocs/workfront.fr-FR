---
product-area: workfront-integrations
keywords: google,doc,document,feuille,diapositive
navigation-topic: workfront-for-g-suite
title: Gérer les  [!DNL Adobe Workfront] détails de notification depuis Google Workspace
description: Dans Google Workspace, lorsque vous ouvrez un Adobe de notification envoyé par courrier électronique,  [!DNL Workfront] vous pouvez afficher les détails de l’élément de travail associé et répondre sans quitter votre boîte de réception. Si des actions sont disponibles, telles que l’approbation d’une requête, vous pouvez effectuer ces actions directement à partir de Workfront pour Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 89%

---

# Gérer les détails des notifications [!DNL Adobe Workfront] à partir de [!DNL Google Workspace]

>[!NOTE]
>
>La dernière version en date du plug-in Adobe Workfront pour Google a été publiée le 26 juin 2023.

Dans [!DNL Google Workspace], lorsque vous ouvrez un e-mail de notification envoyé par [!DNL Adobe Workfront], vous pouvez consulter les détails de l’élément de travail associé et y répondre sans quitter votre [!UICONTROL Boîte de réception]. Si des actions sont disponibles, telles que l’approbation d’une requête, vous pouvez effectuer ces actions directement à partir de [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] prend en charge presque tous les types de notification par e-mail que vous pouvez recevoir de [!DNL Workfront] (environ 120 types différents). Les e-mails de [!UICONTROL synthèse quotidienne] envoyés à partir de [!DNL Workfront] n’apparaissent pas dans [!DNL Workfront for Google Workspace]. Pour plus d’informations sur les types de notification par e-mail [!DNL Workfront], consultez la section [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Avant de pouvoir gérer les détails des notifications à partir de [!DNL Google Workspace], vous devez

* installer [!DNL Workfront for Google Workspace].\
   Pour obtenir des instructions, consultez la section [Installer  [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Gérer les détails des notifications [!DNL Adobe Workfront] à partir de [!DNL Google Workspace]

1. Si le panneau [!DNL Workfront for Google Workspace] n’est pas affiché, cliquez sur l’icône [!DNL Workfront] ![](assets/wf-lion-icon.png) dans la barre latérale des modules complémentaires [!DNL Google Workspace] tout à droite de la page.
1. Dans [!DNL Google Workspace], ouvrez un e-mail de notification [!DNL Workfront].
1. Cliquez sur **[!UICONTROL Afficher toutes les mises à jour]** si cette option est affichée en haut du panneau.
1. Cliquez sur **[!UICONTROL Détails]**.
1. Cliquez sur les options disponibles.

   Les options qui peuvent s’afficher correspondent au type de la notification par e-mail que vous avez ouverte. Par exemple, s’il s’agit d’une notification par e-mail vous demandant d’approuver une tâche, vous voyez les options **[!UICONTROL Approuver]** et **[!UICONTROL Rejeter]** au lieu de **[!UICONTROL Travailler sur ce projet]** ou **[!UICONTROL Terminé]** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type de notification par e-mail</th> 
      <th>Action</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Tâche ou problème</td> 
      <td>Vous pouvez effectuer les opérations suivantes : <strong>[!UICONTROL Approve]</strong>, <strong>[!UICONTROL Reject]</strong>, <strong>[!UICONTROL Grant]</strong> l’accès, <strong>[!UICONTROL Ignore]</strong> la demande d’accès, <strong>[!UICONTROL Work on it]</strong> ou cliquer sur une option pour indiquer que vous avez <strong>[!UICONTROL Done]</strong>.</td> 
     </tr> 
     <tr> 
      <td>Projet</td> 
      <td>Vous pouvez effectuer les opérations suivantes : <strong>[!UICONTROL Approve]</strong>, <strong>[!UICONTROL Reject]</strong>, <strong>[!UICONTROL Grant]</strong> l’accès, ou <strong>[!UICONTROL Ignore]</strong> la demande d’accès.</td> 
     </tr> 
     <tr> 
      <td>Document</td> 
      <td>Vous pouvez effectuer les opérations suivantes : <strong>[!UICONTROL Approve]</strong>, <strong>[!UICONTROL Reject]</strong>, <strong>[!UICONTROL Grant]</strong> l’accès, ou <strong>[!UICONTROL Ignore]</strong> la demande d’accès.</td> 
     </tr> 
     <tr> 
      <td>Mettre à jour </td> 
      <td> <p>Affichez n’importe quelle partie de la liste complète des mises à jour de l’élément afin de disposer du contexte nécessaire pour <strong>[!UICONTROL Post]</strong> une nouvelle mise à jour ou une <strong>[!UICONTROL Reply]</strong>. Cliquez sur <strong>[!UICONTROL Notify]</strong> pour alerter des utilisateurs et des utilisatrices spécifiques de votre réponse. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Répondre à une notification de mise à jour [!DNL Adobe Workfront] de [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Demande d’approbation</td> 
      <td>Vous pouvez effectuer les opérations suivantes : <strong>[!UICONTROL Approve]</strong> ou <strong>[!UICONTROL Reject]</strong> (vous pouvez changer d’avis en cliquant sur l’autre option), télécharger, voir qui en est la personne propriétaire ou afficher son numéro de référence.</td> 
     </tr> 
     <tr> 
      <td>Modification du statut d’un projet</td> 
      <td> Affichez toutes les informations actuelles sur le projet, y compris les formulaires personnalisés. </td> 
     </tr> 
    </tbody> 
   </table>
