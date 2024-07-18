---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Actions à entreprendre après l’installation d’un plan directeur
description: Cet article décrit ce que vous devez faire après avoir installé un plan directeur dans  [!DNL Adobe Workfront]  pour déployer entièrement le plan directeur vers les utilisateurs de votre système.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 1%

---

# Actions à entreprendre après l’installation d’un plan directeur

Cet article décrit ce que vous devez faire après avoir installé un plan directeur dans [!DNL Adobe Workfront] pour déployer entièrement le plan directeur vers les utilisateurs de votre système.

* [Recommandations relatives au modèle de projet](#project-template-recommendations)
* [Recommandations relatives à la structure organisationnelle](#organizational-structure-recommendations)
* [Recommandations relatives au tableau de bord](#dashboard-recommendations)

## Recommandations relatives au modèle de projet {#project-template-recommendations}

Cette section contient des recommandations pour les modèles de projet installés avec vos plans directeurs.

### Affecter des utilisateurs à des rôles et à des équipes nouvellement créés {#assign-users-to-newly-created-roles-and-teams}

Les rôles et/ou équipes créés lors du processus d’installation du plan directeur ne sont pas automatiquement associés à des utilisateurs. Sans affecter d’utilisateurs aux rôles ou équipes nouvellement ajoutés, vous créerez du travail pour une fonction que personne ne sélectionnera. Dans certains cas, vous devrez peut-être créer de nouveaux utilisateurs pour remplir ces rôles et équipes. Pour plus d&#39;informations sur la création de nouveaux utilisateurs, voir [Ajout d&#39;utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Application d’un formulaire personnalisé au modèle et aux tâches du modèle {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Le processus d’installation n’associe pas le modèle de projet à des formulaires personnalisés. Si vos projets ou vos tâches nécessitent que des formulaires ou des champs spécifiques soient renseignés pour créer une cohérence de création de rapports, ou si votre formulaire de demande numérique contient des champs qui doivent être conservés au niveau du projet, nous vous recommandons d’associer les tâches de modèle ou de modèle à ces formulaires. Pour plus d’informations, voir [Ajout d’un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Mise à jour des estimations de la durée et de l’effort des tâches du modèle {#update-template-task-duration-and-effort-estimates}

Chaque tâche du modèle contient une durée planifiée et une estimation de l’effort planifié. Ces estimations servent de point de départ pour les durées et le temps passé pour ces activités. Toutefois, les capacités, les compétences et le rythme de votre organisation sont uniques. Vous devez examiner la durée estimée de chaque tâche et les efforts déployés pour l’ajuster en fonction des besoins de votre entreprise. Pour plus d’informations, voir [Gérer les informations sur la tâche dans la zone [!UICONTROL Présentation des détails de la tâche]](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associer un chemin de jalon et des jalons {#associate-a-milestone-path-and-milestones}

Le processus d’installation n’associe pas le modèle de projet à un chemin de jalon. Appliquez un chemin de jalon au modèle et appliquez des jalons aux tâches clés du modèle afin de prendre en charge vos besoins de création de rapports de jalon. Pour plus d’informations, voir [Association de jalons aux tâches](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Déployer le modèle dans votre équipe {#roll-out-the-template-to-your-team}

Préparez le matériel de formation à la fois pour les chefs de travail qui utiliseront ce modèle et pour les contributeurs qui exécuteront le travail dans le modèle de projet.

### Créer ou mettre à jour des rapports et des tableaux de bord {#create-or-update-reports-and-dashboards}

Si la solution représente un nouveau type de travail que votre organisation n’a pas effectué auparavant dans [!DNL Workfront], vous devrez peut-être créer de nouveaux rapports et tableaux de bord pour prendre en charge le travail. Pour plus d’informations, voir [Création d’un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) et [Création d’un tableau de bord](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Si la solution est similaire au travail que vous avez déjà exécuté dans [!DNL Workfront], vous devez vérifier que le travail se répercute dans les rapports et tableaux de bord existants comme prévu. S’il n’est pas inclus dans vos rapports existants, prenez des mesures pour mettre à jour les filtres ou créer de nouveaux rapports.

## Recommandations relatives à la structure organisationnelle {#organizational-structure-recommendations}

Cette section contient des recommandations pour les éléments de structure organisationnelle installés avec vos plans directeurs.

### Entreprises

Après avoir installé un plan directeur qui comprend une entreprise :

* Ajoutez un formulaire personnalisé pour augmenter l’enregistrement de l’entreprise avec des détails utiles (le formulaire et ses détails vous sont propres). Pour plus d’informations, voir [Ajout d’un formulaire personnalisé à un objet](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Si la société représente un client, vérifiez les taux de remplacement associés à la société. Pour plus d’informations, voir [Remplacer les taux de facturation des rôles de tâche au niveau de l’entreprise](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Si l’entreprise représente un client et s’il existe d’autres modèles de projet propres à cette organisation, commencez par pré-associer les modèles de projet à la nouvelle entreprise ajoutée. Pour plus d’informations, voir [Modifier les modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Si la société représente un client ou un fournisseur, associez les utilisateurs existants de l’organisation externe qui se trouvent déjà dans votre environnement. Pour plus d&#39;informations, voir [Création et modification d&#39;entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Si l’entreprise représente un client ou un fournisseur, créez des utilisateurs collaborateurs supplémentaires pour l’organisation externe dont vous aurez peut-être besoin dans votre environnement afin de rationaliser la communication, l’exécution du travail et les validations. Pour plus d&#39;informations sur la création de nouveaux utilisateurs, voir [Ajout d&#39;utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Mettez à jour les relations des graphiques organisationnels pour tous les utilisateurs associés à la nouvelle société ajoutée. Pour plus d’informations, voir [Création de rapports directs](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) et [Affichage de l’organigramme](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Pour plus d&#39;informations sur les entreprises, voir [Créer et modifier des entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Recommandations relatives au tableau de bord {#dashboard-recommendations}

Cette section contient des recommandations pour les tableaux de bord et les rapports installés avec un plan directeur.

### Mettre à jour les tableaux de bord nouvellement créés pour ajouter/supprimer des rapports

Les tableaux de bord ajoutés à partir d’un plan directeur comportent un ou plusieurs rapports, pages externes ou calendriers. Il est probable que vous n’ayez pas besoin de tous les rapports et autres éléments de tableau de bord ou que vous deviez augmenter le tableau de bord avec les rapports, pages externes et calendriers existants avant qu’il ne soit prêt à être partagé avec d’autres personnes. Pour plus d’informations, voir [Ajout d’un rapport à un tableau de bord](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Mettre à jour les rapports nouvellement créés pour ajouter/supprimer des colonnes ou des critères de filtrage

Les rapports distribués par le biais d’un plan directeur de tableau de bord ne comportent pas toutes les colonnes ou tous les critères de filtre pour prendre en charge votre configuration de [!DNL Workfront]. Il est prévu que vous ajustiez les rapports en fonction de vos normes. Pour garantir la cohérence avec d’autres rapports de votre environnement, vous pouvez ajouter une colonne que vous incluez dans tous les rapports pour l’objet répertorié ou ajouter certains critères de filtrage qui limitent les résultats à un type de projet ou à un groupe d’utilisateurs spécifique. Pour plus d’informations, voir [Créer ou modifier des vues](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) et [Créer ou modifier des filtres](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Partage des tableaux de bord ou des rapports avec les utilisateurs

Si vous n’envisagez pas de placer le tableau de bord sur un modèle de mise en page, partagez le tableau de bord avec les personnes qui le trouveront utile. Pour plus d’informations, voir [Partager un tableau de bord](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) et [Partager un rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Ajouter des tableaux de bord aux modèles de mise en page

La meilleure façon de rendre les informations disponibles pour les autres est d’ajouter des tableaux de bord aux modèles de mise en page. Identifiez les modèles de mise en page des personnes qui auraient le plus intérêt à consulter régulièrement le tableau de bord et ajoutez-y le tableau de bord nouvellement créé. Pour plus d’informations, voir [Créer et gérer des modèles de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Mise à jour d’autres tableaux de bord et rapports

L’introduction d’un nouveau tableau de bord et de ses rapports peut permettre de supprimer et d’ajuster d’autres tableaux de bord et rapports existants. Prenez le temps de consulter vos rapports existants pour identifier les rapports redondants et contradictoires.

### Distribution de données personnalisées aux formulaires pertinents

Certains rapports inclus dans un plan directeur de tableau de bord comportent des champs de données personnalisés dans l’affichage, le filtrage ou le regroupement du rapport. Dans certains cas, le plan directeur comporte également un formulaire auquel ces champs sont associés. Cependant, la plupart du temps, les champs personnalisés ne sont pas appliqués à un formulaire personnalisé. Pour que les colonnes, filtres ou regroupements fonctionnent correctement, ces champs doivent être associés à des formulaires connectés à un utilisateur, à un projet, à une tâche ou à un autre enregistrement d’objet. Pour plus d’informations, voir [Concevoir un formulaire avec le concepteur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
