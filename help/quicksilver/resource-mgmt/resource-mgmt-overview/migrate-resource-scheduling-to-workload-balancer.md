---
filename: migrate-resource-scheduling-to-workload-balancer
product-area: resource-management
navigation-topic: resource-management-overview
title: Migration de la planification des ressources vers la [!UICONTROL Équilibreur de charge de travail]
description: Nous voulons que vous rencontriez le moins possible de perturbations du travail en vous aidant à concevoir un plan de migration. Les étapes ci-dessous vous aideront à former votre équipe et à déterminer le meilleur moment pour passer à l’équilibreur de charge de travail.
author: Alina
exl-id: 4bc08d5f-99c7-40e2-85d6-1de0b585aef8
source-git-commit: d2a8380e3383b97b8245bd2b6d3cb9ff75306e4f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 0%

---

# Migration depuis la ressource [!UICONTROL Planification] au [!UICONTROL Équilibreur de charge de travail]

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu .</span>

<!-- drafted for res scheduling deprecation blurb for PREVIEW release - Oct 2022 - CHANGE THIS BLURB TO SOMETHING ELSE AT PRODUCTION:-->

>[!CAUTION]
>  
>  
> <span class="preview">Les zones de planification ont été supprimées de l’environnement de prévisualisation et seront supprimées de l’environnement de production dans **Janvier 2023**. </span>\
> <span class="preview"> Après janvier 2023, vous devez planifier vos ressources dans l’équilibreur de charge de travail. </span>
>  
><span class="preview"> Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir la section [L’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/workload-balancer.md).</span>

Les informations de cet article ne s’appliquent à vous que si vous avez géré la planification de vos ressources dans la ressource. [!UICONTROL Planification] des zones d’Adobe Workfront. Workfront a commencé à abandonner la fonction [!UICONTROL Planification] en novembre 2020 et les a remplacés par le [!UICONTROL Équilibreur de charge de travail].

Pour plus d’informations sur le plan d’obsolescence de la variable [!UICONTROL Planification des ressources] les outils et la chronologie pour leur remplacement par la fonction [!UICONTROL Équilibreur de charge de travail], voir [Obsolescence des outils de planification des ressources dans Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

Nous voulons que vous rencontriez le moins possible de perturbations du travail en vous aidant à concevoir un plan de migration. Les étapes ci-dessous vous aideront à former votre équipe et à déterminer le meilleur moment pour passer à la [!UICONTROL Équilibreur de charge de travail].

## Localisation des outils de planification des ressources

Vous et vos équipes pouvez utiliser une partie de la ressource [!UICONTROL Planification] dans les zones suivantes de Workfront :

* Le [!UICONTROL Planification] dans la section [!UICONTROL Ressource] area
* Le [!UICONTROL Planification] section d’un projet
* Le [!UICONTROL Planification] section d’une équipe

Avec cette obsolescence, la variable [!UICONTROL Équilibreur de charge de travail] remplace tous les  [!UICONTROL Planification des ressources] dans tous les domaines répertoriés ci-dessus.

## Étape 1 : Entraînez vos équipes

Suivez la formation [Programme de gestion des ressources pour la nouvelle expérience Adobe Workfront](https://one.workfront.com/s/resource-management-program-nwe) (75 minutes) sur Workfront One.

Si vous rencontrez des difficultés pour vous connecter ou accéder au cours, contactez le service clientèle. Pour plus d’informations, voir [Contacter le service clientèle](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Étape 2 : Déterminer le meilleur moment pour migrer {#step-2-determine-the-best-time-to-migrate}

Suivez les étapes ci-dessous pour déterminer le moment idéal pour effectuer la migration :

1. Déterminer les fonctionnalités de la ressource [!UICONTROL Planification] les outils les plus utilisés par votre équipe et assurez-vous que ces fonctionnalités sont disponibles dans la variable [!UICONTROL Équilibreur de charge de travail]. Pour plus d’informations sur les fonctionnalités actuellement disponibles dans la section [!UICONTROL Équilibreur de charge de travail], voir la section &quot;Disponibilité des fonctionnalités&quot; dans l’article [Obsolescence des outils de planification des ressources dans Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

   >[!IMPORTANT]
   >
   >Presque toutes les fonctionnalités des outils de planification se trouvent désormais dans l’équilibreur de charge de travail.

1. Déterminez si votre équipe gère les affectations d’utilisateurs sur les affectations. Ajuster ou modifier les affectations d’utilisateurs signifie modifier les heures planifiées par jour pour chaque utilisateur pendant la durée d’un élément de travail.

   Les affectations modifiées dans les outils de planification ne sont pas transférées vers l’équilibreur de charge de travail. Par défaut, le système répartit également le nombre total d’heures planifiées d’un élément de travail sur toute la durée de l’élément.

   Vous devez gérer manuellement les affectations dans l’équilibreur de charge de travail afin de vous assurer qu’elles correspondent à celles des outils de planification. Pour plus d’informations, voir [Gestion des affectations utilisateur dans l’équilibreur de charge de travail](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. Les filtres enregistrés dans la zone Planification ne sont pas automatiquement transférés vers l’équilibreur de charge de travail. Prenez le temps de créer les filtres dont vous aurez besoin dans l’équilibreur de charge de travail. Pour plus d’informations sur la création de filtres dans l’équilibreur de charge de travail, voir [Filtrage des informations dans l’équilibreur de charge de travail](../workload-balancer/filter-information-workload-balancer.md).

<!--
1. Using the information gathered from Steps 1 and Step 2, decide which version of Step 3 you should continue with based on the needs of your organization.
-->

## Étape 3 : Migrer vers le [!UICONTROL Équilibreur de charge de travail]{#step-3-migrate-to-the-workload-balancer}

Nous avons identifié les versions suivantes pour cette étape, en fonction de vos résultats de l’étape 2 :

* [Étape 3a : Vous ou vos équipes utilisez la variable [!UICONTROL Planification] outils, mais ne modifiez pas l’affectation des utilisateurs](#step-3a-you-or-your-teams-use-the-scheudling-tools-but-do-not-modify-user-allocation)
* [Étape 3b : Vous ou vos équipes gérez les allocations d’utilisateurs dans la variable [!UICONTROL Planification] outils](#step-3b-you-or-your-teams-manage-user-allocations-in-the-scheduling-tools)

### Étape 3a : Vous ou vos équipes utilisez la variable [!UICONTROL Planification] outils, mais ne modifiez pas l’affectation des utilisateurs

Si vous ou vos équipes ne modifiez pas les allocations horaires quotidiennes sur les affectations de travail, vous êtes prêt à transférer les ressources de planification vers la variable [!UICONTROL Équilibreur de charge de travail].

![](assets/nwe-workload-balancer-global-350x125.png)

Procédez comme suit :

* Choisissez une date de transition.

   >[!TIP]
   >
   >Donnez à votre équipe du temps pour suivre la formation sur l’utilisation de l’équilibreur de charge de travail avant la date de transition. Pour plus d’informations sur la formation, voir la section [Migration de la planification des ressources vers l’équilibreur de charge de travail](#migrate-from-resource-uicontrol-scheduling-to-the-uicontrol-workload-balancer) dans cet article.

* Suivez ces instructions pour aider vos équipes :

   * Encouragez vos équipes à visiter le [Présentation de la variable [!UICONTROL Équilibreur de charge de travail]](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) et toutes les pages liées à partir de là pour examiner de plus près la manière dont la variable [!UICONTROL Équilibreur de charge de travail] fonctionne.
   * Hébergez des réunions FAQ pour que vos équipes répondent aux questions la semaine précédant la transition, effectuez l’interrupteur, puis organisez une autre réunion FAQ pour répondre aux questions de suivi.
   * Envoyez vos commentaires à Workfront à l’aide du bouton Commentaires de la barre d’outils supérieure. Nos développeurs de produits sont toujours intéressés par vos cas d’utilisation pour déterminer comment créer la variable [!UICONTROL Équilibreur de charge de travail] fournissez plus de valeur.

### Étape 3b : Vous ou vos équipes gérez les allocations d’utilisateurs dans la variable [!UICONTROL Planification] outils

Si votre workflow correspond à ce scénario, votre plan de transition doit être plus stratégique. Les allocations quotidiennes qui s’affichent dans la variable [!UICONTROL Planification] Les outils sont stockés dans une base de données différente des allocations quotidiennes qui s’affichent dans la variable [!UICONTROL Équilibreur de charge de travail]. Cela signifie que les ajustements des allocations quotidiennes que vous effectuez dans la ressource [!UICONTROL Planification] Les outils ne sont pas transférés vers les allocations quotidiennes dans la variable [!UICONTROL Équilibreur de charge de travail].

>[!CAUTION]
>
>Vous avez jusqu’à **Janvier 2023** pour vous assurer que l’affectation de vos utilisateurs à partir des zones de planification correspond à celle de l’équilibreur de charge de travail dans votre environnement de production. À ce moment-là, nous supprimons les outils de planification de l’environnement de production. Vous devez ajuster manuellement les affectations dans l’équilibreur de charge de travail pour qu’elles correspondent à celles des outils de planification. <span class="preview">Les outils de planification ont déjà été supprimés de l’environnement Aperçu.</span>


Tenez compte de ce qui suit lors de la transition vers le [!UICONTROL Équilibreur de charge de travail] lorsque vous utilisez [!UICONTROL Planification] fonctionnalité :

* Mettez en attente la gestion des allocations dans la [!UICONTROL Planification] à mesure que vos gestionnaires de ressources changent. Pour ce faire :

   * Découvrez la durée moyenne des tâches de vos projets actuels et tenez compte de cela lorsque vous déterminez la durée pendant laquelle vous devez mettre un frein à la gestion des allocations utilisateur.

      >[!TIP]
      >
      >Il vous suffit de consulter vos projets actuels ou de planification, c’est-à-dire ceux pour lesquels vos équipes effectuent activement des affectations et gèrent les allocations quotidiennes.

   * Créez un rapport de tâche et ajoutez le champ Durée de la tâche dans la vue et regroupez-le par Nom du projet. Résumez la colonne Durée dans l’option Afficher par la moyenne, puis enregistrez votre rapport.

      Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) .

   * Analysez votre rapport de tâches. Par exemple, si la durée moyenne de la tâche est de 3 jours, une transition d’une semaine peut être préférable. Demandez à l’équipe d’arrêter la gestion des affectations utilisateur pendant une semaine. La semaine suivante, transférez l’équipe à la variable [!UICONTROL Équilibreur de charge de travail] et commencez à gérer les affectations d’utilisateurs la semaine suivante.
   >[!NOTE]
   >
   >Cette suggestion peut ne pas fonctionner si la durée moyenne de la tâche est supérieure au temps restant avant la suppression des outils de planification.


   ![](assets/timeline-stop-using-resource-scheduler-callouts-350x178.png)

   >[!TIP]
   >
   >Vous pouvez continuer à effectuer des affectations de tâche et de problème pendant la période de transition. Les affectations effectuées seront répercutées dans le planificateur de ressources et [!UICONTROL Équilibreur de charge de travail].

* Si vous êtes une organisation plus importante avec des équipes qui gèrent des ressources pour des centaines de projets, vous pouvez envisager de passer de [!UICONTROL Planification] aux outils [!UICONTROL Équilibreur de charge de travail] un portefeuille à la fois. Envisagez un déploiement par étapes en créant des filtres personnalisés dans la variable [!UICONTROL Équilibreur de charge de travail] pour examiner un portefeuille spécifique à la fois.

* Autoriser vos gestionnaires de ressources à s’associer : des affectations de révision d’une personne effectuées dans la variable  [!UICONTROL Planification des ressources] les outils et l’un d’eux effectuant les réglages appropriés dans [!UICONTROL Équilibreur de charge de travail]. Une fois que cette équipe de deux outils a réconcilié les deux outils, demandez-leur de déplacer leurs workflows vers la [!UICONTROL Équilibreur de charge de travail].

## Besoin d’aide supplémentaire

Si vous avez besoin d’informations supplémentaires sur cette migration, contactez le support personnalisé. Pour plus d’informations sur les moyens de contacter l’assistance, voir [Contacter le service clientèle](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
