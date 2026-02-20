---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Vue d’ensemble de la délégation de travail
description: Lorsque vous prévoyez de quitter le bureau pendant une courte période, vous pouvez temporairement déléguer votre travail à d’autres personnes afin de vous assurer que votre absence ne devienne pas un obstacle à la réalisation de vos travaux.
author: Becky
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: a5f33f914dabaa9368dea919510375bcb6ee03e2
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 90%

---

# Vue d’ensemble de la délégation de travail

Lorsque vous prévoyez de quitter le bureau pendant une courte période, vous pouvez temporairement déléguer votre travail à d’autres personnes afin de vous assurer que votre absence ne devienne pas un obstacle à la réalisation de vos travaux.

Par exemple, si certaines tâches sont attendues avant votre retour, mais que vous n’avez pas le temps de les terminer avant de partir, vous pouvez déléguer vos tâches à une autre personne afin qu’elle puisse les terminer à temps et ne pas retarder la fin du projet jusqu’à votre retour.

Vous pouvez déléguer les objets suivants dans [!DNL Adobe Workfront] :

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Tâches qui vous sont affectées.
* Problèmes qui vous sont affectés.
* Approbations de projets, tâches ou événements qui vous sont affectées.

  >[!TIP]
  >
  >   Vous ne pouvez pas déléguer l’approbation des feuilles de temps, des documents ou des épreuves.


Cet article contient des informations générales sur la délégation de tâches et les événements qui vous sont assignés.

Pour plus d&#39;informations sur la délégation des approbations de projets, de tâches et d&#39;événements, voir [Déléguer la demande d&#39;approbation](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Pour plus d’informations sur la délégation de tâches et d’événements, voir [ Déléguer des tâches et des événements](../../manage-work/delegate-work/how-to-delegate-work.md).

## Vue d’ensemble de la délégation des tâches et des problèmes

Tenez compte des points suivants lorsque vous déléguez des tâches et des problèmes :

* Votre administrateur ou administratrice [!DNL Workfront] ou de groupes doit indiquer les préférences de délégation dans la zone [!UICONTROL Configuration] avant de déléguer votre travail à d’autres personnes.

  Pour plus d’informations, consultez la section [Configurer des préférences de tâche et de problème à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Vous ne pouvez déléguer des tâches et des problèmes qu’à partir de la zone [!UICONTROL Accueil].
* Lors de la délégation de travail, des exceptions existent pour les types de licence suivants :

   * Vous pouvez déléguer du travail aux personnes réviseuses ou demandeuses, bien que [!DNL Workfront] ne le recommande pas.
   * Les personnes réviseuses peuvent déléguer du travail à d’autres personnes. Elles ne peuvent pas afficher les éléments de travail dans leur zone [!UICONTROL Accueil]. Elles ne peuvent afficher que les approbations.
   * Les personnes demandeuses ne peuvent pas déléguer du travail à d’autres personnes. Elles ne peuvent pas afficher les éléments de travail dans leur zone [!UICONTROL Accueil].
* Vous pouvez uniquement déléguer les tâches et les problèmes qui vous sont affectés. Vous ne pouvez pas déléguer des tâches et des problèmes affectés à d’autres personnes, équipes ou fonctions.
* Vous pouvez uniquement déléguer des tâches et des problèmes qui ne sont pas terminés avant la date de début de la délégation.
* Si un élément de travail se termine au cours de la période de délégation, il reste dans la zone Accueil de la personne déléguée et de la personne cessionnaire pendant 2 semaines avant sa suppression automatique par [!DNL Workfront].
* Les personnes que vous choisissez comme déléguées reçoivent les mêmes autorisations que vos autorisations sur les tâches et problèmes que vous leur déléguez. Les autorisations doivent être compatibles avec leurs niveaux d’accès, qui peuvent parfois être inférieurs aux vôtres.

>[!NOTE]
>
>  Pour les éléments affectés après le début de la délégation, il peut s’écouler jusqu’à une heure après l’affectation de l’élément pour que [!DNL Workfront] le partage avec la personne déléguée.

* Si d’autres tâches et problèmes vous sont affectés au cours de la période que vous avez sélectionnée pour que votre travail soit délégué à d’autres personnes, la nouvelle tâche affectée est automatiquement déléguée à la même personne pendant la période que vous avez sélectionnée si les dates pour la tâche ou le problème se situent dans la même période.
* Une même personne déléguée peut être choisie par plusieurs personnes différentes.
* Les tâches et problèmes délégués ne s’affichent pas dans les outils de gestion des ressources, tels que l’[!UICONTROL Équilibreur de charge de travail] ou le [!UICONTROL Planificateur de ressources] pour les personnes déléguées.
* Vous pouvez afficher les noms des tâches déléguées et des personnes déléguées dans plusieurs zones de [!DNL Workfront]. Pour plus d’informations, consultez la section « Localiser le travail délégué et déléguer les informations » de l’article [ Déléguer des tâches et des événements](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Si une personne ne dispose que d’un accès en affichage aux tâches dans son niveau d’accès et que vous disposez d’autorisations de gestion sur les tâches que vous lui déléguez, cette personne reçoit les autorisations de gestion pour les tâches que vous lui déléguez. Cependant, elle ne pourra pas effectuer les mêmes actions que vous sur les tâches déléguées.Elle devra demander à l’administration système un accès en modification aux tâches pour pouvoir mettre à jour les tâches en votre absence.

* L’arrêt de la délégation ne supprime pas les autorisations accordées aux personnes déléguées sur les tâches et problèmes qui ont fait l’objet de la délégation.
* Si l’administration système ou de groupe désactive le paramètre [!UICONTROL Autoriser les personnes à déléguer leurs tâches et problèmes] dans la zone [!UICONTROL Configuration], les personnes actuellement déléguées sont supprimées des tâches et des problèmes auxquels elles ont précédemment été déléguées. Leurs autorisations d’accès aux tâches ou aux problèmes ne sont pas supprimées.

## Différences et similitudes entre les affectations et les délégations

| Action | Affectations | Délégations |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Une personne affectée ou déléguée à un élément de travail peut modifier ou supprimer cet élément de travail. | En fonction des autorisations et du niveau d’accès | En fonction des autorisations et du niveau d’accès |
| Une personne affectée ou déléguée s’affiche dans l’en-tête de l’élément de travail. | Oui | Oui |
| Les tâches et problèmes affectés ou délégués s’affichent dans la page d’accueil de la personne cessionnaire ou déléguée. | Oui, jusqu’à ce que l’élément soit terminé. | Oui, uniquement pour la période de délégation. |
| Vous pouvez affecter ou déléguer du travail aux utilisateurs et utilisatrices à partir de la page d’accueil. | Oui | Oui |
| Vous pouvez affecter ou déléguer du travail aux utilisateurs à l’aide de l’équilibreur de charge de travail | Oui | Non |
| Vous pouvez affecter ou déléguer du travail aux utilisateurs et utilisatrices d’une liste, ou à partir de l’en-tête d’un élément de travail. | Oui | Non |
| Tout utilisateur ou toute utilisatrice peut affecter ou déléguer d’autres utilisateurs et utilisatrices à des éléments de travail qui ne leur ont pas été affectés. | En fonction des autorisations et du niveau d’accès | Non. Seule la personne cessionnaire peut déléguer ses propres éléments. |
| Les heures prévues, effectives ou budgétées pour le travail affecté ou délégué à un utilisateur ou à une utilisatrice s’affichent pour cette personne dans les outils de gestion des ressources. | Oui | Non |
