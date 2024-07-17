---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Approuver une feuille de temps
description: Le processus d’approbation des feuilles de temps permet aux gestionnaires de connaître les heures de travail de leurs rapports directs. Les approbateurs peuvent vérifier que tout le temps enregistré a été alloué dans les zones appropriées et qu’un nombre suffisant d’heures a été enregistré pour la période.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 11%

---

# Approuver une feuille de temps

Le processus d’approbation des feuilles de temps permet aux gestionnaires de connaître les heures de travail de leurs rapports directs. Les approbateurs peuvent vérifier que tout le temps enregistré a été alloué dans les zones appropriées et qu’un nombre suffisant d’heures a été enregistré pour la période.

Adobe Workfront permet de configurer les approbations de la feuille de temps pour la prise en charge dans cette zone.

Pour plus d&#39;informations sur l&#39;envoi d&#39;une feuille de temps, voir [Envoi d&#39;une feuille de temps pour approbation](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Désignation des approbateurs de feuille de temps

En règle générale, les feuilles de temps sont approuvées par les gestionnaires fonctionnels ou par le personnel des ressources humaines. (Les feuilles de temps ne sont pas normalement approuvées par les chefs de projet.)

Un approbateur de feuille de temps est défini lors de la création du profil de feuille de temps. Vous devez disposer d’une licence Plan pour être désigné comme approbateur.

Pour plus d’informations sur la désignation des approbateurs de feuille de temps, reportez-vous à la section [Création ou modification d’un profil de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) dans l’article [Création, modification et affectation de profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Approuver une feuille de temps

Vous pouvez approuver toute feuille de temps qui a été envoyée lorsque vous avez été désigné comme approbateur. Lorsqu’une feuille de temps est soumise à approbation, elle est répertoriée dans la zone **Approbations** de votre ****  page. Pour plus d’informations, voir [Valider le travail](../../review-and-approve-work/manage-approvals/approving-work.md).

Si l’administrateur Workfront a activé les gestionnaires d’événements Approbation de la feuille de temps pour l’utilisateur et Rejet de la feuille de temps vers l’utilisateur, vous en êtes informé une fois la feuille de temps approuvée ou rejetée. Pour plus d’informations sur l’activation des notifications d’événement, voir [Types de notification d’événement](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Pour valider une feuille de temps :

1. Cliquez sur l’icône **Menu Principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur **Feuilles de temps**.
1. Sélectionnez l’option **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez.

   Ou

   Sélectionnez le filtre **Mes approbations de feuille de temps** en haut de la liste de la feuille de temps.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >L’option Mes approbations de feuille de temps ne s’affiche pas en haut de la liste des feuilles de temps ni dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé le filtre Mes approbations de feuille de temps des commandes de liste de la zone Configuration ou de votre modèle de mise en page. Pour plus d’informations, voir les articles suivants :
   >
   >   
   >   
   >   * [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facultatif) Cliquez sur l’icône **search** ![](assets/search-icon.png) en haut de la liste des feuilles de temps et saisissez un mot-clé pour localiser une feuille de temps spécifique. Vous pouvez rechercher une période, ou le nom d’un propriétaire ou d’un approbateur.
1. Cliquez sur la période de la feuille de temps que vous souhaitez approuver. La feuille de temps s’ouvre.

   >[!TIP]
   >
   >Les feuilles de temps en attente d’approbation ont le statut [!UICONTROL Envoyé].


1. Cliquez sur **Approve**

   Ou

   Si vous souhaitez rejeter la feuille de temps, cliquez sur **Rejeter** dans le coin inférieur gauche de la feuille de temps.

   S’il est approuvé, l’état de la feuille de temps passe à **Fermé**.

   Si elle est rejetée, l’état de la feuille de temps passe à **Rejected**.
