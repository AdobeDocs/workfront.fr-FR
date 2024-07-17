---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configurer la consignation des heures en heures ou en jours
description: En tant qu’utilisateur disposant d’une licence Plan, vous pouvez configurer l’heure de connexion dans Adobe Workfront en heures ou en jours. Les administrateurs système peuvent configurer ce paramètre pour des utilisateurs individuels ou pour plusieurs utilisateurs de leur entreprise. Par défaut, les utilisateurs ouvrent une session en heures.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 14%

---

# Configurer la consignation des heures en heures ou en jours

En tant qu’utilisateur disposant d’une licence de planificateur, vous pouvez configurer l’heure de connexion dans Adobe Workfront en heures ou en jours. Les administrateurs système peuvent configurer ce paramètre pour des utilisateurs individuels ou pour plusieurs utilisateurs de leur entreprise. Par défaut, les utilisateurs ouvrent une session en heures. Pour plus d’informations sur la façon de consigner l’heure dans Workfront, voir [Temps du journal](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Il est recommandé d’utiliser le temps de connexion de la même manière, en heures ou en jours, dans l’ensemble de l’organisation, pour garantir la précision des rapports.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Les planificateurs peuvent configurer le temps pour eux-mêmes. Seul un administrateur Workfront peut configurer l’heure pour d’autres utilisateurs.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

1. Selon votre objectif et votre niveau d’accès au système, effectuez l’une des opérations suivantes :

   * **L’utilisateur du planificateur configurant la journalisation du temps pour vous :** Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur votre nom d’utilisateur en regard de votre image de profil. Cliquez ensuite sur l&#39;icône **Plus** en regard de votre nom et sélectionnez **Modifier**.

   * **L’administrateur système configure la journalisation du temps pour les autres :** commencez à modifier un ou plusieurs comptes d’utilisateurs, comme décrit dans [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Dans la boîte de dialogue qui s’affiche, dans la section **Resource Planning**, recherchez l’option **Log Time in** .

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (Conditionnel) Si vous êtes un administrateur système qui modifie plusieurs utilisateurs simultanément, sélectionnez **Temps de connexion à**.
1. Sélectionnez l’une des options suivantes pour la durée de journalisation :

   | Option | Description |
   |---|---|
   | **Heures** | Les utilisateurs indiquent les heures de connexion dans Workfront. |
   | **Days** | Les utilisateurs indiquent les jours lors de la connexion à Workfront. |

1. (Conditionnel) Si vous avez choisi de consigner le temps en jours, dans le champ **Heures équivalentes pour le Workday complet**, saisissez le nombre d’heures égal à une journée entière. Un jour sur la feuille de temps d’un utilisateur correspond au nombre d’heures que vous entrez dans cette zone.

   Tenez compte des points suivants lors de la configuration de ce paramètre :

   * Cette option n’est pas disponible lors de la configuration de l’heure de connexion en heures.
   * Cette option est utilisée uniquement à des fins de journalisation. Cette option n’est pas liée à l’option **Schedule** disponible lors de la modification d’un utilisateur. L’option **Schedule** est utilisée lors du calcul des chronologies et dans d’autres zones de Workfront. (Pour plus d’informations sur l’utilisation de l’option **Schedule**, voir [Création d’une planification](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Cliquez sur **Enregistrer les modifications**.
