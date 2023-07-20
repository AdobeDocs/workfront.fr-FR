---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Temps de connexion
description: Vous pouvez consigner le temps passé sur les tâches dans&nbsp;Adobe Workfront pour indiquer le nombre d’heures passées à y travailler. Vous pouvez également consigner le temps qui n’est pas lié au travail, comme les vacances, le temps de maladie ou le temps que vous passez en réunion. L’heure de connexion s’affiche dans votre feuille de temps.
author: Alina
feature: Timesheets
role: User
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '3337'
ht-degree: 0%

---

# Temps de connexion

<!--remove all preview and production references from this article with 23.3 release-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>-->

Vous pouvez consigner le temps passé sur les tâches dans Adobe Workfront afin d’indiquer le nombre d’heures passées à les traiter. Vous pouvez également consigner le temps qui n’est pas lié au travail, comme les vacances, le temps de maladie ou le temps que vous passez en réunion. L’heure de connexion s’affiche dans votre feuille de temps.

Pour plus d’informations sur le type d’heures de connexion à Workfront, voir [Gestion des types d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Exigences d’accès

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p>
   <p>Legacy license: 
   <ul><li>Review or higher to log General Hours in a timesheet</li>
   <li>Work or higher to log hours on a project, task, or issue</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the type of work item you log time for </p> <p>For example, you need Edit access to Issues, to log time for issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on the work item you log time for that includes permissions to Log Hours</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article et consigner les heures spécifiques au projet :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <ul><li>Passez en revue ou plus pour consigner les heures générales dans une feuille de temps</li>
   <li> Utilisation ou plus élevée pour consigner les heures d’un projet, d’une tâche ou d’un problème</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès au type d’élément de travail pour lequel vous enregistrez le temps </p> <p>Par exemple, vous avez besoin de l’accès Modifier aux problèmes pour consigner le temps de connexion des problèmes.</p> <p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribuez ou modifiez les autorisations de l’élément de travail pour lequel vous enregistrez l’heure, y compris les autorisations de journal des heures.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Remarques concernant le temps de connexion dans Workfront

* Vous pouvez consigner le temps des projets, des tâches ou des problèmes, ou vous pouvez consigner le temps directement dans votre feuille de temps.

  Pour plus d’informations sur la création de feuilles de temps, voir [Création d’une feuille de temps à usage unique](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* Tout le temps passé par des outils autres que la feuille de temps apparaît dans la feuille de temps pour la période correspondante.
* Les tâches et les problèmes d’un projet qui n’est pas en cours ne sont pas prérenseignés dans une feuille de temps.
* L’heure consignée dans la feuille de temps est immédiatement appliquée à la tâche, au problème ou au projet.
* Les feuilles de calcul comprennent la durée totale pour toutes les dates enregistrées. Les week-ends sont toujours inclus, même si des calculs de chronologie ont été configurés pour les exclure (comme décrit dans la section [Configuration des préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* Le nombre maximal d’éléments affichés dans une feuille de temps est de 45. S’il existe plus de 45 éléments dont les dates correspondent à la période de la feuille de temps, seuls les éléments mis à jour le plus récemment s’affichent.
* Les entrées de l’heure incluses dans les enregistrements de facturation sont grisées et ne peuvent pas être modifiées dans la feuille de temps. Pour plus d’informations, voir [Créer des enregistrements de facturation](../../manage-work/projects/project-finances/create-billing-records.md).

## Temps de connexion

Dans Workfront, vous pouvez consigner l’heure de connexion dans les zones suivantes :

* [Feuille de temps](#timesheet)
* [Page d’accueil](#home)
* [Projet, tâche ou problème](#project-task-or-issue)
* [Panneau Résumé](#summary-panel)
* [Panoramas](#boards)
* [Application mobile](#mobile-app)

### Feuille de temps {#timesheet}


#### Temps de connexion sur une feuille de temps {#log-time-on-a-timesheet}

Vous pouvez consigner les heures générales ou les heures spécifiques au projet sur une feuille de temps.

>[!NOTE]
>
>Les utilisateurs chargés de la révision d’un profil de feuille de temps peuvent voir la zone Fiches horaires et consigner les heures générales. Cependant, ils ne peuvent pas consigner les heures sur les tâches ou les problèmes qui leur sont affectés et qui apparaissent sur la feuille de temps.

1. Cliquez sur le bouton [!UICONTROL **Menu Principal**] icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur [!UICONTROL **Feuilles de temps**]. Votre feuille de temps actuelle s’affiche par défaut.
   ![Feuille de temps](assets/timesheet-redesigned-nwe.png)

   La feuille de temps est prérenseignée avec les éléments qui vous sont affectés au cours de la période de la feuille de temps. Pour plus d’informations sur le préremplissage des feuilles de temps, voir [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). Si vous ne voyez pas d’élément sur la feuille de temps, vous pouvez l’ajouter.

   >[!NOTE]
   >
   >La feuille de temps ne préremplit que les éléments qui vous sont affectés. Il ne préremplit pas les éléments affectés à vos équipes ou rôles de tâche.
   >
   >Cliquez sur Travailler dessus pour attribuer l’élément à vos équipes et l’élément s’affichera dans votre feuille de temps.


1. (Facultatif) Cliquez sur le **plein écran** icon ![](assets/full-screen.png) pour afficher la feuille de temps en mode plein écran, cliquez sur le bouton **sortie-plein écran** ![](assets/exit-full-screen.png) pour revenir à la feuille de temps.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Facultatif) Pour ajouter un projet, une tâche ou un problème à la feuille de temps, cliquez sur le bouton **Ajouter un élément** menu déroulant dans le coin supérieur gauche de la feuille de temps, puis cliquez sur **Ajouter des projets**, **Ajout de tâches** ou **Ajout de problèmes**.

   Une liste de projets, de tâches ou de problèmes s’affiche.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Facultatif) Cliquez sur l’icône de recherche. ![Recherche d’un élément](assets/search-icon.png) pour rechercher un élément spécifique à l’aide d’un mot-clé à ajouter à la feuille de temps.

1. (Facultatif) Développez les menus déroulants de filtrage, d’affichage ou de regroupement pour en appliquer ou personnaliser un et afficher les informations sur l’élément de votre choix.

1. Sélectionnez un ou plusieurs éléments de la liste, puis cliquez sur **Ajouter**.

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

1. (Conditionnel) Si votre administrateur Workfront ou de groupe a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** , sélectionnez un rôle de tâche dans le menu déroulant. Le rôle spécifié lorsque vous êtes affecté à l’élément de travail s’affiche par défaut. Si aucun rôle n’est attribué à l’objet, votre rôle Principal s’affiche comme valeur par défaut. Pour plus d’informations sur ce paramètre, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   >   Toutes les modifications apportées à la feuille de temps sont enregistrées automatiquement.

1. (Facultatif) Cliquez sur la ligne d’une tâche ou d’un problème, puis cliquez sur **Résumé ouvert** dans le coin supérieur droit de la feuille de temps pour ajouter une mise à jour ou mettre à jour des informations sur la tâche ou le problème. Le panneau Résumé s’ouvre à droite.

   ![summary-panel-for-task-open-in-timesheet](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   Votre mise à jour s’affiche dans la zone Mises à jour de l’élément de travail associé à l’heure consignée.

   >[!TIP]
   >
   >Vous ne pouvez pas commenter les projets ni les entrées Heure générale.

1. Cliquez sur [!UICONTROL **Fermer le résumé**] pour fermer le panneau Résumé et revenir à la feuille de temps.

1. (Facultatif) Cliquez sur [!UICONTROL **Mises à jour**] dans le panneau de gauche, puis ajoutez une mise à jour à la feuille de temps. Pour plus d’informations sur les mises à jour de Workfront, voir [Mise à jour du travail](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redesigné-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **Fermer**: Fermez la feuille de temps lorsque vous avez terminé de la mettre à jour. Cette option n’est disponible que si votre feuille de temps n’est pas associée à un approbateur.

   * **Soumettre à validation :** Cette option est disponible uniquement si la feuille de temps contient un approbateur. Enregistrez vos modifications et soumettez-les pour approbation. Vous pouvez ouvrir la feuille de temps après l’avoir fermée en cliquant sur **Rappeler**, si aucune validation n’a encore été effectuée. Pour plus d’informations, voir [Envoyer une feuille de temps pour approbation](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Rejeter**: Cette option s’affiche lorsque vous êtes un approbateur de feuille de temps et que la feuille de temps vous a été envoyée pour approbation. En cliquant dessus, l’état de la feuille de temps passe à Refusé et la feuille de temps reste ouverte.

   * **Approuver**: Cette option s’affiche lorsque vous êtes un approbateur de feuille de temps et que la feuille de temps vous a été envoyée pour approbation. En cliquant dessus, le statut de la feuille de temps passe à Approuvé et ferme la feuille de temps.

   >[!TIP]
   >
   >Les options Rejeter et Approuver s’affichent également sur votre feuille de temps lorsque vous êtes administrateur système et que la feuille de temps est associée à un approbateur.

1. (Conditionnel) Si vous avez fermé ou envoyé votre feuille de temps pour approbation, cliquez sur l’une des options suivantes :

   * **Réouvrir**: Cette option est disponible pour les feuilles de temps que vous avez déjà fermées et qui n’ont pas d’approbateurs, ou les feuilles de temps qui ont déjà été approuvées. rouvrez la feuille de temps pour modifier les entrées d’heure.
   * **Rappeler**: Cette option est disponible pour les feuilles de temps qui ont été soumises à validation mais qui n’ont pas encore été approuvées ou rejetées. Cliquez sur **Rappeler** pour rouvrir la feuille de temps et modifier les entrées d’heure.

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

Pour obtenir des informations générales sur l’utilisation de la zone Accueil, voir [Utilisation de la zone Accueil](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

Pour vous connecter à un élément de travail à partir de la zone Accueil :

1. Dans le **Liste de tâches** , sélectionnez l’élément sur lequel vous souhaitez consigner la durée.
1. Dans le panneau de droite, cliquez sur **Temps journal**.

   ![](assets/log-time-home-350x181.png)

1. Dans le **Saisir les heures** dans le menu déroulant, sélectionnez le type d’heure approprié.\
   Les types d’heure sont disponibles en fonction de ce qui a été défini au niveau du système, du projet et de l’utilisateur, comme décrit dans la section [Définition des types d’heures et de la disponibilité des feuilles de temps](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Conditionnel) Si votre administrateur Workfront ou de groupe a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** , sélectionnez un rôle de tâche dans le menu déroulant. Le rôle spécifié lorsque vous êtes affecté à l’élément de travail s’affiche par défaut. Si aucun rôle n’est attribué à l’objet, votre rôle Principal s’affiche comme valeur par défaut. Pour plus d’informations sur ce paramètre, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Spécifiez l’heure de journalisation, puis cliquez sur **Temps journal**.

### Projet, tâche ou problème {#project-task-or-issue}

Vous pouvez consigner l’heure spécifique d’un projet, d’une tâche ou d’un problème dans les sections suivantes :

* [Met à jour la section](#updates-section)
* [Section Heures](#hours-section)

#### Met à jour la section{#updates-section}

<!--remove the note below when the -->

>[!NOTE]
>
> Il existe de légères différences d’aspect de l’interface utilisateur entre la section actuelle et la nouvelle section Mises à jour. Les informations de cette section font référence aux fonctionnalités telles qu’elles s’affichent dans la nouvelle expérience de commentaire.
>
>Pour plus d’informations sur la nouvelle section Mises à jour, voir [Nouvelle expérience de commentaire](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

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

   La boîte de dialogue Durée de journalisation s’affiche.

   >[!TIP]
   >
   >   Si la préférence de votre profil est définie sur l’heure de connexion en jours, la zone Saisir les jours s’affiche.
   >   
   >   Le nombre d’heures incluses dans une journée indique, dans le coin supérieur droit de la zone Enter Days.

   ![](assets/log-time-box-in-updates-stream.png)

1. Indiquez les informations suivantes :

   * **Type d’heure**: Sélectionnez un Type d’heure dans le menu déroulant, s’il est différent de celui affiché par défaut.

     Selon les types d’heures configurés dans votre système, les options disponibles peuvent varier. Pour plus d’informations sur la configuration des types d’heures, voir [Définition des types d’heures et de la disponibilité des feuilles de temps](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Rôle de tâche**: (Conditionnel) Si votre administrateur Workfront ou de groupe a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** , sélectionnez une **Rôle de tâche** dans le menu déroulant. Le rôle spécifié lorsque vous êtes affecté à l’objet s’affiche par défaut. Si aucun rôle n’est attribué à l’objet, votre rôle Principal s’affiche comme valeur par défaut. Pour plus d’informations sur ce paramètre, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   * **Heures**: Saisissez le nombre d’heures pour le projet, la tâche ou le problème.

1. Cliquez sur **Temps journal**.

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

   * **Heures**: Saisissez le nombre d’heures pour le projet, la tâche ou le problème.
   * **Type d’heure**: Sélectionnez un Type d’heure dans le menu déroulant, s’il est différent de celui affiché par défaut.

     Selon les types d’heures configurés dans votre système, les options disponibles peuvent varier. Pour plus d’informations sur la configuration des types d’heures, voir [Définition des types d’heures et de la disponibilité des feuilles de temps](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Rôle de tâche**: (Conditionnel) Si votre administrateur Workfront ou de groupe a activé la variable **Affecter manuellement des rôles de tâche aux entrées d’heure** , sélectionnez une **Rôle de tâche** dans le menu déroulant. Le rôle spécifié lorsque vous êtes affecté à l’objet s’affiche par défaut. Si aucun rôle n’est attribué à l’objet, votre rôle Principal s’affiche comme valeur par défaut. Pour plus d’informations sur ce paramètre, voir l’article [Configuration des préférences de feuille de temps et d’heure](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. Cliquez sur **Heures de journal**.

### Panneau Résumé

Vous pouvez consigner l’heure des tâches et des problèmes dans le panneau Résumé.
Pour plus d’informations, voir [Aperçu du résumé](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Panoramas {#boards}

Vous pouvez consigner le temps de connexion sur les cartes connectées sur un panorama Workfront. Il s’agit du même processus que le temps de connexion à une tâche ou à un problème, et les heures enregistrées sur la carte sont enregistrées sur la tâche ou le problème connecté.
Pour plus d’informations, voir [Utilisation de cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Application mobile {#mobile-app}

Vous pouvez consigner le temps à partir de l’application mobile Workfront.
Pour plus d’informations, voir [Adobe Workfront pour Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) ou [Adobe Workfront pour iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
