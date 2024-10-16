---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Approbation d’une feuille de calcul
description: Le processus d’approbation des feuilles de temps permet aux personnes responsables d’avoir une visibilité sur les heures de travail des personnes travaillant sous leur supervision directe. Les personnes approbatrices peuvent vérifier que toutes les heures consignées ont été affectées aux domaines corrects et qu’un nombre suffisant d’heures a été consigné pour la période.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 53%

---

# Approuver une feuille de temps

<!--Audited: 8/2024-->

Le processus d’approbation des feuilles de temps permet aux personnes responsables d’avoir une visibilité sur les heures de travail des personnes travaillant sous leur supervision directe. Les personnes approbatrices peuvent vérifier que toutes les heures consignées ont été affectées aux domaines corrects et qu’un nombre suffisant d’heures a été consigné pour la période.

Adobe Workfront offre la possibilité de configurer les approbations des feuilles de temps pour aider dans ce domaine.

Pour plus d’informations sur la soumission d’une feuille de temps, voir [Soumettre une feuille de temps pour approbation](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Formule Adobe Workfront</p></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td> <p>Nouveau : Standard</p>
   <p>Actuel : formule </p> 
   <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux feuilles de calcul et aux heures </p> </td> 
  </tr>

</td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Désigner les personnes approbatrices des feuilles de temps

En règle générale, les feuilles de temps sont approuvées par les personnes responsables fonctionnelles ou le personnel des ressources humaines. Les feuilles de temps ne sont généralement pas approuvées par les chefs de projet. Les chefs de projet peuvent approuver le temps de connexion aux projets, mais les chefs d’équipe ou de ressources humaines doivent approuver les feuilles de temps.

Un approbateur de feuille de temps est défini lors de la création du profil de feuille de temps. Vous devez disposer d’une licence Plan pour être désigné comme approbateur.

Pour plus d’informations sur la désignation des personnes approbatrices des feuilles de temps, voir la section [Créer ou modifier un profil de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) dans l’article [Créer, modifier et attribuer des profils de feuille de temps](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Approuver une feuille de temps

Vous pouvez approuver toutes les feuilles de temps qui ont été soumises et pour lesquelles vous êtes une personne approbatrice. Lorsqu’une feuille de temps est soumise à approbation, elle est répertoriée dans le widget **Mes approbations** de votre zone **Accueil**. Pour plus d’informations, voir [Approuver un travail](../../review-and-approve-work/manage-approvals/approving-work.md).

Si les paramètres de notification suivants sont en place, l’utilisateur qui envoie la feuille de temps pour approbation reçoit un courrier électronique après la validation d’une feuille de temps :

* L’administrateur Workfront a activé l’approbation de la feuille de temps pour l’utilisateur et le rejet de la feuille de temps pour les gestionnaires d’événements User. Pour plus d’informations sur l’activation des notifications d’événements, voir [Types de notifications d’événements](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
* La notification personnelle &quot;Ma feuille de temps&quot; est activée sur la page de profil de l’utilisateur. Pour plus d’informations, consultez la section [Modifier vos propres notifications par e-mail](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Approbation d’une feuille de temps à partir de la zone Feuilles de temps

{{step1-to-timesheets}}

La zone **Fiches horaires** s’ouvre.

1. (Conditionnel) Si la dernière fois que vous avez accédé s’ouvre, cliquez sur **Retour à la feuille de temps** dans le coin supérieur gauche de l’écran.

1. Sélectionnez **Mes approbations de feuille de temps** dans le coin supérieur droit de la page pour afficher uniquement les feuilles de temps que vous avez approuvées.

   Ou

   Sélectionnez le filtre **Mes approbations de feuille de temps** en haut de la liste des feuilles de temps.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >L’option Mes approbations de feuille de temps ne s’affiche pas en haut de la liste des feuilles de temps ni dans la liste des filtres si votre administrateur Workfront ou un administrateur de groupe a supprimé le filtre Mes approbations de feuille de temps des commandes de liste de la zone Configuration ou de votre modèle de mise en page.
   >
   >Pour plus d’informations, voir [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
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

### Approuver une feuille de calcul à partir de la zone Accueil

{{step1-to-home}}

La zone Accueil s’ouvre.

1. Assurez-vous que le widget **Mes approbations** a été ajouté à votre zone d’accueil. Pour plus d’informations, voir [Ajout, modification ou suppression de widgets dans Nouvelle page d’accueil](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md).
1. Recherchez une approbation de feuille de temps dans votre widget Mes approbations .
1. (Facultatif) Développez le menu déroulant à droite des boutons Approuver ou Rejeter pour ajouter un commentaire sur votre décision, puis cliquez sur **Ajouter**.
1. Cliquez sur l’un des boutons suivants pour effectuer votre décision de validation :

   * Approuver
   * Rejeter

   L’approbation est supprimée du widget **Mes approbations**.


