---
product-area: workfront-integrations
keywords: google,doc,document,sheet,diapositive
navigation-topic: workfront-for-g-suite
title: Gérer les  [!DNL Adobe Workfront] détails de notification depuis Google Workspace
description: Dans Google Workspace, lorsque vous ouvrez un Adobe de notification envoyé par courrier électronique,  [!DNL Workfront] vous pouvez afficher les détails de l’élément de travail associé et répondre sans quitter votre boîte de réception. Si des actions sont disponibles, telles que l’approbation d’une requête, vous pouvez effectuer ces actions directement à partir de Workfront pour Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 7%

---

# Gérer les détails des notifications [!DNL Adobe Workfront] à partir de [!DNL Google Workspace]

>[!NOTE]
>
>La dernière version du module externe Adobe Workfront pour Google a été publiée le 26 juin 2023.

Dans [!DNL Google Workspace], lorsque vous ouvrez un email de notification [!DNL Adobe Workfront] envoyé, vous pouvez afficher les détails de l’élément de travail associé et répondre sans quitter votre [!UICONTROL boîte de réception]. Si des actions sont disponibles, telles que l’approbation d’une requête, vous pouvez effectuer ces actions directement à partir de [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] prend en charge presque tous les types de notifications électroniques que vous pouvez recevoir de [!DNL Workfront] (environ 120 types différents). Les [!UICONTROL  courriers électroniques de résumé quotidien ] envoyés depuis [!DNL Workfront] n’apparaissent pas dans [!DNL Workfront for Google Workspace]. Pour plus d’informations sur les types de notifications par e-mail [!DNL Workfront], voir [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Avant de pouvoir gérer les détails des notifications depuis [!DNL Google Workspace], vous devez :

* Installer [!DNL Workfront for Google Workspace]\
   Pour obtenir des instructions, voir [Installation [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Gérer les détails des notifications [!DNL Adobe Workfront] à partir de [!DNL Google Workspace]

1. Si le panneau [!DNL Workfront for Google Workspace] n’est pas affiché, cliquez sur l’icône [!DNL Workfront] ![](assets/wf-lion-icon.png) dans la barre latérale des modules complémentaires [!DNL Google Workspace] située à l’extrémité droite de la page.
1. Dans [!DNL Google Workspace], ouvrez un email de notification [!DNL Workfront].
1. Cliquez sur **[!UICONTROL Afficher toutes les mises à jour]** si elles s’affichent près de la partie supérieure du panneau.
1. Cliquez sur **[!UICONTROL Details]**.
1. Cliquez sur les options disponibles.

   Les options qui peuvent s’afficher correspondent au type de notification électronique que vous avez ouverte. Par exemple, s’il s’agit d’une notification par e-mail vous demandant d’approuver une tâche, vous voyez **[!UICONTROL Approve]** et **[!UICONTROL Reject]** au lieu d’options telles que **[!UICONTROL Work on It]** ou **[!UICONTROL Done]** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type de notification électronique</th> 
      <th>Action</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Tâche ou problème</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> accès à cet accès, <strong>[!UICONTROL Ignorer]</strong> demande d’accès, <strong>[!UICONTROL Travailler dessus]</strong> ou cliquez sur une option pour indiquer que vous <strong>[!UICONTROL Terminé]</strong> avec</td> 
     </tr> 
     <tr> 
      <td>Projet</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> accès à ce dernier ou <strong>[!UICONTROL Ignorer]</strong> demande d’accès à ce dernier</td> 
     </tr> 
     <tr> 
      <td>Document</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> accès à ce dernier ou <strong>[!UICONTROL Ignorer]</strong> demande d’accès à ce dernier</td> 
     </tr> 
     <tr> 
      <td>Mettre à jour </td> 
      <td> <p>Affichez toute partie de la liste complète des mises à jour de l’article afin de disposer du contexte dont vous avez besoin pour <strong>[!UICONTROL Post]</strong> une nouvelle mise à jour ou une <strong>[!UICONTROL Répondre]</strong>. Vous pouvez cliquer sur <strong>[!UICONTROL Notifier]</strong> pour alerter certains utilisateurs de votre réponse. </p> <p>Pour plus d'informations, voir <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Réponse à une notification de mise à jour [!DNL Adobe Workfront] de [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Demande d’approbation</td> 
      <td><strong>[!UICONTROL Approuver]</strong> ou <strong>[!UICONTROL Rejeter]</strong> (vous pouvez changer d’avis en cliquant sur l’autre option), télécharger le fichier, afficher son propriétaire ou consulter son numéro de référence.</td> 
     </tr> 
     <tr> 
      <td>Modification de l’état d’un projet</td> 
      <td> Affichez toutes les informations actuelles sur le projet, y compris les formulaires personnalisés. </td> 
     </tr> 
    </tbody> 
   </table>
