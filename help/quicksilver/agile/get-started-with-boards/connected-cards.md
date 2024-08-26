---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Utiliser des cartes connectées sur des panoramas
description: Vous pouvez ajouter sur votre panorama une carte qui est connectée à des tâches et à des problèmes existants dans Workfront.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 5c093edc97afdbd1d88824376ce4b019f71e099f
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 98%

---

# Utiliser des cartes connectées sur des panoramas

<!-- Audited: 2/2024 -->

Vous pouvez ajouter sur votre panorama une cadre qui est connectée à des tâches et à des problèmes existants dans [!DNL Workfront].

Lorsque l’un des détails suivants est mis à jour pour la carte à un emplacement, il est automatiquement mis à jour à l’autre emplacement :

* [!UICONTROL Nom]
* [!UICONTROL Description]
* [!UICONTROL Cessionnaires]
* [!UICONTROL Statut]
* [!UICONTROL Date d’achèvement prévue]
* [!UICONTROL Estimation] / [!UICONTROL Points de l’histroire]
* [!UICONTROL Sous-tâches]
* [!UICONTROL Documents]

>[!NOTE]
>
>Une tâche ou un problème connecté ne peut être ajouté qu’une seule fois par panorama. La même tâche ou le même problème peut être connecté à plusieurs panoramas.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouvelle : contributeur ou contributrice ou supérieure</p>
   <p>Ou</p>
   <p>Actuelle : demande ou supérieure</p>
 </td> 
  </tr> 
  <tr>
   <td role="rowheader">Configurations du niveau d’accès</td>
   <td><p>Affichage ou accès supérieur aux tâches et aux problèmes</p></td>
  </tr>
  <tr>
   <td role="rowheader">Autorisations d’objet</td>
   <td><p>Autorisations d’affichage ou supérieures à une tâche ou à un problème Workfront</p>
   <p><strong>Note : les personnes disposant d’autorisations d’affichage pour une tâche ou un problème ne peuvent pas agir sur les cartes qui y sont connectées, y compris déplacer la carte vers une autre colonne du panorama. </strong> Les personnes avec un accès en affichage peuvent uniquement ouvrir la carte pour afficher ses propriétés et ouvrir la tâche ou le problème connecté. Pour demander un accès supplémentaire, ouvrez la tâche ou le problème et demandez l’accès.</td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajouter une carte connectée

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Ajouter une carte] > [!UICONTROL Carte connectée]**.
1. Choisissez un projet, puis sélectionnez une tâche ou un problème à ajouter sous forme de carte sur le panorama.

   Vous pouvez sélectionner plusieurs objets qui seront tous ajoutés sous forme de cartes distinctes.

   >[!NOTE]
   >
   >* Seuls les objets sur lesquels vous disposez d’autorisations d’accès sont disponibles dans les résultats de la recherche. Si un élément est grisé, cela signifie qu’il a déjà été ajouté au panorama.
   >* Lorsque vous filtrez par Projets dont je suis propriétaire ou Projets auxquels je participe, les projets qui correspondent à un statut Terminé, Immobilisé ou Refusé ne sont pas inclus. ******** Vous pouvez toujours rechercher ces projets avec le filtre **[!UICONTROL Tous]**.

1. Cliquez sur **[!UICONTROL Ajouter]**.

   ![Rechercher une tâche ou un problème à connecter](assets/boards-tasksissues-350x94.png)

   La carte est ajoutée au bas de la colonne la plus à gauche. L’objet [!DNL Workfront] connecté et les personnes qui lui sont affectées s’affichent sur la carte.

   ![Carte connectée](assets/boards-connected-card-first-added.png)

1. Cliquez sur ![Ouvrir une tâche ou un problème](assets/boards-launch-icon.png) pour ouvrir la tâche ou le problème [!DNL Workfront] dans un nouvel onglet du navigateur.
1. Pour modifier les détails de la carte, cliquez sur la carte (ne cliquez pas sur le nom de la carte).

   Ou

   Cliquez sur le menu **[!UICONTROL Plus]** ![Menu Plus](assets/more-icon-spectrum.png) sur la carte et sélectionnez **[!UICONTROL Modifier]**.

1. Dans la zone **[!UICONTROL Détails de la carte]**, ajoutez ou mettez à jour les informations suivantes :

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>La modification du nom modifie également le nom sur l’objet [!DNL Workfront] connecté.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td> 
      <td>La modification de la description modifie également la description sur l’objet  connecté. [!DNL Workfront] Vous pouvez ajouter des URL dans la description ; elles deviennent des liens cliquables lorsque la carte est enregistrée.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>Sélectionnez la colonne de la carte.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Sélectionnez un statut pour la carte. Les valeurs par défaut sont [!UICONTROL New], [!UICONTROL In Progress] et [!UICONTROL Complete], mais les statuts personnalisés définis pour l’élément dans [!DNL Workfront] sont également disponibles.</p>
      <p>Si des politiques de colonne sont activées pour la mise à jour des valeurs de champ, la modification du statut de la carte déplace automatiquement la carte dans la colonne correspondante. Pour plus d’informations, voir « Définir des paramètres et des politiques de colonne » dans l’article <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Gérer les colonnes du panorama</a>.</p>
      <p>Cliquez sur <strong>[!UICONTROL Mark Complete]</strong> dans la partie supérieure de la carte. Le statut passe automatiquement à Terminé.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td>
      <td>La modification de cette date modifie également la date d’achèvement prévue sur l’objet [!DNL Workfront] connecté.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>Le nombre d’heures pour terminer la carte.</p><p>La modification de l’estimation modifie également la valeur des points de l’histoire sur l’objet [!DNL Workfront] connecté.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignments]</strong></td>
      <td><p>Pour affecter d’autres personnes ou une équipe à la carte, cliquez sur [!UICONTROL Add Assignment] et commencez à saisir un nom dans le champ de recherche. <strong></strong> Sélectionnez-le ensuite lorsqu’elle s’affiche dans la liste de résultats. Vous pouvez ajouter des personnes et des équipes. Une seule affectation d’équipe est autorisée sur une carte connectée.</p>
      <p>Les personnes désignées que vous sélectionnez sont également affectées à la tâche ou au problème dans [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Recherchez et sélectionnez des balises pour la carte.</p>
      <p>Pour plus d’informations sur la création de balises, voir <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Ajouter des balises</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom fields]</strong></td>
      <td><p>Tous les champs personnalisés que vous ajoutez s’affichent dans cette zone.</p>
      <p>Pour plus d’informations, voir <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personnaliser les champs affichés sur une carte</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask]</strong></td>
      <td><p>Toutes les sous-tâches existantes pour la tâche apparaissent dans cette section. Cliquez sur <strong>[!UICONTROL Add Subtask]</strong> pour ajouter une nouvelle sous-tâche.</p>
      <p>Le compteur en haut de la section indique le nombre de sous-tâches terminées et le nombre total de sous-tâches.</p>
      <p>Pour plus d’informations sur les sous-tâches, voir <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Gérer les sous-tâches sur les panoramas</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checklist]</strong></td>
      <td><p>Cliquez sur <strong>[!UICONTROL Add checklist item]</strong>. Saisissez ensuite le titre de l’élément et appuyez sur Entrée. Un autre élément est automatiquement ajouté. Continuez à saisir des titres pour ajouter d’autres éléments.</p>
      <p>Le compteur en haut de la liste de contrôle indique le nombre d’éléments terminés et le nombre total d’éléments.</p> <p>Pour plus d’informations sur les éléments de liste de contrôle, voir <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Gérer les éléments de la liste de contrôle sur les cartes</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Documents]</strong></td>
      <td>Pour un document existant, pointez sur la miniature du document, puis cliquez sur Aperçu pour afficher le fichier dans le navigateur ou sur Télécharger pour télécharger le fichier sur votre ordinateur. <strong></strong><strong></strong> Pour un nouveau document, voir <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Ajouter des documents sur les cartes</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>Voir « Consigner les heures sur une carte connectée » ci-dessous.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p>Cliquez dans le champ [!UICONTROL New comment] et saisissez votre commentaire. <strong></strong> Utilisez les outils de formatage pour mettre le texte en forme. Pour taguer une personne ou une équipe, utilisez la zone de recherche située au bas de la zone de commentaire. L’utilisateur ou l’utilisatrice ne doit pas nécessairement être membre du panorama. Les utilisateurs et utilisatrices tagués sur des cartes connectées recevront des notifications par e-mail.</p><p>Cliquez sur <strong>[!UICONTROL Submit]</strong> pour ajouter le commentaire à la carte.</p>
      <p>Pour plus d'informations sur les commentaires, voir <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Mise à jour du travail</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL System activity]</strong></td> 
      <td><p>Si vous avez une <strong>Activité du système</strong> activée en tant que section de carte, l’activité s’affiche dans cette zone.</p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personnaliser les champs affichés sur une carte</a> et <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Mises à jour suivies par le système</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Utilisez le panneau de navigation de gauche pour vous déplacer entre les sections des champs des détails de la carte.

1. Cliquez sur Fermer pour revenir au panorama. ****
L’objet connecté, les personnes désignées, les balises, la date d’échéance, le compteur de liste de contrôle, l’estimation des heures et le statut s’affichent sur la carte.

   ![Carte ajoutée au panorama](assets/boards-connected-card-details-110922.png)

## Déconnecter une carte connectée

Vous pouvez déconnecter une carte connectée de son objet Workfront et la carte reste sur le panorama sous forme de carte ad hoc que vous pouvez modifier.

Pour vous déconnecter au niveau du panorama :

1. Accédez au panorama.
1. Cliquez sur le menu **[!UICONTROL Plus]** ![Menu Plus](assets/more-icon-spectrum.png) sur la carte connectée et sélectionnez **[!UICONTROL Déconnecter]**.
1. Cliquez sur **[!UICONTROL Déconnecter]** dans le message de confirmation.

Pour déconnecter au niveau de la carte :

1. Accédez au panorama et ouvrez la carte connectée.
1. Cliquez sur le menu **[!UICONTROL Plus]** ![icône de menu Plus](assets/more-icon-spectrum.png) dans la zone Connexion des détails de la carte et sélectionnez **[!UICONTROL Déconnecter]**.
1. Cliquez sur **[!UICONTROL Déconnecter]** dans le message de confirmation.

## Convertir une carte ad hoc en carte connectée

Après avoir créé une carte ad hoc, vous pouvez la convertir en carte connectée. Pour plus d’informations sur les cartes ad hoc, voir [Ajouter une carte ad hoc à un panorama](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Accédez au panorama et ouvrez la carte ad hoc.
1. Vérifiez le nom et la description de la carte. Ils seront ajoutés à la tâche ou au problème que vous créez dans [!DNL Workfront].
1. Dans la zone [!UICONTROL Connexion] des détails de la carte, cliquez sur **[!UICONTROL Se connecter à Workfront]**.
1. Dans la fenêtre [!UICONTROL Carte Connect], choisissez si vous créez une tâche ou un problème.
1. Recherchez et sélectionnez un projet auquel ajouter la tâche ou le problème.

   >[!NOTE]
   >
   >* Seuls les objets sur lesquels vous disposez d’autorisations d’accès sont disponibles dans les résultats de la recherche.
   >* Lorsque vous filtrez par **[!UICONTROL Projets dont je suis propriétaire]** ou **[!UICONTROL Projets auxquels je participe]**, les projets qui correspondent à un statut [!UICONTROL Terminé], [!UICONTROL Immobilisé] ou [!UICONTROL Refusé] ne sont pas inclus. Vous pouvez toujours rechercher ces projets avec le filtre **[!UICONTROL Tous]**.

1. Cliquez sur **[!UICONTROL Connecter]**.

   ![Connecter une carte ad hoc à Workfront](assets/boards-connect-ad-hoc-card.png)

   Le nom du projet s’affiche dans la zone Connexion des détails de la carte.

1. Cliquez sur **[!UICONTROL Fermer]** pour revenir au panorama.

## Consigner les heures sur une carte connectée

Vous devez disposer des autorisations appropriées pour consigner les heures sur la tâche ou le problème connecté.

Les champs de journalisation du temps ne s’affichent pas par défaut sur les cartes connectées. Vous devez activer [!UICONTROL **Heures**] dans la zone [!UICONTROL Configurer] sous [!UICONTROL Cartes]. Pour plus d’informations, voir [Personnaliser les champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Saisissez le nombre d’heures pour la tâche ou le problème.
1. Sélectionnez une [!UICONTROL Type d’heure] dans le menu déroulant, s’il est différent de la valeur par défaut.
1. Cliquez sur [!UICONTROL **Consigner le temps**].

   ![Consigner les heures sur une carte](assets/log-hours-on-card.png)

   Le temps consigné sur la carte est également enregistré sur la tâche ou le problème connecté.

La journalisation du temps sur la carte est identique à la journalisation du temps sur une tâche ou un problème. Pour plus d’informations, voir « Consigner le temps sur un projet, une tâche ou un problème » dans l’article [Consigner le temps](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

