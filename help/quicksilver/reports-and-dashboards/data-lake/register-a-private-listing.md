---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Enregistrer une liste privée pour Workfront Data Connect
description: Enregistrez une liste privée Snowflake pour partager vos données Workfront Data Connect directement avec le compte Snowflake de votre entreprise.
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 3%
---
# Enregistrer une liste privée pour Workfront Data Connect

Vous pouvez partager vos données Workfront Data Connect directement avec le compte Snowflake de votre organisation en enregistrant une liste privée. Cette méthode de connexion utilise la fonctionnalité de liste privée de Snowflake pour partager des données en toute sécurité entre les organisations sans les exposer publiquement. Elle fonctionne également entre les régions et les plateformes d’hébergement.

Une liste privée est utile lorsque vous souhaitez joindre vos données Workfront à d’autres données de votre entrepôt de données d’entreprise. Comme les données résident sur votre propre compte Snowflake, vous pouvez les interroger avec le reste de vos données.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

Vous avez également besoin d’un compte Snowflake disposant des autorisations nécessaires pour accepter les listes et créer des bases de données, ainsi que d’un droit Workfront Data Connect.

## Ce que partage une liste privée

Une liste privée vous donne accès aux éléments suivants :

* Plus de 100 vues de données pour les objets Workfront. Pour obtenir une description de chaque vue, consultez le [dictionnaire de données de Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md).
* Les vues de données `*_event`, qui contiennent chaque transaction de modification diffusée aux pipelines de données Data Connect.
* Valeurs de données personnalisées pour les objets extensibles. Pour obtenir un exemple, consultez l’exemple de requête de données personnalisées dans les [exemples de requête de Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md).

## Différences par rapport à une connexion à un compte de lecteur

Une liste privée partage un ensemble de vues différent de celui d’une connexion à un compte de lecteur et les données arrivent selon un planning différent. Gardez à l’esprit les différences suivantes :

* Une liste privée ne partage que les vues `*_event`. Les vues `*_current` et `*_daily_history` sont disponibles via un compte de lecteur, mais pas via une liste privée. Vous pouvez les créer dans votre propre compte Snowflake. Pour plus d&#39;informations, voir [Configurer les vues Historique actuel et quotidien](#set-up-current-and-daily-history-views) dans cet article.
* Une liste privée peut ne pas inclure toutes les vues disponibles via un compte de lecteur. Les objets Workfront Planning, `MONITORING_DATA_REFRESHES`, `BOOKINGS` et `CLASSIFIER` sont des exemples de vues non partagées. Cette liste n&#39;est pas exhaustive.
* Le chargement de Data Connect modifie les événements toutes les 4 heures. Étant donné qu’une liste privée nécessite une étape de réplication supplémentaire pour faire apparaître les données, attendez-vous à ce que les données arrivent environ 1 heure plus tard que par l’intermédiaire d’un compte de lecteur.
* La réplication des données s’exécute à 01:01, 05:01, 09:01, 13:01, 17:01 et 21:01 UTC. Les données sont généralement disponibles environ 10 minutes après chaque exécution.
* Les vues `MONITORING_DATA_REFRESHES` et `JOB_HISTORY` ne reflètent pas les heures auxquelles les données sont disponibles par le biais d’une liste privée. Bien que la vue `JOB_HISTORY` soit partagée via la liste privée, nous vous recommandons de la lire via un compte de lecteur pour identifier plus rapidement les tâches ayant échoué.

## Enregistrer une annonce privée

Pour créer une liste privée, commencez par rassembler les détails de votre compte Snowflake, puis ajoutez la liste dans Workfront.

### Collecter les détails de votre compte Snowflake

Workfront utilise les détails de votre compte Snowflake pour cibler la liste sur votre compte . Rassemblez les détails suivants :

* Localisateur de compte
* URL du compte
* Organisation du compte
* Nom du compte

Chacune de ces valeurs est disponible à partir de la fenêtre modale Détails du compte dans Snowflake.

Pour trouver les détails de votre compte :

1. Lorsque vous êtes connecté à votre compte Snowflake, cliquez sur le menu utilisateur dans le coin inférieur gauche.

1. Sélectionnez votre compte dans la section **Compte** du menu.

1. Cliquez sur **Afficher les détails du compte** pour le compte.

1. Enregistrez chacune des valeurs répertoriées ci-dessus.

Choisissez également le nom de la base de données par laquelle vous souhaitez accéder à vos données Workfront liées. Vous saisissez ce nom lors de l&#39;enregistrement de l&#39;annonce.

### Ajouter la liste privée dans Workfront

Vous pouvez enregistrer la liste privée via l’interface d’Adobe Workfront.

>[!IMPORTANT]
>
>Vous ne pouvez créer qu’une seule annonce privée par localisateur de compte.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Configuration**.

1. Dans le panneau de gauche, cliquez sur **Système** > **Connexion aux données**.

1. Cliquez sur l&#39;onglet **Connexions**.

1. Cliquez sur **Ajouter une liste privée**.

1. Remplissez le formulaire avec les détails du compte que vous avez collectés, y compris votre nom de base de données préféré.

1. Cliquez sur **Ajouter une liste privée**.

### Se connecter à la liste dans Snowflake

Dans votre compte Snowflake, établissez une connexion à la liste privée en tant que source de données externe. Vous pouvez ensuite interroger vos données Workfront avec le reste de vos données.

## Configurer les vues Historique actuel et quotidien

Une connexion au compte de lecteur fournit trois vues de données pour chaque table d’objets :

* **Actuel** : représentation à faible latence des données telles qu’elles existent actuellement dans l’application source.
* **Historique quotidien** — représentation des données telles qu’elles étaient à 23 h 59 UTC pour chaque jour.
* **Événement** : chaque transaction de modification diffusée aux pipelines de données de Data Connect.

Une liste privée ne partage que la vue Événement . Cette section fournit du code SQL pour créer les vues Current, Daily History et Event dans votre propre compte Snowflake.

Toutes les vues d’événement incluses dans la liste comportent les champs nécessaires à la logique d’affichage ci-dessous. Ces exemples supposent que vous ayez créé une base de données et un schéma de votre choix dans le compte Snowflake cible et qu’ils utilisent la vue `projects_event`. Dans chaque exemple, remplacez `<listing_db>` et `<listing_schema>` par vos propres valeurs.

>[!TIP]
>
>Nous vous recommandons de remplacer `select *` par une liste des colonnes que vous utilisez pour vos analyses. Si vous utilisez des `select *` et que des colonnes sont ajoutées ultérieurement à l&#39;affichage d&#39;événements de la liste, vous devez recréer l&#39;affichage pour activer les nouvelles colonnes.

### Affichages actuels

La vue actuelle d’un objet est le dernier enregistrement d’événement de modification stocké dans Data Connect. Si le dernier enregistrement est dans un état supprimé, l&#39;enregistrement est omis de la vue actuelle. Toutes les vues d’événement ont la même structure.

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

Les colonnes `deleted` et `end_effective_timestamp` ne sont pas nécessaires dans la vue actuelle. La vue filtre les données sur une seule valeur et supprime complètement l’enregistrement si celui-ci est supprimé.

### Vues Historique quotidien

La vue Historique quotidien identifie l&#39;enregistrement d&#39;événement de modification qui était actif à 23:59:59 d&#39;une date donnée, afin que vous puissiez suivre la tendance de l&#39;état de l&#39;enregistrement au fil du temps. L’exemple suivant donne le statut d’un enregistrement de projet à la fin de chaque jour calendaire.

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### Vues des événements

Par souci de cohérence, nous vous recommandons de créer une copie de la vue d&#39;événement de la base de données de liste et de la placer dans le même schéma que vos vues Historique actuel et quotidien.

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
