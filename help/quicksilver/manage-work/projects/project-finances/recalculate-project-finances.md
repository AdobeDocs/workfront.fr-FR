---
title: Recalculer les finances du projet
product-area: projects
navigation-topic: financials
description: Les finances sont calculées sur un projet à mesure que des modifications se produisent dans les heures consignées pour le projet ou dans les taux utilisés pour calculer les coûts et les recettes.
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1590'
ht-degree: 0%

---

# Recalculer les finances du projet

Les finances sont calculées sur un projet à mesure que des modifications se produisent dans les heures consignées pour le projet ou dans les taux utilisés pour calculer les coûts et les recettes.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux projets et aux données financières</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations du projet avec les autorisations de gestion financière</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Observations relatives au calcul des finances dans Adobe Workfront

Les finances sont calculées dans les analyses améliorées de la manière suivante :

* Vous pouvez recalculer manuellement les coûts et les recettes d’un projet à l’aide de l’option Recalculer le financement d’un projet.
* En outre, certaines actions déclenchent un recalcul automatique.

Lorsque le taux d’un utilisateur ou d’un rôle change au cours de la vie d’un projet, les événements suivants peuvent se produire :

* Lorsque la modification est effectuée, le taux mis à jour est utilisé à partir de ce moment lors de l’enregistrement des heures et le calcul des informations financières. La modification du taux n’affecte pas la façon dont les éléments ont été calculés avant que la modification ne soit effectuée. Pour toutes les heures enregistrées, l&#39;ancien taux est utilisé pour calculer les informations financières.
* Vous pouvez forcer Adobe Workfront à utiliser le nouveau taux rétroactivement pour toutes les heures enregistrées jusqu’à présent, à l’aide de l’option Recalculer le financement . Cela oblige Workfront à recalculer rétroactivement toutes les heures, les coûts prévus et les revenus saisis précédemment, conformément aux nouvelles informations sur les taux.

>[!CAUTION]
>
>Avant de recalculer manuellement les finances pour un projet donné, vous souhaiterez peut-être conserver toutes les données financières déjà calculées à un taux précédent. Nous vous recommandons d’utiliser l’option Recalculer le financement uniquement lorsque vous êtes certain que vous n’apportez pas de modifications aux informations existantes, ou uniquement lorsque de telles modifications sont souhaitées.

## Préserver les données financières pour les tâches avec les heures existantes {#preserve-financial-data-for-tasks-with-existing-hours}

Lorsque les données financières d’un projet sont recalculées, Workfront recalcule rétroactivement toutes les heures précédemment enregistrées, les coûts prévus, les coûts réels et les recettes prévues et réelles, conformément à toute information financière nouvelle ou mise à jour.

* [Conserver les recettes du projet](#preserve-project-revenue)
* [Conserver le coût du projet](#preserve-project-cost)

### Conserver les recettes du projet  {#preserve-project-revenue}

Les taux de recettes peuvent changer pendant la durée de vie d’un projet.

Pour plus d’informations sur les taux de facturation et les recettes, consultez l’article . [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Les taux de recettes peuvent changer aux niveaux suivants :

* Au niveau du système (pour les rôles de tâche)\
   Pour plus d’informations sur la création de rôles de tâche avec des taux de facturation au niveau du système, consultez l’article . [Création et gestion des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Niveau d’utilisateur\
   Pour plus d’informations sur la modification des informations de taux de facturation sur les utilisateurs, consultez l’article . [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Au niveau de la société (pour les rôles de tâche)\
   Pour plus d’informations, voir [Remplacer les taux de facturation des rôles de tâche au niveau de l’entreprise](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* Niveau du projet (pour les rôles de tâche)\
   Pour plus d’informations sur le remplacement des taux de rôle de tâche au niveau du projet, consultez l’article . [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Par exemple, le taux de facturation d’un utilisateur varie au cours d’un projet de 50 $ à 75 $ de l’heure et vous souhaitez que toutes les données existantes restent calculées selon l’ancien taux (50 $ et heure). Cependant, lorsque les finances du projet sont recalculées, les recettes des tâches qui contiennent déjà des données financières seront mises à jour pour refléter le nouveau taux de facturation (de 75 $ de l’heure).

* [Conserver les recettes du projet en créant un enregistrement de facturation](#preserve-project-revenue-by-creating-a-billing-record)
* [Préserver les recettes du projet en utilisant plusieurs remplacements de taux de facturation](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### Conserver les recettes du projet en créant un enregistrement de facturation {#preserve-project-revenue-by-creating-a-billing-record}

Lorsque les taux de facturation changent à n’importe quel niveau mentionné ci-dessus, vous pouvez conserver les recettes existantes qui ont déjà été calculées sur le projet en évitant d’utiliser l’option Recalculer le financement manuelle ou en verrouillant la durée enregistrée sur le projet et calculée à l’aide de l’ancien taux dans un enregistrement de facturation ayant le statut Facturé.

Lorsque vous ne recalculez pas les finances du projet ou lorsque vous verrouillez les heures consignées dans un enregistrement de facturation, les heures consignées après le changement de taux sont calculées avec le nouveau taux et les heures consignées avant le changement de taux restent calculées à l&#39;ancien taux.

Pour plus d’informations sur la création d’enregistrements de facturation, reportez-vous à l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

#### Préserver les recettes du projet en utilisant plusieurs remplacements de taux de facturation {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

Lorsque les taux de facturation changent pour les rôles de tâche au niveau du projet, vous pouvez conserver les recettes existantes qui ont déjà été calculées sur le projet en utilisant plusieurs remplacements de taux de facturation qui sont verrouillés au cours d’une période spécifiée.

Pour plus d’informations sur l’utilisation de plusieurs remplacements de taux de facturation, voir l’article [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>Cela s’applique uniquement aux taux de facturation des rôles de tâche qui sont modifiés au niveau du projet.

### Conserver le coût du projet {#preserve-project-cost}

Les taux de coût peuvent changer aux niveaux suivants :

* Niveau système (pour les rôles de tâche)\
   Pour plus d’informations sur la création de rôles de tâche avec des taux de coût au niveau du système, consultez l’article . [Création et gestion des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Niveau d’utilisateur\
   Pour plus d’informations sur la modification des informations sur le taux de coût pour les utilisateurs, consultez l’article . [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Lorsque les taux de facturation changent à n&#39;importe quel niveau mentionné ci-dessus, vous pouvez conserver les coûts existants qui ont déjà été calculés sur le projet en verrouillant la durée enregistrée sur le projet et calculée à l&#39;aide de l&#39;ancien taux dans un enregistrement de facturation ayant le statut Facturé. Pour plus d’informations sur la création d’enregistrements de facturation, reportez-vous à l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md).

Vous pouvez également éviter d’utiliser l’option Recalculer Finance manuelle si vous ne souhaitez pas créer d’enregistrement de facturation, comme décrit dans la section . [recalculer manuellement les finances d’un projet](#manually-recalculate-finances-for-a-project) dans cet article.

Lorsque vous ne recalculez pas les finances du projet ou lorsque vous verrouillez les heures consignées dans un enregistrement de facturation, les heures consignées après le changement de taux sont calculées avec le nouveau taux et les heures consignées avant le changement de taux restent calculées à l&#39;ancien taux.

## recalculer manuellement les finances d’un projet {#manually-recalculate-finances-for-a-project}

Si vos taux changent pendant la durée de vie d’un projet et que vous souhaitez que vos calculs de coûts et de recettes reflètent les nouveaux taux, vous devez recalculer manuellement les finances du projet.

>[!NOTE]
>
>Vous pouvez empêcher la mise à jour des valeurs de recettes pour refléter les nouveaux taux lorsque vous recalculez manuellement la finance en suivant les étapes de la section . [Préserver les données financières pour les tâches avec les heures existantes](#preserve-financial-data-for-tasks-with-existing-hours) de cet article. Les valeurs de coût sont toujours mises à jour pour prendre en compte les nouveaux taux lorsque vous recalculez manuellement les finances d’un projet.

Vous pouvez recalculer les finances des projets dans Workfront à partir de la page du projet ou d’une liste de projets ou d’un rapport.

Vous pouvez recalculer les finances lors de leur modification en masse. Pour plus d’informations, voir [recalculer manuellement les finances en bloc dans la zone Modifier les projets](#manually-recalculate-finances-in-bulk-in-the-edit-projects-box) dans cet article.

1. Accédez au projet dans lequel vous souhaitez recalculer les finances et cliquez sur le bouton **Plus** icon ![](assets/qs-more-icon-on-an-object.png) à droite du nom du projet

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Dans une liste de projets ou un rapport, sélectionnez un ou plusieurs projets, puis cliquez sur le bouton **Plus** icon ![](assets/qs-more-icon-on-an-object.png) en haut de la liste.

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lors du re-calcul massif de leurs finances afin d’assurer des performances optimales. Certaines choses qui peuvent rendre un projet trop complexe peuvent être des dépendances ou des affectations multiples ou un grand nombre de champs personnalisés.

1. Cliquez sur **Recalculer la finance**.

   Tous les coûts et recettes prévus du projet sont recalculés avec toute nouvelle information.

   Vous devriez recevoir une confirmation en haut du navigateur que les finances du projet ont été recalculées avec succès.\
   Les valeurs de coût existantes et certaines valeurs de recettes qui n’ont pas été verrouillées sont mises à jour pour refléter les nouveaux taux.

## recalculer manuellement les finances en bloc dans la zone Modifier les projets {#manually-recalculate-finances-in-bulk-in-the-edit-projects-box}

Vous pouvez recalculer manuellement les finances de plusieurs projets en les modifiant en bloc. Les recettes des projets sont ainsi recalculées rétroactivement.

>[!IMPORTANT]
>
>Vous pouvez empêcher la mise à jour des valeurs de recettes pour refléter les nouveaux taux lorsque vous recalculez manuellement la finance en suivant les étapes de la section . [Préserver les données financières pour les tâches avec les heures existantes](#preserve-financial-data-for-tasks-with-existing-hours) de cet article. Les valeurs de coût sont toujours mises à jour pour prendre en compte les nouveaux taux lorsque vous recalculez manuellement les finances des projets.

Pour recalculer manuellement les finances de plusieurs projets :

1. Accédez à une liste de projets.
1. Sélectionnez plusieurs projets dans la liste, puis cliquez sur **Modifier**.

   >[!TIP]
   >
   >En fonction de la complexité de vos projets, nous vous recommandons de ne pas sélectionner un grand nombre de projets lors de leur modification en bloc afin d’assurer des performances optimales. Certaines choses qui peuvent rendre un projet trop complexe peuvent être des dépendances ou des affectations multiples ou un grand nombre de champs personnalisés.

1. Cliquez sur **Paramètres**, puis sélectionnez **Recalculer Les Coûts Et Les Recettes**.

1. Cliquez sur **Enregistrer les modifications**.

## Actions déclenchant un re-calcul automatique des finances

Les actions suivantes déclenchent le recalcul financier des projets dans Workfront :

* Modification de l’état des tâches
* Déplacement d’une tâche avec des heures vers un autre projet
* Passage de l’état Terminé à principal état du projet

>[!NOTE]
>
>Lorsque vous modifiez l’état du projet, seules les valeurs prévues sont recalculées.

Vous pouvez également recalculer manuellement les finances sous la variable **Plus** menu ![](assets/qs-more-menu.png) au niveau du projet, en cliquant sur **Recalculer les finances**.
