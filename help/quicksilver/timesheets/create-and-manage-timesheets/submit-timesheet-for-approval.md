---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Envoyer une feuille de temps pour approbation
description: En soumettant votre feuille de temps à l’approbation de votre supérieur ou supérieure, vous lui donnez une visibilité sur vos heures de travail. Les personnes approbatrices peuvent vérifier que toutes les heures enregistrées ont été affectées aux domaines corrects et qu’un nombre suffisant d’heures a été enregistré pour la période concernée.
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 84%

---

# Soumettre une feuille de temps pour approbation

<!--Audited: 8/2024-->

En soumettant votre feuille de temps à l’approbation de votre supérieur ou supérieure, vous lui donnez une visibilité sur vos heures de travail. Les personnes approbatrices peuvent vérifier que toutes les heures enregistrées ont été affectées aux domaines corrects et qu’un nombre suffisant d’heures a été enregistré pour la période concernée.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Léger ou supérieur </p>
   <p>Actuel : Révision ou supérieur </p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Affichage ou accès supérieur aux tâches et aux problèmes </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures de la feuille de temps</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Soumettre une feuille de temps pour approbation

* [Soumettre une feuille de temps pour approbation](#submit-a-timesheet-for-approval)
* [Afficher le statut d’une feuille de temps soumise](#view-the-status-of-a-submitted-timesheet)

### Soumettre une feuille de temps pour approbation

Une fois qu’un approbateur de feuille de temps est défini (comme décrit dans la section [Désigner les approbateurs de feuille de temps](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) de l’article [Approuver une feuille de temps](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), le bouton **Fermer** au bas de la feuille de temps se transforme en bouton **Soumettre à approbation**.

Pour soumettre une feuille de temps à l’approbation :

1. Accédez à une feuille de temps qui a été configurée pour avoir une personne approbatrice.
1. Consignez les heures, tel que décrit dans [Consigner des heures](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Cliquez sur **Soumettre à approbation** pour lancer le processus d’approbation de la feuille de temps.

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   Le bouton **Soumettre pour approbation** est remplacé par les boutons **Approuver**, **Rejeter** et **Rappeler**. Le statut de la feuille de temps devient **Soumis**.

   Lorsque votre feuille de temps est soumise à approbation, l’approbateur voit la feuille de temps répertoriée dans le widget **Mes approbations** de la zone **Accueil**. Les choses suivantes peuvent se produire :

   * Si elle l’approuve, le bouton **Rappeler** devient **Réouvrir** et le statut de la feuille de temps devient **Ouvrir**.
   * S’ils le rejettent, le bouton **Soumettre pour approbation** remplace le bouton **Rappeler** et l’état de la feuille de temps est mis à jour vers **Refusé**.

1. (Facultatif) Cliquez sur **Rappeler** si vous devez rouvrir la feuille de temps et mettre à jour votre temps. Pour plus d’informations, voir la section [Rappeler une feuille de temps](#recall-a-timesheet) de cet article.

### Afficher le statut d’une feuille de temps soumise {#view-the-status-of-a-submitted-timesheet}

Vous pouvez consulter le statut d’une feuille de temps après l’avoir soumise.

Si l’administrateur ou administratrice Workfront a activé les gestionnaires d’événements Approbation de la feuille de temps à l’utilisateur ou utilisatrice et Rejet de la feuille de temps à l’utilisateur ou utilisatrice, vous recevez une notification lorsque la feuille de temps est approuvée ou rejetée. Pour plus d’informations sur l’activation des notifications d’événements, voir [Types de notifications d’événements](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sans ces notifications, vous pouvez vous renseigner sur le statuts de vos feuilles de temps soumises dans la zone Feuille de temps de Workfront.

Pour consulter le statut d’une feuille de temps :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.
1. Cliquez sur **Feuilles de temps**. Le filtre **Tous** est sélectionné par défaut.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Facultatif) Pour mettre à jour le filtre dans la liste des feuilles de temps, effectuez l’une des opérations suivantes :

   * Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous approuvez.

     Ou

     Sélectionnez **Mes feuilles de temps** pour afficher uniquement vos feuilles de temps.

     Cela applique les filtres Mes approbations de feuille de temps ou Mes feuilles de temps à la liste des feuilles de temps.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Cliquez sur l’icône Filtrer ![](assets/filter-nwepng.png) pour appliquer un autre filtre ou en créer un nouveau. Pour plus d’informations sur la création ou la mise à jour de filtres, voir [Créer ou modifier des filtres dans Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Les options Mes approbations de feuille de temps et Mes feuilles de temps ne s’affichent pas en haut de la liste de feuille de temps ni dans la liste des filtres si votre administrateur ou admnistratrice ou un administrateur ou une administratrice de groupes Workfront a supprimé les filtres Mes approbations de feuille de temps et Mes feuilles de temps des contrôles de liste de la zone Configuration ou de votre modèle de disposition. Pour plus d’informations, voir les articles suivants :
   >
   >   
   >   
   >   * [Personnaliser des filtres, des vues et des regroupements à l’aide d’un modèle de disposition](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Conditionnel) Si vous avez sélectionné **Mes feuilles de calcul**, assurez-vous que la vue **Standard** est appliquée et notez la colonne **État**.

   Les feuilles de temps peuvent avoir les statuts suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ouvertes</td> 
      <td> <p>Votre feuille de temps est actuellement ouverte et vous pouvez consigner le temps. </p> <p>Une feuille de temps rappelée s’affiche avec le statut Ouvert. Pour plus d’informations, consultez la section <a href="#recall-a-timesheet" class="MCXref xref">Rappeler une feuille de temps</a> de cet article. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Soumis</td> 
      <td>Vous avez soumis votre feuille de temps pour approbation mais elle n’a pas encore été approuvée. Vous pouvez rappeler une feuille de temps soumise pour continuer à la modifier. Pour plus d’informations, consultez la section <a href="#recall-a-timesheet" class="MCXref xref">Rappeler une feuille de temps</a> de cet article. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fermé</td> 
      <td> <p>Les scénarios suivants sont possibles :</p> 
       <ul> 
        <li> <p>Si la feuille de temps n’a pas de personne approbatrice, vous avez consigné vos heures et l’avez fermée.</p> </li> 
        <li> <p>Si la feuille de temps a une personne approbatrice, vous l’avez soumise pour approbation et elle a été approuvée.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rejeté</td> 
      <td>Vous avez soumis la feuille de temps pour approbation et la personne approbatrice l’a rejetée.</td> 
     </tr> 
    </tbody> 
   </table>

## Rappeler une feuille de temps {#recall-a-timesheet}

Vous pouvez rappeler une feuille de temps qui a déjà été soumise pour approbation. Seules les feuilles de temps qui n’ont pas été approuvées peuvent être rappelées.

Pour rappeler une feuille de temps, procédez comme suit :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Feuilles de temps**.
1. Cliquez sur **Mes feuilles de temps** dans le coin supérieur droit de l’écran ou sélectionnez **Mes feuilles de temps** dans le menu déroulant **Filtrer** ![](assets/filter-nwepng.png).
1. Cliquez sur la période d’une feuille de temps dont le statut est **Soumis**.
1. Cliquez sur **Rappeler**.

   La feuille de temps redevient modifiable et son statut passe à **Ouvert**.
