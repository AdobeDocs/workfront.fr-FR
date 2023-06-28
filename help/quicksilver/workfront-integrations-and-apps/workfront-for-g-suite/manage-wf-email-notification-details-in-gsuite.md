---
product-area: workfront-integrations
keywords: google,doc,document,sheet,diapositive
navigation-topic: workfront-for-g-suite
title: Gérer [!DNL Adobe Workfront] détails des notifications de G Suite
description: Dans G Suite, lorsque vous ouvrez un Adobe de courrier électronique de notification [!DNL Workfront] a envoyé, vous pouvez afficher les détails de l’élément de travail associé et répondre sans quitter votre boîte de réception. Si des actions sont disponibles, telles que l’approbation d’une requête, vous pouvez effectuer ces actions directement à partir de Workfront for G Suite.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# Gérer [!DNL Adobe Workfront] détails de la notification depuis [!DNL G Suite]

>[!NOTE]
>
>La dernière version du module externe Adobe Workfront pour Google a été publiée le 26 juin 2023.

Dans [!DNL G Suite], lorsque vous ouvrez un email de notification [!DNL Adobe Workfront] a envoyé, vous pouvez afficher les détails de l’élément de travail associé et répondre sans quitter votre [!UICONTROL Boîte de réception]. Si des actions sont disponibles, telles que l’approbation d’une requête, vous pouvez effectuer ces actions directement à partir de [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] prend en charge presque tous les types de notifications électroniques que vous pouvez recevoir. [!DNL Workfront] (environ 120 types différents). [!UICONTROL Résumé quotidien] emails envoyés depuis [!DNL Workfront] n’apparaît pas dans [!DNL Workfront for G Suite]. Pour plus d’informations sur la variable [!DNL Workfront] types de notification par e-mail, voir [Activation ou désactivation de vos propres notifications d’événement](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Avant de gérer les détails des notifications depuis [!DNL G Suite], vous devez

* Installer [!DNL Workfront for G suite]\
   Pour obtenir des instructions, voir [Installer [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Gérer [!DNL Adobe Workfront] détails de la notification depuis [!DNL G Suite]

1. Si la variable [!DNL Workfront for G Suite] ne s’affiche pas, cliquez sur le bouton [!DNL Workfront] icon ![](assets/wf-lion-icon.png) dans le [!DNL G Suite] la barre latérale des modules complémentaires située à l’extrémité droite de la page.
1. Dans [!DNL G Suite], ouvrez un [!DNL Workfront] email de notification.
1. Cliquez sur **[!UICONTROL Afficher toutes les mises à jour]** s’il s’affiche près de la partie supérieure du panneau.
1. Cliquez sur **[!UICONTROL Détails]**.
1. Cliquez sur les options disponibles.

   Les options qui peuvent s’afficher correspondent au type de notification électronique que vous avez ouverte. Par exemple, s’il s’agit d’une notification électronique vous demandant de valider une tâche, vous voyez **[!UICONTROL Approuver]** et **[!UICONTROL Rejeter]** plutôt que des options telles que **[!UICONTROL Travail dessus]** ou **[!UICONTROL Terminé]**:

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
      <td><strong>[!UICONTROL Approuver]</strong> il, <strong>[!UICONTROL Rejeter]</strong> il, <strong>[!UICONTROL Grant]</strong> l'accès, <strong>[!UICONTROL Ignorer]</strong> une demande d'accès à celle-ci, <strong>[!UICONTROL Travailler dessus]</strong>ou cliquez sur une option pour indiquer que vous êtes <strong>[!UICONTROL Terminé]</strong> avec</td> 
     </tr> 
     <tr> 
      <td>Projet</td> 
      <td><strong>[!UICONTROL Approuver]</strong> il, <strong>[!UICONTROL Rejeter]</strong> il, <strong>[!UICONTROL Grant]</strong> l’accès à celle-ci, ou <strong>[!UICONTROL Ignorer]</strong> une demande d’accès à celle-ci</td> 
     </tr> 
     <tr> 
      <td>Document</td> 
      <td><strong>[!UICONTROL Approuver]</strong> il, <strong>[!UICONTROL Rejeter]</strong> il, <strong>[!UICONTROL Grant]</strong> l’accès à celle-ci, ou <strong>[!UICONTROL Ignorer]</strong> une demande d’accès à celle-ci</td> 
     </tr> 
     <tr> 
      <td>Mettre à jour </td> 
      <td> <p>Affichez toute partie de la liste complète des mises à jour de l’élément afin d’avoir le contexte dont vous avez besoin. <strong>[!UICONTROL Post]</strong> une nouvelle mise à jour ou une <strong>[!UICONTROL Réponse]</strong>. Vous pouvez cliquer sur <strong>[!UICONTROL Notifier]</strong> pour alerter des utilisateurs particuliers au sujet de votre réponse. </p> <p>Pour plus d’informations, voir <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Répondre à un [!DNL Adobe Workfront] mettre à jour la notification depuis [!DNL G Suite]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Demande d’approbation</td> 
      <td><strong>[!UICONTROL Approuver]</strong> ou <strong>[!UICONTROL Rejeter]</strong> (vous pouvez changer d’avis en cliquant sur l’autre option), télécharger le fichier, afficher son propriétaire ou afficher son numéro de référence.</td> 
     </tr> 
     <tr> 
      <td>Modification de l’état d’un projet</td> 
      <td> Affichez toutes les informations actuelles sur le projet, y compris les formulaires personnalisés. </td> 
     </tr> 
    </tbody> 
   </table>
