---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Création d’un planning
description: Vous pouvez définir les semaines de travail de vos utilisateurs à l’aide de plannings. Vous pouvez associer un planning à un utilisateur ou à un projet. Cela permet [!DNL Workfront] pour calculer les chronologies et la disponibilité de l’utilisateur.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 3aad2a3d9ad32313cb14670965bc3ad05ab215d3
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Création d’un planning

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

En tant que [!DNL Adobe Workfront] administrateur, vous pouvez définir votre semaine de travail à l’aide de plannings. Vous pouvez associer un planning à un utilisateur ou à un projet. Cela permet [!DNL Workfront] pour calculer les chronologies et la disponibilité de l’utilisateur.

Lorsque des utilisateurs travaillent dans des fuseaux horaires différents, la création d’un planning dans chacun des fuseaux horaires et son association à ces utilisateurs garantissent que leur travail est enregistré dans [!DNL Workfront] en temps réel et que leur disponibilité est toujours exacte en fonction du moment où ils travaillent.

Pour plus d’informations sur l’association des planifications avec des utilisateurs et des projets, consultez les articles suivants :

* [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md)

Les administrateurs de groupe peuvent également créer des planifications associées aux groupes qu’ils gèrent. Pour plus d’informations, voir [Création et modification des plannings d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Pour plus d’informations sur l’utilisation des plannings pour aider les utilisateurs à collaborer dans [!DNL Workfront] à travers les fuseaux horaires, voir [Utilisation des fuseaux horaires](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Pour plus d’informations sur l’utilisation des plannings dans la planification des ressources, voir [Présentation des planifications](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) et [Présentation de Resource Planner](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule [!UICONTROL Adobe Workfront]</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Création d’un planning

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).
1. Cliquez sur **[!UICONTROL Planifications]**.
1. Cliquez sur **[!UICONTROL Nouvelle planification]**.
1. Spécifiez un nom pour le planning.
1. (Facultatif) Sélectionnez **[!UICONTROL Planification par défaut]** pour identifier ce planning comme valeur par défaut.

   Vous pouvez avoir plusieurs planifications dans [!DNL Workfront], mais vous ne pouvez avoir qu’un seul planning par défaut.

   Vous devez avoir au moins une planification dans [!DNL Workfront]. Si vous n’en avez qu’un seul, celui-ci est désigné comme planning par défaut.

   >[!NOTE]
   >
   >Si vous êtes administrateur de groupe, vous ne pouvez pas désigner un planning comme planning par défaut. Une seule [!DNL Workfront] l’administrateur peut désigner une planification comme valeur par défaut pour le système.

   ![](assets/new-schedule.png)

1. Dans le **[!UICONTROL Planification]** sélectionnez une planification quotidienne en faisant glisser le contour bleu sur les blocs d’heure pour les mettre en surbrillance.

   Nous vous recommandons de sélectionner 8 blocs d&#39;une heure sur une période de 9 heures. Cela permet de prendre le déjeuner ou d’autres pauses.

   ![](assets/new-schedule-with-exceptions.png)

1. Sur le **[!UICONTROL Détails]** , indiquez les informations suivantes :

   <table style="table-layout:auto">
    <tr>
     <td>Groupe [!UICONTROL avec accès à l’administration]</td>
     <td><p>Indiquez le groupe dont les administrateurs sont autorisés à modifier ce planning.</p>
     <p><b>IMPORTANT</b>:</p>
      <ul>
       <li>
       <p>Si vous êtes administrateur de groupe et que vous créez un planning, ce champ est obligatoire.</p>
       <p>En tant qu’administrateur de groupe, vous ne pouvez créer un planning que s’il est désigné pour un groupe ou un sous-groupe pour lequel vous êtes désigné administrateur.</p>
       <p>Si vous ne gérez qu’un seul groupe, ce groupe est sélectionné par défaut dans ce champ.</p>
       <p>Si vous gérez plusieurs groupes, vous devez sélectionner un groupe dans ce champ avant de pouvoir enregistrer le planning.</p></li>
       <li>Si vous êtes un [!DNL Workfront] administrateur créant un planning, ce champ est facultatif. Lorsque vous créez une planification sans l’associer à un groupe, elle est enregistrée comme planification au niveau du système et ne peut être gérée par un administrateur de groupe d’un groupe.
       <p>Les planifications affectées à des comptes ou des projets sont visibles par tous les utilisateurs qui peuvent modifier ces objets. Cela est vrai pour les plannings au niveau du système et au niveau du groupe.</p>
       </li>
       <p>La spécification d’un groupe avec accès administrateur pour une planification n’affecte pas la planification aux utilisateurs du groupe ; il permet uniquement aux administrateurs du groupe de modifier, supprimer et copier le planning.</p>
       <p>Les administrateurs de groupe ne peuvent pas modifier, supprimer ou copier des plannings au niveau du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groupes avec accès en vue]</td>
     <td><p>Sélectionnez les groupes ayant accès à [!UICONTROL View] auxquels ce planning est visible.</p>
     <p>Seuls les utilisateurs des groupes spécifiés ici peuvent trouver la planification dans le menu déroulant lorsqu’ils l’affectent aux utilisateurs ou aux projets.</p></tr>
    <tr>
     <td>[!UICONTROL Fuseau horaire]</td>
     <td><p>Sélectionnez le fuseau horaire de votre planning.</p>
     <p>Si vous associez la planification à un utilisateur, nous vous recommandons de faire correspondre le Fuseau horaire de la planification à celui de l’utilisateur. Pour plus d’informations sur les fuseaux horaires de l’utilisateur, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur.
     </td>
    </tr>
   </table>


1. Sur le **[!UICONTROL Exceptions]** , indiquez les exceptions au planning.

   Les exceptions sont des jours complets ou demi qui doivent être exclus du planning, comme les jours fériés ou les événements de la société.

   >[!NOTE]
   >
   >Si vous connaissez déjà les exceptions de planification récurrente, vous pouvez définir vos exceptions de planification pour de nombreuses années à l’avenir.

   Les jours complets ou partiels peuvent être exclus du planning de travail. Cliquez sur la date pour la sélectionner comme exception, puis sélectionnez la variable **[!UICONTROL Toute la journée]** pour indiquer si l’exception est une journée complète ou non.

   ![](assets/schedule-adding-an-all-day-exception.png)

1. Spécifiez les heures de début et de fin pour les exceptions de jour partiel.

   ![jour-partiel-exception-on-schedule.png](assets/partial-day-exception-on-schedules.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**, puis cliquez sur **[!UICONTROL Enregistrer] Modifications**.

1. (Facultatif) Associez la planification à un utilisateur.

   Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Facultatif) Associez le planning à un projet.

   Pour plus d’informations, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).
