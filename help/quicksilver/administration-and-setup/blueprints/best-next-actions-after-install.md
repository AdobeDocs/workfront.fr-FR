---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Actions à entreprendre après l’installation d’un plan directeur
description: Cet article décrit ce que vous devez faire après avoir installé un plan directeur dans  [!DNL Adobe Workfront]  pour déployer complètement le plan directeur aux utilisateurs et utilisatrices de votre système.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 98%

---

# Actions à entreprendre après l’installation d’un plan directeur

Cet article décrit ce que vous devez faire après avoir installé un plan directeur dans [!DNL Adobe Workfront] pour déployer complètement le plan directeur aux utilisateurs et utilisatrices de votre système.

* [Recommandations pour le modèle de projet](#project-template-recommendations)
* [Recommandations pour la structure organisationnelle](#organizational-structure-recommendations)
* [Recommandations pour le tableau de bord](#dashboard-recommendations)

## Recommandations pour le modèle de projet {#project-template-recommendations}

Cette section contient des recommandations pour les modèles de projet installés avec vos plans directeurs.

### Affecter des utilisateurs et utilisatrices à des rôles et à des équipes nouvellement créés {#assign-users-to-newly-created-roles-and-teams}

Les rôles et/ou les équipes créés au cours du processus d’installation du plan directeur ne sont pas automatiquement associés à des utilisateurs et utilisatrices. Si vous n’affectez pas des utilisateurs et utilisatrices aux rôles ou aux équipes nouvellement ajoutés, vous créerez du travail pour une fonction que personne ne prendra en charge. Dans certains cas, il peut être nécessaire de créer de nouveaux utilisateurs et utilisatrices pour remplir ces rôles et ces équipes. Pour plus d’informations sur la création de nouveaux utilisateurs et utilisatrices, voir [Ajouter des utilisateurs et des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Appliquer un formulaire personnalisé au modèle et aux tâches du modèle {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Le processus d’installation n’associe pas le modèle de projet à des formulaires personnalisés. Si vos projets ou vos tâches exigent que des formulaires ou des champs spécifiques soient remplis pour assurer la cohérence des rapports, ou si votre formulaire de demande numérique contient des champs qui doivent être conservés au niveau du projet, nous vous recommandons d’associer le modèle ou les tâches du modèle à ces formulaires. Pour plus d’informations, voir [Ajouter un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Mettre à jour les estimations de la durée et de l’effort de la tâche du modèle {#update-template-task-duration-and-effort-estimates}

Chaque tâche du modèle contient une estimation de la durée et de l’effort prévus. Ces estimations servent de point de départ pour les durées et le temps consacrés à ces activités. Cependant, les capacités, les compétences et le rythme de votre organisation sont uniques. Vous devez examiner la durée et l’effort estimés de chaque tâche pour les adapter aux besoins de votre organisation. Pour plus d’informations, voir [Gérer les informations des tâches dans la zone [!UICONTROL Vue d’ensemble des détails de la tâche]](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associer un chemin jalonné et des jalons {#associate-a-milestone-path-and-milestones}

Le processus d’installation n’associe pas le modèle de projet à un chemin jalonné. Appliquez un chemin jalonné au modèle et appliquez des jalons aux tâches clés du modèle pour répondre à vos besoins en matière de rapports de jalons. Pour plus d’informations, voir [Associer des jalons à des tâches](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Transmettre le modèle à votre équipe {#roll-out-the-template-to-your-team}

Préparez des documents de formation pour les personnes chargées de la gestion du travail qui utiliseront ce modèle et les contributeurs et contributrices individuels qui exécuteront les travaux dans le cadre du modèle de projet.

### Créer ou mettre à jour des rapports et des tableaux de bord {#create-or-update-reports-and-dashboards}

Si la solution représente un nouveau type de travail que votre organisation n’a pas effectué auparavant dans [!DNL Workfront], vous devrez peut-être créer de nouveaux rapports et tableaux de bord pour soutenir le travail. Pour plus d’informations, voir [Créer un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) et [Créer un tableau de bord](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Si la solution est similaire au travail que vous avez déjà effectué sur [!DNL Workfront], vous devez vérifier que le travail alimente les rapports et les tableaux de bord existants comme prévu. S’il n’est pas pris en compte dans vos rapports existants, prenez des mesures pour mettre à jour les filtres ou créer de nouveaux rapports.

## Recommandations pour la structure organisationnelle {#organizational-structure-recommendations}

Cette section contient des recommandations pour les éléments de la structure organisationnelle installés avec vos plans directeurs.

### Entreprises

Après l’installation d’un plan directeur qui comprend une entreprise :

* Ajoutez un formulaire personnalisé pour compléter l’enregistrement de l’entreprise avec des détails utiles (le formulaire et ses détails vous sont propres). Pour plus d’informations, voir [Ajouter un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Si l’entreprise représente un client, examinez les taux de remplacement associés à l’entreprise. Pour plus d’informations, voir [Remplacer les taux de facturation des fonctions à l’échelle de l’entreprise](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Si l’entreprise représente un client et s’il existe d’autres modèles de projet propres à cette organisation, associez d’abord les modèles de projet à l’entreprise nouvellement ajoutée. Pour plus d’informations, voir [Modifier les modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Si l’entreprise représente un client ou un fournisseur, associez les utilisateurs et utilisatrices existants de l’organisation externe qui se trouvent peut-être déjà dans votre environnement. Pour plus d’informations, voir [Créer et modifier des entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Si l’entreprise représente un client ou un fournisseur, créez des profils collaborateurs supplémentaires pour l’organisation externe dont vous pourriez avoir besoin dans votre environnement pour rationaliser la communication, l’exécution du travail et les approbations. Pour plus d’informations sur la création de nouveaux utilisateurs et utilisatrices, voir [Ajouter des utilisateurs et des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Mettez à jour les relations de l’organigramme pour tous les utilisateurs et utilisatrices associés à l’entreprise nouvellement ajoutée. Pour plus d’informations, voir [Créer des rapports directs](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) et [Afficher l’organigramme](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Pour plus d’informations sur les entreprises, voir [Créer et modifier des entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Recommandations pour le tableau de bord {#dashboard-recommendations}

Cette section contient des recommandations relatives aux tableaux de bord et aux rapports installés avec un plan directeur.

### Mettre à jour les nouveaux tableaux de bord pour y ajouter/supprimer des rapports

Les tableaux de bord ajoutés à partir d’un plan directeur comportent un ou plusieurs rapports, pages externes ou calendriers. Vous n’aurez probablement pas besoin de tous les rapports et autres éléments du tableau de bord, ou vous devrez compléter le tableau de bord avec des rapports, pages externes et calendriers existants avant de le partager avec d’autres personnes. Pour plus d’informations, voir [Ajouter un rapport à un tableau de bord](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Mettre à jour les nouveaux rapports pour y ajouter/supprimer des colonnes ou des critères de filtre

Les rapports distribués par le biais d’un plan directeur de tableau de bord ne comportent pas toutes les colonnes ou tous les critères de filtre nécessaires pour prendre en charge votre configuration de [!DNL Workfront]. Vous devez ajuster les rapports pour les adapter à vos normes. Pour assurer la cohérence avec d’autres rapports de votre environnement, vous pouvez ajouter une colonne que vous incluez dans tous les rapports de l’objet répertorié, ou ajouter des critères de filtre qui limitent les résultats à un type de projet ou à un groupe d’utilisateurs et utilisatrices particulier. Pour plus d’informations, voir [Créer ou modifier des vues](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) et [Créer ou modifier des filtres](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Partager les tableaux de bord ou les rapports avec les utilisateurs et utilisatrices

Si vous n’envisagez pas de placer le tableau de bord sur un modèle de disposition, vous devrez le partager les personnes qui en feront usage. Pour plus d’informations, voir [Partager un tableau de bord](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) et [Partager un rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Ajouter des tableaux de bord aux modèles de disposition

La meilleure façon de mettre des informations à la disposition d’autres personnes est d’ajouter des tableaux de bord aux modèles de disposition. Identifiez les modèles de disposition des personnes qui ont le plus besoin de consulter régulièrement le tableau de bord et ajoutez-le à ces modèles. Pour plus d’informations, voir [Créer et gérer des modèles de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Mettre à jour d’autres tableaux de bord et rapports

L’introduction d’un nouveau tableau de bord et de ses rapports peut permettre de retirer et d’ajuster d’autres tableaux de bord et rapports existants. Prenez le temps d’examiner vos rapports existants afin d’identifier tout rapport redondant ou contradictoire.

### Distribuer les données personnalisées dans les formulaires appropriés

Certains rapports inclus dans le plan directeur d’un tableau de bord comportent des champs de données personnalisés dans la vue, le filtre ou le regroupement du rapport. Dans certains cas, le plan directeur comporte également un formulaire auquel ces champs sont associés. Cependant, le plus souvent, les champs personnalisés ne sont pas appliqués à un formulaire personnalisé. Pour que les colonnes, les filtres ou les regroupements fonctionnent correctement, ces champs doivent être associés à des formulaires liés à un enregistrement d’utilisateur ou utilisatrice, de projet, de tâche ou d’un autre objet. Pour plus d’informations, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
