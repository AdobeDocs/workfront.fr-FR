---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Outils de serveur MCP Adobe Workfront
description: Liste de référence des outils disponibles via le serveur MCP Adobe Workfront, regroupés par zone Workfront.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 6%

---


# Outils de serveur MCP Adobe Workfront

Cet article répertorie les outils que le serveur MCP [!DNL Adobe Workfront] expose à une plateforme agentic d’IA connectée. La plateforme appelle ces outils en votre nom lorsque vous lui demandez de rechercher, créer, mettre à jour ou supprimer des éléments Workfront.

Les outils sont regroupés par domaine Workfront : Approbations, Planification et Workflow.

Pour plus d’informations sur l’utilisation de ces outils par le biais d’une plateforme agentic d’IA, consultez [Utilisation du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md). Pour plus d’informations sur la configuration de la connexion, voir [Configuration du serveur Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

>[!IMPORTANT]
>
>La plateforme agentic d’IA agit dans Workfront à l’aide de votre compte Workfront, de votre niveau d’accès et des autorisations d’objet. Un outil ne fonctionne que si vous disposez de l’accès correspondant dans Workfront. Adobe n’est pas responsable des modifications apportées par la plateforme IA agentic à vos données Workfront.

## Outils de validation (23 au total)

### Documents

<!-- 
VERIFY BEFORE PUBLISHING: The following three tools may not be customer-facing. If engineering confirms they're internal-only, delete these rows from the table below:
- approvals_get_document_by_version_id
- approvals_list_aem_linked_folders
- approvals_send_documents_to_aem_folder
-->

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Rechercher la version du document par nom | `approvals_find_document_version_by_name` | Recherche l’ID de version actuelle d’un document par nom de fichier. Prend en charge les correspondances partielles. |
| Obtenir le document par ID de version | `approvals_get_document_by_version_id` | Récupère les détails du document (nom, taille, date de chargement, chargeur) pour un ID de version de document connu. |
| Obtenir des documents par projet | `approvals_get_documents_by_project` | Répertorie les documents au sein d’un projet Workfront, avec l’ID de version actuelle de chaque document. |
| Résoudre la portée du document | `approvals_resolve_document_scope` | Développe un projet ou un dossier dans la liste des ID de version de document qu’il contient. Prend en charge les portées de projet, de dossier et de dossier par nom. |
| Liste des dossiers liés à AEM | `approvals_list_aem_linked_folders` | Répertorie les dossiers de documents Workfront liés à Adobe Experience Manager. |
| Envoyer des documents vers le dossier AEM | `approvals_send_documents_to_aem_folder` | Déplace un ou plusieurs documents Workfront vers un dossier lié à AEM. |

### Workflows d’approbation

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Obtenir les informations sur le workflow d’approbation | `approvals_get_approval_info` | Retourne le workflow d&#39;approbation en cours (étapes, participants, statut) pour une version de document. |
| Créer ou mettre à jour un workflow d’approbation | `approvals_create_or_update_approval_workflow` | Crée ou met à jour les étapes d&#39;un workflow d&#39;approbation pour une version de document. Prend en charge les dépendances d’étape linéaires et parallèles (graphique). |
| Créer une approbation à partir d’un modèle | `approvals_create_approval_from_template` | Crée un workflow d&#39;approbation sur un document à partir d&#39;un modèle existant. |
| Demander l&#39;approbation du document | `approvals_request_document_approval` | Ouvre un formulaire assisté pour demander l’approbation d’une version de document (titre, approbateurs/réviseurs, échéance facultative et message). |
| Supprimer l’étape d’approbation | `approvals_delete_approval_stage` | Supprime une seule étape d&#39;un workflow d&#39;approbation par nom ou par position. Seules les étapes non démarrées peuvent être supprimées. |

### Rappels

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Envoyer un rappel aux participants | `approvals_send_reminder_to_participants` | Envoie des e-mails de rappel à des participants spécifiques à une étape d’approbation. Fonctionne uniquement pour les étapes commencées, non terminées et non verrouillées. |
| Envoyer un rappel aux participants indécis | `approvals_send_reminder_to_undecided` | Envoie des e-mails de rappel à tous les participants et participantes indécis (avertis, ouverts ou commentés) dans une étape d’approbation. |

### Modèles d’approbation

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Liste des modèles d&#39;approbation | `approvals_list_templates` | Répertorie les modèles d’approbation disponibles dans cette instance Workfront. Prend en charge le filtrage par créateur, participant et le tri par utilisation. |
| Rechercher un modèle par nom | `approvals_search_template_by_name` | Recherche les modèles de validation par nom (correspondance partielle non sensible à la casse). |
| Créer un modèle d&#39;approbation | `approvals_create_template` | Crée un modèle d&#39;approbation avec des dépendances d&#39;étape linéaires ou basées sur des graphiques. |
| Mettre à jour le modèle d&#39;approbation | `approvals_update_template` | Met à jour un modèle existant avec des modifications structurées (ajout ou suppression de participants, changement du nom des étapes, définition d’échéances, etc.). |

### Recherches et utilisateurs

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Obtenir l’utilisateur actuel | `approvals_get_current_user` | Renvoie l’identité Workfront de l’utilisateur appelant, y compris le nom, l’ID utilisateur, le nom de l’équipe interne et l’ID de l’équipe interne. |
| Rechercher un utilisateur par nom | `approvals_find_user_by_name` | Recherche l’ID d’un utilisateur Workfront par nom (correspondance approximative ou partielle). Renvoie le nom, l’ID, l’adresse électronique, le titre et l’URL de l’avatar. |
| Rechercher une équipe par nom | `approvals_find_team_by_name` | Recherche l’identifiant d’une équipe Workfront par nom (correspondance approximative ou partielle). |
| Rechercher un projet par nom | `approvals_find_project_by_name` | Recherche les projets Workfront par correspondance de noms partielle dans tout le système. |
| Obtenir les projets par propriétaire | `approvals_get_projects_by_owner` | Répertorie les projets Workfront dont l’utilisateur appelant est le propriétaire. |
| Obtenir la région Adobe | `approvals_get_adobe_region` | Renvoie le nom Adobe d’une région de fournisseur de cloud. |

## Outils de planification (43 au total)

### Espaces de travail

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Obtenir l’espace de travail | `planning_get_workspace` | Récupère les détails complets d’un espace de travail par identifiant ou alias. |
| Obtenir la liste des espaces de travail | `planning_get_workspace_list` | Répertorie tous les espaces de travail disponibles avec pagination basée sur le curseur. |
| Créer un espace de travail | `planning_create_workspace` | Crée un espace de travail vide pour organiser les types d’enregistrements, les champs et les données. |
| Créer un espace de travail à partir d’un modèle | `planning_create_workspace_from_template` | Crée un espace de travail pré-renseigné à l’aide d’un modèle existant. |
| Mettre à jour l’espace de travail | `planning_update_workspace` | Met partiellement à jour un espace de travail (nom, description, icône, sections ou propriétaire). |
| Supprimer l’espace de travail | `planning_delete_workspace` | Supprime définitivement un espace de travail et toutes ses données. |
| Convertir l’espace de travail en modèle | `planning_convert_workspace_to_template` | Enregistre un espace de travail existant en tant que modèle réutilisable (nécessite admin). |
| Obtenir le partage de l’espace de travail | `planning_get_workspace_sharing` | Renvoie la configuration de partage et d’autorisations actuelle pour un espace de travail. |
| Modifier le partage de l’espace de travail | `planning_modify_workspace_sharing` | Met à jour qui a accès à un espace de travail et à quel niveau d’autorisation. |

### Types d’enregistrements

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Obtenir le type d’enregistrement | `planning_get_record_type` | Récupère les détails complets d’un type d’enregistrement, y compris ses champs et vues. |
| Créer des types d’enregistrements | `planning_create_record_types` | Crée un ou plusieurs types d’enregistrements dans une section Workspace. |
| Mettre à jour le type d’enregistrement | `planning_update_record_type` | Met partiellement à jour le nom, la description, l’icône ou la couleur d’un type d’enregistrement. |
| Supprimer le type d’enregistrement | `planning_delete_record_type` | Supprime définitivement un type d’enregistrement et tous ses enregistrements, champs et vues. |
| Répertorier les types d’enregistrements globaux | `planning_list_global_record_types` | Répertorie tous les types d’enregistrements définis de manière centralisée (globaux) visibles pour l’utilisateur actuel. |
| Répertorier les types d’enregistrements globaux pouvant être ajoutés | `planning_list_addable_global_record_types` | Répertorie les types d’enregistrements globaux qui peuvent être ajoutés à un espace de travail spécifique. |
| Ajouter un type d’enregistrement global à l’espace de travail | `planning_add_global_record_type_to_workspace` | Associe un type d’enregistrement global dans un espace de travail spécifié. |
| Supprimer le type d’enregistrement global de l’espace de travail | `planning_remove_global_record_type_from_workspace` | Annule le lien d&#39;un type d&#39;enregistrement global d&#39;un espace de travail ; supprime tous ses enregistrements dans cet espace de travail. |
| Obtenir des espaces de travail d’enregistrement externes | `planning_get_external_record_workspaces` | Recherche les espaces de travail et les types d’enregistrements connectés à un enregistrement externe spécifique. |
| Obtenir le partage du type d’enregistrement | `planning_get_record_type_sharing` | Retourne le partage et les autorisations pour un type d’enregistrement spécifique. |
| Modifier le partage de type d’enregistrement | `planning_modify_record_type_sharing` | Met à jour qui peut accéder à un type d’enregistrement et à quel niveau d’autorisation. |

### Enregistrements

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Obtenir l’enregistrement | `planning_get_record` | Récupère les détails complets d’un enregistrement unique par ID. |
| Rechercher des enregistrements | `planning_search_records` | Recherche et filtre les enregistrements dans un type d’enregistrement. |
| Actions d’enregistrement en bloc | `planning_bulk_record_actions` | Crée, met à jour, supprime ou restaure plusieurs enregistrements dans une seule demande. |
| Créer un enregistrement de connexion | `planning_create_connection_record` | Crée un nouvel enregistrement dans un système externe connecté (par exemple, un projet Workfront). |
| Mettre à jour l’ordre des enregistrements | `planning_update_records_order` | Modifie l’ordre d’affichage des enregistrements dans un type d’enregistrement. |
| Obtenir le journal des modifications d&#39;enregistrement | `planning_get_record_change_log` | Renvoie l’historique des modifications au niveau du champ d’un enregistrement. |
| Obtenir le partage des enregistrements | `planning_get_record_sharing` | Renvoie la configuration de partage pour un enregistrement spécifique. |
| Modifier le partage d’enregistrements | `planning_modify_records_sharing` | Met à jour qui peut accéder à un ou plusieurs enregistrements et à quel niveau d&#39;autorisation. |

### Champs

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Obtenir le champ | `planning_get_field` | Récupère les détails complets et le schéma des valeurs d’un champ par ID. |
| Créer des champs | `planning_create_fields` | Ajoute un ou plusieurs champs (colonnes) à un type d’enregistrement. |
| Mettre le champ à jour | `planning_update_field` | Met partiellement à jour le nom, la description, les options ou la configuration d’un champ. |
| Supprimer le champ | `planning_delete_field` | Supprime de manière permanente un champ et toutes ses données d’un type d’enregistrement. |

### Vues

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Obtenir la vue | `planning_get_view` | Renvoie les détails complets d’une vue par ID. |
| Créer une vue | `planning_create_view` | Crée une nouvelle vue de table, de chronologie ou de calendrier pour un type d&#39;enregistrement. |
| Mettre à jour la vue | `planning_update_view` | Met partiellement à jour la configuration, les filtres ou le tri d’une vue existante. |
| Supprimer la vue | `planning_delete_view` | Supprime définitivement une vue (les enregistrements ne sont pas affectés). |
| Obtenir le partage des vues | `planning_get_view_sharing` | Renvoie la configuration de partage pour une vue spécifique. |
| Modifier le partage de vues | `planning_modify_view_sharing` | Met à jour qui peut accéder à une vue et à quel niveau d’autorisation. |

### Modèles

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Obtenir la liste des modèles | `planning_get_template_list` | Répertorie tous les modèles d’espace de travail disponibles avec des informations récapitulatives. |
| Obtenir le modèle | `planning_get_template` | Récupère les détails complets d’un modèle spécifique par ID. |

### Recherche et utilitaires

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Rechercher des ressources | `planning_search_resources` | Effectue des recherches dans les espaces de travail, les types d’enregistrements et les vues par nom. |
| Rechercher des données de partage | `planning_search_sharing_data` | Recherche les utilisateurs, les groupes, les équipes, les rôles et les entreprises par nom pour le partage et les autorisations. |
| Rechercher des utilisateurs | `planning_search_users` | Recherche des utilisateurs avec prise en charge de la pagination. |

## Outils de workflow (5 au total)

Les outils de workflow sont les actions d’usage général que la plateforme agentic d’IA utilise pour travailler avec n’importe quel objet Workfront : projets, tâches, événements, heures, affectations, programmes, portefeuilles, etc.

| Titre | Nom de l’outil | Fonctionnement |
|---|---|---|
| Rechercher des objets | `workflow_search_any_object` | Recherche des objets Workfront avec des paramètres de filtre flexibles, l’ordre et la pagination. |
| Créer un objet | `workflow_create_any_object` | Crée un objet Workfront tel qu’un projet, une tâche, un événement, une heure, une affectation, un programme ou un portfolio. |
| Mettre à jour l’objet | `workflow_update_any_object` | Met à jour les champs d’un objet Workfront existant. |
| Supprimer l’objet | `workflow_delete_any_object` | Supprime un objet Workfront par ID. Nécessite une confirmation explicite de l’utilisateur avant l’exécution de l’action. |
| Résoudre les noms de champ | `workflow_resolve_field_names_any_object` | Convertit les noms ou les libellés des champs fournis par l’utilisateur aux noms des champs de l’API Workfront sous-jacents afin que la plateforme agentique d’IA puisse créer des requêtes précises. |

## Mise à jour des outils

Lorsqu’Adobe publie une nouvelle version du serveur MCP Workfront, la plateforme IA agentic utilise automatiquement le nouvel ensemble d’outils. Vous n’avez pas besoin de vous reconnecter ou de changer quoi que ce soit de votre côté.
