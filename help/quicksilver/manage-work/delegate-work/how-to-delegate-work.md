---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Déléguer des tâches et problèmes
description: Vous pouvez déléguer temporairement le travail qui vous est confié pendant que vous n’êtes pas au bureau. Cet article décrit comment déléguer des attributions de tâches et de problèmes.
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


Vous pouvez déléguer l’affectation des tâches et des problèmes, ou déléguer les approbations. Cet article décrit comment déléguer des attributions de tâches et de problèmes.

Pour des informations générales sur la délégation du travail, voir [Vue d’ensemble de la délégation du travail](../../manage-work/delegate-work/delegate-work-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

>[!IMPORTANT]
>
>* Les personnes que vous choisissez comme déléguées reçoivent les mêmes autorisations que vos autorisations sur les tâches et problèmes que vous leur déléguez.
>* Les autorisations doivent être compatibles avec leurs niveaux d’accès, qui peuvent parfois être inférieurs aux vôtres.
>
>   
>   Par exemple, si un utilisateur ou une utilisatrice n’a qu’un accès en affichage aux tâches de son niveau d’accès et que vous avez des autorisations en gestion sur les tâches que vous lui déléguez, des autorisations de gestion lui sont accordées pour les tâches que vous lui déléguez. Cependant, elle ne pourra pas effectuer les mêmes actions que vous sur les tâches déléguées.Pour pouvoir mettre à jour les tâches en votre absence, l’administrateur ou administratrice système doit leur accorder l’accès en modification pour les tâches.
>
>   
>   Pour savoir comment un administrateur ou une administratrice système peut modifier votre niveau d’accès, voir [Créer ou modifier des niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Pour les éléments attribués après le début de la délégation, il peut s’écouler jusqu’à une heure après l’attribution de l’élément pour que [!DNL Workfront] partage les éléments nouvellement attribués avec la personne déléguée.


Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : contributeur ou supérieure</p><p>Ou</p><p>Actuel : Révision ou supérieur</p>

>[!NOTE]
>
>Bien que du travail peut vous être attribué lorsque vous avez une licence de demande, vous ne pouvez pas déléguer votre travail à d’autres personnes. [!DNL Workfront] ne recommande pas d’affecter du travail aux utilisateurs et utilisatrices des catégories Révision, Demande ou Contribution.

</tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux tâches et aux problèmes 
     </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations en affichage ou supérieures pour les tâches ou les problèmes qui vous sont affectés</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Conditions préalables

Avant de pouvoir effectuer les activités décrites dans cet article, vous devez vous assurer des points suivants :

* Votre administrateur ou administratrice de groupes ou [!DNL Workfront] a activé le paramètre [!UICONTROL Autoriser les utilisateurs et utilisatrices à supprimer les tâches et les problèmes comportant des heures consignées] dans la zone [!UICONTROL Configuration] de votre instance [!DNL Workfront].

  Pour plus d’informations, voir [Configurer les préférences en matière de tâches et de problèmes à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Déléguer des tâches et des problèmes à un autre utilisateur ou utilisatrice

Avant de déléguer du travail à d’autres personnes, nous vous recommandons de les contacter et de les informer qu’elles seront désignées comme déléguées pour vos éléments de travail. Demandez leur approbation verbale avant de déléguer du travail afin de vous assurer qu’elles disposent du temps nécessaire pour terminer le travail en votre absence.

Pour des informations générales sur la délégation de tâches et de problèmes, voir [Vue d’ensemble de la délégation de tâches et de problèmes](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

Pour déléguer vos tâches et problèmes à d’autres personnes :

1. Accédez à la zone [!UICONTROL **Accueil**], puis cliquez sur [!UICONTROL **Déléguer**] en haut de la [!UICONTROL **liste de travail**].

   ![](assets/delegate-button-in-home.png)

1. Dans l’onglet [!UICONTROL **Déléguer des tâches et problèmes**], mettez à jour les éléments suivants :

   * [!UICONTROL **Déléguer vos tâches et problèmes à**] : commencez à saisir le nom de la personne à laquelle vous souhaitez déléguer vos tâches et problèmes, puis sélectionnez-la lorsqu’elle s’affiche dans la liste. Vous ne pouvez sélectionner qu’une seule personne.

     La personne que vous sélectionnez comme déléguée reçoit les mêmes autorisations que les vôtres pour les tâches et les problèmes que vous lui déléguez.

   * [!UICONTROL **Date de début**] : sélectionnez une date dans le calendrier à laquelle la délégation de vos éléments de travail doit commencer.

     >[!TIP]
     >
     >La date de début ne peut pas être antérieure.

   * [!UICONTROL **Pas de date de fin**] : sélectionnez cette option si vous ne souhaitez pas indiquez la date de fin de votre délégation.

   * [!UICONTROL **Date de fin**] : sélectionnez une date dans le calendrier à laquelle la délégation doit prendre fin.

     >[!TIP]
     >
     >Si le champ Date de fin est vide et que l’option Pas de date de fin n’est pas sélectionnée, la délégation n’est fixée que pour le jour en cours.

     ![](assets/delegate-box-expanded-in-home.png)

1. Cliquer sur [!UICONTROL **Enregistrer**].

   Les événements suivants se produisent :

   * Votre travail est délégué à la personne spécifiée. Les tâches et problèmes incomplets dont la date se situe dans le délai que vous avez sélectionné (y compris ceux attribués récemment, après l’activation de la délégation) sont délégués.

     >[!TIP]
     >
     >   Les éléments de travail achevés dont la date se situe dans la période de délégation ne sont pas délégués.


   * Vous recevez un message dans le coin supérieur droit de l’écran pour confirmer que vous avez activé la délégation de votre travail à une autre personne.Le nom de la personne déléguée s’affiche dans le message de confirmation.

   * Une indication selon lequel vos tâches et problèmes sont délégués à d’autres personnes s’affiche dans la plupart des zones où vous pouvez voir les affectations dans [!DNL Workfront]. Pour plus d’informations sur les domaines dans lesquels les noms des personnes déléguées ne figurent pas, voir [Vue d’ensemble de la délégation de travail](delegate-work-overview.md).

   * Le bouton [!UICONTROL **Déléguer**] dans la zone [!UICONTROL Accueil] devient [!UICONTROL **Modifier la délégation**] pour indiquer qu’une délégation est en place.
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Si vos notifications de l’événement et vos notifications personnelles sont activées, vous recevez également un e-mail de confirmation de votre délégation.

   * La personne que vous avez sélectionnée comme déléguée reçoit un e-mail concernant la délégation, si ses notifications d’événements sont activées.

     Pour plus d’informations sur l’activation des notifications personnelles par e-mail, voir [Modifier vos propres notifications par e-mail](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Modifier ou arrêter la délégation

Vous pouvez laisser une délégation expirer si vous avez sélectionné une date de fin, ou bien l’arrêter manuellement. Vous pouvez également modifier la durée de la délégation, si ses dates ont changé.

1. Allez dans la zone [!UICONTROL Accueil], puis cliquez sur [!UICONTROL Modifier la délégation] dans le coin supérieur droit de la liste de travail.
1. Dans l’onglet [!UICONTROL Déléguer des tâches et problèmes], effectuez l’une des opérations suivantes :
   * Modifiez la [!UICONTROL **date de début**] ou la [!UICONTROL **date de fin**].
   * Cliquez sur [!UICONTROL **Arrêter la délégation**].

   >[!TIP]
   >
   >    Vous ne pouvez modifier que la date de fin d’une délégation si celle-ci a déjà commencé.

   ![](assets/stop-delegation-screen-in-home.png)

1. (conditionnel) Cliquez sur [!UICONTROL **Enregistrer**] pour enregistrer les nouvelles dates de délégation.

   Ou

   Cliquez sur [!UICONTROL **Arrêter la délégation**] dans la boîte de confirmation pour confirmer l’arrêt de la délégation.

   La délégation a soit mis à jour les dates, soit cessé. Les personnes déléguées ont été supprimées de vos tâches et problèmes. Leurs autorisations pour les tâches et les problèmes restent en place.


## Localiser le travail délégué et les informations sur les personnes déléguées

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Lorsque des tâches et des problèmes sont délégués, plusieurs zones de [!DNL Workfront] vous permettent de voir le travail délégué ou l’identité des personnes déléguées.

* [Localiser les personnes déléguées dans la boîte Affectations](#locate-delegates-in-the-assignments-box)
* [Localiser le travail délégué sur la page d’[!UICONTROL accueil]](#locate-delegated-work-in-home)


### Localiser les personnes déléguées dans la boîte [!UICONTROL Affectations] 

Lorsque votre administrateur ou administratrice système ou de groupe active la délégation de travaux dans votre système, la boîte [!UICONTROL Affectations] affiche les onglets suivants partout où vous pouvez y accéder :

* [!UICONTROL **Affectations**] : les personnes affectées à la tâche ou au problème s’affichent ici.
* [!UICONTROL **Délégations**] : les personnes désignées comme déléguées par les destinataires de la tâche ou de la question s’affichent ici.

Vous pouvez accéder à la boîte [!UICONTROL Affectations] dans les zones suivantes :

* L’en-tête de la tâche ou du problème

  Le champ [!UICONTROL Affectations] dans l’en-tête de la tâche ou du problème devient [!UICONTROL Affectations et délégations].

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

* L’[!UICONTROL Équilbreur de charge de travail] lors de l’attribution manuelle des tâches ou des problèmes.

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Vous ne pouvez pas voir les personnes déléguées dans la section [!UICONTROL Affectations] de la boîte d’édition d’une tâche ou d’un problème.

Si une tâche ou un problème est délégué et que le sous-onglet [!UICONTROL Délégations] est vide, l’un des scénarios suivants peut se produire :

* La tâche ou le problème ne vous est pas affecté.
* Les dates de la tâche ou du problème sont en dehors de la période de délégation.

>[!TIP]
>
>Les heures prévues ou effectives pour les tâches et les problèmes délégués ne sont pas prises en compte dans les outils de gestion des ressources, tels que l’[!UICONTROL Équilbreur de charge de travail] ou le [!DNL Resource Planner] pour les personnes déléguées. Les heures restent associées uniquement à la personne affectée.

### Localiser le travail délégué sur la page d’[!UICONTROL accueil]

1. Allez dans la zone d’[!UICONTROL **accueil**], puis cliquez sur le menu déroulant du filtre et sélectionnez une ou plusieurs des options suivantes :
   * [!UICONTROL **Délégué**] : pour visualiser les tâches et les problèmes qui vous ont été délégués ou qui ont été déléguées par vous.
   * [!UICONTROL **M’a été délégué**] : pour visualiser les tâches et les problèmes qui vous ont été délégués par une autre personne.
   * [!UICONTROL **Délégué par moi-même**] : pour visualiser les tâches et les problèmes que vous avez délégués à d’autres personnes.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Cliquez sur le menu déroulant de [!UICONTROL tri] pour trier la liste selon les critères suivants :
   * [!UICONTROL Date d’achèvement prévue]. Il s’agit de l’option de tri par défaut.
   * [!UICONTROL Date de début prévue]
   * [!UICONTROL Date d’engagement]
   * [!UICONTROL Projet]
   * [!UICONTROL Ma priorité]
1. Développez les regroupements dans la [!UICONTROL **liste de travail**] pour afficher les éléments de travail délégués. Les scénarios suivants sont possibles :
   * Pour les éléments que vous avez délégués à d’autres personnes, le nom de la personne déléguée s’affiche dans la [!UICONTROL **liste de travail**] ainsi que dans le champ [!UICONTROL **Affectations et délégations**] à droite.

   * Pour les éléments qui vous sont délégués, le nom de la personne cessionnaire s’affiche dans la [!UICONTROL **liste de travail**] ainsi que dans le champ **[!UICONTROL Affectations et délégations]** à droite.

   >[!TIP]
   >
   >    Si la délégation doit commencer à une date postérieure à celle d’aujourd’hui, la date de début de la délégation s’affiche également dans la [!UICONTROL liste de travail]. Les éléments délégués s’affichent dans le regroupement que vous avez sélectionné pour la [!UICONTROL liste de travail], en fonction du type de regroupement. Par exemple, si vous effectuez un regroupement par [!UICONTROL Date d’achèvement prévue], les éléments délégués s’affichent dans le regroupement qui correspond à leur date d’achèvement prévue.
