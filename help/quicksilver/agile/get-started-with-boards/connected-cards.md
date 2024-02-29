---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Utilisation de cartes connectées sur les panoramas
description: Vous pouvez ajouter sur votre panorama une carte qui est connectée aux tâches et problèmes existants dans Workfront.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 246750d2a7a053d74df2ceb150f14fdb50f32ade
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 0%

---

# Utilisation de cartes connectées sur les panoramas

<!-- Audited: 2/2024 -->

Vous pouvez ajouter sur votre panorama une carte qui est connectée à des tâches et à des problèmes existants dans [!DNL Workfront].

Lorsque l’un des détails suivants est mis à jour pour la carte à un emplacement donné, il est automatiquement mis à jour à l’autre emplacement :

* [!UICONTROL Nom]
* [!UICONTROL Description]
* [!UICONTROL Assignation]
* [!UICONTROL Statut]
* [!UICONTROL Date d’achèvement prévue]
* [!UICONTROL Estimation] / [!UICONTROL Points d’article]
* [!UICONTROL Sous-tâches]
* [!UICONTROL Documents]

>[!NOTE]
>
>Une seule tâche ou problème connecté ne peut être ajouté qu’une seule fois par panorama. La même tâche ou le même problème peut être connecté à plusieurs panoramas.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license</strong></td> 
   <td>
   <p>Nouveau : contributeur ou version ultérieure</p>
   <p>Ou</p>
   <p>Actuel : requête ou version ultérieure</p>
 </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>Paramétrages du niveau d'accès</strong></td>
   <td><p>Affichage ou accès supérieur aux tâches et aux problèmes</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>Autorisations d’objet</strong></td>
   <td><p>Affichage ou autorisation ultérieure d’une tâche ou d’un problème Workfront</p></td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ajout d’une carte connectée

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Panoramas]**.
1. Accédez à un panorama. Pour plus d’informations, voir [Créer ou modifier un panorama](../../agile/get-started-with-boards/create-edit-board.md).
1. Cliquez sur **[!UICONTROL Ajouter une carte] > [!UICONTROL Carte connectée]**.
1. Choisissez un projet, puis sélectionnez une tâche ou un problème à ajouter sous forme de carte sur le panorama.

   Vous pouvez sélectionner plusieurs objets qui seront tous ajoutés sous forme de cartes distinctes.

   >[!NOTE]
   >
   >* Seuls les objets pour lesquels vous êtes autorisé à accéder sont disponibles dans les résultats de la recherche. Si un élément est grisé, il a déjà été ajouté au panorama.
   >* Lorsque vous filtrez par **[!UICONTROL Projets que je possède]** ou **[!UICONTROL Projets actifs]**, les projets qui correspondent à un état Terminé, Mort ou Refusé ne sont pas inclus. Vous pouvez toujours rechercher ces projets avec le **[!UICONTROL Tous]** filtre.

1. Cliquez sur **[!UICONTROL Ajouter]**.

   ![Recherche d’une tâche ou d’un problème à connecter](assets/boards-tasksissues-350x94.png)

   La carte est ajoutée au bas de la colonne la plus à gauche. La connexion [!DNL Workfront] et les personnes qui lui sont affectées s’affichent sur la carte.

   ![Carte connectée](assets/boards-connected-card-first-added.png)

1. Cliquez sur ![Ouvrir une tâche ou un problème](assets/boards-launch-icon.png) pour ouvrir le [!DNL Workfront] tâche ou problème dans un nouvel onglet du navigateur.
1. Pour modifier les détails de la carte, cliquez sur la carte (et non dans le nom de la carte).

   Ou

   Cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) sur la carte et sélectionnez **[!UICONTROL Modifier]**.

1. Dans le **[!UICONTROL Détails de la carte]** , ajoutez ou mettez à jour les informations suivantes :

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>La modification du nom change également le nom sur la connexion [!DNL Workfront] .</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td> 
      <td>La modification de la description modifie également la description sur la connexion [!DNL Workfront] . Vous pouvez ajouter des URL dans la description ; elles deviennent des liens cliquables lors de l’enregistrement de la carte.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>Sélectionnez la colonne de la carte.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Sélectionnez l’état de la carte. Les valeurs par défaut sont [!UICONTROL Nouveau], [!UICONTROL En cours] et [!UICONTROL Terminé], mais les états personnalisés définis pour l’élément dans [!DNL Workfront] sont également disponibles.</p>
      <p>Si des stratégies de colonne sont activées pour la mise à jour des valeurs de champ, la modification de l’état de la carte déplace automatiquement la carte vers la colonne correspondante. Pour plus d’informations, voir "Définition des paramètres et des stratégies de colonne" dans l’article <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Gestion des colonnes de panorama</a>.</p>
      <p>Cliquez sur <strong>[!UICONTROL Mark Complete]</strong> dans la partie supérieure de la carte, l’état devient automatiquement Terminé.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Fin planifiée]</strong></td>
      <td>La modification de cette date modifie également la date d’achèvement prévue pour la connexion. [!DNL Workfront] .</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>Nombre d’heures pendant lesquelles la carte doit être complétée.</p><p>La modification de l’estimation modifie également la valeur des points de l’histoire sur le [!DNL Workfront] .</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Affectations]</strong></td>
      <td><p>Pour affecter d’autres personnes ou une équipe à la carte, cliquez sur <strong>[!UICONTROL Ajouter une affectation]</strong> et commencez à saisir un nom dans le champ de recherche. Sélectionnez-la ensuite lorsqu’elle s’affichera dans la liste de résultats. Vous pouvez ajouter des individus et des équipes. Une seule affectation d’équipe est autorisée sur une carte connectée.</p>
      <p>Les personnes désignées que vous sélectionnez sont également affectées à la tâche ou au problème dans [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Balises]</strong></td>
      <td><p>Recherchez et sélectionnez des balises pour la carte.</p>
      <p>Pour plus d’informations sur la création de balises, voir <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Ajout de balises</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Champs personnalisés]</strong></td>
      <td><p>Tous les champs personnalisés que vous ajoutez s’affichent dans cette zone.</p>
      <p>Pour plus d’informations, voir <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personnalisation des champs affichés sur une carte</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask]</strong></td>
      <td><p>Toutes les sous-tâches existantes pour la tâche apparaissent dans cette section. Cliquez sur <strong>[!UICONTROL Ajouter une sous-tâche]</strong> pour ajouter une nouvelle sous-tâche.</p>
      <p>Le compteur en haut de la section indique le nombre de sous-tâches terminées et le nombre total de sous-tâches.</p>
      <p>Pour plus d’informations sur les sous-tâches, voir <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Gestion des sous-tâches sur les panoramas</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Liste de contrôle]</strong></td>
      <td><p>Cliquez sur <strong>[!UICONTROL Ajouter un élément de liste de contrôle]</strong>. Saisissez ensuite le titre de l’élément et appuyez sur Entrée. Un autre élément est automatiquement ajouté. Continuez à saisir des titres pour ajouter d’autres éléments.</p>
      <p>Le compteur en haut de la liste de contrôle indique le nombre d’éléments terminés et le nombre total d’éléments.</p> <p>Pour plus d’informations sur les éléments de liste de contrôle, voir <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Gérer les éléments de liste de contrôle sur les cartes</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Documents]</strong></td>
      <td>Pour un document existant, passez la souris sur la miniature du document, puis cliquez sur <strong>Aperçu</strong> pour afficher le fichier dans le navigateur ou <strong>Télécharger</strong> pour télécharger le fichier sur votre ordinateur. Pour obtenir un nouveau document, voir <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Ajout de documents sur les cartes</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>Voir "Journal des heures sur une carte connectée" ci-dessous.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p>Cliquez sur dans le <strong>[!UICONTROL Nouveau commentaire]</strong> et saisissez votre commentaire. Utilisez les outils de formatage pour mettre le texte en forme, puis cliquez sur le bouton <strong>Ajouter une pièce jointe</strong> icon <img src="assets/attachment-icon.png" alt="Icône Pièce jointe"> pour joindre un fichier au commentaire. Pour baliser une personne ou une équipe, utilisez la zone de recherche située au bas de la zone de commentaire. L’utilisateur n’a pas à être membre du panorama. Les utilisateurs balisés sur des cartes connectées recevront des notifications par e-mail.</p><p>Cliquez sur <strong>[!UICONTROL Submit]</strong> pour ajouter le commentaire à la carte.</p>
      <p><strong>REMARQUE :</strong> La zone de commentaire sur les cartes utilise la nouvelle expérience de commentaire d’Adobe Workfront. Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Mise à jour du travail</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Activité Système]</strong></td> 
      <td><p>Si vous avez <strong>Activité du système</strong> activée en tant que section de carte, l’activité s’affiche dans cette zone.</p> <p>Pour plus d’informations, voir <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personnalisation des champs affichés sur une carte</a> et <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Mises à jour suivies par le système</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Utilisez le panneau de navigation de gauche pour vous déplacer entre les sections des champs des détails de la carte.

1. Cliquez sur **[!UICONTROL Fermer]** pour revenir au panorama.
L’objet connecté, les personnes désignées, les balises, la date d’échéance, le compteur de liste de contrôle, l’estimation des heures et l’état s’affichent sur la carte.

   ![Carte ajoutée au panorama](assets/boards-connected-card-details-110922.png)

## Déconnexion d’une carte connectée

Vous pouvez déconnecter une carte connectée de son objet Workfront et la carte reste sur le panorama sous la forme d’une carte ad hoc que vous pouvez modifier.

Pour vous déconnecter au niveau du panorama, procédez comme suit :

1. Accédez au panorama.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) sur la carte connectée et sélectionnez **[!UICONTROL Déconnecter]**.
1. Cliquez sur **[!UICONTROL Déconnecter]** sur le message de confirmation.

Pour vous déconnecter au niveau de la carte :

1. Accédez au panorama et ouvrez la carte connectée.
1. Cliquez sur le bouton **[!UICONTROL Plus]** menu ![Plus de menu](assets/more-icon-spectrum.png) dans la zone Connexion des détails de la carte, puis sélectionnez **[!UICONTROL Déconnecter]**.
1. Cliquez sur **[!UICONTROL Déconnecter]** sur le message de confirmation.

## Convertir une carte ad hoc en carte connectée

Après avoir créé une carte ad hoc, vous pouvez la convertir en carte connectée. Pour plus d’informations sur les cartes ad hoc, voir [Ajouter une carte ad hoc à un panorama](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Accédez au panorama et ouvrez la carte ad hoc.
1. Vérifiez le nom et la description de la carte. Ils seront ajoutés à la tâche ou au problème que vous créez dans [!DNL Workfront].
1. Dans le [!UICONTROL Connexion] des détails de la carte, cliquez sur **[!UICONTROL Connexion à Workfront]**.
1. Sur le [!UICONTROL Connect Card] , choisissez si vous créez une tâche ou un problème.
1. Recherchez et sélectionnez un projet auquel ajouter la tâche ou le problème.

   >[!NOTE]
   >
   >* Seuls les objets pour lesquels vous êtes autorisé à accéder sont disponibles dans les résultats de la recherche.
   >* Lorsque vous filtrez par **[!UICONTROL Projets que je possède]** ou **[!UICONTROL Projets actifs]**, projets qui équivalent à un [!UICONTROL Terminer], [!UICONTROL Mort], ou [!UICONTROL Rejetés] ne sont pas inclus. Vous pouvez toujours rechercher ces projets avec le **[!UICONTROL Tous]** filtre.

1. Cliquez sur **[!UICONTROL Connexion]**.

   ![Connexion d’une carte ad hoc à Workfront](assets/boards-connect-ad-hoc-card.png)

   Le nom du projet s’affiche dans la zone Connexion sur les détails de la carte.

1. Cliquez sur **[!UICONTROL Fermer]** pour revenir au panorama.

## Journal des heures sur une carte connectée

Vous devez disposer des autorisations appropriées pour consigner les heures de connexion à la tâche ou au problème connecté.

Par défaut, les champs de journalisation de l’heure ne s’affichent pas sur les cartes connectées. Vous devez activer [!UICONTROL **Heures**] dans le [!UICONTROL Configurer] area under [!UICONTROL Cartes]. Pour plus d’informations, voir [Personnalisation des champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Saisissez le nombre d’heures pour la tâche ou le problème.
1. Sélectionnez une [!UICONTROL Type d’heure] dans le menu déroulant, s’il est différent de la valeur par défaut.
1. Cliquez sur [!UICONTROL **Temps journal**].

   ![Heures de connexion sur la carte](assets/log-hours-on-card.png)

   La durée de connexion à la carte est également enregistrée sur la tâche ou le problème connecté.

Le temps de journalisation sur la carte est identique à celui d’une tâche ou d’un problème. Pour plus d’informations, voir &quot;Temps de connexion à un projet, une tâche ou un problème&quot; dans l’article . [Temps de connexion](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

