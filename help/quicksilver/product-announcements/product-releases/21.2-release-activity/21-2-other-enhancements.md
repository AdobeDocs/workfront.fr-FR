---
content-type: release-notes
keywords: notes,trimestriel,mise à jour,version
navigation-topic: 2021-2-release-activity
title: 21.2 Autres améliorations
description: Cette page décrit toutes les autres améliorations apportées à la version 21.2 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir Vue d’ensemble de la version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 100%

---

# 21.2 Autres améliorations

Cette page décrit toutes les autres améliorations apportées à la version 21.2 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, voir [Vue d’ensemble de la version 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Nous devenons officiellement Adobe Workfront.

Workfront s’appelle maintenant Adobe Workfront.

Les zones les plus visibles de l’application Adobe Workfront et nos sites web accessibles aux clientes et clients reflètent ce changement. D’autres zones suivront le pas.

**Zones renommées**

* Écran de connexion, Navigation supérieure, Relecture
* Interface utilisateur des modèles de disposition, Menu principal, Export des formulaires personnalisés (disponible uniquement dans la nouvelle expérience Adobe Workfront)
* Application mobile Workfront (iOS et Android)

Zones bientôt renommées

* Applications de relecture pour ordinateur de bureau et mobile
* Exports de PDF pour les listes et les rapports
* Icône Favicon dans l’onglet du navigateur

**Zones renommées ultérieurement**

* Notifications par e-mail

## Validation de la liste autorisée d’e-mails

>[!NOTE]
>
>Disponible uniquement dans la nouvelle version d’Adobe Workfront.

Si vous utilisez la liste autorisée d’e-mails, les nouvelles adresses e-mails et celles mises à jour sont désormais validées par rapport à la liste autorisée. Lorsque vous ajoutez un nouvel utilisateur ou une nouvelle utilisatrice, ou modifiez une personne existante, et que vous saisissez un domaine d’adresse e-mail qui ne figure pas dans la liste autorisée, un message vous informe que cette personne ne recevra pas d’e-mails. Vous pouvez toujours enregistrer le profil utilisateur, mais vous devez ajouter le domaine à la liste autorisée pour que la personne puisse recevoir des e-mails.

Pour plus d’informations, consultez la section [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nouvel aspect des en-têtes d’objet

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement de production le 10 mars 2020.
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Pour renforcer davantage la hiérarchie des informations et aider les utilisateurs et utilisatrices à mieux comprendre la page sur laquelle ils se trouvent, chaque en-tête d’objet dispose désormais des éléments suivants :

* Icônes colorées et plus modernes pour chaque type d’objet
* Type d’objet répertorié au-dessus du nom de l’objet
* Style et taille de texte de police mis à jour
* Autres améliorations de style mineures

Auparavant, il n’existait pas d’icône et un badge portant le nom de l’objet s’affichait en regard du titre de l’objet.

Les en-têtes de page des zones de la nouvelle expérience Workfront (par exemple, Analytique améliorée, gestion des ressources, etc.) adoptent également ce nouvel aspect.

Pour en savoir plus sur les nouveaux en-têtes d’objet dans la nouvelle expérience Workfront, consultez la section [Nouveaux en-têtes d’objet](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Mises à jour des réponses à la recherche de statuts d’objet

Workfront stocke désormais les statuts des objets d’une nouvelle manière.

Ces modifications n’affectent pas la manière dont les demandes de recherche de statuts sont effectuées. Toutefois, les requêtes d’API contenant une recherche de statuts d’objet renverront une liste incomplète de statuts de groupe.

Pour plus d’informations, consultez la section [Modifications principales de l’API : réponses à la recherche de statuts](../../../wf-api/api/api-changes-search.md).

## Mise à jour des payloads d’abonnement aux événements de manière à inclure tous les champs se terminant par ID

Tous les payloads d’abonnement aux événements contiennent désormais chaque champ qui se termine par « ID ».

Gardez à l’esprit que chaque objet possède son propre jeu de champs associés, y compris un jeu de champs unique se terminant par ID. Cela signifie que même si chaque payload contient tous les champs associés de cet objet qui se terminent par ID, chaque objet a un jeu différent de champs qui se terminent par ID.

## La version bêta des plans directeurs est désormais disponible dans l’environnement de prévisualisation.

>[!NOTE]
>
>Cette fonctionnalité ne sera pas disponible de manière générale dans l’environnement de production avant la version 21.3, qui sera publiée plus tard dans l’année. Disponible uniquement dans la nouvelle version d’Adobe Workfront.

Les plans directeurs fournissent des éléments de base pour vous aider à créer un système de gestion du travail qui s’adapte à vos besoins. Les administrateurs et administratrices système peuvent parcourir le catalogue de plans directeurs et installer des modèles de projet prêts à l’emploi.

Pour plus d’informations, consultez la section [Plans directeurs](../../../administration-and-setup/blueprints/blueprints.md).
