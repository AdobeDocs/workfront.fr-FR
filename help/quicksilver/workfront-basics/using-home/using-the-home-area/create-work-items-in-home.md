---
product-area: projects
navigation-topic: use-the-home-area
title: Créer des éléments de travail à partir de la zone Accueil
description: Vous pouvez créer des éléments de travail à partir de la zone [!UICONTROL Accueil]. Vous pouvez créer des tâches personnelles pour vous-même, demander du travail à d’autres utilisateurs et utilisatrices ou ajouter des tâches à des projets spécifiques.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 100%

---

# Créer des éléments de travail à partir de la zone Accueil

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

Vous pouvez créer des éléments de travail à partir de la zone [!UICONTROL Accueil]. Vous pouvez créer des tâches personnelles pour vous-même, demander du travail à d’autres utilisateurs et utilisatrices ou ajouter des tâches à des projets spécifiques.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Worker]</p> <p><b>NOTE</b></p> 
   <p>Si vous ne disposez toujours pas d’un accès, demandez à votre équipe d’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires pour votre niveau d’accès. Pour plus d’informations sur la manière dont un un administrateur ou une administratrice de [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Accès [!UICONTROL Edit] ou supérieur aux tâches</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Créer une tâche personnelle

Vous pouvez créer une tâche personnelle qui n’est accessible que par vous dans la zone [!UICONTROL Accueil] :

1. Cliquez sur le **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Cliquez sur **[!UICONTROL Nouvelle tâche]** > **[!UICONTROL Personnelle]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. Dans le champ **[!UICONTROL Nom]**, saisissez le nom de la tâche.
1. (Facultatif) Cliquez sur **[!UICONTROL Sélectionner la date]**, puis sélectionnez la date d’échéance de la tâche. Cette option définit la [!UICONTROL Date d’achèvement prévue] pour la tâche.\
   Vous pouvez modifier la **[!UICONTROL Date d’achèvement prévue]** en cliquant sur la date dans le panneau de droite ou en modifiant la date **[!UICONTROL La tâche sera terminée d’ici le...]** directement dans la tâche.

1. Cliquez sur **[!UICONTROL Créer]** pour enregistrer la tâche.\
   La tâche vous est affectée et est disponible dans la zone [!UICONTROL Accueil].

>[!NOTE]
>
>* Lorsque vous créez une tâche personnelle, elle est stockée dans un projet « caché » qui n’est pas consultable dans [!UICONTROL Workfront]. Le projet est nommé « Tâches de &lt; User Name > ». Le « User Name » est le nom complet de l’utilisateur ou de l’utilisatrice qui a créé la tâche. Vous ne pouvez accéder à ce projet que lorsque vous cliquez sur la tâche personnelle dans la zone [!UICONTROL Accueil], à partir du chemin de navigation de la tâche, par exemple.
>
>* Contrairement aux tâches de projet ordinaires, les tâches personnelles ont un ensemble limité de champs visibles dans l’interface de Workfront et n’influencent pas le calendrier ou l’avancement d’un projet. La réaffectation d’une tâche personnelle à un autre utilisateur ou à une autre utilisatrice ajoute tous les champs de la tâche à une tâche personnelle, mais la tâche reste dans le projet personnel de l’utilisateur ou de l’utilisatrice qui l’a créée.
>
>
>* Les tâches personnelles ne s’affichent sur les feuilles de temps que lorsqu’elles ont des heures consignées ou qu’elles sont épinglées à la feuille de temps. Vous ne pouvez épingler une tâche personnelle à une feuille de temps que si des heures ont été consignées pour cette tâche. Pour plus d’informations, voir [Consigner le temps](../../../timesheets/create-and-manage-timesheets/log-time.md).
> 
>* Nous vous conseillons de créer un projet et d’y déplacer toutes vos tâches personnelles, si vous souhaitez que les tâches personnelles fassent partie du workflow normal.
>
> ![[!UICONTROL Projet pour des tâches personnelles]](assets/createworkitems-personal--project-350x105.png)

## Demander du travail à un autre utilisateur ou à une autre utilisatrice

Vous pouvez demander du travail à un autre utilisateur ou à une autre utilisatrice directement à partir de la zone Accueil. Lorsque vous demandez du travail à un autre utilisateur ou à une autre utilisatrice comme décrit dans cette section, la tâche est affichée comme une demande dans la zone Accueil de la personne jusqu’à ce que celle-ci clique sur **[!UICONTROL Travailler sur cette tâche]**.

Pour demander du travail à un autre utilisateur ou à une autre utilisatrice à partir de la zone [!UICONTROL Accueil], procédez comme suit :

1. Cliquez sur le **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. Cliquez sur **[!UICONTROL Nouvelle tâche]**, puis sélectionnez **[!UICONTROL Demande]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. Dans le champ **[!UICONTROL Nom]**, saisissez le nom de la tâche.
1. Dans le champ **[!UICONTROL Affecter à]**, commencez à saisir le nom de l’utilisateur, de l’utilisatrice, de l’équipe ou du rôle que vous voulez affecter, puis cliquez sur le nom lorsqu’il apparaît dans le menu déroulant.
1. Dans le menu déroulant [!UICONTROL Ajouter en tant que], choisissez d’ajouter soit une tâche soit un problème.
1. Cliquez sur **[!UICONTROL Sélectionner une date]**, puis sélectionnez la date et l’heure d’échéance de la tâche.
1. Cliquez sur **[!UICONTROL Créer]** pour enregistrer la tâche.\
   La tâche est affichée en tant que demande de travail dans la zone [!UICONTROL Accueil] de l’utilisateur ou de l’utilisatrice de votre choix.

## Ajouter une tâche ou un problème à un projet

Vous pouvez ajouter une tâche ou un problème à un projet existant directement à partir de la zone Accueil :

1. Cliquez sur le **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **Accueil**.
1. Cliquez sur **[!UICONTROL Nouvelle tâche]**, puis sélectionnez **[!UICONTROL Tâche de projet]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. Dans le champ **[!UICONTROL Nom]**, indiquez un nom pour la tâche ou le problème.
1. Dans le champ **[!UICONTROL Affecter à]**, commencez à saisir le nom de l’utilisateur ou utilisatrice, de l’équipe ou du rôle à qui vous souhaitez l’affecter, puis cliquez sur le nom lorsqu’il apparaît dans le menu déroulant.
1. Commencez à saisir le nom du projet dans lequel vous souhaitez créer la tâche ou le problème, puis cliquez sur le nom lorsqu’il apparaît dans le menu déroulant.

   >[!IMPORTANT]
   >
   >La tâche ou le problème apparaît dans la [!UICONTROL liste de travail] uniquement lorsque le [!UICONTROL statut] du projet est défini sur [!UICONTROL Actuel].

1. (Le cas échéant) Pour créer un problème, sélectionnez **[!UICONTROL Problème]** dans le menu déroulant **[!UICONTROL Ajouter en tant que]**. Par défaut, **[!UICONTROL Tâche]** est sélectionné.

1. Cliquez sur **[!UICONTROL Sélectionner une date]**, puis sélectionnez la date et l’heure d’échéance de la tâche.
1. Cliquez sur **[!UICONTROL Créer]** pour enregistrer la tâche.
