---
title: Vue d’ensemble des journaux d’audit
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez effectuer le suivi des modifications utilisateur déclenchées dans le système au cours des 90 derniers jours à l’aide des journaux d’audit.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 85c6985d27ef0806e9152ecf2cbd90ca63a588c6
workflow-type: tm+mt
source-wordcount: '1523'
ht-degree: 93%

---

# Présentation des journaux d’audit

<!--Audited: 08/2025-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez effectuer le suivi des modifications utilisateur déclenchées dans le système au cours des 90 derniers jours à l’aide des journaux d’audit décrits ci-dessous.

Pour plus d’informations sur l’affichage et le filtrage de ce que vous souhaitez voir dans ces journaux d’audit, voir [Afficher et exporter des journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Informations disponibles dans un journal d’audit

Les champs suivants sont enregistrés dans chaque entrée du journal d’audit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Date et heure</td> 
   <td>Moment où l’action s’est produite.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type de journal</td> 
   <td>Type du journal d’audit, tel que Niveau d’accès ou Formulaire personnalisé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nom d'utilisateur</td> 
   <td> <p>Nom de l’utilisateur ou l’utilisatrice qui a effectué l’action.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Action</td> 
   <td> Actions effectuées, telles que Modifier, Créer et Supprimer. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objet</td> 
   <td> Nom de l’objet affecté par l’action. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Détails</td> 
   <td>Informations supplémentaires sur l’action. Placez le pointeur de la souris sur le texte pour lire le message complet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adresse IP</td> 
   <td> <p>Adresse IP de la personne ayant exécuté l’action au moment de l’action.</p> <p>L’adresse IP n’est pas disponible pour certaines actions système.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Types de journaux d’audit et actions qui les déclenchent

* [Niveau d’accès](#access-level)
* [Règles métier](#business-rules)
* [Entreprise](#company)
* [Condition](#condition)
* [Champ personnalisé](#custom-field)
* [Formulaire personnalisé](#custom-forms)
* [Section personnalisée](#custom-section)
* [Taux de change](#exchange-rate)
* [Groupe](#group)
* [Fonction](#job-role)
* [Priorité](#priority)
* [Préférence du projet](#project-preference)
* [Gravité](#severity)
* [Statut](#status)
* [Préférences des tâches et des problèmes](#tasks-issues-preferences)
* [l’utilisateur ou de l’utilisatrice](#user)
<!--* [Login Attempt](#login-attempt) -->

### Niveau d’accès {#access-level}

Le système génère une entrée de journal de niveau d’accès lorsqu’une personne effectue l’une des actions suivantes :

* Crée un niveau d’accès
* Supprime un niveau d’accès
* Modifie un niveau d’accès :

   * Modifie le type de licence
   * Modifie les autorisations en ce qui concerne les projets, tâches, problèmes, Portfolios, programmes, rapports, documents, utilisateurs, utilisatrices ou modèles

     >[!NOTE]
     >
     >Le système n’enregistre aucune modification des autorisations dans les données financières ou dans les types d’accès suivants : Afficher et Modifier.
     >
     >Par exemple, si une personne passe le type d’accès Planificateur ou planificatrice d’Afficher à Modifier, le système n’affiche pas les informations contenues dans le menu déroulant Affiner vos paramètres.

### Règles métier

Les règles métier ne sont disponibles que pour les clients qui ont acheté un plan Ultimate Workfront. Pour plus d’informations, voir [Créer et modifier des règles métier](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

Le système génère une entrée du journal d’audit des règles métier lorsqu’un utilisateur effectue l’une des opérations suivantes :

* Crée une règle métier
* Modifie une règle métier :

   * Modifie le nom.
   * Ajoute ou supprime des expressions
   * Change un déclencheur

* Supprime une règle métier

### Entreprise {#company}

Le système génère une entrée de journal d’audit d’une entreprise lorsqu’un utilisateur ou une utilisatrice effectue l’une des opérations suivantes :

* Crée une entreprise.
* Modifie une entreprise :

   * Modifie le nom.
   * Ajoute ou supprime des personnes membres.
   * Ajoute, modifie ou supprime la valeur dans son champ Groupe.
   * Ajoute ou modifie un taux de facturation d’entreprise pour une fonction.
   * Supprime un taux de facturation d’entreprise pour une fonction.
   * Définit cette variable comme entreprise principale pour l’organisation.
   * Joint ou supprime un formulaire personnalisé.

* Supprime une entreprise.

Pour plus d’informations sur les statuts, voir [Vue d’ensemble des statuts](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condition {#condition}

Le système génère une entrée de journal d’audit d’une condition lorsqu’un utilisateur ou une utilisatrice effectue l’une des opérations suivantes :

* Crée une condition.
* Modifie une condition :

   * Modifie le nom.
   * Modifie la couleur
   * Définit comme valeur par défaut
   * Modifie ou supprime la description de la condition.
   * Masque ou affiche la condition.

* Supprime une condition.

Pour plus d’informations sur la configuration des fonctions, voir [Créer ou modifier une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Champ personnalisé {#custom-field}

Le système génère une entrée de journal d’audit d’un champ personnalisé lorsqu’un utilisateur ou une utilisatrice effectue l’une des actions suivantes :

* Crée un champ personnalisé.
* Modifie un champ personnalisé :

   * Modifie le nom, le libellé, les instructions ou le format.
   * Modifie le type d’affichage.

     Cette option est disponible uniquement si le champ est de l’un des types suivants : une seule ligne, paragraphe, liste déroulante, case à cocher, case d’option.

   * Modifie la taille du champ.

     Cette option est disponible uniquement si le champ est de l’un des types suivants : une seule ligne, paragraphe, texte avec formatage.

   * Ajoute, supprime ou masque un choix de champ.
   * Modifie une valeur ou un libellé de choix de champ.
   * Configure le choix du champ à sélectionner ou non par défaut.
   * Configure un champ déroulant pour permettre plusieurs sélections ou une sélection unique.
   * Configure un champ de date pour afficher ou non l’heure.
   * Modifie l’hyperlien ou modifie la valeur d’un champ de texte descriptif.

* Supprime un champ personnalisé.
* Partage un champ personnalisé.

### Formulaire personnalisé {#custom-form}

Le système génère une entrée de journal d’audit de formulaire personnalisé lorsqu’un utilisateur ou une utilisatrice effectue l’une des actions suivantes :

* Modifie un formulaire personnalisé.
* Modifie un formulaire personnalisé :

   * Modifie le nom ou la description.
   * Active ou désactive la fonction Est actif.
   * Ajoute ou supprime un champ ou une section.
   * Pour une section personnalisée, modifie un paramètre sous Paramètres supplémentaires.
   * Remplace un champ par obligatoire ou non obligatoire.
   * Modifie un calcul dans un champ personnalisé.
   * Masque ou affiche la formule associée à un champ calculé dans le texte de survol Instructions.
   * Active ou désactive la mise à jour des calculs précédents.
   * Ajoute ou modifie une logique de saut ou une logique d’affichage.

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Modifie un formulaire personnalisé.
* Partage un formulaire personnalisé.

### Section personnalisée {#custom-section}

Le système génère une entrée de journal d’audit Section personnalisée lorsqu’un utilisateur ou une utilisatrice effectue l’une des actions suivantes dans un formulaire personnalisé :

* Crée une section personnalisée.
* Modifie le nom ou de la description d’une section personnalisée.
* Supprime une section personnalisée.

Pour plus d’informations sur les sections personnalisées dans les formulaires personnalisés, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Taux de change {#exchange-rate}

Le système génère une entrée de journal d’audit Taux de change lorsqu’un utilisateur ou une utilisatrice effectue l’une des actions suivantes :

* Crée un taux de change.
* Modifie un taux de change :

   * Ajoute une devise.
   * Modifie le taux de la devise.
   * Définit la devise comme devise de base (par défaut) pour tous les projets et rapports du système.

* Supprime un taux de change.

Pour plus d’informations sur la configuration des taux de change, voir [Configurer les taux de change](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Groupe {#group}

Le système génère une entrée de journal d’audit Groupe lorsqu’un utilisateur ou une utilisatrice effectue l’une des actions suivantes :

* Crée un groupe.
* Supprime un groupe.
* Modifie un groupe :

   * Ajoute ou supprime des utilisateurs et utilisatrices.
   * Ajoute ou supprime des sous-groupes.

### Fonctions {#job-role}

Le système génère une entrée de journal d’audit Fonctions lorsqu’un utilisateur ou une utilisatrice effectue l’une des actions suivantes :

* Crée une fonction.
* Modifie une fonction :

   * Modifie le nom.
   * Ajoute, modifie ou supprime la description.
   * Ajoute, modifie ou supprime le coût par heure (Coût/heure).
   * Ajoute, modifie ou supprime le taux de facturation (Fact/Hr.).

* Supprime une fonction.

Pour plus d’informations sur la configuration des fonctions, voir [Créer et gérer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Tentative de connexion {#login-attempt}

Le système génère une entrée de journal d’audit Tentative de connexion lorsqu’un utilisateur ou une utilisatrice effectue l’une des actions suivantes :

* Se connecte, se déconnecte ou effectue une tentative de connexion qui échoue dans Workfront (dans un navigateur et dans l’application mobile).
* Se connecte, se déconnecte ou échoue lors d’une tentative de connexion dans toute intégration de Workfront (telle que Workfront pour Slack)
* Se connecte ou se déconnecte de l’API Workfront.

Les journaux de tentative de connexion n’enregistrent pas lorsqu’un administrateur ou une administratrice Workfront utilise la fonction Connexion en tant que.

>[!NOTE]
>
>Cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

### Priorité {#priority}

Le système génère une entrée de journal d’audit Priorité lorsqu’un utilisateur ou une utilisatrice effectue l’une des actions suivantes :

* Crée une priorité.
* Modifie une priorité :

   * Modifie le nom.
   * Modifie la couleur
   * Définit comme valeur par défaut
   * Ajoute, modifie ou supprime la description de la priorité
   * Masque ou affiche la priorité

* Supprime une priorité

Pour plus d’informations sur la configuration des priorités, voir [Créer et personnaliser les priorités](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Préférence du projet {#project-preference}

Le système génère une entrée de journal d’audit Préférences du projet lorsqu’une personne effectue l’une des actions suivantes :

* Crée un calendrier personnalisé
* Modifie une préférence de projet :

   * La verrouille ou déverrouille
   * Modifie l’un de ses paramètres
   * L’active, la désactive ou la modifie
   * Modifie un calcul de chronologie

* Supprime un trimestre personnalisé

Pour plus d’informations sur les préférences de projet, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Gravité {#severity}

Le système génère une entrée de journal d’audit de gravité lorsqu’une personne effectue l’une des actions suivantes :

* Crée une gravité de problème
* Modifie une gravité de problème :

   * Modifie le nom.
   * Modifie la couleur
   * Définit comme valeur par défaut
   * Modifie ou supprime la description de la gravité
   * Masque ou affiche la gravité

* Supprime une gravité de problème

Pour plus d’informations sur la configuration des fonctions, voir [Créer ou personnaliser la gravité des problèmes](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Statut {#status}

Le système génère une entrée de journal d’audit Statut lorsqu’une personne effectue l’une des actions suivantes :

* Crée un statut au niveau du système ou du groupe
* Modifie un statut au niveau du système ou du groupe :

   * Modifie le nom.
   * Fait du statut le statut par défaut
   * La verrouille ou déverrouille
   * Le masque ou annule son masquage
   * Modifie la couleur ou la description

* Supprime un statut au niveau du système ou du groupe

Pour plus d’informations sur les statuts, voir [Vue d’ensemble des statuts](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Préférences des tâches et des événements {#tasks-issues-preferences}

Le système génère une entrée de journal d’audit des préférences relatives aux tâches et problèmes lorsqu’une personne modifie une préférence relative aux tâches et problèmes de l’une des manières suivantes :

* Verrouille ou déverrouille une préférence
* Modifie le paramètre d’une préférence
* Modifie un paramètre Accès pour les tâches, les problèmes ou les requêtes

Pour plus d’informations sur les préférences relatives aux tâches et problèmes, voir [Configurer les préférences en matière de tâches et de problèmes à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### l’utilisateur ou de l’utilisatrice {#user}

Le système génère une entrée de journal d’audit utilisateur lorsqu’une personne effectue l’une des actions suivantes :

* Crée une personne

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

* Supprime une personne
* Modifie le niveau d’accès, l’entreprise, l’équipe ou le groupe d’une personne.
* Active une personne.
* Désactive une personne.
