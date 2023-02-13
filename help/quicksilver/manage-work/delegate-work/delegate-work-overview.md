---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Présentation de la délégation de travail
description: Lorsque vous prévoyez de quitter le bureau pendant une courte période, vous pouvez temporairement déléguer votre travail à d’autres utilisateurs afin de vous assurer que votre absence ne devienne pas un obstacle à la réalisation de vos travaux.
author: Alina
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: f3ae487f53f7c4f8c389cf0d35323f21e76ece35
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 1%

---

# Présentation de la délégation de travail

Lorsque vous prévoyez de quitter le bureau pendant une courte période, vous pouvez temporairement déléguer votre travail à d’autres utilisateurs afin de vous assurer que votre absence ne devienne pas un obstacle à la réalisation de vos travaux.

Par exemple, si certaines tâches sont attendues avant votre retour, mais que vous n’avez pas le temps de les terminer avant de partir, vous pouvez déléguer vos tâches à un autre utilisateur afin qu’il puisse les terminer à temps et ne pas retarder la fin du projet jusqu’à votre retour.

Vous pouvez déléguer les objets suivants dans [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Tâches qui vous sont assignées
* Problèmes qui vous sont affectés
* Projet, tâche, problème, validations de document qui vous ont été attribuées.

Cet article contient des informations générales sur la délégation des tâches et des problèmes.

Pour plus d’informations sur la délégation des approbations de projet, de tâche, de problème et de document, voir [Déléguer la demande d’approbation](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Pour plus d’informations sur la manière de déléguer des tâches et des problèmes, voir [Délégation de tâches et de problèmes](../../manage-work/delegate-work/how-to-delegate-work.md).

## Présentation de la délégation de travail

Tenez compte des points suivants lorsque vous déléguez des tâches et des problèmes :

* Votre [!DNL Workfront] ou l’administrateur de groupe doit activer les préférences de délégation dans la [!UICONTROL Configuration] avant de déléguer votre travail à d’autres personnes.

   Pour plus d’informations, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Vous ne pouvez déléguer des tâches et des problèmes qu’à partir du [!UICONTROL Accueil] zone.
* Des exceptions existent pour les types de licence suivants :

   * Vous pouvez déléguer du travail aux réviseurs ou aux demandeurs, bien que [!DNL Workfront] ne le recommande pas.
   * Les réviseurs peuvent déléguer du travail à d’autres personnes. Ils ne peuvent pas afficher les tâches dans leur [!UICONTROL Accueil] zone. Ils ne peuvent afficher que les approbations.
   * Les demandeurs ne peuvent pas déléguer du travail à d’autres personnes. Ils ne peuvent pas afficher les tâches dans leur [!UICONTROL Accueil] area
* Vous pouvez uniquement déléguer les tâches et les problèmes qui vous sont affectés. Vous ne pouvez pas déléguer des tâches et des problèmes affectés à d’autres utilisateurs, équipes ou rôles de tâche.
* Vous pouvez uniquement déléguer des tâches et des problèmes qui ne sont pas terminés avant la date de début de la délégation.
* Si un élément de travail se termine au cours de la période de délégation, il reste dans la zone Accueil du délégué et de la personne désignée pendant 2 semaines avant [!DNL Workfront] le supprime automatiquement.
* Les utilisateurs que vous sélectionnez comme délégués reçoivent les mêmes autorisations que vos autorisations sur les tâches et problèmes que vous leur déléguez. Les autorisations doivent fonctionner dans leurs niveaux d’accès, et leurs niveaux d’accès peuvent parfois être inférieurs aux vôtres.

>[!NOTE]
>
>  Pour les éléments affectés après le démarrage de la délégation, il peut s’écouler jusqu’à une heure après l’attribution de l’élément pour [!DNL Workfront] pour partager les éléments nouvellement affectés avec le délégué.

* Si d’autres tâches et problèmes vous sont assignés au cours de la période que vous avez sélectionnée pour que votre travail soit délégué à d’autres utilisateurs, la nouvelle tâche affectée est automatiquement déléguée à la même personne pendant la période que vous avez sélectionnée si la tâche ou les dates d’émission se trouvent dans cette période.
* Un même utilisateur peut être sélectionné en tant que délégué par plusieurs utilisateurs.
* Les tâches et problèmes délégués ne s’affichent pas dans les outils de gestion des ressources, tels que le [!UICONTROL Équilibreur de charge de travail] ou le [!UICONTROL Resource Planner] pour les utilisateurs délégués.
* Vous pouvez afficher les noms des tâches déléguées et des délégués dans plusieurs zones [!DNL Workfront]. Pour plus d’informations, voir la section &quot;Localisation du travail délégué et informations sur les délégués&quot; dans l’article . [Gérer la délégation des tâches et des problèmes](../delegate-work/how-to-delegate-work.md).


   >[!IMPORTANT]
   >
   >  Si un utilisateur ne dispose que de l’accès Afficher aux tâches de son niveau d’accès et que vous disposez des autorisations Gérer sur les tâches que vous lui déléguez, il reçoit les autorisations Gérer pour les tâches que vous lui déléguez. Cependant, ils ne pourront pas effectuer les mêmes actions que vous sur les tâches déléguées. Ils doivent demander à l’administrateur système l’accès Modifier aux tâches pour pouvoir mettre à jour les tâches en votre absence.

* L’arrêt de la délégation ne supprime pas les autorisations accordées aux utilisateurs délégués sur les tâches et problèmes sur lesquels ils ont été délégués.
* Si un système ou désactive la fonction [!UICONTROL Autoriser les utilisateurs à déléguer leurs tâches et problèmes] dans le [!UICONTROL Configuration] , les utilisateurs actuellement délégués sont supprimés des tâches et des problèmes auxquels ils ont précédemment été délégués. Leurs autorisations d’accès aux tâches ou aux problèmes ne sont pas supprimées.

## Différences et similitudes entre les affectations et les délégations

| Action | Affectations | Délégations |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Un utilisateur affecté ou délégué peut modifier ou supprimer l’élément de travail auquel il est affecté ou délégué. | En fonction des autorisations et du niveau d’accès | En fonction des autorisations et du niveau d’accès |
| Un utilisateur affecté ou délégué s’affiche dans l’en-tête de l’élément de travail. | Oui | Oui |
| Les tâches ou problèmes affectés ou délégués s’affichent dans la zone d’accueil de la personne désignée ou du délégué. | Oui, jusqu’à ce que l’élément soit terminé | Oui, uniquement pour la période de la délégation |
| Vous pouvez affecter ou déléguer du travail aux utilisateurs de la zone d’accueil. | Oui | Oui |
| Vous pouvez affecter ou déléguer du travail aux utilisateurs à l’aide de la fonction | Oui | Non |
| Vous pouvez affecter ou déléguer du travail aux utilisateurs d’une liste, ou à partir de l’en-tête d’une tâche | Oui | Non |
| Tout utilisateur peut affecter ou déléguer d’autres utilisateurs à des tâches auxquelles il n’est pas associé. | En fonction des autorisations et du niveau d’accès | Non. Seul le cessionnaire peut déléguer ses propres éléments. |
| Heures planifiées, réelles ou budgétées pour le travail assigné ou délégué à un utilisateur s’affiche pour cet utilisateur dans les outils de gestion des ressources. | Oui | Non |
