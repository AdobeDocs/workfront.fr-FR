---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Indiquer si le temps est consigné en heures ou en jours
description: En tant qu’utilisateur ou utilisatrice disposant d’une licence de plan, vous pouvez indiquer si vous consignez le temps dans Adobe Workfront en heures ou en jours. Les administrateurs et administratrices système peuvent configurer ce paramètre pour des utilisateurs et utilisatrices individuels ou pour plusieurs utilisateurs et utilisatrices de leur organisation. Par défaut, les utilisateurs et utilisatrices consignent le temps en heures.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 100%

---

# Indiquer si le temps est consigné en heures ou en jours

En tant qu’utilisateur ou utilisatrice disposant d’une licence de plan, vous pouvez indiquer si vous consignez le temps dans Adobe Workfront en heures ou en jours. Les administrateurs et administratrices système peuvent configurer ce paramètre pour des utilisateurs et utilisatrices individuels ou pour plusieurs utilisateurs et utilisatrices de leur organisation. Par défaut, les utilisateurs et utilisatrices consignent le temps en heures. Pour plus d’informations sur la consignation du temps dans Workfront, consultez [Consigner le temps](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Il est recommandé de consigner le temps de la même manière, en heures ou en jours, dans l’ensemble de l’organisation, pour garantir la précision des rapports.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Les planificateurs et planificatrices peuvent configurer le temps pour eux-mêmes. Seul un administrateur ou une administratrice Workfront peut configurer le temps pour d’autres utilisateurs ou utilisatrices.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

1. Selon votre objectif et votre niveau d’accès au système, effectuez l’une des opérations suivantes :

   * **Si vous êtes un planificateur ou une planificatrice configurant la consignation du temps pour vous-même :** cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur votre nom d’utilisateur en regard de votre image de profil. Cliquez ensuite sur l’icône **Plus** en regard de votre nom et sélectionnez **Modifier**.

   * **Si vous êtes un administrateur ou une administratrice système configurant la consignation du temps pour d’autres utilisateurs et utilisatrices :** commencez à modifier un ou plusieurs comptes d’utilisateurs et d’utilisatrices, comme décrit dans la section [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Dans la boîte de dialogue qui s’affiche, dans la section **Planification des ressources**, recherchez l’option **Consigner le temps**.

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (Le cas échéant) Si vous êtes un administrateur ou une administratrice système modifiant plusieurs utilisateurs et utilisatrices simultanément, sélectionnez **Consigner le temps en**.
1. Sélectionnez l’une des options suivantes pour la consignation du temps :

   | Option | Description |
   |---|---|
   | **Heures** | Les utilisateurs et utilisatrices indiquent des heures lors de la consignation du temps dans Workfront. |
   | **Jours** | Les utilisateurs et utilisatrices indiquent des jours lors de la consignation du temps dans Workfront. |

1. (Le cas échéant) Si vous avez choisi de consigner le temps en jours, dans le champ **Heures équivalentes pour une journée de travail complète**, saisissez le nombre d’heures correspondant à une journée complète. Un jour sur la feuille de temps d’un utilisateur ou d’une utilisatrice est égal au nombre d’heures que vous entrez dans ce champ.

   Tenez compte des points suivants lors de la configuration de ce paramètre :

   * Cette option n’est pas disponible lors que vous choisissez la consignation du temps en heures.
   * Cette option est utilisée uniquement pour la consignation du temps. Cette option n’est pas liée à l’option **Planning** qui est également disponible lors de la modification d’un utilisateur ou d’une utilisatrice. L’option **Planning** est utilisée lors du calcul des chronologies et dans d’autres zones de Workfront. (Pour plus d’informations sur l’utilisation de l’option **Planning**, consultez [Créer un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

1. Cliquez sur **Enregistrer les modifications**.
