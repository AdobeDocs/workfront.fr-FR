---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Déléguer des tâches et problèmes
description: Vous pouvez déléguer temporairement le travail qui vous est confié pendant que vous n’êtes pas au bureau. Cet article décrit comment déléguer des affectations de tâches et de problèmes.
author: Lisa
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '1460'
ht-degree: 100%

---

# Gérer la délégation des tâches et des problèmes

<!-- Audited: 1/2024 -->


<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote this as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Vous pouvez déléguer temporairement le travail qui vous est confié pendant que vous n’êtes pas au bureau.

Vous pouvez déléguer des affectations de tâches et de problèmes ou des approbations. Cet article décrit comment déléguer des affectations de tâches et de problèmes.

Pour obtenir des informations générales sur la délégation de travail, voir [Vue d’ensemble de la délégation de travail](../../manage-work/delegate-work/delegate-work-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

>[!IMPORTANT]
>
>* Les personnes que vous choisissez comme déléguées reçoivent les mêmes autorisations que vos autorisations sur les tâches et problèmes que vous leur déléguez.
>* Les autorisations doivent être compatibles avec leurs niveaux d’accès, qui peuvent parfois être inférieurs aux vôtres.
>
>   
>   Par exemple, si une personne ne dispose que d’un accès en affichage aux tâches dans son niveau d’accès et que vous disposez d’autorisations de gestion sur les tâches que vous lui déléguez, cette personne reçoit les autorisations de gestion pour les tâches que vous lui déléguez. Cependant, elle ne pourra pas effectuer les mêmes actions que vous sur les tâches déléguées.Pour pouvoir mettre à jour les tâches en votre absence, elle doit demander à l’administrateur ou l’administratrice système l’accès en modification aux tâches.
>
>   
>   Pour plus d’informations sur la façon dont un administrateur ou une administratrice système peut modifier votre niveau d’accès, voir [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Pour les éléments affectés après le début de la délégation, il peut s’écouler jusqu’à une heure après l’affectation de l’élément pour que [!DNL Workfront] le partage avec la personne déléguée.


Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : contributeur ou contributrice ou supérieure</p><p>Ou</p><p>Actuel : révision ou supérieur</p>

>[!NOTE]
>
>Bien que vous puissiez être affecté à un travail lorsque vous disposez d’une licence de demande, vous ne pouvez pas déléguer votre travail à d’autres personnes. [!DNL Workfront] ne recommande pas d’affecter du travail aux personnes réviseuses, demandeuses ou contributrices.

</tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès en modification aux tâches et problèmes 
     </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures aux tâches ou aux problèmes auxquels vous êtes affecté</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Conditions préalables

Avant de pouvoir effectuer les activités décrites dans cet article, vous devez vous assurer des points suivants :

* Votre administrateur ou administratrice [!DNL Workfront] ou administrateur ou administratrice de groupes a activé le paramètre [!UICONTROL Autoriser les utilisateurs à supprimer les tâches et les événements comportant des heures consignées] dans la zone [!UICONTROL Configuration] de votre instance [!DNL Workfront].

  Pour plus d’informations, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Déléguer des tâches et des problèmes à une autre personne

Avant de déléguer du travail à d’autres personnes, nous vous recommandons de les contacter et de les informer qu’elles seront désignées comme personnes déléguées sur vos éléments de travail. Demandez leur approbation verbale avant de déléguer du travail afin de vous assurer qu’elles disposent du temps nécessaire pour terminer le travail pendant que vous n’êtes pas au bureau.

Pour obtenir des informations générales sur la délégation de tâches et de problèmes, voir [Vue d’ensemble de la délégation de tâches et de problèmes](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

Pour déléguer vos tâches et problèmes à d’autres personnes :

1. Accédez à la zone [!UICONTROL **Accueil**], puis cliquez sur [!UICONTROL **Déléguer**] en haut de la [!UICONTROL **Liste de travail**].

   ![](assets/delegate-button-in-home.png)

1. Dans l’onglet [!UICONTROL **Déléguer des tâches et des problèmes**], mettez à jour les informations suivantes :

   * [!UICONTROL **Déléguer vos tâches et problèmes à : commencez à saisir le nom d’un utilisateur ou d’une utilisatrice auquel vous souhaitez déléguer vos tâches et problèmes, puis sélectionnez-le lorsqu’il s’affiche dans la liste.**] Vous ne pouvez sélectionner qu’un seul utilisateur ou qu’une seule utilisatrice.

     La personne que vous choisissez comme déléguée reçoivent les mêmes autorisations que vos autorisations sur les tâches et problèmes que vous lui déléguez.

   * [!UICONTROL **Date de début**] : sélectionnez une date dans le calendrier à laquelle la délégation de vos éléments de travail doit commencer.

     >[!TIP]
     >
     >La date de début ne peut pas être dans le passé.

   * [!UICONTROL **Pas de date de fin**] : sélectionnez cette option si vous ne souhaitez pas spécifier la date de fin de votre délégation.

   * [!UICONTROL **Date de fin**] : sélectionnez une date dans le calendrier à laquelle la délégation doit s’arrêter.

     >[!TIP]
     >
     >Si vous laissez le champ Date de fin vide et que l’option Pas de date de fin n’est pas sélectionnée, la délégation n’est définie que pour le jour en cours.

     ![](assets/delegate-box-expanded-in-home.png)

1. Cliquer sur [!UICONTROL **Enregistrer**].

   Les événements suivants surviennent :

   * Votre travail est délégué à l’utilisateur ou l’utilisatrice spécifié. Les tâches ou les problèmes non terminés dont les dates sont comprises dans la période que vous avez sélectionnée (y compris les tâches nouvellement affectées après l’activation de la délégation) sont délégués.

     >[!TIP]
     >
     >   Les éléments de travail terminés dont les dates sont comprises dans la période de la délégation ne sont pas délégués.


   * Un message s’affiche dans le coin supérieur droit de l’écran pour confirmer que vous avez activé la délégation de votre travail à une autre personne.Le nom de la personne déléguée s’affiche dans le message de confirmation.

   * Un message indiquant que vos tâches et problèmes sont délégués à d’autres personne s’affiche dans la plupart des zones où vous pouvez voir des affectations dans . [!DNL Workfront] Pour plus d’informations sur les zones qui n’incluent pas le nom des personnes délégués, voir [Vue d’ensemble de la délégation de travail](delegate-work-overview.md).

   * Le bouton [!UICONTROL **Déléguer**] dans la zone [!UICONTROL Accueil] devient [!UICONTROL **Modifier la délégation**] pour indiquer qu’une délégation a été mise en place.
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Si vos notifications d’événement et vos notifications personnelles sont activées, vous recevez également une confirmation par e-mail de votre délégation.

   * L’utilisateur ou l’utilisatrice que vous avez sélectionné en tant que personne déléguée reçoit un e-mail sur la délégation, si ses notifications d’événement sont activées.

     Pour plus d’informations sur l’activation des notifications personnelles par e-mail, voir [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Modifier ou arrêter la délégation

Vous pouvez laisser une délégation expirer si vous avez sélectionné une date de fin ou vous pouvez l’arrêter manuellement. Vous pouvez également modifier la période de la délégation si ses dates ont changé.

1. Accédez à la zone [!UICONTROL Accueil], puis cliquez sur [!UICONTROL Modifier la délégation] dans le coin supérieur droit de la liste de travail.
1. Dans l’onglet [!UICONTROL Déléguer des tâches et des problèmes], effectuez l’une des opérations suivantes :
   * Modifiez la [!UICONTROL **Date de début**] ou la [!UICONTROL **Date de fin**].
   * Cliquez sur [!UICONTROL **Arrêter la délégation**].

   >[!TIP]
   >
   >    Vous ne pouvez modifier la date de fin d’une délégation que si la délégation a déjà commencé.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Le cas échéant) Cliquez sur [!UICONTROL **Enregistrer**] pour enregistrer les nouvelles dates de délégation.

   Ou

   Cliquez sur [!UICONTROL **Arrêter la délégation**] dans la boîte de confirmation pour confirmer l’arrêt de la délégation.

   La délégation a mis à jour les dates ou elle s’est arrêtée et les personnes déléguées ont été supprimées de vos tâches et problèmes. Leurs autorisations sur les tâches et les problèmes restent en place.


## Rechercher des informations sur le travail délégué et les personnes déléguées

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Lorsque des tâches et des problèmes sont délégués, il existe plusieurs zones dans [!DNL Workfront] où vous pouvez voir le travail délégué ou qui sont les personnes déléguées.

* [Rechercher des personnes déléguées dans la zone Affectations](#locate-delegates-in-the-assignments-box)
* [Rechercher du travail délégué dans [!UICONTROL Accueil]](#locate-delegated-work-in-home)


### Rechercher des personnes déléguées dans la zone [!UICONTROL Affectations]

Lorsque votre administrateur ou administratrice système ou administrateur ou administratrice de groupes active la délégation de travail dans votre système, la zone [!UICONTROL Affectations] affiche les onglets suivants partout où vous pouvez y accéder :

* [!UICONTROL **Affectations**] : les personnes affectées à la tâche ou au problème s’affichent ici.
* [!UICONTROL **Délégations**] : les utilisateurs et utilisatrices désignées comme délégués par les personnes cessionnaires sur la tâche ou le problème s’affichent ici.

Vous pouvez accéder à la zone [!UICONTROL Affectations] dans les zones suivantes :

* L’en-tête de tâche ou de problème.

  Le champ [!UICONTROL Affectations] dans l’en-tête de tâche ou de problème devient [!UICONTROL Affectations et délégations].

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

* L’[!UICONTROL Équilibreur de charge de travail] lors de l’affectation manuelle de tâches ou de problèmes.

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Vous ne pouvez pas afficher les personnes déléguées dans la section [!UICONTROL Affectations] de la zone Modifier d’une tâche ou d’un problème.

Si une tâche ou un problème est délégué et que le sous-onglet [!UICONTROL Délégations] est vide, l’un des scénarios suivants peut exister :

* Vous n’êtes pas affecté à la tâche ou au problème.
* Les dates de la tâche ou du problème se trouvent en dehors de la période de délégation.

>[!TIP]
>
>Les heures prévues ou effectives des tâches et des problèmes délégués ne sont pas prises en compte dans les outils de gestion des ressources, tels que Équilibreur de charge de travail ou le  pour les personnes déléguées. [!DNL Resource Planner] Les heures restent associées à l’utilisateur ou l’utilisatrice affecté uniquement.

### Rechercher du travail délégué dans [!UICONTROL Accueil]

1. Accédez à la zone [!UICONTROL **Accueil**], puis cliquez sur le menu déroulant de filtre et sélectionnez une ou plusieurs des options suivantes :
   * [!UICONTROL **Délégué**] : pour afficher les tâches et les problèmes qui vous ont été délégués ou que vous avez délégués.
   * [!UICONTROL **M’a été délégué**] : pour afficher les tâches et les problèmes qui vous ont été délégués par une autre personne.
   * [!UICONTROL **Délégué par moi-même**] : pour afficher les tâches et les problèmes que vous avez délégués à d’autres personnes.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Cliquez sur le menu déroulant de [!UICONTROL tri] pour trier la liste selon les critères suivants :
   * [!UICONTROL Achèvement prévu. ] Il s’agit de l’option de tri par défaut.
   * [!UICONTROL Début prévu]
   * [!UICONTROL Date d’engagement]
   * [!UICONTROL Projet]
   * [!UICONTROL Ma priorité]
1. Développez les regroupements dans la [!UICONTROL **Liste de travail**] pour afficher les éléments de travail délégués. Les scénarios suivants sont possibles :
   * Pour les éléments que vous avez délégués à d’autres personnes, le nom de la personne déléguée s’affiche dans la [!UICONTROL **Liste de travail**] ainsi que le champ [!UICONTROL **Affectations et délégations**] à droite.

   * Pour les éléments qui vous sont délégués, le nom de la personne cessionnaire s’affiche dans la [!UICONTROL **Liste de travail**] ainsi que le champ **[!UICONTROL Affectations et délégations]** à droite.

   >[!TIP]
   >
   >    Si la délégation est définie pour commencer à une date postérieure à la date du jour, la date de début de la délégation s’affiche également dans la Liste de travail.  Les éléments délégués s’affichent dans le regroupement que vous sélectionnez pour la Liste de travail en fonction du type du regroupement.  Par exemple, si vous regroupez par [!UICONTROL Date d’achèvement prévue], les éléments délégués s’affichent dans le regroupement correspondant à leurs dates d’achèvement prévues.
