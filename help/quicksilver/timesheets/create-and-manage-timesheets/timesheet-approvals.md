---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Approuver une feuille de temps
description: Le processus d’approbation des feuilles de temps permet aux personnes responsables d’avoir une visibilité sur les heures de travail des personnes travaillant sous leur supervision directe. Les personnes approbatrices peuvent vérifier que toutes les heures consignées ont été affectées aux domaines corrects et qu’un nombre suffisant d’heures a été consigné pour la période.
author: Lisa
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 53%

---

# Approuver une feuille de temps

<!--Audited: 8/2024-->

Le processus d’approbation des feuilles de temps permet aux personnes responsables d’avoir une visibilité sur les heures de travail des personnes travaillant sous leur supervision directe. Les personnes approbatrices peuvent vérifier que toutes les heures consignées ont été affectées aux domaines corrects et qu’un nombre suffisant d’heures a été consigné pour la période.

Adobe Workfront offre la possibilité de configurer les approbations des feuilles de temps pour aider dans ce domaine.

Pour plus d’informations sur la soumission d’une feuille de temps, voir [Soumettre une feuille de temps pour approbation](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td><p>Accès administratif aux feuilles de temps et aux heures</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Désigner les personnes approbatrices des feuilles de temps

En règle générale, les feuilles de temps sont approuvées par les personnes responsables fonctionnelles ou le personnel des ressources humaines. Les feuilles de temps ne sont généralement pas approuvées par les chefs de projet. Les chefs de projet peuvent approuver les heures consignées pour les projets, mais les chefs d&#39;équipe ou de ressources humaines doivent approuver les feuilles de temps.

Un approbateur de feuille de temps est défini lors de la création du profil de feuille de temps. Vous devez disposer d&#39;une licence de plan pour être désigné comme approbateur.

Pour plus d’informations sur la désignation des personnes approbatrices des feuilles de temps, voir la section [Créer ou modifier un profil de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) dans l’article [Créer, modifier et attribuer des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Approuver une feuille de temps

Vous pouvez approuver toutes les feuilles de temps qui ont été soumises et pour lesquelles vous êtes une personne approbatrice. Lorsqu’une feuille de temps est soumise à approbation, elle est répertoriée dans le widget **Mes approbations** de votre zone **Accueil**. Pour plus d’informations, voir [Approuver un travail](../../review-and-approve-work/manage-approvals/approving-work.md).

Si les paramètres de notification suivants sont en place, l’utilisateur qui soumet la feuille de temps pour approbation reçoit un e-mail une fois qu’une feuille de temps est approuvée :

* L&#39;administrateur Workfront a activé les gestionnaires d&#39;événements Approbation de feuille de temps pour l&#39;utilisateur et Rejet de feuille de temps pour l&#39;utilisateur. Pour plus d’informations sur l’activation des notifications d’événements, voir [Types de notifications d’événements](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
* La notification personnelle Ma feuille de temps est approuvée est activée sur la page de profil de l’utilisateur. Pour plus d’informations, consultez la section [Modifier vos propres notifications par e-mail](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Approuver une feuille de temps à partir de la zone Feuilles de temps

{{step1-to-timesheets}}

La zone **Feuilles de temps** s’ouvre.

1. (Conditionnel) Si la dernière fois que vous avez accédé à s’ouvre, cliquez sur **Retour aux feuilles de temps** dans le coin supérieur gauche de l’écran.

1. Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous avez approuvées.

   Ou

   Sélectionnez le filtre **Mes approbations de feuille de temps** en haut de la liste des feuilles de temps.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >L&#39;option Mes approbations de feuilles de temps ne s&#39;affiche pas en haut de la liste des feuilles de temps ou dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé le filtre Mes approbations de feuilles de temps des contrôles de liste de la zone Configuration ou de votre modèle de mise en page.
   >
   >Pour plus d&#39;informations, voir [Personnaliser des filtres, des vues et des regroupements à l&#39;aide d&#39;un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facultatif) Cliquez sur l’icône **Rechercher** ![](assets/search-icon.png) en haut de la liste des feuilles de temps et tapez un mot-clé pour localiser une feuille de temps spécifique. Vous pouvez rechercher une période, le nom d’une personne propriétaire ou d’une personne approbatrice.
1. Cliquez sur la période de la feuille de temps que vous souhaitez approuver. La feuille de temps s’ouvre.

   >[!TIP]
   >
   >Les feuilles de temps en attente d’approbation ont le statut suivant : [!UICONTROL Soumis].


1. Cliquez sur **Approuver**.

   Ou

   Si vous souhaitez rejeter la feuille de temps, cliquez sur **Rejeter** dans le coin inférieur gauche de la feuille de temps.

   En cas d’approbation, le statut de la feuille de temps devient **Clos**.

   En cas de rejet, le statut de la feuille de temps devient **Rejeté**.

### Approuver une feuille de temps depuis la zone Accueil

{{step1-to-home}}

La zone Accueil s’ouvre.

1. Vérifiez que le widget **Mes approbations** est ajouté à votre zone d’Accueil. Pour plus d’informations, voir [Ajouter, modifier ou supprimer des widgets dans la nouvelle page d’accueil](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).
1. Recherchez une approbation de feuille de temps dans votre widget Mes approbations .
1. (Facultatif) Développez le menu déroulant à droite des boutons Approuver ou Rejeter pour ajouter un commentaire sur votre décision, puis cliquez sur **Ajouter**.
1. Cliquez sur l’un des boutons suivants pour prendre votre décision d’approbation :

   * Approuver
   * Rejeter

   L’approbation est supprimée du widget **Mes approbations**.


