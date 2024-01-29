---
title: Journaux d’audit
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur Adobe Workfront, vous pouvez effectuer le suivi des modifications utilisateur déclenchées dans le système au cours des 90 derniers jours à l’aide des journaux d’audit.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '1464'
ht-degree: 2%

---

# Journaux d’audit

<!--Audited: 01/2024-->

En tant qu’administrateur Adobe Workfront, vous pouvez effectuer le suivi des modifications utilisateur déclenchées dans le système au cours des 90 derniers jours à l’aide des journaux d’audit décrits ci-dessous.

Pour plus d’informations sur l’affichage et le filtrage de ce que vous souhaitez voir dans ces journaux d’audit, voir [Affichage et exportation des journaux d’audit](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Informations disponibles dans un journal d’audit

Les champs suivants sont enregistrés dans chaque entrée du journal d’audit :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Date et heure</td> 
   <td>Lorsque l’action s’est produite.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type de journal</td> 
   <td>Type du journal d’audit, tel que Niveau d’accès ou Formulaire personnalisé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nom d'utilisateur</td> 
   <td> <p>Nom de l’utilisateur qui a exécuté l’action.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Action</td> 
   <td> Actions effectuées par l’utilisateur, telles que Modifier, Créer et Supprimer. </td> 
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
   <td> <p>Adresse IP de l’utilisateur qui a exécuté l’action au moment de l’action.</p> <p>L’adresse IP n’est pas disponible pour certaines actions système.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Types de journaux d’audit et actions qui les déclenchent

* [Niveau d’accès](#access-level)
* [Société](#company)
* [Condition](#condition)
* [Champ personnalisé](#custom-field)
* [Formulaires personnalisés](#custom-forms)
* [Section personnalisée](#custom-section)
* [Taux de change](#exchange-rate)
* [Groupe](#group)
* [Rôles de tâche](#job-roles)
* [Tentative de connexion](#login-attempt)
* [Priorité](#priority)
* [Préférence du projet](#project-preference)
* [Gravité](#severity)
* [État](#status)
* [Tâches et problèmes](#tasks-issues-preferences)
* [l’utilisateur ou de l’utilisatrice](#user)

### Niveau d’accès {#access-level}

Le système génère une entrée de journal de niveau d’accès lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée un niveau d’accès
* Supprime un niveau d&#39;accès
* Modifie un niveau d’accès :

   * Modification du type de licence
   * Modifie les autorisations en ce qui concerne les projets, tâches, problèmes, Portfolios, programmes, rapports, documents, utilisateurs ou modèles.

     >[!NOTE]
     >
     >Le système n’enregistre aucune modification des autorisations dans les données financières ou dans les types d’accès suivants : Afficher et Modifier.
     >
     >Par exemple, si un utilisateur passe du type d’accès Planificateur Vue à Modifier, le système n’affiche pas les informations contenues dans le menu déroulant Régler vos paramètres .

### Entreprise {#company}

Le système génère une entrée de journal d’audit de l’entreprise lorsqu’un utilisateur effectue l’une des opérations suivantes :

* Création d’une entreprise
* Modifie une société :

   * Renomme
   * Ajoute ou supprime des membres
   * Ajoute, modifie ou supprime la valeur dans son champ Groupe .
   * Ajoute ou modifie un taux de facturation d’entreprise pour un rôle de tâche
   * Suppression d’un taux de facturation d’entreprise pour un rôle de tâche
   * Définit cette variable comme entreprise principale pour l’organisation.
   * Joindre ou supprimer un formulaire personnalisé

* Suppression d’une entreprise

Pour plus d’informations sur les états, voir [Présentation des états](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condition {#condition}

Le système génère une entrée de journal de contrôle des conditions lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée une condition.
* Modifie une condition :

   * Modifie le nom
   * Modifie la couleur
   * Définit comme valeur par défaut
   * Modifie ou supprime la description de la condition.
   * Masque ou affiche la condition.

* Supprime une condition.

Pour plus d’informations sur la configuration des rôles de tâche, voir [Création ou modification d’une condition personnalisée](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Champ personnalisé {#custom-field}

Le système génère une entrée de journal d’audit Champ personnalisé lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée un champ personnalisé
* Modifie un champ personnalisé :

   * Modifie le nom, le libellé, les instructions ou le format
   * Modification du type d’affichage

     Cette option est disponible uniquement si le champ est de l’un des types suivants : une seule ligne, un paragraphe, une liste déroulante, une case à cocher, un bouton radio.

   * Modification de la taille du champ

     Cette option est disponible uniquement si le champ est de l’un des types suivants : une seule ligne, un paragraphe, du texte avec formatage.

   * Ajoute, supprime ou masque un choix de champ.
   * Modifie une valeur ou une étiquette de choix de champ
   * Configure le choix du champ à sélectionner ou non par défaut.
   * Configure un champ de liste déroulante pour permettre plusieurs sélections ou une sélection unique.
   * Configure un champ de date pour afficher ou non l’heure
   * Modifie l’hyperlien ou modifie la valeur d’un champ de texte descriptif.

* Supprime un champ personnalisé
* Partage d’un champ personnalisé

### Formulaires personnalisés {#custom-forms}

Le système génère une entrée de journal d’audit Forms personnalisé lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée un formulaire personnalisé
* Modifie un formulaire personnalisé :

   * Modification du nom ou de la description
   * Active ou désactive la fonction est active
   * Ajoute ou supprime un champ ou une section
   * Pour une section personnalisée, modifie un paramètre sous Paramètres supplémentaires
   * Remplace un champ par obligatoire ou non obligatoire.
   * Modification d’un calcul dans un champ personnalisé
   * Masque ou affiche la formule associée à un champ calculé dans le texte de survol Instructions
   * Active ou désactive la mise à jour des calculs précédents
   * Ajoute ou modifie une logique de saut ou une logique d’affichage

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Suppression d’un formulaire personnalisé
* Partage d’un formulaire personnalisé

### Section personnalisée {#custom-section}

Le système génère une entrée de journal d’audit Section personnalisée lorsqu’un utilisateur effectue l’une des actions suivantes dans un formulaire personnalisé :

* Crée une section personnalisée
* Modification du nom ou de la description d’une section personnalisée
* Suppression d’une section personnalisée

Pour plus d’informations sur les sections personnalisées des formulaires personnalisés, voir [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### Taux de change {#exchange-rate}

Le système génère une entrée de journal d’audit de taux de change lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée un taux de change
* Change un taux de change :

   * Ajoute une devise
   * Modification du taux de la devise
   * Définit la devise comme devise de base (par défaut) pour tous les projets et rapports du système.

* Supprime un taux de change

Pour plus d’informations sur la configuration des taux de change, voir [Configurer les taux de change](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Groupe {#group}

Le système génère une entrée de journal d’audit de groupe lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée un groupe
* Supprime un groupe
* Modifie un groupe :

   * Ajoute ou supprime des utilisateurs
   * Ajoute ou supprime des sous-groupes

### Fonctions {#job-roles}

Le système génère une entrée de journal d’audit des rôles de tâche lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée un rôle de tâche
* Modifie un rôle de tâche :

   * Modifie le nom
   * Ajoute, modifie ou supprime la description
   * Ajoute, modifie ou supprime le coût horaire (coût/heure).
   * Ajoute, modifie ou supprime le taux de facturation (facturation/heures).

* Supprime un rôle de tâche

Pour plus d’informations sur la configuration des rôles de tâche, voir [Création et gestion des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Tentative de connexion {#login-attempt}

Le système génère une entrée de journal de contrôle de tentative de connexion lorsqu’un utilisateur effectue l’une des actions suivantes :

* Se connecte, se déconnecte ou échoue à une tentative de connexion dans Workfront (dans un navigateur et dans l’application mobile).
* Connexion, déconnexion ou échec d’une tentative de connexion dans une intégration Workfront (Workfront pour Slack et Workfront pour Salesforce, par exemple)
* Se connecter ou se déconnecter de l’API Workfront

Les journaux de tentative de connexion ne sont pas enregistrés lorsqu’un administrateur Workfront utilise la fonction Se connecter en tant que .

>[!NOTE]
>
>Cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

### Priorité {#priority}

Le système génère une entrée de journal d’audit de priorité lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée une priorité
* Modifie une priorité :

   * Modifie le nom
   * Modifie la couleur
   * Définit comme valeur par défaut
   * Ajoute, modifie ou supprime la description de la priorité.
   * Masque ou affiche la priorité

* Supprime une priorité

Pour plus d’informations sur la configuration des priorités, voir [Créer et personnaliser des priorités](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Préférence du projet {#project-preference}

Le système génère une entrée de journal d’audit Préférences du projet lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée un trimestre personnalisé
* Modifie une préférence de projet :

   * Verrouille ou déverrouille-la
   * Modifie l’un de ses paramètres.
   * Active, désactive ou modifie le
   * Modification d’un calcul de chronologie

* Supprime un trimestre personnalisé

Pour plus d’informations sur les préférences du projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Gravité {#severity}

Le système génère une entrée de journal d’audit de gravité lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée une gravité de problème
* Modifie une gravité de problème :

   * Modifie le nom
   * Modifie la couleur
   * Définit comme valeur par défaut
   * Modifications ou suppression de la description de la gravité
   * Masque ou affiche la gravité

* Supprime une gravité de problème

Pour plus d’informations sur la configuration des rôles de tâche, voir [Création ou personnalisation des gravité de problème](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Statut {#status}

Le système génère une entrée de journal d’audit d’état lorsqu’un utilisateur effectue l’une des actions suivantes :

* Crée un état au niveau du système ou du groupe.
* Modifie un état au niveau du système ou du groupe :

   * Renomme
   * Rend l’état par défaut
   * Verrouille ou déverrouille-la
   * Masque ou annule cette opération
   * Modification de la couleur ou de la description

* Supprime un état au niveau du système ou du groupe.

Pour plus d’informations sur les états, voir [Présentation des états](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Préférences des tâches et des événements {#tasks-issues-preferences}

Le système génère une entrée de journal d’audit des préférences Tâches et problèmes lorsqu’un utilisateur modifie une préférence Tâches et problèmes de l’une des manières suivantes :

* Verrouille ou déverrouille une préférence
* Modification du paramètre d’une préférence
* Modification d’un paramètre Accès pour les tâches, les problèmes ou les requêtes

Pour plus d’informations sur les préférences de tâche et de problème, voir [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### l’utilisateur ou de l’utilisatrice {#user}

Le système génère une entrée de journal d’audit utilisateur lorsqu’un utilisateur effectue l’une des actions suivantes :

* Création d’un utilisateur

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

* Suppression d’un utilisateur
* Modification du niveau d’accès, de la société, de l’équipe ou du groupe d’un utilisateur
* Active un utilisateur
* Désactive un utilisateur
