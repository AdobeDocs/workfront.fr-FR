---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Outils de serveur MCP Adobe Workfront
description: Liste de référence des outils disponibles via le serveur MCP Adobe Workfront, regroupés par zone Workfront.
author: Courtney
feature: Get Started with Workfront
source-git-commit: c52aa353d5b9856cc6c7de458596f0145fb2c6e0
workflow-type: tm+mt
source-wordcount: '2721'
ht-degree: 6%

---


# Outils de serveur MCP Adobe Workfront

{{preview-fast-release-general}}

Cet article répertorie les outils que le serveur MCP [!DNL Adobe Workfront] expose à une plateforme agentic d’IA connectée. La plateforme appelle ces outils en votre nom lorsque vous lui demandez de rechercher, créer, mettre à jour ou supprimer des éléments Workfront.

Pour plus d’informations sur l’utilisation de ces outils par le biais d’une plateforme agentic d’IA, consultez [Utilisation du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md). Pour plus d’informations sur la configuration de la connexion, voir [Configuration du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

>[!IMPORTANT]
>
>La plateforme agentic d’IA agit dans Workfront à l’aide de votre compte Workfront, de votre niveau d’accès et des autorisations d’objet. Un outil ne fonctionne que si vous disposez de l’accès correspondant dans Workfront. Adobe n’est pas responsable des modifications apportées par la plateforme IA agentic à vos données Workfront.


## Actions de lecture et d’écriture

Chaque outil des tableaux suivants est classé dans la colonne Action en tant qu’action Lecture ou Écriture :

* **Lecture** : récupère des informations de Workfront sans modifier vos données. Par exemple, la recherche d’un projet, la liste des documents ou l’obtention des détails d’un enregistrement.
* **Write** : crée, met à jour ou supprime des données Workfront. Par exemple, la création d’un projet, la mise à jour d’un enregistrement ou la suppression d’une vue.

Votre administrateur Workfront contrôle les catégories d’outils que la plateforme agentic d’IA peut utiliser grâce à deux boutons (bascule) dans les Préférences système :

* **Outils MCP en lecture seule** (activé par défaut)
* **Outils Write MCP** (désactivé par défaut)

Si la plateforme agentic d’IA peut rechercher des éléments Workfront, mais ne peut pas les créer, les mettre à jour ni les supprimer, demandez à votre administrateur Workfront d’activer les actions d’écriture. Pour plus d’informations, voir [Conditions préalables d’administration](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#admin-prerequisites) dans *Configuration du serveur Adobe Workfront MCP*.

## Outils de validation

### Documents

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Rechercher la version du document par nom | `approvals_find_document_version_by_name` | Recherche l’ID de version actuelle d’un document par nom de fichier. Prend en charge les correspondances partielles. | Lire |
| Obtenir le document par ID de version | `approvals_get_document_by_version_id` | Récupère les détails du document (nom, taille, date de chargement, chargeur) pour un ID de version de document connu. | Lire |
| Résoudre la portée du document | `approvals_resolve_document_scope` | Développe un projet ou un dossier dans la liste des ID de version de document qu’il contient. Prend en charge les portées de projet, de dossier et de dossier par nom. | Lire |
| Obtenir des documents par portée | `approvals_get_documents_by_scope` | Obsolète. Utilisez `insights_find_workfront_data` à la place. Cet outil répertorie les documents dans un projet ou un dossier. | Lire |
| Liste des dossiers liés à AEM* | `approvals_list_aem_linked_folders` | Répertorie les dossiers de documents Workfront liés à Adobe Experience Manager. | Lire |
| Rechercher un document | `approvals_find_document` | Obsolète. Utilisez `insights_find_workfront_data` à la place. Cet outil a recherché un document par nom de fichier ou ID de version de document. | Lire |
| Envoi de documents vers un dossier AEM* | `approvals_send_documents_to_aem_folder` | Déplace un ou plusieurs documents Workfront vers un dossier lié à AEM. | Write |

*Pour utiliser ces outils, vous devez disposer d’une intégration native [!DNL Adobe Experience Manager] configurée dans votre instance Workfront. Pour plus d’informations, voir [Présentation des intégrations Adobe Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/aem-asset-integrations.md).


*L’envoi de documents vers un dossier AEM n’est pas encore pris en charge pour les projets sur l’espace de stockage Adobe. La prise en charge est attendue dans une version ultérieure.


<!--
| List AEM-linked folders* | `approvals_list_aem_linked_folders` | Lists Workfront document folders that are linked to Adobe Experience Manager. | Read |
-->

### Workflows d’approbation

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Obtenir les informations sur le workflow d’approbation | `approvals_get_approval_info` | Retourne le workflow d&#39;approbation en cours (étapes, participants, statut) pour une version de document. <span class="preview">Pour les validations comportant plusieurs chemins d’accès, il affiche chaque chemin et ses étapes.</span> | Lire |
| Créer ou mettre à jour un workflow d’approbation | `approvals_create_or_update_approval_workflow` | Crée ou met à jour les étapes d&#39;un workflow d&#39;approbation pour une version de document. <span class="preview">Prend en charge un seul suivi des étapes ou plusieurs chemins de révision parallèles.</span> | Write |
| Créer une approbation à partir d’un modèle | `approvals_create_approval_from_template` | Crée un workflow d’approbation sur un document à partir d’un modèle existant, <span class="preview">y compris des modèles qui définissent plusieurs chemins d’accès parallèles</span>. | Write |
| Supprimer l’étape d’approbation | `approvals_delete_approval_stage` | Supprime une seule étape d&#39;un workflow d&#39;approbation par nom ou par position. Seules les étapes non démarrées peuvent être supprimées. | Write |
| <span class="preview">Ajouter un chemin à l’approbation</span> | <span class="preview">`approvals_add_path_to_approval`</span> | <span class="preview">Ajoute un nouveau chemin de révision parallèle à un workflow d’approbation existant, de sorte que plusieurs pistes de révision s’exécutent simultanément sur une version de document.</span> | <span class="preview">Write</span> |
| <span class="preview">Supprimer le chemin de l’approbation</span> | <span class="preview">`approvals_remove_path_from_approval`</span> | <span class="preview">Supprime un chemin parallèle d’un workflow d’approbation. Le premier chemin ne peut pas être supprimé et les chemins qui contiennent des étapes terminées ou verrouillées sont protégés.</span> | <span class="preview">Write</span> |
| <span class="preview">Ajouter une étape au chemin d’accès</span> | <span class="preview">`approvals_add_stage_to_path`</span> | <span class="preview">Ajoute une étape de révision à la fin d’un chemin spécifique dans un workflow d’approbation parallèle.</span> | <span class="preview">Write</span> |
| <span class="preview">Supprimer l’étape du chemin</span> | <span class="preview">`approvals_remove_stage_from_path`</span> | <span class="preview">Supprime une étape non démarrée d’un chemin spécifique dans un workflow d’approbation parallèle. Chaque chemin doit contenir au moins une étape.</span> | <span class="preview">Write</span> |
| <span class="preview">Réorganiser les étapes dans le chemin</span> | <span class="preview">`approvals_reorder_stages_in_path`</span> | <span class="preview">Modifie l’ordre des étapes dans un chemin d’accès unique d’un workflow d’approbation parallèle.</span> | <span class="preview">Write</span> |

<!--
| Add and remove participants for an approval in bulk | `approvals_bulk_update_approval_participants`<br>`approvals__submit_bulk_update_approval_participants` | Adds or removes participants to or from multiple approvals at the same time. Currently, bulk updates can be applied only across a single project. Bulk updates across multiple projects will be available in the near future. | Write |
-->

<!--
| Request document approval | `approvals_request_document_approval` | Opens a guided form for requesting approval on a document version (title, approvers/reviewers, optional due date and message). | Write |
-->

### Rappels

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Envoyer un rappel aux participants | `approvals_send_reminder_to_participants` | Envoie des e-mails de rappel à des participants spécifiques à une étape d’approbation. Fonctionne uniquement pour les étapes commencées, non terminées et non verrouillées. | Write |
| Envoyer un rappel aux participants indécis | `approvals_send_reminder_to_undecided` | Envoie des e-mails de rappel à tous les participants et participantes indécis (avertis, ouverts ou commentés) dans une étape d’approbation. | Write |

### Modèles d’approbation

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Liste des modèles d&#39;approbation | `approvals_list_templates` | Répertorie les modèles d’approbation disponibles dans cette instance Workfront. Prend en charge le filtrage par créateur, participant et le tri par utilisation. | Lire |
| Rechercher un modèle par nom | `approvals_search_template_by_name` | Recherche les modèles de validation par nom (correspondance partielle non sensible à la casse). | Lire |
| Créer un modèle d&#39;approbation | `approvals_create_template` | Crée un modèle d&#39;approbation avec des dépendances d&#39;étape linéaires ou basées sur des graphiques. | Write |
| Mettre à jour le modèle d&#39;approbation | `approvals_update_template` | Met à jour un modèle existant avec des modifications structurées (ajout ou suppression de participants, changement du nom des étapes, définition d’échéances, etc.). | Write |
| Rappeler aux parties prenantes les approbations en bloc | `approvals_send_approval_reminder` | Envoyer des e-mails de rappel d’approbation à tous les approbateurs en attente dans un projet, un dossier, une campagne ou une fenêtre d’échéance entière. | Write |
| Mettre à jour les modèles d’approbation en bloc | `approvals_update_template` | Mettez à jour les modèles pour plusieurs modèles, par exemple en appliquant des modèles aux ressources, en créant de nouveaux modèles à partir de zéro ou à partir de flux d’approbation existants, en modifiant les modèles et en effectuant des opérations en bloc sur les modèles et les ressources. | Write |
| Ajouter ou supprimer des participants à l&#39;approbation en bloc. | `approvals_update_approval_participants` et `approvals__submit_update_approval_participants` | Ajouter, supprimer ou remplacer des participants à l&#39;échelle d&#39;un portefeuille, d&#39;un programme ou d&#39;un projet en une seule opération. | Write |


### Recherches et utilisateurs

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Rechercher un projet par nom | `approvals_find_project_by_name` | Supprimé le 13 août 2026. Utilisez `insights_find_id_by_name` à la place. Cet outil a recherché des projets Workfront par correspondance de noms partielle dans le système. | Lire |
| Obtenir les projets par propriétaire | `approvals_get_projects_by_owner` | Supprimé le 13 août 2026. Utilisez `insights_find_workfront_data` à la place. Cet outil répertorie les projets Workfront dont l’utilisateur appelant était le propriétaire. | Lire |
| Obtenir l’utilisateur actuel | `approvals_get_current_user` | Supprimé le 13 août 2026. Cet outil a renvoyé l&#39;identité Workfront de l&#39;utilisateur appelant, y compris le nom, l&#39;ID utilisateur, le nom de l&#39;équipe interne et l&#39;ID de l&#39;équipe interne. Pour des fonctionnalités similaires, voir [Obtenir l’utilisateur actuel](#insights-tools) sous les outils Insights. | Lire |
| Rechercher un utilisateur par nom | `approvals_find_user_by_name` | Obsolète. Utilisez `insights_search_users` à la place. Cet outil recherche l’ID d’un utilisateur Workfront par nom (correspondance approximative ou partielle), puis renvoie le nom, l’ID, l’adresse électronique, le titre et l’URL de l’avatar. | Lire |
| Rechercher une équipe par nom | `approvals_find_team_by_name` | Obsolète. Utilisez `insights_find_id_by_name` à la place. Cet outil a recherché l’identifiant d’une équipe Workfront par nom (correspondance approximative ou partielle). | Lire |
| Rechercher des projets | `approvals_find_projects` | Obsolète. Utilisez `insights_find_workfront_data` à la place. Cet outil a recherché des projets Workfront, éventuellement filtrés par nom et/ou limités aux projets détenus par l’utilisateur appelant. | Lire |

## Outils de planification

>[!IMPORTANT]
>
>* Pour utiliser MCP avec Workfront Planning, votre entreprise doit disposer d’un package Workfront incluant Adobe Workfront Planning.

### Espaces de travail

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Obtenir l’espace de travail | `planning_get_workspace` | Récupère les détails complets d’un espace de travail par identifiant ou alias. | Lire |
| Obtenir la liste des espaces de travail | `planning_get_workspace_list` | Répertorie tous les espaces de travail disponibles avec pagination basée sur le curseur. | Lire |
| Créer un espace de travail | `planning_create_workspace` | Crée un espace de travail vide pour organiser les types d’enregistrements, les champs et les données. | Write |
| Créer un espace de travail à partir d’un modèle | `planning_create_workspace_from_template` | Crée un espace de travail pré-renseigné à l’aide d’un modèle existant. | Write |
| Mettre à jour l’espace de travail | `planning_update_workspace` | Met partiellement à jour un espace de travail (nom, description, icône, sections ou propriétaire). | Write |
| Supprimer l’espace de travail | `planning_delete_workspace` | Supprime définitivement un espace de travail et toutes ses données. | Write |
| Convertir l’espace de travail en modèle | `planning_convert_workspace_to_template` | Enregistre un espace de travail existant en tant que modèle réutilisable (nécessite admin). | Write |
| Obtenir le partage de l’espace de travail | `planning_get_workspace_sharing` | Renvoie la configuration de partage et d’autorisations actuelle pour un espace de travail. | Lire |
| Modifier le partage de l’espace de travail | `planning_modify_workspace_sharing` | Met à jour qui a accès à un espace de travail et à quel niveau d’autorisation. | Write |

### Types d’enregistrements

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Obtenir le type d’enregistrement | `planning_get_record_type` | Récupère les détails complets d’un type d’enregistrement, y compris ses champs et vues. | Lire |
| Créer des types d’enregistrements | `planning_create_record_types` | Crée un ou plusieurs types d’enregistrements dans une section Workspace. | Write |
| Mettre à jour le type d’enregistrement | `planning_update_record_type` | Met partiellement à jour le nom, la description, l’icône ou la couleur d’un type d’enregistrement. | Write |
| Supprimer le type d’enregistrement | `planning_delete_record_type` | Supprime définitivement un type d’enregistrement et tous ses enregistrements, champs et vues. | Write |
| Répertorier les types d’enregistrements globaux | `planning_list_global_record_types` | Répertorie tous les types d’enregistrements définis de manière centralisée (globaux) visibles pour l’utilisateur actuel. | Lire |
| Répertorier les types d’enregistrements globaux pouvant être ajoutés | `planning_list_addable_global_record_types` | Répertorie les types d’enregistrements globaux qui peuvent être ajoutés à un espace de travail spécifique. | Lire |
| Ajouter un type d’enregistrement global à l’espace de travail | `planning_add_global_record_type_to_workspace` | Associe un type d’enregistrement global dans un espace de travail spécifié. | Write |
| Supprimer le type d’enregistrement global de l’espace de travail | `planning_remove_global_record_type_from_ws` | Annule le lien d&#39;un type d&#39;enregistrement global d&#39;un espace de travail ; supprime tous ses enregistrements dans cet espace de travail. | Write |
| Obtenir des espaces de travail d’enregistrement externes | `planning_get_external_record_workspaces` | Recherche les espaces de travail et les types d’enregistrements connectés à un enregistrement externe spécifique. | Lire |
| Obtenir le partage du type d’enregistrement | `planning_get_record_type_sharing` | Retourne le partage et les autorisations pour un type d’enregistrement spécifique. | Lire |
| Modifier le partage de type d’enregistrement | `planning_modify_record_type_sharing` | Met à jour qui peut accéder à un type d’enregistrement et à quel niveau d’autorisation. | Write |

### Enregistrements

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Obtenir l’enregistrement | `planning_get_record` | Récupère les détails complets d’un enregistrement unique par ID. | Lire |
| Rechercher des enregistrements | `planning_search_records` | Recherche et filtre les enregistrements dans un type d’enregistrement. | Lire |
| Actions d’enregistrement en bloc | `planning_bulk_record_actions` | Crée, met à jour, supprime ou restaure plusieurs enregistrements dans une seule demande. | Write |
| Créer un enregistrement de connexion | `planning_create_connection_record` | Crée un nouvel enregistrement dans un système externe connecté (par exemple, un projet Workfront). | Write |
| Mettre à jour l’ordre des enregistrements | `planning_update_records_order` | Modifie l’ordre d’affichage des enregistrements dans un type d’enregistrement. | Write |
| Obtenir le journal des modifications d&#39;enregistrement | `planning_get_record_change_log` | Renvoie l’historique des modifications au niveau du champ d’un enregistrement. | Lire |
| Obtenir le partage des enregistrements | `planning_get_record_sharing` | Renvoie la configuration de partage pour un enregistrement spécifique. | Lire |
| Modifier le partage d’enregistrements | `planning_modify_records_sharing` | Met à jour qui peut accéder à un ou plusieurs enregistrements et à quel niveau d&#39;autorisation. | Write |

### Champs

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Obtenir le champ | `planning_get_field` | Récupère les détails complets et le schéma des valeurs d’un champ par ID. | Lire |
| Créer des champs | `planning_create_fields` | Ajoute un ou plusieurs champs (colonnes) à un type d’enregistrement. | Write |
| Mettre le champ à jour | `planning_update_field` | Met partiellement à jour le nom, la description, les options ou la configuration d’un champ. | Write |
| Supprimer le champ | `planning_delete_field` | Supprime de manière permanente un champ et toutes ses données d’un type d’enregistrement. | Write |

### Vues

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Obtenir la vue | `planning_get_view` | Renvoie les détails complets d’une vue par ID. | Lire |
| Créer une vue | `planning_create_view` | Crée une nouvelle vue de table, de chronologie ou de calendrier pour un type d&#39;enregistrement. | Write |
| Mettre à jour la vue | `planning_update_view` | Met partiellement à jour la configuration, les filtres ou le tri d’une vue existante. | Write |
| Supprimer la vue | `planning_delete_view` | Supprime définitivement une vue (les enregistrements ne sont pas affectés). | Write |
| Obtenir le partage des vues | `planning_get_view_sharing` | Renvoie la configuration de partage pour une vue spécifique. | Lire |
| Modifier le partage de vues | `planning_modify_view_sharing` | Met à jour qui peut accéder à une vue et à quel niveau d’autorisation. | Write |

### Modèles

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Obtenir la liste des modèles | `planning_get_template_list` | Répertorie tous les modèles d’espace de travail disponibles avec des informations récapitulatives. | Lire |
| Obtenir le modèle | `planning_get_template` | Récupère les détails complets d’un modèle spécifique par ID. | Lire |

### Recherche et utilitaires

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Rechercher des ressources | `planning_search_resources` | Effectue des recherches dans les espaces de travail, les types d’enregistrements et les vues par nom. | Lire |
| Rechercher des données de partage | `planning_search_sharing_data` | Recherche les utilisateurs, les groupes, les équipes, les rôles et les entreprises par nom pour le partage et les autorisations. | Lire |
| Rechercher des utilisateurs | `planning_search_users` | Recherche des utilisateurs avec prise en charge de la pagination. | Lire |

## Outils de workflow

Les outils de workflow sont les actions d’usage général que la plateforme agentic d’IA utilise pour travailler avec n’importe quel objet Workfront : projets, tâches, événements, heures, affectations, programmes, portefeuilles, etc.

### Objets et champs

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Rechercher des objets | `workflow_search_any_object` | Recherche des objets Workfront avec des paramètres de filtre flexibles, l’ordre et la pagination. | Lire |
| Créer un objet | `workflow_create_any_object` | Crée un objet Workfront tel qu’un projet, une tâche, un événement, une heure, une affectation, un programme ou un portfolio. | Write |
| Mettre à jour l’objet | `workflow_update_any_object` | Met à jour les champs d’un objet existant. Prend également en charge le déplacement d’une tâche ou d’un événement vers un autre projet, la conversion d’une tâche ou d’un événement en un nouveau projet (ou d’un événement en une tâche) et la définition de tâches antérieures (dépendances). | Write |
| Supprimer l’objet | `workflow_delete_any_object` | Supprime un objet Workfront par ID. Nécessite une confirmation explicite de l’utilisateur avant l’exécution de l’action. | Write |
| Résoudre les noms de champ | `workflow_resolve_field_names_any_object` | Convertit les noms ou les libellés des champs fournis par l’utilisateur aux noms des champs de l’API Workfront sous-jacents afin que la plateforme agentique d’IA puisse créer des requêtes précises. | Lire |
| Lire la documentation des workflows | `workflow_read_workflow_docs` | Charge la documentation du workflow Workfront, y compris les guides d’utilisation des outils et les playbooks d’opérations spécifiques aux objets. Il s’agit de la première étape obligatoire avant d’effectuer des actions de workflow. | Lire |

### Mise à jour des fonctionnalités de l’outil d’objet

L’outil Mettre à jour l’objet fait plus que modifier les valeurs de champ. Il peut également déplacer le travail entre les projets, convertir des éléments de travail en de nouveaux objets et relier les dépendances des tâches.

#### Déplacer une tâche ou un événement vers un autre projet

Le déplacement redéfinit un élément de travail en place. L’objet conserve son identité et ses liens, il réside simplement dans un projet ou une tâche parent différent(e).

>[!NOTE]
>
>La définition d’un champ Projet dans une mise à jour de champ brut ne déplace pas une tâche ou un événement. Utilisez plutôt la fonctionnalité de déplacement .

* **Déplacer une tâche** : déplace la tâche vers un projet cible, et éventuellement sous une tâche parent cible.
* **Déplacer un événement** : déplace l’événement (demande) vers un projet cible.

Exemples d’invites :

* « Déplacez la tâche *Maquettes* vers le projet *Reconception de l’application mobile*. »
* « Déplacez cette requête sous le projet *Lancement du 4e trimestre*. »

#### Convertir un événement ou une tâche en projet

>[!NOTE]
>
>La conversion génère un nouvel objet . L’élément source est consommé dans le processus.

* **Convertir une tâche en projet** : permet de créer un projet à partir de la tâche. Vous pouvez éventuellement copier les données personnalisées de la tâche et baser le nouveau projet sur un modèle de projet.
* **Convertir un événement (demande) en projet** : crée un projet à partir de l’événement. Vous avez la possibilité de copier les données personnalisées du problème, de copier ses valeurs de champ natives et d’appliquer un modèle de projet.
* **Convertir un événement (demande) en tâche** : crée une tâche sur un projet existant à partir de l’événement.

Chaque conversion renvoie l’objet nouvellement créé, ainsi qu’un lien afin que vous puissiez l’ouvrir directement dans Workfront.

Exemples d’invites :

* « Convertissez la tâche *Actualisation du site web* en un projet appelé *Actualisation du site web 2026* à l’aide de notre modèle standard. »
* « Transformer cette demande en projet et copier ses champs personnalisés. »

#### Définir les tâches antérieures (dépendances)

Vous pouvez définir les prédécesseurs d&#39;une tâche. Les prédécesseurs prennent en charge les types de dépendance suivants, ainsi qu’un délai facultatif :

* **Fin-Début (FS)** : la tâche commence lorsque sa tâche antérieure se termine. (Par Défaut)
* **Démarrer-Démarrer (SS)** : la tâche démarre au démarrage de la tâche précédente.
* **Terminer-Terminer (FF)** : la tâche se termine lorsque sa tâche antérieure se termine.
* **Début-Fin (SF)** : la tâche se termine au début de sa tâche précédente.

Vous pouvez ajouter un retard (un retard) ou une avance (un retard négatif) dans les jours ouvrés, enchaîner plusieurs prédécesseurs sur une seule tâche et référencer une tâche dans un autre projet.

Exemples d’invites :

* « Faites en sorte que le *développement* commence une fois le *conception* terminé. »
* « Définissez *QA* pour qu’il commence au moment du lancement de *Development*, avec un décalage de deux jours. »
* « Ajoutez des #3 de tâches et des #5 de tâches en tant que prédécesseurs de *Launch*. »

### Commentaires

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Commentaires sur la requête | `comment-stream_query_comments` | Requête sur les commentaires par ID d’objet, avec pagination. | Lire |
| Obtenir un commentaire | `comment-stream_get_comment` | Obtenir un seul commentaire par ID. | Lire |
| Nombre de commentaires reçus | `comment-stream_get_comments_count` | Obtenez le nombre total de commentaires de niveau supérieur pour un objet. | Lire |
| Créer un commentaire | `comment-stream_create_comment` | Créez un commentaire sur un objet. | Write |
| Créer une réponse | `comment-stream_create_reply` | Créez une réponse à un commentaire existant. | Write |
| Mettre à jour le commentaire | `comment-stream_update_comment` | Mettre à jour un commentaire ou une réponse existant | Write |
| Supprimer un commentaire | `comment-stream_delete_comment` | Supprimer un commentaire par son identifiant. | Write |
| Ajouter une réaction | `comment-stream_add_reaction` | Ajouter une réaction (aimer) à un commentaire. | Write |
| Supprimer la réaction | `comment-stream_remove_reaction` | Supprimer une réaction (comme) d’un commentaire. | Write |

### Outils Insights

Les outils Insights récupèrent des informations sur les objets Workfront.

| Titre | Nom de l’outil | Fonctionnement | Action |
| --- | --- | --- | --- |
| Lecture de documents | `insights_read_docs` | Chargez la documentation du playbook ou du domaine Workfront, telle que les conditions, le statut, les dates ou les chemins d’accès aux champs. Il s’agit de la première étape obligatoire avant d’interroger les données. | Lire |
| Obtenir l’utilisateur actuel | `insights_get_current_user` | Récupérez votre propre identité Workfront, y compris son nom, son identifiant et son URL. | Lire |
| Champs de recherche | `insights_search_fields` | Recherchez les champs disponibles (standard et personnalisés) dans les projets, tâches, événements, utilisateurs, portfolios, équipes, etc. | Lire |
| Obtenir les chemins d’accès aux champs | `insights_get_field_paths` | Résolvez les chemins d’accès aux champs de notation par points pour les entités, requis par l’outil de requête de données. | Lire |
| Rechercher l’ID par nom | `insights_find_id_by_name` | Recherchez l’ID d’un objet Workfront par nom, tel que des projets, des tâches, des utilisateurs, des portfolios, etc. | Lire |
| Recherche de données Workfront | `insights_find_workfront_data` | Rechercher, filtrer, compter, trier et agréger les données Workfront. Il s’agit du principal outil de requête et de rapport. | Lire |
| Résumer l’objet | `insights_summarize_object` | Récupérez et résumez un seul objet Workfront par ID. | Lire |
| Liste des entités | `insights_list_entities` | Répertoriez tous les types d’objets Workfront disponibles pour la requête. | Lire |
| Rechercher des utilisateurs | `insights_search_users` | Recherchez des personnes par nom dans votre instance Workfront. Saisissez un nom complet ou partiel, puis récupérez les utilisateurs qui correspondent le mieux. Cela peut également inclure de manière facultative des « robots » collaborateurs de l’IA aux côtés des utilisateurs réguliers. | Lire |




## Mise à jour des outils

Lorsqu’Adobe publie une nouvelle version du serveur MCP de Workfront, la plateforme IA agentic utilise automatiquement l’ensemble d’outils mis à jour. Vous n’avez pas besoin de vous reconnecter ou de changer quoi que ce soit de votre côté.



## Outils supplémentaires bientôt disponibles

Nous nous efforçons d’ajouter les outils suivants au serveur MCP Workfront à l’avenir :

* Panneaux


