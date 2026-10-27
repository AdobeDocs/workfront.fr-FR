---
product-area: documents
navigation-topic: approvals
title: Nouveautés du stockage dans le cloud Adobe
description: Découvrez les principales différences sur les objets d’espace de stockage Adobe dans le cloud, notamment la nouvelle zone Documents, la visionneuse Frame.io, les autorisations de document, les règles de dénomination des objets, le quota de stockage et Workfront Fusion.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 2b5d95ed0a5c72062700bf026a18b8301e4be421
workflow-type: tm+mt
source-wordcount: '1702'
ht-degree: 0%
---
# Nouveautés du stockage dans le cloud Adobe

Avec l’espace de stockage dans le cloud d’Adobe, votre environnement peut contenir deux types d’objets : des objets sur l’espace de stockage Workfront hérité (les objets dont vous disposez aujourd’hui) et des objets créés à l’aide de l’espace de stockage dans le cloud d’Adobe. La nouvelle zone Documents, la visionneuse Frame.io et les autres comportements décrits ici s’appliquent uniquement aux objets qui utilisent l’espace de stockage dans le cloud Adobe.

Pour obtenir une orientation sur le déplacement, voir [Déplacer vers Workfront sur l’espace de stockage dans le cloud d’Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Comprendre le stockage Workfront hérité et le stockage dans le cloud Adobe

À un niveau élevé, les deux modèles de stockage diffèrent en ce qui concerne l’emplacement des données, les produits Adobe qui peuvent les voir et les fonctionnalités disponibles :

|  | Objet sur l’ancien stockage Workfront | Objet sur l’espace de stockage dans le cloud Adobe |
|---|---|---|
| Serveur principal de stockage | Workfront uniquement | Espace de stockage Adobe |
| Visibilité sur l’ensemble des produits | Workfront uniquement | Workfront, Frame.io et Creative Cloud |
| Fonction | Fonctionnalités héritées | Nouvelle fonctionnalité |

Les objets créés avant l’espace de stockage dans le cloud d’Adobe sont conservés par défaut sur l’espace de stockage Workfront hérité. Les comportements décrits dans cet article s’appliquent uniquement aux objets d’espace de stockage dans le cloud Adobe que vous et vos utilisateurs créez une fois que l’espace de stockage dans le cloud Adobe est la valeur par défaut.

## Résumé des différences

Le plus grand changement au quotidien avec l’espace de stockage dans le cloud d’Adobe est la nouvelle zone Documents et la visionneuse Frame.io qui alimente la révision et l’approbation qu’elle contient. D’autres différences affectent la gestion des objets, des documents et des révisions. Chaque zone du tableau suivant renvoie vers la section détaillée ci-dessous.

| Zone | Qu’est-ce qui est différent ? | Ce qu’il faut savoir |
|---|---|---|
| [la zone Nouveaux documents](#the-new-documents-area) | Une zone Documents unifiée et repensée remplace l’ancienne zone Documents. | Il n’y a pas de zone globale Documents. Vous accédez aux documents d&#39;un programme, d&#39;un portefeuille, d&#39;un projet, d&#39;une tâche ou d&#39;un événement. |
| [Autorisations de document](#document-permissions) | Les documents héritent des autorisations du projet, de la tâche ou du problème auxquels ils sont liés. | Vous ne pouvez pas partager ni définir d’autorisations sur des documents individuels. Vous gérez tous les accès par le biais de la fenêtre modale de partage d’objet dans Workfront, qui applique en cascade des dossiers de documents générés par le système. |
| [Mappage des autorisations d’objet](#object-permissions-mapping) | Les autorisations Gérer et Contribuer sont toutes deux mappées à Modifier et partager dans Frame.io. Affichez les mappages en commentaire uniquement. | Vous gérez les autorisations dans Workfront. Les utilisateurs des fonctions Gérer et Contribuer bénéficient de la fonctionnalité de partage externe de Frame.io. |
| [Observateur de révision et d’approbation](#review-and-approval-viewer) | La visionneuse Frame.io remplace la visionneuse de relecture Workfront. | Il est inclus pour tous les utilisateurs de Workfront, y compris les utilisateurs externes affectés à une révision ou à une approbation. Il prend en charge les balises, les commentaires horodatés, l’historique des versions, les appareils mobiles, les formats de plus de 40 et les fichiers d’une capacité maximale de 500 Go. |
| [Règles de dénomination des objets](#object-naming-rules) | Des règles de nommage strictes s’appliquent : noms uniques dans un portfolio ou un projet, aucun caractère spécial, aucun point ou espace de fin et une limite de 255 caractères. | Workfront renomme automatiquement les objets en cas de conflit. Contrôlez les modèles qui génèrent de nouveaux noms et une nouvelle structure de projet. |
| [Portabilité des objets](#object-portability) | Dans la plupart des scénarios, vous ne pouvez déplacer, copier et convertir des objets qu’entre des modèles de stockage similaires. | Vous pouvez convertir un objet hérité en espace de stockage Adobe dans trois cas spécifiques. Les documents et les dossiers de documents ne sont pas déplacés du stockage hérité pendant la conversion. |
| [Fonctionnalités non disponibles](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, la visionneuse de documents Workfront, les documents favoris et les documents de demande ne font pas partie de l’expérience. | Les objets hérités conservent ces fonctionnalités. Workfront Proof ne recevra pas de nouvel investissement et sera mis hors service dans une version ultérieure. |
| [Quota de stockage](#storage-quota) | Le stockage est mis en pool pour les projets Workfront hérités et les projets de stockage dans le cloud Adobe, à 60 Go par utilisateur sous licence sans limite stricte. | Les administrateurs système peuvent afficher l&#39;utilisation du stockage sur la page Informations sur le client de la configuration. |
| [Limite de révision vidéo annuelle](#annual-video-review-cap) | Au niveau de l’entreprise, les demandes de BAT vidéo sont limitées à 10 % des licences d’utilisation payantes de Workfront (Standard et Light). | Une fois la limite atteinte, vous ne pouvez plus créer de nouvelles critiques vidéo avant la prochaine période annuelle. Vous recevez des notifications in-app à 80 % et 100 %. La limite ne s&#39;applique pas aux clients Frame.io Enterprise. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | Les scénarios Fusion existants basés sur des BAT ne fonctionnent pas automatiquement avec les projets de stockage dans le cloud Adobe. | Les scénarios définis pour les projets hérités continuent de fonctionner. Chaque scénario affecté emprunte l’un des trois chemins suivants : modifier, recréer ou supprimer. |

## La nouvelle zone Documents

La nouvelle zone Documents est une expérience de documents unifiée conçue pour le stockage dans le cloud Adobe. Il simplifie la navigation, consolide les activités de révision et d’approbation et constitue le point d’entrée de la visionneuse Frame.io.

La zone globale Documents ne fait pas partie de la nouvelle expérience . Dans les projets de stockage dans le cloud Adobe, vous accédez aux documents d’un programme, d’un portfolio, d’un projet, d’une tâche ou d’un événement.

Pour plus d’informations, voir [la zone Documents](/help/quicksilver/documents/managing-documents/documents-area.md).

## Autorisations de documents

Les autorisations de document sont fondamentalement différentes sur les projets de stockage dans le cloud Adobe :

* Vous ne pouvez pas partager ni définir d’autorisations sur des documents individuels. Au lieu de cela, les autorisations sont appliquées aux dossiers de documents générés par le système qui contiennent les documents.
* Les dossiers de documents générés par le système héritent des autorisations de leur projet, tâche ou problème parent.
* Les sous-dossiers héritent des autorisations du dossier de documents parent généré par le système.
* Les sous-tâches n’héritent pas des autorisations des tâches parents. Vous devez être ajouté directement à une sous-tâche pour accéder à son dossier de documents généré par le système.

Pour plus d’informations sur le fonctionnement des autorisations de document, voir [Présentation des autorisations d’objet et des niveaux d’accès pour le modèle de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Mappage des autorisations d’objet

Les autorisations sont définies dans Workfront et s’étendent dans un sens jusqu’à Frame.io. Vous ne pouvez pas inviter des utilisateurs à un projet de stockage dans le cloud Adobe dans Frame.io ni modifier les autorisations utilisateur dans Frame.io.

>[!TIP]
>
>Formez les coordinateurs de projet à l’idée que l’accès à Frame.io reflète en aval les autorisations Workfront. Si une personne concernée signale qu’elle ne peut pas accéder à une révision d’un projet de stockage dans le cloud Adobe, le correctif se trouve dans Workfront, et non dans Frame.io.

Le tableau suivant met en correspondance les autorisations d’objet Workfront avec les autorisations Frame.io :

| Autorisation Workfront | Autorisation Frame.io |
|---|---|
| Gérer | Modifier et partager |
| Contribuer | Modifier et partager |
| Afficher | Commentaire uniquement |

Gérez et contribuez mappent pour modifier et partager dans Frame.io. Lorsque vous passez en revue vos modèles de partage pour les projets de stockage dans le cloud Adobe, déterminez s’il est conforme à votre modèle de gouvernance que les contributeurs disposent des mêmes fonctionnalités de révision que les responsables, y compris le partage externe.

Pour plus d’informations, voir [Présentation des autorisations d’objet et des niveaux d’accès pour le modèle de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).

## Observateur de révision et d’approbation

Sur les objets d’espace de stockage Adobe, la visionneuse Frame.io est la surface de révision et d’approbation à la place de Workfront Proof. La visionneuse Frame.io est incluse sans frais supplémentaires pour tous les utilisateurs de Workfront, y compris les utilisateurs externes qui sont affectés à une révision ou une approbation.

La visionneuse Frame.io fournit les éléments suivants :

* Outils de balisage et de commentaires, notamment le dessin à main levée et les formes standard telles que les cercles, les flèches et les carrés
* Commentaires horodatés avec précision d’image pour les révisions vidéo
* Historique des versions et comparaison des versions
* Accès mobile pour les révisions et les approbations en cours de route
* Prise en charge de plus de 40 formats de fichiers, y compris tous les types courants de fichiers vidéo, image, audio, PDF et Microsoft Office, avec lecture native pour les formats vidéo professionnels tels que ProRes, H.265 et DNxHD, et prise en charge de fichiers jusqu’à 500 Go

## Règles de dénomination des objets

L’espace de stockage dans le cloud Adobe applique des règles structurelles et de dénomination strictes pour maintenir la cohérence de la couche de stockage entre les produits Adobe. Ces règles s’appliquent aux objets que vous créez dans les projets d’espace de stockage Adobe. Les projets hérités existants conservent leurs noms actuels.

Les règles suivantes s’appliquent aux projets de stockage dans le cloud Adobe :

| Règle | Détail |
|---|---|
| Noms de programmes et de projets uniques | Les programmes et les projets ne peuvent pas porter le même nom s&#39;ils appartiennent au même portefeuille. |
| Noms de documents uniques | Les documents ne peuvent pas porter le même nom s&#39;ils appartiennent au même projet. Les noms de document doivent être uniques dans le même parent de la hiérarchie des dossiers. |
| Caractères interdits | Les programmes, portfolios, projets, modèles, tâches, événements, dossiers de documents et documents ne peuvent pas contenir les caractères spéciaux suivants : `\ / : * ? " \| < >` |
| Caractères de fin | Les programmes, portfolios, projets, modèles, tâches, événements et dossiers de documents ne peuvent pas avoir de noms qui se terminent par un point ou un espace. |
| Limite de longueur du nom | Les noms d’objet sont limités à 255 caractères. |

Si un nom entre en conflit avec ces règles, Workfront renomme automatiquement l’objet pour résoudre le conflit.

>[!TIP]
>
>Si vous créez des projets de stockage dans le cloud Adobe à partir de modèles, passez en revue vos modèles existants afin que les noms de projet et la structure qu’ils génèrent respectent les règles ci-dessus.

## Portabilité des objets

Dans la plupart des scénarios, vous ne pouvez déplacer, copier et convertir des objets Workfront qu’entre des modèles de stockage similaires. Par exemple, vous pouvez déplacer une tâche d’un projet d’espace de stockage dans le cloud Adobe vers un autre projet d’espace de stockage dans le cloud Adobe. Dans trois cas spécifiques, vous pouvez convertir un objet de stockage Workfront hérité en espace de stockage dans le cloud Adobe.

<!--
During a group-scoped rollout, only members of the group that has Adobe cloud storage can convert an Adobe cloud storage object, such as a request, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."

For more information, see [Plan your Adobe cloud storage rollout](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md).
-->

Pour plus d’informations, voir [Conversion d’objets hérités en espace de stockage Adobe](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md).

## Fonctionnalités non disponibles sur les objets d’espace de stockage dans le cloud Adobe

Les fonctionnalités suivantes ne font pas partie des objets d’espace de stockage dans le cloud Adobe :

* Workfront Proof
* Visionneuse de documents Workfront
* Documents favoris
* Demander des documents

Les projets hérités conservent l’accès à Workfront Proof et aux fonctionnalités des documents hérités répertoriées ci-dessus. Workfront Proof ne recevra plus de nouveaux investissements et sera abandonné dans une version ultérieure.

## Quota de stockage

Le stockage est mis en pool pour les objets Workfront hérités et les objets de stockage dans le cloud Adobe. Chaque utilisateur sous licence reçoit 60 Go de stockage. Il n’existe pas de limite stricte à l’utilisation du stockage, mais les administrateurs de Workfront reçoivent des notifications par e-mail lorsque l’utilisation atteint 75 %, 90 % et 100 % du quota.

Pour afficher l’utilisation et le quota de stockage actuels, accédez à **Configuration** > **Système** > **Informations client**.

Pour plus d’informations, voir [Vérification des limites de stockage du document](/help/quicksilver/documents/managing-documents/check-document-storage.md).

## Limite de révision vidéo annuelle

Les demandes d’épreuves vidéo sont plafonnées à 10 % du nombre total de licences d’utilisation payantes de Workfront de votre entreprise (standard et light). Cette limite est appliquée au niveau de l’organisation.

* Les administrateurs de Workfront reçoivent des notifications in-app lorsque l’utilisation atteint 80 % et 100 % de la limite.
* Une fois la limite atteinte, vous ne pouvez plus créer de demandes de révision vidéo avant la prochaine période annuelle.
* Cette limite ne s&#39;applique pas aux clients Frame.io Enterprise. Si votre entreprise examine régulièrement d’importants volumes de contenu vidéo, contactez votre représentant de compte Adobe pour en savoir plus sur les licences Frame.io Enterprise.

Pour plus d’informations, consultez la FAQ sur la révision et l’approbation des ressources et des vidéos dans [Présentation de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Workfront Fusion sur les projets de stockage dans le cloud Adobe

Les scénarios Workfront Fusion existants reposant sur une relecture héritée ne fonctionnent pas automatiquement par rapport aux projets de stockage dans le cloud Adobe. Les modules, webhooks et points d’entrée d’API spécifiques à une épreuve ont des équivalents directs dans certains cas et des changements significatifs dans d’autres. Les scénarios définis pour les projets hérités continuent de fonctionner comme aujourd’hui.

Pour plus d’informations sur l’impact sur les types de scénario courants et sur la manière de classer chaque scénario en tant que Modifier, Recréer ou Supprimer en fonction de ses fonctionnalités, consultez [Mise à jour des scénarios Workfront Fusion pour une révision et une approbation unifiées](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).
