---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Création d’une planification
description: Vous pouvez définir les semaines de travail de vos utilisateurs avec des plannings. Vous pouvez associer un planning à un utilisateur ou à un projet. Cela permet à  [!DNL Workfront] de calculer la chronologie et la disponibilité de l’utilisateur.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 6%

---

# Créer un planning

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

En tant qu&#39;administrateur [!DNL Adobe Workfront], vous pouvez définir votre semaine de travail avec des plannings. Vous pouvez associer un planning à un utilisateur ou à un projet. Cela permet à [!DNL Workfront] de calculer la chronologie et la disponibilité de l’utilisateur.

Lorsque des utilisateurs travaillent dans des fuseaux horaires différents, la création d’un planning dans chacun des fuseaux horaires et son association avec ces utilisateurs garantissent que leur travail est enregistré en [!DNL Workfront] en temps réel et que leur disponibilité est toujours exacte en fonction de leur moment de travail.

Pour plus d’informations sur l’association des plannings avec les utilisateurs et les projets, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) et [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

Les administrateurs de groupe peuvent également créer des planifications associées aux groupes qu’ils gèrent. Pour plus d’informations, voir [Création et modification des plannings d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Pour plus d’informations sur l’utilisation des plannings pour aider les utilisateurs à collaborer dans [!DNL Workfront] fuseaux horaires, voir [Utilisation des fuseaux horaires](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Pour plus d’informations sur l’utilisation des plannings dans la planification des ressources, voir [Aperçu des plannings](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) et [ ](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

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

1. Cliquez sur **[!UICONTROL Planifications]**.
1. Cliquez sur **[!UICONTROL Nouvelle Planification]**.
1. Saisissez le nom du planning.
1. (Facultatif) Sélectionnez **[!UICONTROL Planification par défaut]** pour identifier cette planification comme valeur par défaut.

   Vous devez avoir au moins une planification dans [!DNL Workfront]. Si vous n’en avez qu’une, elle est désignée comme planning par défaut.

   Vous pouvez avoir plusieurs planifications, mais vous ne pouvez avoir qu’une seule planification par défaut.

   >[!NOTE]
   >
   >Si vous êtes administrateur de groupe, vous ne pouvez pas désigner un planning comme planning par défaut. Seul un administrateur [!DNL Workfront] peut désigner une planification comme valeur par défaut pour le système.

   ![Nouvelle planification](assets/new-schedule.png)

1. Dans l’onglet **[!UICONTROL Planning]** , sélectionnez un planning quotidien en faisant glisser le contour bleu sur les blocs d’heure pour le mettre en surbrillance.

   Nous vous recommandons de sélectionner 8 blocs d&#39;une heure sur une période de 9 heures. Cela permet de prendre le déjeuner ou d’autres pauses.

   ![Blocs de temps sur un planning](assets/new-schedule-with-exceptions.png)

1. Dans l&#39;onglet **[!UICONTROL Details]**, saisissez les informations suivantes :

   <table style="table-layout:auto">
    <tr>
     <td>Groupe [!UICONTROL avec accès à l’administration]</td>
     <td><p>Sélectionnez le groupe dont les administrateurs sont autorisés à modifier ce planning.</p>
     <p><b>IMPORTANT</b> :</p>
      <ul>
       <li>
       <p>Si vous êtes administrateur de groupe et que vous créez un planning, ce champ est obligatoire.</p>
       <p>En tant qu’administrateur de groupe, vous ne pouvez créer un planning que s’il est désigné pour un groupe ou un sous-groupe pour lequel vous êtes désigné administrateur.</p>
       <p>Si vous ne gérez qu’un seul groupe, ce groupe est sélectionné par défaut dans ce champ.</p>
       <p>Si vous gérez plusieurs groupes, vous devez sélectionner un groupe dans ce champ avant de pouvoir enregistrer le planning.</p></li>
       <li>Si vous êtes un administrateur [!DNL Workfront] qui crée un planning, ce champ est facultatif. Lorsque vous créez une planification sans l’associer à un groupe, elle est enregistrée comme planification au niveau du système et ne peut être gérée par un administrateur de groupe d’un groupe.
       <p>Les planifications affectées à des comptes ou des projets sont visibles par tous les utilisateurs qui peuvent modifier ces objets. Cela est vrai pour les plannings au niveau du système et au niveau du groupe.</p>
       </li>
       <p>La définition d’un groupe avec accès à l’administration pour une planification n’affecte pas la planification aux utilisateurs du groupe. Elle permet uniquement aux administrateurs du groupe de modifier, supprimer et copier la planification.</p>
       <p>Les administrateurs de groupe ne peuvent pas modifier, supprimer ou copier des plannings au niveau du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs de groupe</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groupes avec accès en vue]</td>
     <td><p>Sélectionnez les groupes ayant accès à [!UICONTROL Vue] qui peuvent voir cette planification.</p>
     <p>Seuls les utilisateurs des groupes spécifiés ici peuvent trouver la planification dans le menu déroulant lorsqu’ils l’affectent aux utilisateurs ou aux projets.</p></tr>
    <tr>
     <td>[!UICONTROL Fuseau horaire]</td>
     <td><p>Sélectionnez le fuseau horaire du planning.</p>
     <p>Si vous associez le planning à un utilisateur, il est recommandé que le fuseau horaire du planning corresponde à celui de l’utilisateur. Pour plus d'informations sur les fuseaux horaires d'un utilisateur, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d'un utilisateur.
     </td>
    </tr>
   </table>


1. Sous l’onglet **[!UICONTROL Exceptions]**, spécifiez les exceptions au planning.

   Les exceptions sont des jours complets ou demi qui doivent être exclus du planning, comme les jours fériés ou les événements de la société.

   >[!NOTE]
   >
   >Si vous connaissez déjà les exceptions de planification récurrente, vous pouvez définir vos exceptions de planification pour de nombreuses années à l’avenir.

   Les jours complets ou partiels peuvent être exclus du planning de travail. Cliquez sur la date pour la sélectionner comme exception, puis sélectionnez le champ **[!UICONTROL Toute la journée]** pour indiquer si l’exception est une journée complète ou non.

   ![ {Toute l&#39;exception ](assets/schedule-adding-an-all-day-exception.png)

1. Saisissez les heures de début et de fin pour les exceptions du jour partiel.

   ![Exception de jour partiel](assets/partial-day-exception-on-schedules.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**, puis sur **[!UICONTROL Enregistrer] modifications**.

1. (Facultatif) Associez la planification à un utilisateur.

   Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Facultatif) Associez le planning à un projet.

   Pour plus d’informations, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).
