---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Création d’une planification
description: Vous pouvez définir les semaines de travail de vos utilisateurs et utilisatrices avec des plannings. Vous pouvez associer un planning à une personne ou à un projet. Cela permet à  [!DNL Workfront]  de calculer les chronologies et la disponibilité des utilisateurs et utilisatrices.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 99%

---

# Créer un planning

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

En tant qu’administrateur ou administratrice , vous pouvez définir votre semaine de travail avec des plannings. [!DNL Adobe Workfront] Vous pouvez associer un planning à une personne ou à un projet. Cela permet à [!DNL Workfront] de calculer les chronologies et la disponibilité des utilisateurs et utilisatrices.

Lorsque des utilisateurs et utilisatrices travaillent dans des fuseaux horaires différents, la création d’un planning dans chacun des fuseaux horaires et son association à ces utilisateurs et utilisatrices garantissent que leur travail est enregistré dans [!DNL Workfront] en temps réel et que leur disponibilité est toujours exacte en fonction du moment où ils travaillent.

Pour plus d’informations sur l’association de plannings à des utilisateurs, à des utilisatrices et à des projets, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) et [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Les administrateurs et administratrices de groupes peuvent également créer des plannings associés aux groupes qu’ils gèrent. Pour plus d’informations, voir [Créer et modifier les plannings d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Pour plus d’informations sur l’utilisation des plannings pour aider les personnes à collaborer dans [!DNL Workfront] avec des fuseaux horaires, voir [Travailler avec des fuseaux horaires](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Pour plus d’informations sur l’utilisation des plannings dans la planification des ressources, voir [Vue d’ensemble des plannings](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) et [Vue d’ensemble du planificateur de ressources](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
       <p>Ou</p>
       <p>Actuelle : [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un planning

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Plannings]**.
1. Cliquez sur **[!UICONTROL Nouveau planning]**.
1. Saisissez un nom pour le planning.
1. (Facultatif) Sélectionnez **[!UICONTROL Planning par défaut]** pour identifier ce planning comme valeur par défaut.

   Vous devez avoir au moins un planning dans . [!DNL Workfront] Si vous n’en avez qu’un, il est désigné comme le planning par défaut.

   Vous pouvez avoir plusieurs plannings, mais vous ne pouvez en avoir qu’un seul par défaut.

   >[!NOTE]
   >
   >Si vous êtes administrateur ou administratrice de groupes, vous ne pouvez pas désigner un planning comme planning par défaut. Seul un administrateur ou une administratrice [!DNL Workfront] peut désigner un planning comme planning par défaut pour le système.

   ![Nouveau planning](assets/new-schedule.png)

1. Dans l’onglet **[!UICONTROL Planning]**, sélectionnez un planning quotidien en faisant glisser le contour bleu sur les blocs d’heure pour les mettre en surbrillance.

   Nous vous recommandons de sélectionner huit blocs d’une heure sur une période de neuf heures. Cela permet d’inclure le déjeuner ou d’autres pauses.

   ![Blocs de temps sur un planning](assets/new-schedule-with-exceptions.png)

1. Dans l’onglet **[!UICONTROL Détails]**, saisissez les informations suivantes :

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group with Administration Access]</td>
     <td><p>Sélectionnez le groupe dont les administrateurs et administratrices sont autorisés à modifier ce planning.</p>
     <p><b>IMPORTANT</b> :</p>
      <ul>
       <li>
       <p>Si vous êtes administrateur ou administratrice de groupes et que vous créez un planning, ce champ est obligatoire.</p>
       <p>En tant qu’administrateur ou administratrice de groupes, vous ne pouvez créer un planning que s’il est désigné pour un groupe ou un sous-groupe pour lequel vous êtes désigné administrateur ou administratrice.</p>
       <p>Si vous ne gérez qu’un seul groupe, ce groupe est sélectionné par défaut dans ce champ.</p>
       <p>Si vous gérez plusieurs groupes, vous devez sélectionner un groupe dans ce champ avant de pouvoir enregistrer le planning.</p></li>
       <li>Si vous êtes administrateur ou administratrice  et que vous créez un planning, ce champ est facultatif. [!DNL Workfront] Lorsque vous créez un planning sans l’associer à un groupe, il est enregistré comme planning au niveau du système et ne peut être géré par un administrateur ou une administratrice de groupes.
       <p>Les plannings affectés à des comptes ou des projets sont visibles par tous les utilisateurs et utilisatrices qui peuvent modifier ces objets. Cela est vrai pour les plannings au niveau du système et au niveau du groupe.</p>
       </li>
       <p>La définition d’un groupe avec accès administrateur pour un planning n’affecte pas le planning aux utilisateurs et utilisatrices du groupe. Elle permet uniquement aux administrateurs et administratrice du groupe de modifier, supprimer et copier le planning.</p>
       <p>Les administrateurs et administratrices de groupes ne peuvent pas modifier, supprimer ou copier des plannings au niveau du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupes</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access]</td>
     <td><p>Sélectionnez les groupes ayant l’accès [!UICONTROL View] qui peuvent voir ce planning.</p>
     <p>Seuls les utilisateurs et utilisatrices des groupes spécifiés ici peuvent trouver le planning dans le menu déroulant lorsqu’ils l’affectent aux utilisateurs, aux utilisatrices ou aux projets.</p></tr>
    <tr>
     <td>[!UICONTROL Time Zone]</td>
     <td><p>Sélectionnez le fuseau horaire du planning.</p>
     <p>Si vous associez le planning à un utilisateur ou une utilisatrice, il est recommandé que le fuseau horaire du planning corresponde à celui de l’utilisateur ou de l’utilisatrice. Pour plus d’informations sur les fuseaux horaires des utilisateurs et utilisatrices, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’un utilisateur ou d’une utilisatrice.
     </td>
    </tr>
   </table>


1. Dans l’onglet **[!UICONTROL Exceptions]**, indiquez les exceptions au planning.

   Les exceptions sont des journées complètes ou des demi-journées, telles que les jours fériés ou les événements de l’entreprise, qui doivent être exclues du planning.

   >[!NOTE]
   >
   >Si vous connaissez déjà les exceptions récurrentes du planning, vous pouvez définir vos exceptions de planning pour de nombreuses années à venir.

   Des journées complètes ou des demi-journées peuvent être exclues du planning de travail. Cliquez sur la date pour la sélectionner comme exception, puis sélectionnez le champ **[!UICONTROL Toute la journée]** pour indiquer si l’exception est une journée complète ou non.

   ![Exception Toute la journée](assets/schedule-adding-an-all-day-exception.png)

1. Saisissez les heures de début et de fin pour les exceptions de demi-journées.

   ![Exception Demi-journée](assets/partial-day-exception-on-schedules.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**, puis sur **[!UICONTROL Enregistrer] les modifications**.

1. (Facultatif) Associez le planning à un utilisateur ou une utilisatrice.

   Pour plus d’informations, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Facultatif) Associez le planning à un projet.

   Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).
