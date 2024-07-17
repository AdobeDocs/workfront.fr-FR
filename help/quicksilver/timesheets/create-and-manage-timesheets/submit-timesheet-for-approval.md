---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Soumettre une feuille de temps pour approbation
description: L’envoi de votre feuille de temps pour approbation offre une visibilité sur vos heures de travail à votre responsable. Les approbateurs peuvent vérifier que tout le temps enregistré a été alloué dans les zones appropriées et qu’un nombre suffisant d’heures a été enregistré pour la période.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 19%

---

# Soumettre une feuille de temps pour approbation

L’envoi de votre feuille de temps pour approbation offre une visibilité sur vos heures de travail à votre responsable. Les approbateurs peuvent vérifier que tout le temps enregistré a été alloué dans les zones appropriées et qu’un nombre suffisant d’heures a été enregistré pour la période.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en affichage ou autorisations supérieures pour les tâches et problèmes</p> <p>Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures pour les tâches et les problèmes</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire, consultez <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Soumettre une feuille de temps pour approbation

* [Envoyer une feuille de temps pour approbation](#submit-a-timesheet-for-approval)
* [Afficher l’état d’une feuille de temps envoyée](#view-the-status-of-a-submitted-timesheet)

### Soumettre une feuille de temps pour approbation

Une fois qu’un approbateur de feuille de temps est défini (comme décrit dans la section [Désigner les approbateurs de feuille de temps](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) de l’article [Approuver une feuille de temps](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), le bouton **Fermer** au bas de la feuille de temps se transforme en bouton **Soumettre pour approbation**.

Pour soumettre une feuille de temps à validation :

1. Accédez à une feuille de temps qui a été configurée pour avoir un approbateur.
1. Temps du journal, comme décrit dans [Temps du journal](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Cliquez sur **Soumettre pour approbation** pour lancer le processus d’approbation de la feuille de temps.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   Le bouton **Submit for Approval** (Envoyer pour approbation) est remplacé par les boutons **Approve**, **Reject** et **Recall**. L’état de la feuille de temps passe à **Submitted**.

   Lorsque votre feuille de temps est soumise à approbation, l’approbateur voit la feuille de temps répertoriée dans la zone **Approbations** de la page **Accueil**. Les événements suivants peuvent se produire :

   * S’ils l’approuvent, le bouton **Rappeler** se transforme en **Rouvrir** et l’état de la feuille de temps est mis à jour en **Ouvrir**.
   * S’ils le rejettent, le bouton **Submit for Approval** (Envoyer pour approbation) remplace le bouton **Rappeler** et l’état de la feuille de temps est mis à jour vers **Rejected** (Refusé).

1. (Facultatif) Cliquez sur **Rappeler** si vous devez rouvrir la feuille de temps et mettre à jour votre heure. Pour plus d’informations, reportez-vous à la section [Rappeler une feuille de temps](#recall-a-timesheet) de cet article.

### Afficher l’état d’une feuille de temps envoyée {#view-the-status-of-a-submitted-timesheet}

Vous pouvez afficher l’état d’une feuille de temps après l’avoir envoyée.

Si l’administrateur Workfront a activé les gestionnaires d’événements Approbation de la feuille de temps pour l’utilisateur et Rejet de la feuille de temps vers l’utilisateur, vous en êtes informé une fois la feuille de temps approuvée ou rejetée. Pour plus d’informations sur l’activation des notifications d’événement, voir [Types de notification d’événement](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sans ces notifications, vous pouvez en savoir plus sur l’état de vos feuilles de temps envoyées dans la zone Feuille de temps de Workfront.

Pour afficher l’état d’une feuille de temps :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur **Feuilles de temps**. Le filtre **Tous** est sélectionné par défaut.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez.

     Ou

     Sélectionnez **Mes feuilles de calcul** pour n’afficher que vos feuilles de calcul.

     Cela applique les filtres Mes approbations de feuille de temps ou Ma feuille de temps à la liste des feuilles de temps.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Cliquez sur l’icône Filtrer ![](assets/filter-nwepng.png) pour appliquer un autre filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Création ou modification de filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste de feuille de temps ni dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé les filtres Mes approbations de feuille de temps et Mes feuilles de temps des commandes de liste de la zone Configuration ou de votre modèle de mise en page. Pour plus d’informations, voir les articles suivants :
   >
   >   
   >   
   >   * [Personnaliser les filtres, les vues et les regroupements à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Conditionnel) Si vous avez sélectionné **Mes feuilles de calcul**, assurez-vous que la vue **Standard** est appliquée et notez la colonne **État**.

   Les feuilles de calcul peuvent avoir les états suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ouvertes</td> 
      <td> <p>Votre feuille de temps est actuellement ouverte et vous pouvez consigner l’heure. </p> <p>Une feuille de temps rappelée s’affiche avec l’état Ouvrir. Pour plus d’informations, reportez-vous à la section <a href="#recall-a-timesheet" class="MCXref xref">Rappeler une feuille de temps</a> de cet article. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Soumis</td> 
      <td>Vous avez soumis votre feuille de temps pour approbation, mais elle n’a pas encore été approuvée. Vous pouvez vous souvenir d’une feuille de temps envoyée pour continuer à la modifier. Pour plus d’informations, reportez-vous à la section <a href="#recall-a-timesheet" class="MCXref xref">Rappeler une feuille de temps</a> de cet article. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fermé</td> 
      <td> <p>Les scénarios suivants sont possibles :</p> 
       <ul> 
        <li> <p>Si la feuille de temps n’a pas d’approbateur, vous avez gagné du temps et l’avez fermée.</p> </li> 
        <li> <p>Si la feuille de temps comporte un approbateur, vous l’avez envoyée pour approbation et elle a été approuvée.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rejeté</td> 
      <td>Vous avez soumis la feuille de temps à validation et l’approbateur l’a rejetée.</td> 
     </tr> 
    </tbody> 
   </table>

## Rappel d’une feuille de temps {#recall-a-timesheet}

Vous pouvez vous souvenir d’une feuille de temps qui a déjà été soumise à validation. Seules les feuilles de temps qui n’ont pas été approuvées peuvent être rappelées.

Pour rappeler une feuille de temps :

1. Cliquez sur l’icône **Menu Principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Feuilles de temps**.
1. Cliquez sur **Mes feuilles de calcul** dans le coin supérieur droit de l’écran ou sélectionnez **Mes feuilles de calcul** dans le menu déroulant **Filtre** ![](assets/filter-nwepng.png) .
1. Cliquez sur la période d’une feuille de temps dont l’état est **Envoyé**.
1. Cliquez sur **Rappeler**.

   La feuille de temps peut à nouveau être modifiée et son état passe à **Ouvrir**.
