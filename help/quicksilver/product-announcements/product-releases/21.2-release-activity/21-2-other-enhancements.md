---
content-type: release-notes
keywords: notes,trimestriel,mise à jour,version
navigation-topic: 2021-2-release-activity
title: Autres améliorations (version 21.2)
description: Cette page décrit toutes les autres améliorations apportées à la version 21.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, reportez-vous à la présentation de la version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 1%

---

# Autres améliorations (version 21.2)

Cette page décrit toutes les autres améliorations apportées à la version 21.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 10 mai 2021. Pour obtenir la liste de toutes les modifications disponibles avec la version 21.2, consultez la [présentation de la version 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Nous sommes maintenant officiellement Adobe Workfront

Workfront a été renommé Adobe Workfront.

Les zones les plus importantes de l’application Adobe Workfront et de nos sites web accessibles aux clients sont désormais mises à jour. D’autres zones seront bientôt mises à jour.

**Zones mises à jour**

* Écran de connexion, Navigation supérieure, Vérification
* Interface utilisateur des modèles de mise en page, menu principal, exportation Forms personnalisée (disponible uniquement dans la nouvelle expérience Adobe Workfront)
* Application mobile Workfront (iOS et Android)

Mise à jour des zones bientôt

* Application de test pour ordinateur de bureau et mobile
* Exports de PDF pour les listes et les rapports
* Icône Favicon dans l’onglet du navigateur

**Zones mises à jour ultérieurement**

* Notifications par e-mail

## Validation de la liste autorisée de messagerie

>[!NOTE]
>
>Disponible uniquement dans la nouvelle expérience Adobe Workfront.

Si vous utilisez la liste autorisée de courrier électronique, les adresses électroniques des utilisateurs nouvelles et mises à jour sont désormais validées par rapport à la liste autorisée. Lorsque vous ajoutez un nouvel utilisateur ou modifiez un utilisateur existant et que vous saisissez un domaine d’adresse électronique qui ne figure pas dans la liste autorisée, un message vous informe que l’utilisateur ne recevra pas de messages électroniques. Vous pouvez toujours enregistrer le profil utilisateur, mais vous devez ajouter le domaine à la liste autorisée pour que l’utilisateur puisse recevoir des courriers électroniques.

Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Nouvelle apparence des en-têtes d’objet

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement de production le 10 mars 2020.
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Pour renforcer davantage la hiérarchie des informations et aider les utilisateurs à mieux comprendre la page sur laquelle ils se trouvent, chaque en-tête d’objet dispose désormais :

* Des icônes colorées et plus modernes pour chaque type d’objet
* Type d’objet répertorié au-dessus du nom de l’objet.
* Style et taille de texte de police mis à jour
* Autres changements de style mineurs

Auparavant, il n’existait pas d’icône et un badge portant le nom de l’objet s’affichait à droite du titre de l’objet.

Les en-têtes de page des zones de la nouvelle expérience Workfront (par exemple, l’analyse améliorée, la gestion des ressources, etc.) ont également cette apparence mise à jour.

Pour en savoir plus sur les nouveaux en-têtes d’objet dans la nouvelle expérience Workfront, voir [Nouveaux en-têtes d’objet](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Mises à jour des réponses de recherche d’état d’objet

Workfront stocke désormais les statuts des objets d’une nouvelle manière.

Ces modifications n’affectent pas la manière dont les demandes de recherche d’état sont effectuées. Toutefois, les requêtes d’API contenant une recherche d’état d’objet renverront une liste incomplète d’états de groupe.

Pour plus d’informations, voir [Modifications de l’API Core : réponses de recherche d’état](../../../wf-api/api/api-changes-search.md) .

## Mise à jour des payloads d’abonnement d’événement pour inclure tous les champs se terminant par ID

Tous les payloads d’abonnement d’événement contiennent désormais chaque champ qui se termine par &quot;ID&quot;.

Il est important de noter que chaque objet possède son propre ensemble unique de champs associés, qui comprend un ensemble unique de champs associés se terminant par ID. Cela signifie que même si chaque payload contient tous les champs associés de cet objet qui se terminent par ID, chaque objet a un ensemble différent de champs qui se terminent par ID.

## La version bêta des plans directeurs est désormais disponible dans Aperçu.

>[!NOTE]
>
>Cette fonctionnalité ne sera généralement pas disponible dans l’environnement de production avant la version 21.3, plus tard dans l’année. Disponible uniquement dans la nouvelle expérience Adobe Workfront.

Les plans directeurs fournissent des éléments de base pour vous aider à créer un système de gestion du travail qui s’adapte à vos besoins. Les administrateurs système peuvent parcourir le catalogue de plans directeurs et installer des modèles de projet prêts à l’emploi.

Pour plus d’informations, voir [Blueprints](../../../administration-and-setup/blueprints/blueprints.md).
