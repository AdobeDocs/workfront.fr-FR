---
product-area: documents
navigation-topic: approvals
title: Passer à Workfront sur l’espace de stockage dans le cloud Adobe
description: Planifiez le déploiement de Workfront sur l’espace de stockage cloud Adobe. Découvrez les différences entre les objets d’espace de stockage dans le cloud Adobe, y compris la nouvelle zone Documents et l’expérience de révision Frame.io, et décidez de la manière dont l’espace de stockage dans le cloud Adobe se déploie dans votre environnement.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '2359'
ht-degree: 0%

---

# Passer à Workfront sur l’espace de stockage dans le cloud Adobe

Le stockage dans le cloud Workfront sur Adobe offre une expérience de révision et d’approbation entièrement unifiée : révisions dans la visionneuse Frame.io, workflows d’approbation puissants, visibilité des ressources sur l’ensemble des produits, etc.

Vos objets existants continuent à fonctionner de la même manière qu’aujourd’hui. La nouvelle zone Documents, la visionneuse Frame.io et d’autres comportements d’espace de stockage dans le cloud Adobe s’appliquent uniquement aux objets utilisant l’espace de stockage dans le cloud Adobe.

Cet article s’adresse aux administrateurs Workfront qui se préparent à déployer Workfront sur l’espace de stockage dans le cloud Adobe. Elle couvre les différences majeures sur les objets d’espace de stockage dans le cloud Adobe, la manière de choisir votre type de déploiement et les éléments à prendre en compte avant d’activer l’espace de stockage dans le cloud Adobe pour vos utilisateurs et utilisatrices.

>[!IMPORTANT]
>
>Vous devez utiliser une version de Workfront prenant en charge l’espace de stockage dans le cloud Adobe. Si votre organisation ne dispose pas déjà d’une version prise en charge, contactez votre représentant de compte Adobe.



## Comprendre le stockage Workfront hérité et le stockage dans le cloud Adobe

Une fois votre contrat mis à jour afin d’inclure la nouvelle expérience de révision et d’approbation unifiée, votre environnement peut contenir deux types d’objets : des objets sur l’ancien stockage Workfront (les objets que vous possédez aujourd’hui) et des objets créés à l’aide de l’espace de stockage dans le cloud Adobe. À un niveau élevé, les deux modèles de stockage diffèrent en ce qui concerne l’emplacement des données, les produits Adobe qui peuvent les voir et les fonctionnalités disponibles :

|  | Objet sur l’ancien stockage Workfront | Objet sur l’espace de stockage dans le cloud Adobe |
|---|---|---|
| Serveur principal de stockage | Workfront uniquement | Adobe cloud storage |
| Visibilité sur l’ensemble des produits | Workfront uniquement | Workfront, Frame.io et Creative Cloud |
| Fonction | Fonctionnalités héritées | Nouvelle fonctionnalité |

Les objets créés avant l’activation de l’espace de stockage dans le cloud Adobe dans la zone Configuration restent sur l’espace de stockage Workfront hérité. Les nouveaux comportements décrits dans cet article s’appliquent uniquement aux objets d’espace de stockage dans le cloud Adobe que vous et vos utilisateurs créez une fois que l’espace de stockage dans le cloud Adobe est activé.

## En quoi le stockage dans le cloud Adobe est-il différent ?

Le plus grand changement au quotidien avec l’espace de stockage dans le cloud d’Adobe est la nouvelle zone Documents et la visionneuse Frame.io qui alimente la révision et l’approbation qu’elle contient. D’autres différences affectent la gestion des objets, des documents et des révisions.

Le tableau suivant résume les principales différences lors du passage à l’espace de stockage dans le cloud Adobe. Chaque zone du tableau renvoie vers la section détaillée ci-dessous.

| Zone | Qu’est-ce qui est différent ? | Ce qu’il faut savoir |
|---|---|---|
| [la zone Nouveaux documents](#the-new-documents-area) | Une zone Documents unifiée et repensée remplace l’ancienne zone Documents. | Zone Aucun document global. Accéder aux documents d&#39;un programme, d&#39;un portefeuille, d&#39;un projet, d&#39;une tâche ou d&#39;un événement. |
| [Autorisations de document](#document-permissions) | Les documents héritent des autorisations du projet, de la tâche ou du problème auxquels ils sont liés. | Vous ne pouvez pas partager ni définir d’autorisations sur des documents individuels. Vous gérez tous les accès par le biais de la fenêtre modale de partage d’objet dans Workfront, qui applique en cascade des dossiers de documents générés par le système. |
| [Mappage des autorisations d’objet](#object-permissions-mapping) | Les autorisations de gestion de Workfront et de contribution sont toutes deux mappées à Modifier et partager dans Frame.io. Affichez les mappages en commentaire uniquement. | Les autorisations sont gérées dans Workfront. Les utilisateurs des fonctions Gérer et Contribuer bénéficient de la fonctionnalité de partage externe de Frame.io. |
| [Observateur de révision et d’approbation](#review-and-approval-viewer) | La visionneuse Frame.io remplace la visionneuse de relecture Workfront. | Inclus pour tous les utilisateurs de Workfront disposant d’une licence payante. Prend en charge les balises, les commentaires horodatés, l’historique des versions, les appareils mobiles, plus de 40 formats, les fichiers jusqu’à 500 Go. |
| [Règles de dénomination des objets](#object-naming-rules) | Des règles de nommage strictes s’appliquent : noms uniques dans un portfolio ou un projet, aucun caractère spécial, aucune période ou espace de fin, limite de 255 caractères. | Workfront renomme automatiquement les objets en cas de conflit. Modèles d’audit qui génèrent de nouveaux noms et une nouvelle structure de projet. |
| [Portabilité des objets](#object-portability) | Vous ne pouvez déplacer, copier et convertir des objets qu’entre des modèles de stockage similaires. | Les objets de stockage dans le cloud Adobe ne peuvent pas être déplacés vers des projets hérités, ou l’inverse. Le déplacement d’un projet d’espace de stockage dans le cloud Adobe vers un portfolio ou un programme hérité convertit le parent en espace de stockage dans le cloud Adobe. |
| [Fonctionnalités non disponibles](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, la visionneuse de documents Workfront, les documents favoris et les documents de demande ne font pas partie de l’expérience. | Les objets hérités conservent ces fonctionnalités. Workfront Proof ne recevra pas de nouvel investissement et sera mis hors service dans une version ultérieure. |
| [Quota de stockage](#storage-quota) | Le stockage est mis en pool pour les projets Workfront hérités et les projets de stockage dans le cloud Adobe. 60 Go par utilisateur sous licence. Pas de capuchon. | Les administrateurs système peuvent afficher l’utilisation du stockage sur la page Informations sur le client de la configuration. |
| [Limite de révision vidéo annuelle](#annual-video-review-cap) | Au niveau de l’entreprise, la limite fixée à 10 % des licences payantes d’utilisation de Workfront (standard et light) pour les demandes d’épreuves vidéo est de 10 %. | Une fois atteinte, aucune nouvelle critique vidéo ne sera publiée avant la prochaine période annuelle. Notifications in-app à 80 % et 100 %. Ne s’applique pas aux clients Frame.io Enterprise. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | Les scénarios Fusion existants basés sur des BAT ne fonctionnent pas automatiquement avec les projets de stockage dans le cloud Adobe. | Les scénarios définis pour les projets hérités continuent de fonctionner. Chaque scénario affecté reçoit l’un des trois chemins suivants : modifier, recréer ou supprimer. Nouveaux connecteurs attendus au 3ème trimestre 2026. |

### La nouvelle zone Documents

La nouvelle zone Documents est une expérience de documents unifiée conçue pour le stockage dans le cloud Adobe. Il simplifie la navigation, consolide les activités de révision et d’approbation et constitue le point d’entrée de la visionneuse Frame.io.

La zone globale Documents ne fait pas partie de la nouvelle expérience . Dans les projets de stockage dans le cloud Adobe, vous accédez aux documents d’un programme, d’un portfolio, d’un projet, d’une tâche ou d’un événement.

Pour plus d’informations, voir [la zone Documents](/help/quicksilver/documents/managing-documents/documents-area.md).

### Autorisations de documents

Les autorisations de document sont fondamentalement différentes sur les projets de stockage dans le cloud Adobe :

* Vous ne pouvez pas partager ni définir d’autorisations sur des documents individuels. Au lieu de cela, les autorisations sont appliquées aux dossiers de documents générés par le système qui contiennent les documents.
* Les dossiers de documents générés par le système héritent des autorisations de leur projet, tâche ou problème parent.
* Les sous-dossiers héritent des autorisations du dossier de documents parent généré par le système.
* Les sous-tâches n’héritent pas des autorisations des tâches parents. Vous devez être ajouté directement à une sous-tâche pour accéder à son dossier de documents généré par le système.


Pour plus d’informations sur le fonctionnement des autorisations de document, voir [Présentation des autorisations d’objet et des niveaux d’accès pour le modèle de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).


### Mappage des autorisations d’objet

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

Les options Gérer et Contribuer mappent toutes deux à **Modifier et partager** dans Frame.io. Lorsque vous passez en revue vos modèles de partage pour les projets de stockage dans le cloud Adobe, déterminez s’il est conforme à votre modèle de gouvernance que les contributeurs disposent des mêmes fonctionnalités de révision que les responsables, y compris le partage externe.

Pour plus d’informations, voir [Présentation des autorisations d’objet et des niveaux d’accès pour le modèle de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).


### Observateur de révision et d’approbation

Sur les objets d’espace de stockage Adobe, la visionneuse Frame.io est la surface de révision et d’approbation à la place de Workfront Proof. La visionneuse Frame.io est incluse pour tous les utilisateurs de Workfront disposant d’une licence payante.

La visionneuse Frame.io fournit les éléments suivants :

* Outils de balisage et de commentaires, notamment le dessin à main levée et les formes standard telles que les cercles, les flèches et les carrés
* Commentaires horodatés avec précision d’image pour les révisions vidéo
* Historique des versions et comparaison des versions
* Accès mobile pour les révisions et les approbations en cours de route
* Prise en charge de plus de 40 formats de fichiers, y compris tous les types courants de fichiers vidéo, image, audio, PDF et Microsoft Office, avec lecture native pour les formats vidéo professionnels tels que ProRes, H.265 et DNxHD, et prise en charge de fichiers jusqu’à 500 Go


### Règles de dénomination des objets

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


### Portabilité des objets

Vous pouvez déplacer, copier et convertir des objets Workfront entre des modèles de stockage similaires. Par exemple, vous pouvez déplacer une tâche d’un projet d’espace de stockage dans le cloud Adobe vers un autre projet d’espace de stockage dans le cloud Adobe. Vous ne pouvez pas déplacer ou copier une tâche ou un événement d’un projet d’espace de stockage Adobe vers un projet hérité, ou l’inverse.

Aujourd’hui, lorsque vous créez ou déplacez un projet d’espace de stockage dans le cloud Adobe vers un portfolio ou un programme hérité, le portfolio ou le programme est automatiquement converti en un objet d’espace de stockage dans le cloud Adobe. Une prochaine version donnera aux administrateurs système plus de contrôle sur les objets qui sont automatiquement convertis.

### Fonctionnalités non disponibles sur les objets d’espace de stockage dans le cloud Adobe

Les fonctionnalités suivantes ne font pas partie des objets d’espace de stockage dans le cloud Adobe :

* Workfront Proof
* Visionneuse de documents Workfront
* Documents favoris
* Demander des documents

Les projets hérités conservent l’accès à Workfront Proof et aux fonctionnalités des documents hérités répertoriées ci-dessus. Workfront Proof ne recevra plus de nouveaux investissements et sera abandonné dans une version ultérieure.

### Quota de stockage

Le stockage est mis en pool pour les objets Workfront hérités et les objets de stockage dans le cloud Adobe. Chaque utilisateur sous licence reçoit 60 Go de stockage. Il n’existe pas de limite stricte à l’utilisation du stockage, mais les administrateurs de Workfront reçoivent des notifications par e-mail lorsque l’utilisation atteint 75 %, 90 % et 100 % du quota.

Les administrateurs système peuvent accéder à **Configuration** > **Système** > **Informations clients** pour afficher l’utilisation actuelle du stockage et le quota.

Pour plus d’informations, voir [Vérification des limites de stockage du document](/help/quicksilver/documents/managing-documents/check-document-storage.md).


### Limite de révision vidéo annuelle

Les demandes d’épreuves vidéo sont plafonnées à 10 % du nombre total de licences d’utilisation payantes de Workfront de votre entreprise (standard et light). Cette limite est appliquée au niveau de l’organisation.

* Les administrateurs de Workfront reçoivent des notifications in-app lorsque l’utilisation atteint 80 % et 100 % de la limite.
* Une fois la limite atteinte, vous ne pouvez plus créer de demandes de révision vidéo avant la prochaine période annuelle.
* Cette limite ne s&#39;applique pas aux clients Frame.io Enterprise. Si votre entreprise examine régulièrement d’importants volumes de contenu vidéo, contactez votre représentant de compte Adobe pour en savoir plus sur les licences Frame.io Enterprise.

Pour plus d’informations, consultez la FAQ sur la révision et l’approbation des ressources et des vidéos dans [Présentation de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

### Workfront Fusion sur les projets de stockage dans le cloud Adobe

Les scénarios Workfront Fusion existants reposant sur une relecture héritée ne fonctionnent pas automatiquement par rapport aux projets de stockage dans le cloud Adobe. Les modules, webhooks et points d’entrée d’API spécifiques à une épreuve ont des équivalents directs dans certains cas et des changements significatifs dans d’autres. Les scénarios définis pour les projets hérités continuent de fonctionner comme aujourd’hui.

Les connecteurs Fusion avec prise en charge native de la révision et de l’approbation unifiées devraient être disponibles au 3e trimestre 2026.

Pour plus d’informations sur l’impact sur les types de scénario courants et sur la manière de classer chaque scénario en tant que Modifier, Recréer ou Supprimer en fonction de ses fonctionnalités, consultez [Mise à jour des scénarios Workfront Fusion pour une révision et une approbation unifiées](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Choisir comment l’espace de stockage dans le cloud Adobe se déploie

Vous décidez de la manière dont l’espace de stockage dans le cloud Adobe apparaîtra à vos utilisateurs. Il existe deux configurations, dont l’une peut être appliquée à l’ensemble de l’organisation ou à des groupes Workfront spécifiques.

Pour obtenir des instructions détaillées, voir [Activer l’espace de stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

* **Espace de stockage Adobe uniquement** : les nouveaux projets utilisent l’espace de stockage Adobe par défaut. Les utilisateurs ne peuvent pas créer de projets hérités.
* **Stockage dans le cloud Adobe et stockage Workfront hérité** : lorsque les utilisateurs créent un projet, ils choisissent entre le stockage dans le cloud Adobe (appelé « Nouveau projet ») et le stockage Workfront hérité (appelé « Stockage hérité »).

  ![choisir un type de projet](assets/choose-project-type.png)



>[!TIP]
>
>Pour placer l’espace de stockage cloud d’Adobe devant une équipe plus petite en premier, appliquez l’une des configurations à un seul groupe Workfront. Vous pouvez ainsi exécuter un pilote ciblé avant d’effectuer un déploiement plus large. Nous vous recommandons de commencer par un déploiement au niveau du groupe pour contrôler la fréquence, puis de l’étendre à l’ensemble de l’organisation une fois que le groupe pilote a validé l’expérience.

Les objets existants conservent le modèle de stockage avec lequel ils ont été créés. La modification de la préférence de stockage par défaut ne modifie aucun objet existant.

## Planifier le déploiement

Chaque environnement Workfront est différent. Avant d’activer le stockage dans le cloud Adobe pour vos utilisateurs, prenez le temps de planifier un déploiement réussi pour votre organisation. Les suggestions ci-dessous ne sont pas une liste de contrôle, mais un point de départ pour votre propre plan.

**1. Choisir un groupe pilote.** Un déploiement à l’échelle d’un groupe vous permet de placer l’espace de stockage cloud d’Adobe devant une équipe plus petite, de recueillir des commentaires et de procéder à des ajustements avant un déploiement plus large. Sélectionnez un groupe dont les modèles de travail sont suffisamment représentatifs pour faire apparaître rapidement les problèmes que vous souhaitez connaître.

**2. Communiquez le changement aux utilisateurs finaux.** La plus grande modification visible pour les réviseurs, les approbateurs et les propriétaires de projet est la nouvelle zone Documents et la visionneuse Frame.io qui alimente la révision et l’approbation des projets d’espace de stockage dans le cloud Adobe. Planifiez l’introduction de ces éléments afin que les utilisateurs sachent à quoi s’attendre lorsqu’ils rencontrent leur premier projet de stockage dans le cloud Adobe. L’article [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) est un point de départ utile pour les ressources destinées aux utilisateurs finaux.

**3. Planifiez la disponibilité du connecteur Workfront Fusion.** Les connecteurs Fusion avec prise en charge native de la révision et de l’approbation unifiées devraient être disponibles au 3e trimestre 2026. Les scénarios Fusion existants basés sur des preuves continuent de fonctionner sur les projets existants. Avant d’intégrer les équipes qui dépendent de ces scénarios dans votre projet pilote de stockage dans le cloud Adobe, décidez s’il faut attendre les nouveaux connecteurs, recréer l’API actuelle ou remplacer ces scénarios par des fonctionnalités de révision et d’approbation unifiées natives.

Pour plus d’informations sur l’impact sur les types de scénario courants et sur la manière de classer chaque scénario en tant que Modifier, Recréer ou Supprimer en fonction de ses fonctionnalités, consultez [Mise à jour des scénarios Workfront Fusion pour une révision et une approbation unifiées](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Articles connexes

* [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Activer le stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [Aperçu de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [La zone Documents](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)

