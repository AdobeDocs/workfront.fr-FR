---
product-area: documents
navigation-topic: approvals
title: Vue d’ensemble du stockage d’entreprise Adobe
description: Vue d’ensemble du stockage d’entreprise Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: 7f17ffc179914747d29c4acb08b34341c5a4b7b4
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# Vue d’ensemble du stockage d’entreprise Adobe

Le stockage d’entreprise Adobe est une solution de stockage dans le cloud qui sert de référentiel central pour les ressources des produits d’entreprise Adobe. L’intégration de Workfront et Frame.io repose sur le stockage d’entreprise d’Adobe, ce qui permet une collaboration et une gestion des ressources transparentes entre ces plateformes.

Cette option de stockage ouvre également la voie à de futures intégrations de la gestion des ressources avec d’autres produits Adobe, tels que Adobe Creative Cloud.

## Principales fonctionnalités

* **Couche de stockage unifié** : le stockage d’entreprise Adobe agit comme un serveur principal de stockage partagé pour Workfront, Frame.io, Document Cloud et Creative Cloud. Cela permet une collaboration et une gestion des ressources transparentes sur ces plateformes.

* **Activation de Content supply chain** : le stockage d’entreprise d’Adobe est un composant fondamental pour la vision d’Adobe Content Supply chain, qui permet aux équipes de gérer les ressources en cours de travail sans avoir à effectuer de téléchargements manuels ou de rechargements dans diverses applications Adobe.

* **Autorisations et accès centralisés** : le stockage d’entreprise Adobe prend en charge les contrôles d’accès au niveau de l’entreprise, en s’intégrant à Adobe IMS (système Identity Management) pour des autorisations utilisateur sécurisées et évolutives.

* **Visibilité de bout en bout des ressources** : le stockage d’Assets dans le stockage d’entreprise Adobe peut être affiché et géré directement dans les applications Workfront, Frame.io et Creative Cloud, fournissant ainsi des métadonnées, un contrôle de version et des journaux d’audit cohérents.

* **Intégration aux workflows de révision et d’approbation** : le stockage d’entreprise Adobe permet des workflows de révision et d’approbation créatifs en servant de source de vérité pour toutes les ressources, en s’assurant que le suivi des commentaires et des approbations est centralisé.

* **Gestion évolutive du stockage et des quotas** : le stockage d’entreprise Adobe offre des options de stockage évolutives et un suivi unifié des quotas pour les produits Adobe.

## Intégration aux workflows de révision et d’approbation

L’intégration de Workfront et Frame.io utilise le stockage d’entreprise d’Adobe pour fournir une expérience de révision et d’approbation unifiée. Cette intégration permet aux coordinateurs de projet de gérer les projets et de planifier le travail dans Workfront, tandis que les créatifs, les spécialistes marketing et les parties prenantes peuvent examiner et approuver les ressources dans Frame.io. Cela permet de s’assurer que toutes les parties prenantes ont accès aux dernières versions des ressources et que les commentaires sont centralisés au même endroit.

Pour plus d’informations sur l’intégration de Workfront et de Frame.io, voir [Présentation de l’intégration de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).

## Différences entre le stockage d’entreprise Adobe et le stockage Workfront hérité

Les environnements Workfront existants associent un stockage d’entreprise Adobe et un stockage Workfront hérité. Tous les objets créés avant la publication du stockage d’entreprise d’Adobe utilisent le stockage Workfront hérité.

Une fois le stockage d’entreprise Adobe activé dans votre environnement, vous pouvez créer des projets de stockage d’entreprise Adobe et de stockage Workfront hérité.

>[!NOTE]
>
>Les nouveaux environnements nets disposent par défaut d’un stockage d’entreprise Adobe activé et n’ont pas la possibilité d’utiliser le stockage Workfront hérité.


### Documents

#### Zone des nouveaux documents

La nouvelle zone de documents est une zone de documents unifiée repensée pour le stockage d’entreprise d’Adobe.

Cette interface mise à jour simplifie la navigation, améliore la clarté et permet aux équipes de gérer plus facilement les révisions et les approbations dans un environnement unifié. Pour plus d’informations, voir la [présentation de la zone Documents](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Nouveau modèle d’autorisation de document

>[!IMPORTANT]
>
>Dans le stockage d’entreprise Adobe, les autorisations de document fonctionnent différemment du stockage Workfront hérité. Les documents héritent des autorisations du projet, de la tâche ou du problème auxquels ils sont liés.

Les documents ne peuvent pas être partagés individuellement. Au lieu de cela, le système génère automatiquement un dossier pour chaque tâche ou événement et hérite des autorisations de la tâche ou de l’événement. Tous les documents chargés vers la tâche ou l’événement sont stockés dans ce dossier généré.

Pour plus d’informations sur le nouveau modèle d’autorisation de document, voir [ Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Objets liés dans des dossiers

Au niveau du projet, les dossiers générés par le système affichent un objet lié. Le dossier est automatiquement nommé de la même manière que la tâche ou l’événement auquel il appartient. Les dossiers liés permettent au système de déterminer la tâche ou le problème sur lequel le dossier doit s’afficher.

Pour plus d’informations, voir [Fonctionnement des autorisations de document](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Objets Workfront

Le tableau ci-dessous compare les fonctionnalités du stockage d’entreprise Adobe et du stockage Workfront hérité pour les objets Workfront.

Les objets Workfront incluent les portfolios, les programmes, les projets, les modèles, les tâches et les événements.

| Stockage d’entreprise Adobe | Stockage Workfront hérité |
|---|---|
| <ul><li>Utilise le stockage d’entreprise Adobe</li><li>Intégré à Frame.io</li><li>Utilise la nouvelle expérience Documents</li><li>Applique des conventions de nommage strictes</li><li>Le partage direct de documents n’est pas disponible.</li><li>Les documents sont disponibles dans d’autres produits Adobe tels que Frame.io et Creative Cloud</li></ul> | <ul><li>Utilise le stockage Workfront</li><li>Utilise le lecteur de vérification</li><li>Prend en charge le partage de documents individuels</li></ul> |

### Déplacer, copier et convertir des objets

Vous pouvez déplacer, copier et convertir des objets Workfront entre des modèles de stockage similaires. Par exemple, vous pouvez déplacer une tâche d’un projet de stockage d’entreprise Adobe vers un autre projet de stockage d’entreprise Adobe. Vous ne pouvez pas déplacer une tâche d’un projet de stockage d’entreprise Adobe vers un projet de stockage Workfront hérité.

Ces actions sont disponibles à partir du menu Plus sur une tâche ou un événement. Chaque action respecte l’intégrité du document, l’héritage des autorisations et les règles de stockage d’entreprise Adobe.

## Activer le stockage d’entreprise d’Adobe

Les clients existants peuvent activer le stockage d’entreprise Adobe dans leur environnement lors du renouvellement du contrat. Pour plus d’informations sur l’activation du stockage d’entreprise Adobe, voir [ Activer le stockage d’entreprise Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Le stockage d’entreprise Adobe est activé par défaut pour les nouveaux clients qui n’ont pas la possibilité d’utiliser le stockage Workfront hérité.



## Considérations

* Il est possible que Workfront ne soit pas synchronisé avec Frame.io ou Creative Cloud. Par exemple, une ressource supprimée dans Workfront apparaît toujours dans Frame.io, contactez le support technique de Workfront pour resynchroniser votre environnement.


