---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Création d’une planification
description: Vous pouvez définir les semaines de travail de vos utilisateurs et utilisatrices avec des plannings. Vous pouvez associer un planning à une personne ou à un projet. Cela permet à  [!DNL Workfront]  de calculer les chronologies et la disponibilité des personnes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 99%

---

# Créer un planning

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez définir votre semaine de travail avec des plannings. Vous pouvez associer un planning à une personne ou à un projet. Cela permet à [!DNL Workfront] de calculer les chronologies et la disponibilité des personnes.

Lorsque des personnes travaillent dans des fuseaux horaires différents, la création d’un planning dans chacun des fuseaux horaires et son association à ces personnes garantissent que leur travail est enregistré dans [!DNL Workfront] en temps réel et que leur disponibilité est toujours exacte en fonction du moment où elles travaillent.

Pour plus d’informations sur l’association de plannings à des personnes et à des projets, voir [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) et [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Les administrateurs et administratrices de groupe peuvent également créer des plannings associés aux groupes qu’ils ou elles gèrent. Pour plus d’informations, voir [Créer et modifier les plannings d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Pour plus d’informations sur l’utilisation des plannings pour aider les personnes à collaborer dans [!DNL Workfront] à travers les fuseaux horaires, voir [Travailler avec les fuseaux horaires](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Pour plus d’informations sur l’utilisation des plannings dans la planification des ressources, voir [Vue d’ensemble des plannings](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) et [Vue d’ensemble du planificateur de ressources](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un planning

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Plannings]**.
1. Cliquez sur **[!UICONTROL Nouveau planning]**.
1. Saisissez un nom pour le planning.
1. (Facultatif) Sélectionnez **[!UICONTROL Planning par défaut]** pour identifier ce planning comme celui par défaut.

   Vous devez avoir au moins un planning dans [!DNL Workfront]. Si vous n’en avez qu’un, il est désigné comme planning par défaut.

   Vous pouvez avoir plusieurs plannings, mais vous ne pouvez en avoir qu’un seul par défaut.

   >[!NOTE]
   >
   >Si vous êtes administrateur ou administratrice de groupe, vous ne pouvez pas désigner un planning comme planning par défaut. Il n’y a qu’un administrateur ou une administratrice [!DNL Workfront] qui peut désigner un planning comme celui par défaut pour le système.

   ![Nouveau planning](assets/new-schedule.png)

1. Sur l’onglet **[!UICONTROL Planning]**, sélectionnez un planning quotidien en faisant glisser le contour bleu sur les blocs d’heure pour les mettre en surbrillance.

   Nous vous recommandons de sélectionner 8 blocs d’une heure sur une période de 9 heures. Cela permet de prendre le déjeuner ou d’autres pauses.

   ![Blocs de temps sur un planning](assets/new-schedule-with-exceptions.png)

1. Sur l’onglet **[!UICONTROL Détails]**, saisissez les informations suivantes :

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group with Administration Access]</td>
     <td><p>Sélectionnez le groupe dont les administrateurs et administratrices peuvent modifier ce planning.</p>
     <p><b>IMPORTANT</b></p>
      <ul>
       <li>
       <p>Si vous êtes administrateur ou administratrice de groupe et que vous créez un planning, ce champ est obligatoire.</p>
       <p>En tant qu’administrateur ou administratrice de groupe, vous ne pouvez créer un planning que s’il est désigné pour un groupe ou un sous-groupe pour lequel vous êtes administrateur ou administratrice.</p>
       <p>Si vous ne gérez qu’un seul groupe, ce groupe est sélectionné par défaut dans ce champ.</p>
       <p>Si vous gérez plusieurs groupes, vous devez sélectionner un groupe dans ce champ avant de pouvoir enregistrer le planning.</p></li>
       <li>Si vous êtes administrateur ou administratrice [!DNL Workfront] créant un planning, ce champ est facultatif. Lorsque vous créez un planning sans l’associer à un groupe, il est enregistré comme planning au niveau du système et ne peut être géré par un administrateur ou une administratrice de groupe d’un quelconque groupe.
       <p>Les plannings affectés à des comptes ou des projets sont visibles par toutes les personnes qui peuvent modifier ces objets. Cela est vrai pour les plannings au niveau du système et au niveau du groupe.</p>
       </li>
       <p>La définition d’un groupe avec accès pour l’administration pour un planning n’affecte pas le planning aux personnes du groupe. Elle permet uniquement aux administrateurs et administratrices du groupe de modifier, supprimer et copier le planning.</p>
       <p>Les administrateurs et administratrices de groupe ne peuvent pas modifier, supprimer ou copier des plannings au niveau du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access]</td>
     <td><p>Sélectionnez les groupes ayant un accès [!UICONTROL View] qui peuvent voir ce planning.</p>
     <p>Seules les personnes des groupes spécifiés ici peuvent trouver la planification dans le menu déroulant lorsqu’elles l’affectent aux utilisateurs et utilisatrices ou aux projets.</p></tr>
    <tr>
     <td>[!UICONTROL Time Zone]</td>
     <td><p>Sélectionnez le fuseau horaire du planning.</p>
     <p>Si vous associez le planning à une personne, il est recommandé que le fuseau horaire du planning corresponde à celui de la personne. Pour plus d’informations sur les fuseaux horaires des personnes, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’une personne
     </td>
    </tr>
   </table>


1. Sur l’onglet **[!UICONTROL Exceptions]**, indiquez les exceptions au planning.

   Les exceptions sont des jours complets ou des.demi-journées qui doivent être exclus du planning, comme les jours fériés ou les événements de l’entreprise.

   >[!NOTE]
   >
   >Si vous connaissez déjà les exceptions récurrentes de votre planning, vous pouvez définir vos exceptions au planning pour de nombreuses années à venir.

   Les jours complets ou partiels peuvent être exclus du planning de travail. Cliquez sur la date pour la sélectionner comme exception, puis sélectionnez le champ **[!UICONTROL Toute la journée]** pour indiquer si l’exception est une journée complète ou non.

   ![Exception Toute la journée](assets/schedule-adding-an-all-day-exception.png)

1. Saisissez les heures de début et de fin pour les exceptions de jour partiel.

   ![Exception Jour partiel](assets/partial-day-exception-on-schedules.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**, puis sur **[!UICONTROL Enregistrer] les modifications**.

1. (Facultatif) Associez le planning à une personne.

   Pour plus d’informations, voir [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Facultatif) Associez le planning à un projet.

   Pour plus d’informations, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).
