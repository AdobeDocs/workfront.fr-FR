---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Enregistrer des heures
description: Vous pouvez consigner le temps passé sur les tâches dans&nbsp;Adobe Workfront pour indiquer le nombre d’heures passées à y travailler. Vous pouvez également consigner le temps qui n’est pas lié au travail, comme les vacances, le temps de maladie ou le temps que vous passez en réunion. L’heure de connexion s’affiche dans votre feuille de temps.
author: Alina
feature: Timesheets
role: User
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '3526'
ht-degree: 0%

---

# Enregistrer des heures

<!--Audited: 12/2023-->

<!--remove all preview and production references from this article with 23.3 release-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). 

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 
-->

Vous pouvez consigner le temps passé sur les tâches dans Adobe Workfront afin d’indiquer le nombre d’heures passées à les traiter. Vous pouvez également consigner le temps qui n’est pas lié au travail, comme les vacances, le temps de maladie ou le temps que vous passez en réunion. L’heure de connexion s’affiche dans votre feuille de temps.

Pour plus d’informations sur le type d’heures de connexion à Workfront, voir [Gestion des types d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article et consigner les heures spécifiques au projet :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : clair ou supérieur</p>
   <p>Actuel : 
   <ul><li>Passez en revue ou plus pour consigner les heures générales dans une feuille de temps</li>
   <li>Travailler ou plus pour consigner les heures sur un projet, une tâche ou un problème</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès au type d’élément de travail pour lequel vous enregistrez le temps </p> <p>Par exemple, vous avez besoin de l’accès Modifier aux problèmes pour consigner le temps de connexion des problèmes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribuez à l’élément de travail pour lequel vous enregistrez des autorisations, y compris les autorisations d’heures de journal.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Remarques concernant le temps de connexion dans Workfront

* Vous pouvez consigner le temps des projets, des tâches ou des problèmes, ou vous pouvez consigner le temps directement dans votre feuille de temps.

  Pour plus d’informations sur la création de feuilles de temps, voir [Création d’une feuille de temps à usage unique](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* Tout le temps passé par des outils autres que la feuille de temps apparaît dans la feuille de temps pour la période correspondante.
* Les tâches et les problèmes d’un projet qui n’est pas en cours ne sont pas prérenseignés dans une feuille de temps.
* L’heure consignée dans la feuille de temps est immédiatement appliquée à la tâche, au problème ou au projet.
* Les feuilles de calcul comprennent la durée totale pour toutes les dates enregistrées. Les week-ends sont toujours inclus, même si des calculs de chronologie ont été configurés pour les exclure (comme décrit dans la section [Configuration des préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* Le nombre maximal d’éléments affichés dans une feuille de temps est de 45. S’il existe plus de 45 éléments dont les dates correspondent à la période de la feuille de temps, seuls les éléments mis à jour le plus récemment s’affichent.
* Les entrées de l’heure incluses dans les enregistrements de facturation sont grisées et ne peuvent pas être modifiées dans la feuille de temps. Pour plus d’informations, voir [Créer des enregistrements de facturation](../../manage-work/projects/project-finances/create-billing-records.md).
* Par défaut, les tâches personnelles ne s’affichent pas dans la feuille de temps. Les tâches personnelles ne s’affichent dans la feuille de temps que lorsqu’elles ont été enregistrées. Après avoir consigné le temps sur une tâche personnelle, vous pouvez épingler la tâche dans la feuille de temps et elle restera sur la feuille de temps si elle reste épinglée. Pour plus d’informations, voir [Création d’éléments de travail à partir de la zone Accueil](../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Enregistrer des heures {#log-time-section}

Dans Workfront, vous pouvez consigner l’heure de connexion dans les zones suivantes :

* [Feuille de calcul](#timesheet)
* [Accueil](#home)
* [Projet, tâche ou problème](#project-task-or-issue)
* [Panneau Résumé](#summary-panel)
* [Panneaux](#boards)
* [Application mobile](#mobile-app)

### Feuille de temps {#timesheet}

#### Temps de connexion sur une feuille de temps {#log-time-on-a-timesheet}

Vous pouvez consigner l’heure aux éléments suivants dans la feuille de temps :

* Tâches, problèmes et projets prérenseignés qui s’affichent automatiquement, en fonction de la manière dont votre administrateur Workfront définit les préférences de la feuille de temps. Pour plus d’informations sur la façon dont les feuilles de temps sont préremplies, voir [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  Seules les tâches et les problèmes qui vous sont affectés sont préremplis dans votre feuille de temps. Les tâches et les problèmes affectés à vos équipes ou rôles de tâche ne renseignent pas automatiquement votre feuille de temps.

  Cliquez sur Travailler dessus pour attribuer l’élément à vos équipes et l’élément s’affichera dans votre feuille de temps.

* Tâches, problèmes ou projets que vous ajoutez manuellement.
* Tâches, problèmes ou projets pour lesquels vous avez déjà effectué une connexion ailleurs dans Workfront.
* Heure générale (vacances, formation, temps de surcharge).

>[!NOTE]
>
>Les utilisateurs chargés de la révision d’un profil de feuille de temps peuvent voir la zone Fiches horaires et consigner les heures générales. Cependant, ils ne peuvent pas consigner les heures sur les tâches ou les problèmes qui leur sont affectés et qui apparaissent sur la feuille de temps.

Pour consigner l’heure sur une feuille de temps :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche.

1. Cliquez sur [!UICONTROL **Feuilles de temps**]. Votre feuille de temps actuelle s’affiche par défaut.
   ![Feuille de calcul](assets/timesheet-redesigned-nwe.png)


1. (Facultatif) Cliquez sur le **plein écran** icon ![](assets/full-screen.png) pour afficher la feuille de temps en mode plein écran, cliquez sur le bouton **exit-full-screen** ![](assets/exit-full-screen.png) pour revenir à la feuille de temps.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Facultatif) Pour ajouter un projet, une tâche ou un problème à la feuille de temps, cliquez sur le bouton **Ajouter un élément** menu déroulant dans le coin supérieur gauche de la feuille de temps, puis cliquez sur **Ajouter des projets**, **Ajout de tâches**, ou **Ajout de problèmes**.

   Une liste de projets, de tâches ou de problèmes s’affiche.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Facultatif) Cliquez sur l’icône de recherche. ![Recherche d’un élément](assets/search-icon.png) pour rechercher un élément spécifique à l’aide d’un mot-clé à ajouter à la feuille de temps.

1. (Facultatif) Développez les menus déroulants de filtrage, d’affichage ou de regroupement pour en appliquer ou personnaliser un et afficher les informations sur l’élément de votre choix.

1. Sélectionnez un ou plusieurs éléments de la liste, puis cliquez sur **Ajouter**.

   Si vous avez ajouté moins de 50 éléments à la fois, ils sont ajoutés à la feuille de temps. Les tâches et les problèmes sont répertoriés sous le nom du projet.

   >[!NOTE]
   >
   >Lorsque vous ajoutez des tâches ou des problèmes à la feuille de temps, le projet est également ajouté.


1. (Conditionnel) Si vous ajoutez 50 éléments ou plus à la fois, un message de confirmation affichant le nombre d’éléments ajoutés à votre feuille de temps s’affiche.

   Cliquez sur **Tout ajouter** Pour ajouter tous les éléments, cliquez sur **Annuler** pour arrêter l’ajout des éléments sélectionnés, puis **Annuler** pour fermer la liste des éléments.

   Les tâches et les problèmes sont répertoriés sous le nom du projet.

   >[!NOTE]
   >
   >Les éléments que vous ajoutez manuellement à la feuille de temps sont épinglés et resteront sur les feuilles de temps actuelles et futures jusqu’à ce que vous les vidiez manuellement pour les supprimer. Pour plus d’informations sur l’annulation d’éléments pour les supprimer de la feuille de temps, passez à l’étape 10.

   <!--(ensure this stays accurate)-->

1. (Facultatif) Cliquez sur le **Réduire** ![](assets/collapse-icon.png) ou **Développer** ![](assets/expand-icon.png) icônes en regard du nom du projet pour afficher ou masquer la liste des tâches et des problèmes du projet.


   >[!TIP]
   >
   >   Lors de l’utilisation d’un clavier QWERTY standard et après avoir cliqué sur le nom d’un projet dans la feuille de temps, appuyez sur l’ensemble de clés suivant pour réduire ou développer le projet :
   >   * Pour développer le projet et afficher ses tâches :
   >     * Maj + Alt + flèche Haut pour les ordinateurs Windows
   >     * Maj + Option + flèche haut pour les ordinateurs Mac
   >   * Pour réduire le projet et masquer ses tâches :
   >     * Maj + Alt + Flèche Bas pour les ordinateurs Windows
   >     * Maj + Option + Flèche Bas pour les ordinateurs Mac.


1. (Facultatif) Pour épingler manuellement un élément qui s’affiche automatiquement sur la feuille de temps, passez la souris sur le nom de l’élément, puis cliquez sur l’icône **pin** icon ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   Lorsque vous utilisez un clavier QWERTY standard après avoir cliqué sur un élément dans la feuille de temps, appuyez sur l’ensemble de touches suivant pour épingler un élément :
   >   * Option + P pour les ordinateurs Windows et Mac.


1. (Facultatif) Cliquez sur l’icône de recherche. ![](assets/search-icon.png) et commencez à saisir un mot-clé pour rechercher un projet, une tâche ou un problème dans la feuille de temps.

1. (Conditionnel) Si votre administrateur Workfront ou de groupe a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** , sélectionnez un rôle de tâche dans le menu déroulant. Le rôle spécifié lorsque vous êtes affecté à l’élément de travail s’affiche par défaut. Si aucun rôle ne vous est attribué sur l’objet, votre rôle de Principal s’affiche comme valeur par défaut. Pour plus d’informations sur ce paramètre, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![Temps de journalisation de plusieurs rôles dans la feuille de temps](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Facultatif) Cliquez sur le **+** pour ajouter une autre ligne, puis sélectionnez un nouveau type d’heure dans le menu déroulant du [!UICONTROL Type d’heure] pour consigner l’heure d’un autre type d’heure.

   ![Menu déroulant Type d’heure](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)


   >[!TIP]
   >
   >   Selon votre système d’exploitation ou navigateur et lors de l’utilisation d’un clavier QWERTY standard, appuyez sur l’ensemble de touches suivant pour ajouter une autre ligne :
   >   * Ctrl + Option + + + pour les ordinateurs Windows
   >   * Cmd + Option + + + pour les ordinateurs Mac

   Les types d’heure sont disponibles en fonction de ce qui a été défini au niveau du système, du projet et de l’utilisateur, comme décrit dans la section [Définition des types d’heures et de la disponibilité des feuilles de temps](define-hour-types-and-availability.md).

   Le type d’heure ne peut pas être modifié après la fermeture d’une feuille de temps.

   >[!TIP]
   >
   >Si vous avez précédemment consigné l’heure et que le type d’heure sélectionné est maintenant désactivé, la ligne entière de l’heure consignée est grisée. Si vous sélectionnez un autre type d’heure et actualisez la page, l’option de type d’heure désactivée est supprimée de la liste déroulante. Vous ne pouvez donc pas ajouter d’heures supplémentaires à ce type d’heure.
   >
   >Envisagez d’ajouter une nouvelle ligne pour l’élément de travail pour lequel vous souhaitez consigner de l’heure supplémentaire et de sélectionner un nouveau type d’heure, si vous souhaitez conserver le type d’heure désactivé associé à l’heure consignée passée.

1. Cliquez sur le bouton **delete** icon  ![](assets/delete.png) en regard du rôle de tâche pour le supprimer. Toute heure enregistrée pour le rôle est également supprimée.

   >[!TIP]
   >
   >   Selon votre système d’exploitation ou navigateur et lors de l’utilisation d’un clavier QWERTY standard, appuyez sur l’ensemble de touches suivant pour supprimer une ligne :
   >   * Ctrl + Option + - pour les ordinateurs Windows
   >   * Cmd + Option + - pour les ordinateurs Mac

1. Spécifiez la durée de connexion à un jour donné dans la section chronologie de la feuille de temps, puis cliquez en dehors de la zone d’heure pour enregistrer l’entrée d’heure. Les heures sont enregistrées automatiquement. La ligne pour laquelle vous enregistrez l’heure est mise en surbrillance en bleu clair et la zone de saisie de l’heure est indiquée en bleu foncé.

   ![Zone de consignation de l’heure dans la feuille de temps](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   Le temps de connexion est exprimé en heures ou en jours. Ce paramètre est configuré par les utilisateurs disposant d’une licence Plan ou l’administrateur système, comme décrit dans la section [Configurer si l’heure est connectée en heures ou en jours](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >Vous devez enregistrer manuellement la feuille de temps si l’un des scénarios suivants se produit :
   >
   >* Le rôle de tâche associé à l’heure que vous avez précédemment enregistrée a changé et l’événement **Affecter manuellement des rôles de tâche aux entrées d’heure** a été désactivé. L’heure de journalisation des nouvelles dates l’associe à un rôle de tâche différent.
   >   
   >   Si le rôle a été modifié et que la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** est activé, vous pouvez consigner l’heure ou mettre à jour le rôle et vos modifications sont enregistrées automatiquement.
   >
   >* Le rôle de tâche affecté à une tâche ou à un problème est différent du rôle de tâche avec lequel le propriétaire de la feuille de temps consigne le temps. <!--or assigned to them_ this last  piece came from a Support note but but sure what role it's referring to. Leaving it out for now.-->.
   >
   >La feuille de temps permet de gagner du temps automatiquement lorsqu’il n’y a plus d’entrées en conflit entre les deux rôles.
   >

1. (Facultatif) Indiquez le nombre d’heures supplémentaires dans le champ Heure de dépassement de délai de l’en-tête de la feuille de temps.

   >[!TIP]
   >
   >Vous ne pouvez pas consigner un nombre d’heures supplémentaires supérieur au nombre total actuel d’heures sur la feuille de temps. Par exemple, si vous vous êtes connecté 7 heures sur la feuille de temps jusqu’à présent, vous ne pouvez pas consigner 8 heures supplémentaires.

1. (Facultatif) Cliquez sur **Commentaire** pour ajouter un commentaire pour votre entrée &quot;heure&quot;.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Lorsque vous utilisez un clavier QWERTY standard après avoir cliqué sur la zone de saisie de l’heure, appuyez sur l’ensemble de touches suivant pour ouvrir la zone de commentaire :
   >   * Maj + F2 pour les ordinateurs Windows et Mac.

1. Cliquez sur **Terminé** pour enregistrer le commentaire.

   >[!TIP]
   >
   >   Lors de l’utilisation d’un clavier QWERTY standard, dans la zone de commentaire, appuyez sur l’ensemble de clés suivant pour enregistrer le commentaire :
   >   * Ctrl + Entrée pour les ordinateurs Windows.
   >   * Cmd + Retour pour les ordinateurs Mac.


1. (Facultatif) Cliquez sur **Afficher les commentaires** dans la barre d’outils pour afficher les commentaires de saisie d’heure sous l’élément de travail .

   ![Commentaires répertoriés sous l’élément dans la feuille de temps](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Toutes les modifications que vous apportez à la feuille de temps sont enregistrées automatiquement.

1. (Facultatif) Cliquez sur la ligne d’une tâche ou d’un problème, puis cliquez sur **Résumé ouvert** dans le coin supérieur droit de la feuille de temps pour ajouter une mise à jour ou mettre à jour des informations sur la tâche ou le problème. Le panneau Résumé s’ouvre à droite.

   ![summary-panel-for-task-open-in-timesheet](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   Votre mise à jour s’affiche dans la zone Mises à jour de l’élément de travail associé à l’heure consignée.

   >[!TIP]
   >
   >Vous ne pouvez pas commenter les projets ni les entrées Heure générale.

1. Cliquez sur [!UICONTROL **Fermer le résumé**] pour fermer le panneau Résumé et revenir à la feuille de temps.

1. (Facultatif) Cliquez sur [!UICONTROL **Mises à jour**] dans le panneau de gauche, puis ajoutez une mise à jour à la feuille de temps. Pour plus d’informations sur les mises à jour de Workfront, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redesigné-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

1. (Facultatif) Revenez au **Feuille de calcul** pour fermer ou envoyer votre feuille de temps.

   * **Fermer**: fermez la feuille de temps lorsque vous l’avez mise à jour. Cette option n’est disponible que si votre feuille de temps n’est pas associée à un approbateur.

   * **Soumettre à validation :** Cette option est disponible uniquement si la feuille de temps contient un approbateur. Enregistrez vos modifications et soumettez-les pour approbation. Vous pouvez ouvrir la feuille de temps après l’avoir fermée en cliquant sur **Rappeler**, si aucune validation n’a encore été effectuée. Pour plus d’informations, voir [Envoyer une feuille de temps pour approbation](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Rejeter**: cette option s’affiche lorsque vous êtes un approbateur de feuille de temps et que la feuille de temps vous a été envoyée pour approbation. En cliquant dessus, l’état de la feuille de temps passe à Refusé et la feuille de temps reste ouverte.

   * **Approuver**: cette option s’affiche lorsque vous êtes un approbateur de feuille de temps et que la feuille de temps vous a été envoyée pour approbation. En cliquant dessus, le statut de la feuille de temps passe à Approuvé et ferme la feuille de temps.

   >[!TIP]
   >
   >Les options Rejeter et Approuver s’affichent également sur votre feuille de temps lorsque vous êtes administrateur système et que la feuille de temps est associée à un approbateur.

1. (Conditionnel) Si vous avez fermé ou envoyé votre feuille de temps pour approbation, cliquez sur l’une des options suivantes :

   * **Réouvrir**: cette option est disponible pour les feuilles de temps que vous avez déjà fermées et qui n’ont pas d’approbateurs, ou les feuilles de temps qui ont déjà été approuvées. rouvrez la feuille de temps pour modifier les entrées d’heure.
   * **Rappeler**: cette option est disponible pour les feuilles de temps qui ont été soumises à validation mais qui n’ont pas encore été approuvées ou rejetées. Cliquez sur **Rappeler** pour rouvrir la feuille de temps et modifier les entrées d’heure.

#### Supprimer un élément de la feuille de temps

Vous pouvez supprimer une entrée d’heure ou un élément (projet, tâche ou problème) d’une feuille de temps.

Pour supprimer une entrée d’heure d’une feuille de temps :

1. Accédez à la feuille de temps et recherchez l’entrée d’heure à supprimer.
1. Remplacez les heures saisies par 0 ou supprimez les heures et remplacez-les par 0, puis appuyez sur Entrée.

   Les heures sont supprimées et la feuille de temps est enregistrée automatiquement.

Vous pouvez supprimer un élément (projet, tâche ou problème) de la feuille de temps en l’annulant, si vous ne l’avez pas encore consigné et si vous avez ajouté manuellement l’élément (comme décrit aux étapes 4 à 8 dans la section [Temps de connexion sur une feuille de temps](#log-time-on-a-timesheet) dans cet article). <!--ensure this stays accurate-->

Vous ne pouvez pas supprimer automatiquement les éléments inclus dans la feuille de temps en fonction des préférences de la feuille de temps dans votre système Workfront ou groupe configuré pour préremplir la feuille de temps (comme décrit dans la section [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)). Les éléments cessent de préremplir la feuille de temps lorsque les dates des éléments se trouvent en dehors de la période de la feuille de temps.

Pour supprimer un élément de la feuille de temps qui a été ajouté manuellement :

1. Assurez-vous qu’aucune heure n’est enregistrée pour l’élément.
1. Cliquez sur le bouton **unpin** icon ![Epinglage d’un élément](assets/pin-icon.png) en regard de l’élément pour dissocier l’élément de la feuille de temps.

   >[!TIP]
   >
   >   Lors de l’utilisation d’un clavier QWERTY standard après avoir cliqué sur un élément dans la feuille de temps, appuyez sur l’ensemble de touches suivant pour dissocier un élément :
   > * Option + P pour les ordinateurs Windows et Mac.

   L’élément est supprimé de la feuille de temps après avoir actualisé la page.

### Page d’accueil {#home}

Vous pouvez consigner l’heure spécifique au projet dans la page d’accueil.

Pour obtenir des informations générales sur l’utilisation de la zone Accueil, reportez-vous aux sections suivantes :

* Pour plus d’informations sur l’utilisation de la zone d’accueil héritée, voir [Utilisation de la zone Accueil](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).
* Pour plus d’informations sur l’utilisation de la nouvelle zone d’accueil, voir [Prise en main du nouvel accueil](../../workfront-basics/using-home/new-home/get-started-with-new-home.md).

#### Temps de connexion à un élément de travail de la nouvelle zone d’accueil

Vous pouvez consigner le temps d’accès à n’importe quel objet dans n’importe quel widget à l’aide du panneau Résumé. Pour plus d’informations, voir [Panneau Résumé](#summary-panel) dans cet article.

En outre, pour consigner l’heure d’un élément dans le widget Mon travail :

1. L’accès au **Accueil** zone.
1. Ajoutez la variable **Mon travail** de votre page d’accueil.
1. Sélectionnez une tâche, un problème ou une requête dans une liste, puis cliquez sur **Travailler dessus**
1. Passez la souris sur la tâche ou le problème pour lequel vous souhaitez consigner le temps, puis cliquez sur le bouton **Temps journal** icon ![](assets/log-time-icon-in-new-home.png) à droite des informations de la tâche.

   ![](assets/log-time-ui-for-task-from-new-home.png)

1. Cliquez sur **Temps de connexion**.

#### Connexion à un élément de travail à partir de la zone d’accueil héritée

1. Dans le **Liste de tâches** , sélectionnez l’élément sur lequel vous souhaitez consigner la durée.
1. Dans le panneau de droite, cliquez sur **Temps journal**.

   ![](assets/log-time-home-350x181.png)

1. Dans le **Saisir les heures** dans le menu déroulant, sélectionnez le type d’heure approprié.\
   Les types d’heure sont disponibles en fonction de ce qui a été défini au niveau du système, du projet et de l’utilisateur, comme décrit dans la section [Définition des types d’heures et de la disponibilité des feuilles de temps](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Conditionnel) Si votre administrateur Workfront ou de groupe a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** , sélectionnez un rôle de tâche dans le menu déroulant. Le rôle spécifié lorsque vous êtes affecté à l’élément de travail s’affiche par défaut. Si aucun rôle ne vous est attribué sur l’objet, votre rôle de Principal s’affiche comme valeur par défaut. Pour plus d’informations sur ce paramètre, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Spécifiez l’heure de journalisation, puis cliquez sur **Temps journal**.

### Projet, tâche ou problème {#project-task-or-issue}

Vous pouvez consigner l’heure spécifique d’un projet, d’une tâche ou d’un problème dans les sections suivantes :

* [Section Mises à jour](#updates-section)
* [Section Heures](#hours-section)

#### Met à jour la section{#updates-section}

Pour vous connecter à la section Mises à jour d’un projet, d’une tâche ou d’un problème, vous devez disposer des éléments suivants :

* Une licence Work or Plan.
* Attribuez ou modifiez des autorisations au projet, à la tâche ou au problème d’accès aux heures de journal.\
  Pour plus d’informations sur l’octroi d’autorisations sur les projets, voir [Partage d’un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* Votre administrateur Workfront doit activer le paramètre Temps de connexion directement sur les projets sous [!UICONTROL **Frise chronologique et heures**]> [!UICONTROL **Préférences**], si vous souhaitez consigner le temps directement dans un projet.

  Pour plus d’informations sur l’autorisation des utilisateurs de consigner des heures directement dans des projets, voir [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour consigner l’heure dans la section Mises à jour d’un projet, d’une tâche ou d’un problème :

1. Accédez à un projet, à une tâche ou à un problème.
1. Dans le panneau de gauche, sélectionnez **Mises à jour**.
1. Cliquez sur **Temps journal**. <!-- did Anna B change the casing for this button? If yes and if she changed it for the other areas, update screen shot too-->

   La boîte de dialogue Temps journal s’affiche.

   >[!TIP]
   >
   >   Si la préférence de votre profil est définie sur l’heure de connexion en jours, la zone Saisir les jours s’affiche.
   >   
   >   Le nombre d’heures incluses dans une journée indique, dans le coin supérieur droit de la zone Enter Days.

   ![](assets/log-time-box-in-updates-stream.png)

1. Indiquez les informations suivantes :

   * **Type d’heure**: sélectionnez un type d’heure dans le menu déroulant, s’il est différent de celui affiché par défaut.

     Selon les types d’heures configurés dans votre système, les options disponibles peuvent varier. Pour plus d’informations sur la configuration des types d’heures, voir [Définition des types d’heures et de la disponibilité des feuilles de temps](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Rôle de tâche**: (Conditionnel) si votre administrateur Workfront ou de groupe a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** , sélectionnez une **Rôle de tâche** dans le menu déroulant. Le rôle spécifié lorsque vous êtes affecté à l’objet s’affiche par défaut. Si aucun rôle n’est attribué à l’objet, votre rôle de Principal s’affiche comme valeur par défaut. Pour plus d’informations sur ce paramètre, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   * **Heures**: saisissez le nombre d’heures pour le projet, la tâche ou le problème.

1. Cliquez sur **Temps de connexion**.

#### Section Heures{#hours-section}

Vous devez être un administrateur Workfront pour consigner le temps de connexion des projets, tâches et problèmes de la section Heures,

Ou

Vous devez disposer de tous les éléments suivants :

* Une licence Plan avec accès administratif aux Fiches horaires et aux heures. Pour plus d’informations sur l’octroi de l’accès administratif aux feuilles de calcul et aux heures, voir [Octroi aux utilisateurs un accès administratif à certaines zones](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* Accordez des autorisations ou des autorisations supérieures au projet avec accès aux heures de journal. Pour plus d’informations sur l’octroi d’autorisations sur les projets, voir [Partage d’un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* Votre administrateur Workfront doit activer le paramètre Temps de connexion directement sur les projets sous Frise chronologique et heures > Préférences si vous souhaitez que la durée de connexion soit directement associée à un projet. Pour plus d’informations sur l’autorisation des utilisateurs de consigner des heures directement dans des projets, voir [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour consigner l’heure dans la section Heures d’un projet, d’une tâche ou d’un problème :

1. Accédez à un projet, à une tâche ou à un problème.
1. Dans le panneau de gauche, cliquez sur **Heures**.
1. Cliquez sur **Temps journal**.

   La boîte de dialogue Heures de journal s’affiche.

1. Indiquez les informations suivantes :

   * **Propriétaire :** Par défaut, votre nom s’affiche dans ce champ.\
     Si vous enregistrez les heures pour un autre utilisateur, indiquez son nom.

   * **Type d’heure**: sélectionnez un type d’heure dans le menu déroulant, s’il est différent de celui affiché par défaut.

     Selon les types d’heures configurés dans votre système, les options disponibles peuvent varier. Pour plus d’informations sur la configuration des types d’heures, voir [Définition des types d’heures et de la disponibilité des feuilles de temps](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Rôle de tâche**: (Conditionnel) si votre administrateur Workfront ou de groupe a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** , sélectionnez une **Rôle de tâche** dans le menu déroulant. Le rôle spécifié lorsque vous êtes affecté à l’objet s’affiche par défaut. Si aucun rôle n’est attribué à l’objet, votre rôle de Principal s’affiche comme valeur par défaut. Pour plus d’informations sur ce paramètre, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     ![](assets/log-time-box-in-hours-section-on-task.png)
   * **Heures**: saisissez le nombre d’heures pour le projet, la tâche ou le problème.

1. Cliquez sur **Temps journal**.

### Panneau Résumé

Vous pouvez consigner l’heure des tâches et des problèmes dans le panneau Résumé.
Pour plus d’informations, voir [Aperçu du résumé](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Panneaux {#boards}

Vous pouvez consigner le temps de connexion sur les cartes connectées sur un panorama Workfront. Il s’agit du même processus que le temps de connexion à une tâche ou à un problème, et les heures enregistrées sur la carte sont enregistrées sur la tâche ou le problème connecté.
Pour plus d’informations, voir [Utilisation de cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Application mobile {#mobile-app}

Vous pouvez consigner le temps à partir de l’application mobile Workfront.
Pour plus d’informations, voir [Adobe Workfront pour Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) ou [Adobe Workfront pour iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
