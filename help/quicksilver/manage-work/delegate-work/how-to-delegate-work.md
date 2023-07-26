---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Déléguer des tâches et problèmes
description: Vous pouvez déléguer temporairement la tâche à laquelle vous êtes affecté lorsque vous êtes absent du bureau. Cet article décrit comment déléguer des tâches et des affectations de problèmes.
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 1%

---

# Gérer la délégation des tâches et des problèmes

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Vous pouvez déléguer temporairement la tâche à laquelle vous êtes affecté lorsque vous êtes absent du bureau.

Vous pouvez déléguer des tâches et des affectations d’émission ou déléguer des approbations. Cet article décrit comment déléguer des tâches et des affectations de problèmes.

Pour obtenir des informations générales sur la délégation de travail, voir [Présentation de la délégation de travail](../../manage-work/delegate-work/delegate-work-overview.md).

## Exigences d’accès

>[!IMPORTANT]
>
>* Les utilisateurs que vous sélectionnez comme délégués reçoivent les mêmes autorisations que vos autorisations sur les tâches et problèmes que vous leur déléguez.
>* Les autorisations doivent fonctionner dans leurs niveaux d’accès, et leurs niveaux d’accès peuvent parfois être inférieurs aux vôtres.
>
>   
>   Par exemple, si un utilisateur dispose uniquement de l’accès Afficher aux tâches de son niveau d’accès et que vous disposez de l’option Gérer les autorisations sur les tâches que vous lui déléguez, il reçoit l’autorisation Gérer les autorisations pour les tâches que vous lui déléguez. Cependant, ils ne pourront pas effectuer les mêmes actions que vous sur les tâches déléguées. Ils doivent demander à l’administrateur système l’accès Modifier aux tâches pour pouvoir mettre à jour les tâches en votre absence.
>
>   
>   Pour plus d’informations sur la façon dont un peut modifier votre niveau d’accès, voir [Création ou modification de niveaux d’accès personnalisés](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Pour les éléments affectés après le démarrage de la délégation, il peut s’écouler jusqu’à une heure après l’attribution de l’élément pour [!DNL Workfront] pour partager les éléments nouvellement affectés avec le délégué.


Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Révision ou version ultérieure</p>

>[!NOTE]
>
>Bien que vous puissiez être affecté à un travail lorsque vous disposez d’une licence de demande, vous ne pouvez pas déléguer votre travail à d’autres personnes. [!DNL Workfront] ne recommande pas d’affecter du travail aux utilisateurs de la révision ou de la demande.

</tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux problèmes Si vous n’y avez toujours pas accès, demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher ou des autorisations supérieures aux tâches ou aux problèmes auxquels vous êtes affecté</p> 
    <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Conditions préalables

Avant de pouvoir exécuter les activités décrites dans cet article, vous devez vous assurer que :

* Votre [!DNL Workfront] ou l’administrateur de groupe a activé [!UICONTROL Autoriser les utilisateurs à supprimer les tâches et les problèmes liés aux heures enregistrées] dans le [!UICONTROL Configuration] de votre [!DNL Workfront] instance.

  Pour plus d’informations, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Délégation de tâches et de problèmes à un autre utilisateur

Avant de déléguer le travail à d’autres, nous vous recommandons de vous adresser à eux et de les informer qu’ils seront désignés comme délégués sur vos tâches. Demandez leur approbation verbale avant de déléguer le travail afin de vous assurer qu’ils disposent du temps nécessaire pour terminer le travail pendant que vous êtes absent du bureau.

Pour obtenir des informations générales sur la délégation des tâches et des problèmes, voir [Présentation de la délégation des tâches et des problèmes](delegate-work.md).

Pour déléguer vos tâches et problèmes à d’autres personnes :

1. Accédez au [!UICONTROL **Accueil**] , puis cliquez sur [!UICONTROL **Déléguer**] en haut de la page [!UICONTROL **Liste de tâches**].

   ![](assets/delegate-button-in-home.png)

1. Dans le [!UICONTROL **Délégation de tâches et de problèmes**] , mettez à jour les éléments suivants :

   * [!UICONTROL **Déléguez vos tâches et problèmes à**]: commencez à saisir le nom d’un utilisateur auquel vous souhaitez déléguer vos tâches et problèmes, puis sélectionnez-le lorsqu’il s’affiche dans la liste. Vous ne pouvez sélectionner qu’un seul utilisateur.\

     L’utilisateur que vous sélectionnez en tant que délégué reçoit les mêmes autorisations que vos autorisations sur les tâches et problèmes que vous lui déléguez. Pour plus d’informations, voir [Présentation de la tâche déléguée et du problème](delegate-work-overview.md).

   * [!UICONTROL **Date de début**]: sélectionnez une date dans le calendrier où doit commencer la délégation de vos tâches.

     >[!TIP]
     >
     >La date de début ne peut pas se trouver dans le passé.

   * [!UICONTROL **Aucune date de fin**]: sélectionnez cette option si vous ne souhaitez pas spécifier la date de fin pour votre délégation.

   * [!UICONTROL **Date de fin**]: sélectionnez une date du calendrier à laquelle la délégation doit s’arrêter.

     >[!TIP]
     >
     >Si vous ne sélectionnez pas de Date de fin, la délégation n’est activée que pour le jour en cours.

     ![](assets/delegate-box-expanded-in-home.png)

1. Cliquer sur [!UICONTROL **Enregistrer**].

   Les événements suivants se produisent :

   * Votre travail est délégué à l’utilisateur spécifié. Les tâches incomplètes ou les problèmes dont les dates sont comprises dans la période que vous avez sélectionnée (y compris les tâches nouvellement attribuées, une fois la délégation activée) sont délégués.

   >[!TIP]
   >
   >   Les tâches terminées qui comportent des dates dans la période de la délégation ne sont pas déléguées.


   * Vous recevez un message dans le coin supérieur droit de l’écran pour confirmer que vous avez activé la délégation de votre travail à un autre utilisateur. Le nom de l’utilisateur délégué s’affiche dans le message de confirmation.

   * Une indication indiquant que vos tâches et problèmes sont délégués à d’autres utilisateurs s’affiche dans la plupart des zones où vous pouvez voir des affectations. [!DNL Workfront]. Pour plus d’informations sur les zones qui n’incluent pas le nom des délégués, voir [Présentation de la tâche déléguée et du problème](delegate-work-overview.md).

   * La variable [!UICONTROL **Déléguer**] dans le [!UICONTROL Accueil] change de zone [!UICONTROL **Modifier la délégation**] pour indiquer qu’une délégation a été mise en place.
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Si vos notifications d’événement et vos notifications personnelles sont activées, vous recevez également une confirmation par email de votre délégation.

   * L’utilisateur que vous avez sélectionné en tant que délégué reçoit un e-mail sur la délégation, si ses notifications d’événement sont activées.

     Pour plus d’informations sur l’activation des notifications électroniques personnelles, voir [Activation ou désactivation de vos propres notifications d’événement](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).




## Modifier ou arrêter la délégation

Vous pouvez laisser une délégation expirer si vous avez sélectionné une Date de fin ou vous pouvez l’arrêter manuellement. Vous pouvez également modifier la période de la délégation, si les dates de celle-ci ont changé.

1. Accédez au [!UICONTROL Accueil] , puis cliquez sur [!UICONTROL Modifier la délégation] dans le coin supérieur droit de la liste de tâches.
1. Dans le [!UICONTROL Délégation de tâches et de problèmes] , effectuez l’une des opérations suivantes :
   * Modifiez la variable [!UICONTROL **Date de début**] ou le [!UICONTROL **Date de fin**]
   * Cliquez sur [!UICONTROL **Arrêter la délégation**]

   >[!TIP]
   >
   >    Vous ne pouvez modifier que la Date de fin d&#39;une délégation si la délégation a déjà commencé.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Conditionnel) cliquez sur [!UICONTROL **Enregistrer**] pour enregistrer les nouvelles dates de délégation

   Ou

   Cliquez sur [!UICONTROL **Arrêter la délégation**] dans la boîte de confirmation pour confirmer l’arrêt de la délégation.

   La délégation a mis à jour les dates ou elle s’est arrêtée et les utilisateurs délégués ont été supprimés de vos tâches et problèmes. Leurs autorisations pour les tâches et les problèmes restent en place.


## Recherche des informations sur les tâches déléguées et les délégués

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Lorsque des tâches et des problèmes sont délégués, il existe plusieurs domaines dans [!DNL Workfront] où vous pouvez voir le travail délégué ou qui sont les délégués.

* [Localisation des délégués dans la zone Affectations](#locate-delegates-in-the-assignments-box)
* [Localisation du travail délégué dans [!UICONTROL Accueil]](#locate-delegated-work-in-home)


### Localisation des délégués dans le [!UICONTROL Affectations] box

Lorsque votre administrateur système ou groupe active la délégation de travail dans votre système, la variable [!UICONTROL Affectations] affiche les onglets suivants partout où vous pouvez y accéder :

* [!UICONTROL **Affectations**]: les utilisateurs affectés à la tâche ou au problème s’affichent ici.
* [!UICONTROL **Délégations**]: les utilisateurs désignés comme délégués par les personnes désignées pour la tâche ou le problème s’affichent ici.

Vous pouvez accéder au [!UICONTROL Affectations] dans les zones suivantes :

* En-tête de tâche ou de problème

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

  La variable [!UICONTROL Affectations] du champ de la tâche ou de l’en-tête du problème se transforme en [!UICONTROL Affectations et délégations].

* La variable [!UICONTROL Équilibreur de charge de travail] lors de l’affectation manuelle de tâches ou de problèmes

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Vous ne pouvez pas afficher les délégués dans le [!UICONTROL Affectations] de la boîte de dialogue Modifier d’une tâche ou d’un problème.

Si une tâche ou un problème est délégué et que la variable [!UICONTROL Délégations] sous-onglet est vide, l’un des scénarios suivants peut exister :

* Vous n’êtes pas affecté à la tâche ou au problème.
* Les dates de la tâche ou du problème se situent en dehors de la période de délégation.

>[!TIP]
>
>Les heures prévues ou réelles pour les tâches et les problèmes délégués ne sont pas prises en compte dans les outils de gestion des ressources, tels que [!UICONTROL Équilibreur de charge de travail] ou le [!DNL Resource Planner] pour les utilisateurs délégués. Les heures restent associées uniquement à l’utilisateur affecté.

### Localisation du travail délégué dans [!UICONTROL Accueil]

1. Accédez au [!UICONTROL **Accueil**] , puis cliquez sur le menu déroulant de filtrage et sélectionnez une ou plusieurs des options suivantes :
   * [!UICONTROL **Délégué**]: pour afficher les tâches et les problèmes qui vous ont été délégués ou par vous.
   * [!UICONTROL **Délégué à moi**]: pour afficher les tâches et les problèmes qui vous ont été délégués par un autre utilisateur.
   * [!UICONTROL **Délégué par moi**]: pour afficher les tâches et les problèmes que vous avez délégués à d’autres utilisateurs.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Cliquez sur le bouton [!UICONTROL tri] pour trier la liste selon les critères suivants :
   * [!UICONTROL Date d’achèvement prévue]. Il s’agit de l’option de tri par défaut.
   * [!UICONTROL Date de début prévue]
   * [!UICONTROL Date d&#39;engagement]
   * [!UICONTROL Projet]
   * [!UICONTROL Ma priorité]
1. Développez les regroupements dans le [!UICONTROL **Liste de tâches**] pour afficher les tâches déléguées. Les scénarios suivants existent :
   * Pour les éléments que vous avez délégués à d’autres, le nom du délégué s’affiche dans la variable [!UICONTROL **Liste de tâches**] ainsi que la variable [!UICONTROL **Affectations et délégations**] sur la droite.

   * Pour les éléments qui vous sont délégués, le nom de la personne désignée s’affiche dans la variable [!UICONTROL **Liste de tâches**] ainsi que la variable **[!UICONTROL Affectations et délégations]** sur la droite.

   >[!TIP]
   >
   >    Si la délégation est définie pour commencer à une date postérieure à la date du jour, la date de début de la délégation s’affiche également dans la variable [!UICONTROL Liste de tâches]. Les éléments délégués s’affichent dans le regroupement que vous sélectionnez pour le [!UICONTROL Liste de tâches], en fonction du type de groupement. Si, par exemple, vous effectuez un regroupement par [!UICONTROL Date d’achèvement prévue], les éléments délégués s’affichent dans le regroupement correspondant aux dates d’achèvement prévues.
