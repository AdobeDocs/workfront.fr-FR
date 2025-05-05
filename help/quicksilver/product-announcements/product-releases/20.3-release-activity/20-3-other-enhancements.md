---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: Autres améliorations (version 20.3)
description: Cette page décrit toutes les autres améliorations apportées par la version 20.3 à l’environnement de production. Ces améliorations ont été mises à disposition dans l’environnement de production au cours de la semaine du 10 août 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 99%

---

# Autres améliorations (version 20.3)

Cette page décrit toutes les autres améliorations apportées par la version 20.3 à l’environnement de production. Ces améliorations ont été mises à disposition dans l’environnement de production au cours de la semaine du 10 août 2020.

Pour une liste de tous les changements disponibles avec la version 20.3, voir [Vue d’ensemble de la version 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Partager un calendrier avec un lien privé

Pour faciliter le partage de calendriers dans Workfront, vous pouvez partager un lien privé qui permet aux utilisateurs et utilisatrices d’accéder directement au calendrier. Le calendrier doit être partagé avec l’utilisateur ou l’utilisatrice, qui doit alors se connecter pour le consulter.

Auparavant, vous pouviez partager une URL publique qui ne nécessitait pas de connexion pour afficher le calendrier.

Pour plus d’informations, voir [Partager un rapport de calendrier](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Nouvelle zone Brouillons lors de la création de demandes

Pour une utilisation des demandes plus flexible, Workfront enregistre désormais automatiquement chaque demande créée en tant que brouillon dans la nouvelle zone Brouillons. Si vous ne disposez pas de toutes les informations nécessaires pour terminer la nouvelle demande, vous pouvez la laisser en tant que brouillon, y revenir et la terminer ultérieurement. Workfront enregistre une demande par rubrique de file d’attente dans la nouvelle zone Brouillons. Les brouillons de demande peuvent être enregistrés aussi longtemps que nécessaire, jusqu’à ce que vous décidiez de les terminer et de les envoyer. Vous pouvez également supprimer ou repositionner la zone Brouillons du panneau de gauche à l’aide d’un modèle de mise en page.

Pour plus d’informations sur la création de demandes, voir [Créer et envoyer des demandes Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Pour la version préliminaire, si un modèle de mise en page personnalisé vous est attribué, vous devez ajouter la zone Brouillons de vos demandes en modifiant votre modèle de mise en page.

## Développer ou réduire les éléments de la feuille de temps

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Afin de faciliter la gestion des feuilles de temps avec plusieurs éléments, vous pouvez désormais développer ou réduire tous les éléments en cliquant sur un bouton.

Auparavant, vous deviez cliquer sur chaque élément individuellement.

Pour plus d’informations, voir [Consigner les heures](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ignorer les dates effectives dans les calendriers Workfront

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement de prévisualisation le 5 juin 2020. Elle sera disponible dans l’environnement de production le 19 juin 2020.

Pour un meilleur contrôle de l’affichage des objets dans les rapports de calendrier, vous pouvez choisir d’ignorer les dates effectives même lorsqu’elles sont disponibles.

Auparavant, ce calendrier utilisait automatiquement les dates effectives une fois disponibles.

Pour plus d’informations, voir [Vue d’ensemble des rapports de calendrier](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Utiliser les champs de date personnalisés dans un rapport de calendrier

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement de prévisualisation le 29 mai 2020. Elle sera disponible dans l’environnement de production le 12 juin 2020.

Pour faciliter la visualisation et la gestion de votre travail quotidien avec les calendriers, les champs de date personnalisés sont désormais disponibles en tant qu’option de date.

Auparavant, vous ne pouviez gérer votre calendrier qu’avec des dates prévisionnelles et prévues lorsque les dates effectives n’étaient pas disponibles.

Pour plus d’informations, voir [Utiliser les champs de date personnalisés dans un rapport de calendrier](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (ou si vous utilisez Workfront Classic, voir [Utiliser les champs de date personnalisés dans un rapport de calendrier](https://experienceleague.adobe.com/fr/docs/workfront/using/home)).

## Modifications d’e-mails

**Modifications d’e-mails sortants :** tous les e-mails de Workfront proviennent de notifications@my.workfront.com. Cela inclut les alertes automatisées et la communication entres utilisateurs et utilisatrices.

Auparavant, les administrateurs et administratrices système pouvaient ajouter une adresse e-mail personnalisée dans la zone Configuration de l’e-mail.

**Modifications des réponses e-mail entrantes POP :** les administrateurs et administratrices système n’auront plus la possibilité de configurer un serveur e-mail POP personnalisé pour les réponses e-mail entrantes aux notifications.

Pour plus d’informations, voir [Usurpation d’adresses e-mail et modifications des réponses e-mail POP](https://experienceleague.adobe.com/fr/docs/workfront/using/home).

## La technique DKIM (DomainKeys Identified Mail) est désormais incluse dans les e-mails Workfront sortants.

Une technique d’authentification des e-mails (DKIM) sera incluse sur tous les e-mails sortants. Cette signature DKIM n’est pas visible pour l’utilisateur final ou l’utilisatrice finale mais permet la validation à l’échelle du serveur et renforce notre framework d’authentification existant.

## Mises à jour de l’inscription dans la nouvelle expérience Workfront

Pour faciliter l’inscription des utilisateurs et utilisatrices dans la nouvelle expérience Workfront, les administrateurs et administratrices de groupes ont désormais accès à l’inscription et à la désinscription des personnes appartenant aux groupes sous leur gestion.

Il existe également un lien Détails sur l’utilisateur ou l’utilisatrice qui affiche les informations suivantes :

* Nom
* Fonction
* Adresse e-mail
* Image de profil

## Nouveautés pour les administrateurs et les administratrices : Personnaliser le branding de Workfront pour des groupes, des équipes, des fonctions et des utilisateurs et utilisatrices spécifiques

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Désormais, vous pouvez utiliser un modèle de disposition pour modifier les logos de la zone de navigation supérieure et du menu principal pour des groupes, des équipes, des fonctions et des utilisateurs et utilisatrices spécifiques ayant leur propre branding.

Pour plus d’informations, voir [Personnaliser le branding de votre instance Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Les administrateurs et administratrices de groupes peuvent créer et gérer des processus d’approbation.

Afin de garantir une plus grande autonomie et un meilleur contrôle des workflows de ses groupes, un administrateur ou une administratrice de groupes peut désormais accéder à la zone Processus d’approbation dans Configuration et créer et modifier des processus d’approbation pour un groupe qu’il gère. Ces processus d’approbation sont basés sur les status de ce groupe.

Pour s’assurer que les administrateurs et administratrices de groupes ne modifient pas par inadvertance les processus d’approbation utilisés dans tout le système ou créés par d’autres groupes, ils ne peuvent accéder qu’aux processus d’approbation associés aux groupes qu’ils gèrent.

Pour plus d’informations, voir [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Pour les administrateurs et administratrices : la nouvelle page Groupes facilite la création et la gestion des groupes

Les administrateurs et administratrices de groupes peuvent gérer plus facilement les groupes, maintenant que tout ce dont ils ont besoin se trouve sur la nouvelle page Groupes. Il n’est plus nécessaire de naviguer entre les différentes zones de superposition et les pages de configuration pour créer et modifier des groupes.

Voici les principaux points forts :

* Détails du groupe : affichez et modifiez des informations de base sur le groupe, telles que le nom, la description, les noms des administrateurs et administratrices du groupe et si le groupe est public ou privé.
* Liste des membres du groupe : affichez toutes les personnes membres du groupe et utilisez la nouvelle barre d’outils pour ajouter, supprimer, exporter, activer et désactiver rapidement les appartenances. Vous pouvez également modifier les profils des membres et leur envoyer des commentaires de mise à jour.
* Champ Administrateur ou administratrice de groupes dans l’en-tête : lorsque vous affichez un groupe que vous gérez, affectez ou annulez rapidement l’affectation d’une personne membre du groupe en tant qu’administrateur ou administratrice de groupes. Vous pouvez également le faire dans la liste des membres du groupe à l’aide de la nouvelle colonne Rôle du groupe.
* Liste des sous-groupes : affichez, modifiez, copiez, exportez et supprimez les sous-groupes d’un groupe que vous gérez.
* Liste des status : affichez et gérez les status de votre groupe.

Pour plus d’informations, voir [Créer un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Nouveauté pour les administrateurs et les administratrices : créer jusqu’à 14 niveaux de sous-groupes

Pour faciliter l’organisation de vos groupes Workfront en fonction de la hiérarchie de votre organisation, nous avons augmenté de 3 à 14 le nombre de niveaux de sous-groupes que vous pouvez créer dans un groupe.

Pour plus d’informations, voir [Vue d’ensemble des groupes](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Nouveauté pour les administrateurs et les administratrices : nouvelle barre latérale dans Configuration

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

La barre latérale gauche dans Configuration est désormais plus rapide et plus facile à utiliser. Elle tire parti de la disposition et des fonctionnalités de base que vous connaissez déjà. En plus d’un aspect plus moderne, voici les autres nouveautés :

* Un nouvel arrière-plan blanc cassé dans la barre latérale facilite la différenciation du reste de la zone Configuration.
* Les icônes dans la barre latérale sont un peu plus grandes et certaines sont reconçues afin de suggérer plus clairement ce que fait l’option.
* Un plus grand espace vertical entre les éléments de la barre latérale les rend plus faciles à lire.
* Vous pouvez réduire la barre latérale lorsque vous avez besoin d’espace dans la zone principale pour afficher plus et effectuer davantage d’actions, par exemple pour afficher d’autres colonnes. Vous pouvez également redévelopper la barre latérale lorsque vous avez besoin d’afficher les noms des fonctionnalités.
* Lorsque la barre latérale est réduite, seules les icônes de chaque fonction s’affichent. Pour afficher les sous-éléments sous un élément de la barre latérale principale, pointez sur son icône pour les afficher dans un menu déroulant. Par exemple, pointez sur l’icône Processus pour afficher un menu contenant les approbations et les chemins jalonnés.
* Vous pouvez accéder aux deux options de lancement (Importer des données et Exporter des données) en un clic plus rapide. Elles ont quitté le système pour s’afficher au niveau principal de la barre latérale.

Pour plus d’informations sur l’utilisation de la zone Configuration, voir [Administration et configuration](../../../administration-and-setup/administration-and-setup.md).

## Inclure le numéro de cluster dans la zone Infos client

En tant qu’administrateur ou administratrice Workfront, vous pouvez désormais facilement trouver le numéro de cluster dans Workfront, sans avoir à consacrer plus de temps et d’efforts à l’obtenir de notre équipe d’assistance. Nous avons ajouté un champ Configuration du cluster dans la zone Infos client de la configuration.

Pour plus d’informations sur la zone Infos client, voir [Configurer des informations de base pour votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Encodage Base64 pour les abonnements à des événements

Le champ de codage base64Encoding est un champ facultatif qui est utilisé pour activer le codage Base64 des payloads d’abonnement aux événements. Si une demande est effectuée à l’aide du champ de codage base64Encoding défini sur true, les objets newState et oldState du payload sont fournis sous la forme de chaînes de codage Base64. Cette fonctionnalité peut s’avérer utile si votre réseau est configuré de manière à ne pas autoriser les caractères spéciaux dans les abonnements à des événements.

Pour plus d’informations, voir [API d’abonnement à un événement](../../../wf-api/general/event-subs-api.md).

## Suppression de la possibilité de créer des abonnements à des événements en double

Pour empêcher la diffusion de messages en double, vous ne pouvez plus créer d’abonnements en double. De plus, les abonnements en double créés précédemment ont été supprimés.

Pour plus d’informations, voir [Questions fréquentes - Abonnements aux événements](../../../wf-api/general/event-subs-faq.md).
