---
product-area: documents
navigation-topic: approvals
title: Présentation de l’espace de stockage dans le cloud Adobe
description: Présentation de l’espace de stockage dans le cloud Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YOO4BspMzbMr8iPoXRBKK65IbU5yfpiJndNuYvYF5SM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 958
ht-degree: 0%

---

# Présentation de l’espace de stockage dans le cloud Adobe

Le stockage dans le cloud d’Adobe est une solution de stockage dans le cloud qui sert de référentiel central pour les ressources de l’ensemble des produits d’entreprise Adobe. L’intégration de Workfront et Frame.io repose sur le stockage cloud Adobe, ce qui permet une collaboration et une gestion des ressources transparentes entre ces plateformes.

Cette option de stockage ouvre également la voie à de futures intégrations de la gestion des ressources avec d’autres produits Adobe, tels que Adobe Creative Cloud.

## Principales fonctionnalités

* **Couche de stockage unifié** : le stockage cloud Adobe agit comme un serveur principal de stockage partagé pour Workfront, Frame.io, Document Cloud et Creative Cloud. Cela permet une collaboration et une gestion des ressources transparentes sur ces plateformes.

* **Activation de Content supply chain** : l’espace de stockage dans le cloud d’Adobe est un composant fondamental pour la vision d’Adobe Content Supply chain, qui permet aux équipes de gérer les ressources en cours de travail sans avoir à effectuer de téléchargements manuels ou de rechargements dans diverses applications Adobe.

* **Autorisations et accès centralisés** : le stockage dans le cloud Adobe prend en charge les contrôles d’accès au niveau de l’entreprise, en s’intégrant à Adobe IMS (système Identity Management) pour des autorisations utilisateur sécurisées et évolutives.

* **Visibilité de bout en bout des ressources** : Assets stocké dans l’espace de stockage cloud d’Adobe peut être affiché et géré directement dans les applications Workfront, Frame.io et Creative Cloud, fournissant ainsi des métadonnées, un contrôle de version et des journaux d’audit cohérents.

* **Intégration aux workflows de révision et d’approbation** : le stockage dans le cloud Adobe permet des workflows de révision et d’approbation créatifs en servant de source de vérité pour toutes les ressources, en s’assurant que le suivi des commentaires et des approbations est centralisé.

* **Stockage évolutif et gestion des quotas** : le stockage dans le cloud Adobe offre des options de stockage évolutives et un suivi unifié des quotas sur l’ensemble des produits Adobe.

## Intégration aux workflows de révision et d’approbation

L’intégration de Workfront et Frame.io utilise l’espace de stockage cloud d’Adobe pour fournir une expérience de révision et d’approbation unifiée. Cette intégration permet aux coordinateurs de projet de gérer les projets et de planifier le travail dans Workfront, tandis que les créatifs, les spécialistes marketing et les parties prenantes peuvent examiner et approuver les ressources dans Frame.io. Cela permet de s’assurer que toutes les parties prenantes ont accès aux dernières versions des ressources et que les commentaires sont centralisés au même endroit.

Pour plus d’informations sur l’intégration de Workfront et Frame.io, voir [Aperçu de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Différences entre le stockage dans le cloud Adobe et le stockage Workfront hérité

Les environnements Workfront existants combinent l’espace de stockage cloud Adobe et l’ancien espace de stockage Workfront. Tous les objets créés avant la publication de l’espace de stockage dans le cloud d’Adobe utilisent l’ancien stockage Workfront.

Une fois que vous avez activé le stockage dans le cloud Adobe dans votre environnement, vous pouvez créer des projets de stockage dans le cloud Adobe et des projets de stockage Workfront hérités.

>[!NOTE]
>
>Les nouveaux environnements nets disposent par défaut d’un stockage dans le cloud Adobe activé et n’ont pas la possibilité d’utiliser le stockage Workfront hérité.


### Documents

#### Zone Nouveaux documents

La nouvelle zone Documents est une zone de documents unifiés repensée pour le stockage dans le cloud Adobe.

Cette interface mise à jour simplifie la navigation, améliore la clarté et permet aux équipes de gérer plus facilement les révisions et les approbations dans un environnement unifié. Pour plus d’informations, voir la [présentation de la zone Documents](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Nouveau modèle d’autorisation de document

>[!IMPORTANT]
>
>Dans l’espace de stockage cloud Adobe, les autorisations de document fonctionnent différemment de l’espace de stockage Workfront hérité. Les documents héritent des autorisations du projet, de la tâche ou du problème auxquels ils sont liés.

Les documents ne peuvent pas être partagés individuellement. Au lieu de cela, le système génère automatiquement un dossier pour chaque tâche ou événement et hérite des autorisations de la tâche ou de l’événement. Tous les documents chargés vers la tâche ou l’événement sont stockés dans ce dossier généré.

Pour plus d’informations sur le nouveau modèle d’autorisation du document, voir [ Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage dans le cloud d’Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Objets liés dans des dossiers

Au niveau du projet, les dossiers générés par le système affichent un objet lié. Le dossier est automatiquement nommé de la même manière que la tâche ou l’événement auquel il appartient. Les dossiers liés permettent au système de déterminer la tâche ou le problème sur lequel le dossier doit s’afficher.

Pour plus d’informations, voir [Fonctionnement des autorisations de document](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Objets Workfront

Le tableau ci-dessous compare les fonctionnalités de l’espace de stockage dans le cloud Adobe et de l’ancien espace de stockage Workfront pour les objets Workfront.

Les objets Workfront incluent les portfolios, les programmes, les projets, les modèles, les tâches et les événements.

| Espace de stockage Adobe | Stockage Workfront hérité |
|---|---|
| <ul><li>Utilise le stockage dans le cloud d’Adobe</li><li>Intégré à Frame.io</li><li>Utilise la nouvelle expérience Documents</li><li>Applique des conventions de nommage strictes</li><li>Le partage direct de documents n’est pas disponible.</li><li>Les documents sont disponibles dans d’autres produits Adobe tels que Frame.io et Creative Cloud</li></ul> | <ul><li>Utilise le stockage Workfront</li><li>Utilise le lecteur de vérification</li><li>Prend en charge le partage de documents individuels</li></ul> |

### Déplacer, copier et convertir des objets

Vous pouvez déplacer, copier et convertir des objets Workfront entre des modèles de stockage similaires. Par exemple, vous pouvez déplacer une tâche d’un projet d’espace de stockage dans le cloud Adobe vers un autre projet d’espace de stockage dans le cloud Adobe. Vous ne pouvez pas déplacer une tâche d’un projet de stockage dans le cloud Adobe vers un projet de stockage Workfront hérité.

Ces actions sont disponibles à partir du menu Plus sur une tâche ou un événement. Chaque action respecte l’intégrité du document, l’héritage des autorisations et les règles de stockage dans le cloud d’Adobe.

## Activer le stockage dans le cloud d’Adobe

Vous devez utiliser une version de Workfront prenant en charge l’espace de stockage dans le cloud Adobe. Si votre organisation ne dispose pas déjà d’une version prise en charge, contactez votre représentant de compte Adobe.

Pour plus d’informations sur l’activation de l’espace de stockage cloud Adobe dans votre environnement, voir [Activer l’espace de stockage cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Le stockage dans le cloud Adobe est activé par défaut pour les nouveaux clients qui n’ont pas la possibilité d’utiliser le stockage Workfront hérité.



## stockage dans le cloud Adobe dans les environnements sandbox

L’espace de stockage dans le cloud d’Adobe est disponible dans [!DNL Workfront] environnements sandbox afin que vous puissiez le tester avant de l’activer en production. Cependant, la visionneuse Frame.io n’étant pas disponible dans le sandbox, l’expérience complète de révision et d’approbation unifiée doit être validée en production.

Si vous disposez d’un sandbox d’actualisation personnalisé, vous devez l’actualiser après la mise à niveau vers une version de Workfront qui prend en charge l’espace de stockage dans le cloud Adobe pour accéder à la fonctionnalité d’espace de stockage dans le sandbox d’Adobe. Pour plus d’informations, voir [Environnement  [!DNL Adobe Workfront]  sandbox d’actualisation personnalisée](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

## Considérations

* Il est possible que Workfront ne soit pas synchronisé avec Frame.io ou Creative Cloud. Par exemple, une ressource supprimée dans Workfront mais toujours affichée dans Frame.io, contactez l’assistance Workfront pour resynchroniser votre environnement.


