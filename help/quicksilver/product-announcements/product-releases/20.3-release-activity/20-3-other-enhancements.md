---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 autres améliorations
description: Cette page décrit toutes les autres améliorations apportées à la version 20.3 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 10 août 2020.
author: Luke
feature: Product Announcements
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 0%

---

# 20.3 autres améliorations

Cette page décrit toutes les autres améliorations apportées à la version 20.3 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 10 août 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 20.3, voir [Présentation de la version 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Partage d’un calendrier avec un lien privé

Pour alléger le fardeau du partage de calendriers dans Workfront, vous pouvez partager un lien privé qui permet aux utilisateurs d’accéder directement au calendrier. Le calendrier doit être partagé avec l’utilisateur, qui doit alors se connecter pour l’afficher.

Auparavant, vous pouviez partager une URL publique qui ne nécessitait pas de connexion pour s’afficher.

Pour plus d’informations, voir [Partage d’un rapport de calendrier](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Nouvelle zone Brouillons lors de la création de requêtes

Pour vous offrir davantage de flexibilité lors de l’utilisation des requêtes, Workfront enregistre désormais automatiquement chaque requête que vous créez en tant que brouillon dans la nouvelle zone Brouillons. Si vous ne disposez pas de toutes les informations nécessaires pour terminer la nouvelle requête, vous pouvez la laisser en tant que brouillon, y revenir et la terminer ultérieurement. Workfront enregistre une requête par rubrique de file d’attente dans la nouvelle zone Brouillons. Les brouillons de requêtes peuvent être enregistrés tant que vous en avez besoin jusqu’à ce que vous soyez prêt à les terminer et à les envoyer. Vous pouvez également supprimer ou repositionner la zone Brouillons du panneau de gauche à l’aide d’un modèle de mise en page.

Pour plus d’informations sur la création de requêtes, voir [Création et envoi de requêtes Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Pour la version Aperçu, si un modèle de mise en page personnalisé vous est attribué, vous devez ajouter la zone Brouillons de vos requêtes en modifiant votre modèle de mise en page.

## Développer ou réduire les éléments de la feuille de temps

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront

Pour vous aider à gérer facilement les feuilles de temps avec plusieurs éléments, vous pouvez désormais développer ou réduire tous les éléments en cliquant sur un bouton.

Auparavant, vous deviez cliquer individuellement sur chaque élément.

Pour plus d’informations, voir [Temps de connexion](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ignorer les dates réelles dans les calendriers Workfront

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement Aperçu le 5 juin 2020. Il sera disponible dans l’environnement de production le 19 juin 2020.

Pour mieux contrôler l’affichage des objets dans les rapports du calendrier, vous pouvez choisir d’ignorer les dates réelles même lorsqu’elles sont disponibles.

Auparavant, le calendrier utilisait automatiquement les dates réelles une fois qu’elles étaient disponibles.

Pour plus d’informations, voir [Présentation des rapports sur les calendriers](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Utilisation de champs de date personnalisés dans les rapports de calendrier

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement Aperçu le 29 mai 2020. Il sera disponible dans l’environnement de production le 12 juin 2020.

Pour vous aider à mieux visualiser et gérer votre travail quotidien avec des calendriers, des champs de date personnalisés sont désormais disponibles sous la forme d’une option de date.

Auparavant, vous ne pouviez gérer votre calendrier qu’avec des projections, planifiées lorsque les dates réelles n’étaient pas disponibles.

Pour plus d’informations, voir [Utilisation de champs de date personnalisés dans un rapport de calendrier](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (ou si vous utilisez Workfront Classic, voir [Utilisation de champs de date personnalisés dans un rapport de calendrier](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US)).

## Modifications des emails

**Modifications des emails sortants :** Tous les courriers électroniques de Workfront proviennent de notifications@my.workfront.com. Cela inclut les alertes automatisées et la communication utilisateur-utilisateur.

Auparavant, les administrateurs système pouvaient ajouter une adresse électronique personnalisée dans la zone Configuration du courrier électronique .

**Modifications de la réponse POP d&#39;un email entrant :** Les administrateurs système n’auront plus la possibilité de configurer un serveur de messagerie POP personnalisé pour les réponses aux emails entrants aux notifications.

Pour plus d’informations, voir [Mise en file d’attente des emails et modifications des emails de réponse POP](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## DomainKeys Identified Mail (DKIM) désormais inclus dans les emails Workfront sortants

Une technique d&#39;authentification des emails (DKIM) sera incluse sur tous les emails sortants. Cette signature DKIM n’est pas visible par l’utilisateur final mais permet la validation au niveau du serveur et renforce notre structure d’authentification existante.

## Mises à jour de l’inscription dans la nouvelle expérience Workfront

Pour rendre plus gérable l’inscription des utilisateurs à la nouvelle expérience Workfront, les administrateurs de groupe ont désormais accès à l’inscription et à l’inscription des utilisateurs appartenant aux groupes qu’ils gèrent.

Il existe également un lien Détails de l’utilisateur qui affiche les informations suivantes :

* Nom
* Rôle de tâche
* Adresse e-mail
* Image de profil

## Nouveautés pour les administrateurs : Brand Workfront pour des groupes, équipes, rôles de tâche et utilisateurs spécifiques

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront

Vous pouvez désormais utiliser un modèle de mise en page pour modifier les logos de la zone de navigation supérieure et du menu principal pour des groupes, des équipes, des rôles de travail et des utilisateurs spécifiques ayant leur propre valorisation de marque.

Pour plus d’informations, voir [Marque votre instance Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Les administrateurs de groupe peuvent créer et gérer des processus d’approbation.

Afin de garantir une plus grande autonomie et un meilleur contrôle des workflows de leurs groupes, un administrateur de groupe peut désormais accéder à la zone Processus d’approbation dans Configuration et créer et modifier des processus d’approbation pour un groupe qu’il gère. Ces processus de validation sont basés sur les états de ce groupe.

Pour s’assurer que les administrateurs de groupe ne modifient pas par inadvertance les processus de validation utilisés dans tout le système ou créés par d’autres groupes, ils ne peuvent accéder qu’aux processus de validation associés aux groupes qu’ils gèrent.

Pour plus d’informations, voir [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Pour les administrateurs : La nouvelle page Groupes facilite la création et la gestion des groupes.

Les administrateurs de groupe peuvent gérer plus facilement les groupes, maintenant que tout ce dont ils ont besoin se trouve sur la nouvelle page Groupes . Il n’est plus nécessaire de naviguer entre les différentes zones de superposition et les pages de configuration pour créer et modifier des groupes.

Voici les principaux points forts :

* Détails du groupe : Affichez et modifiez des informations de base sur le groupe, telles que le nom, la description, les noms des administrateurs de groupe et si le groupe est public ou privé.
* Liste des membres du groupe : Affichez tous les membres du groupe et utilisez la nouvelle barre d’outils pour ajouter, supprimer, exporter, activer et désactiver rapidement les appartenances. Vous pouvez également modifier les profils des membres et leur envoyer des commentaires de mise à jour.
* Champ Administrateur de groupe dans l’en-tête : Lorsque vous affichez un groupe que vous gérez, affectez ou annulez rapidement l’affectation d’un membre du groupe en tant qu’administrateur du groupe. Vous pouvez également le faire dans la liste des membres du groupe à l’aide de la nouvelle colonne Rôle du groupe .
* Liste Sous-groupes : Affichez, modifiez, copiez, exportez et supprimez les sous-groupes d’un groupe que vous gérez.
* Liste des états : Affichez et gérez les états de votre groupe.

Pour plus d’informations, voir [Création d’un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Nouveautés pour les administrateurs : Créer jusqu’à 14 niveaux de sous-groupes

Pour faciliter l’organisation de vos groupes Workfront en fonction de la hiérarchie de votre organisation, nous avons augmenté les niveaux de sous-groupes que vous pouvez créer dans un groupe de 3 à 14.

Pour plus d’informations, voir [Présentation des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Nouveautés pour les administrateurs : Nouvelle barre latérale de configuration

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront

La barre latérale gauche dans Configuration est désormais plus rapide et plus facile à utiliser. Elle tire parti de la disposition et des fonctionnalités de base que vous connaissez déjà. En plus d&#39;un aspect plus moderne, voici ce qui est nouveau :

* Un nouvel arrière-plan non blanc dans la barre latérale facilite la différenciation du reste de la zone Configuration.
* Les icônes dans la barre latérale sont un peu plus grandes et certaines sont reconçues afin de suggérer plus clairement ce que fait l’option.
* Un plus grand espace vertical entre les éléments de la barre latérale les rend plus faciles à lire.
* Vous pouvez réduire la barre latérale lorsque vous avez besoin d’espace dans la zone principale pour afficher et faire plus, par exemple afficher des colonnes supplémentaires. Et vous pouvez développer à nouveau la barre latérale lorsque vous avez besoin d’afficher les noms des fonctionnalités.
* Lorsque la barre latérale est réduite, seules les icônes de chaque fonction s’affichent. Pour afficher les sous-éléments sous un élément de la barre latérale principale, passez la souris sur son icône pour les afficher dans un menu déroulant. Par exemple, passez la souris sur l’icône Processus pour afficher un menu contenant les approbations et les chemins jalons.
* Vous pouvez accéder aux deux options de démarrage (Importer des données et Exporter des données) en un clic plus rapide. Ils ont quitté le système pour s’afficher au niveau principal de la barre latérale.

Pour plus d’informations sur l’utilisation de la zone Configuration, voir [Administration et configuration](../../../administration-and-setup/administration-and-setup.md).

## Inclure le numéro de cluster dans la zone Informations sur le client

En tant qu’administrateur Workfront, vous pouvez désormais facilement trouver le numéro de grappe dans Workfront, sans avoir à consacrer plus de temps et d’efforts à l’obtenir de notre équipe d’assistance. Nous avons ajouté un champ Configuration de grappe dans la zone Informations sur le client de la configuration.

Pour plus d’informations sur la zone Informations sur le client, voir [Configuration des informations de base pour votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Encodage Base64 pour les abonnements à des événements

Le champ de codage base64Encoding est un champ facultatif qui est utilisé pour activer le codage Base64 des payloads d’abonnement aux événements. Si une requête est effectuée à l’aide du champ de codage base64Encoding défini sur true, les objets newState et oldState de la payload sont fournis sous la forme de chaînes de codage Base64. Cette fonctionnalité peut s’avérer utile si votre réseau est configuré de manière à ne pas autoriser les caractères spéciaux dans les abonnements à des événements.

Pour plus d’informations, voir [API d’abonnement à un événement](../../../wf-api/general/event-subs-api.md).

## Suppression de la possibilité de créer des abonnements à des événements en double

Pour empêcher la diffusion de messages en double, vous ne pouvez plus créer de doublons d&#39;abonnements. De plus, les abonnements en double créés précédemment ont été supprimés.

Pour plus d’informations, voir [Questions fréquentes - Abonnements à un événement](../../../wf-api/general/event-subs-faq.md).
