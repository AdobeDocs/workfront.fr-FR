---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: Améliorations de la relecture (version 2019.2)
description: Cette page décrit toutes les améliorations de l’authentification incluses dans la version 2019.2. Cette fonctionnalité devrait être disponible dans l’environnement de production au cours de la semaine du 20 mai 2019.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: e8b67a10-1c9a-427e-96d5-0bcee47333f3
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 2%

---

# Améliorations de la relecture (version 2019.2)

Cette page décrit toutes les améliorations de l’authentification incluses dans la version 2019.2. Cette fonctionnalité devrait être disponible dans l’environnement de production au cours de la semaine du 20 mai 2019.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.2, consultez la [présentation de l’activité de version 2019.2](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## Autoriser les utilisateurs sans licence de vérification à appliquer des actions et à résoudre des commentaires

Désormais, les utilisateurs sans licence de vérification peuvent appliquer des actions aux commentaires et résoudre les commentaires. Vous pouvez accorder une autorisation pour ces activités lorsque vous ajoutez un utilisateur à un BAT.

Auparavant, seuls les utilisateurs disposant d’une licence de vérification et du rôle de modération d’auteur ou de modérateur pouvaient appliquer des actions et résoudre des commentaires sur un BAT.

## Balisage d’un utilisateur lors de la commentaire sur un BAT dans la visionneuse de vérification

Lorsque vous commentez un BAT, si vous disposez de droits d&#39;édition sur le BAT, vous pouvez désormais marquer ou &quot;@mention&quot; toute personne ayant une adresse email reconnue par Workfront. Cela inclut :

* Toute personne qui a été ajoutée à un BAT dans le compte Workfront de votre entreprise à l’aide de l’adresse électronique.
* Toute personne qui a utilisé l’adresse électronique pour s’abonner à un BAT dans le compte Workfront de votre entreprise.

Auparavant, vous pouviez baliser uniquement les utilisateurs qui avaient été ajoutés au workflow du BAT. C’est toujours ainsi que fonctionne le balisage si vous n’avez pas de modification correcte sur le BAT.

## Filtrage du rapport Approbation de BAT pour Omettre les versions de BAT précédentes

>[!NOTE]
>
>Cette fonctionnalité a été publiée directement dans l’environnement de production au cours de la période d’aperçu 2019.2.

Dans n’importe quel rapport Approbation de BAT, vous pouvez désormais utiliser le nouveau filtre Est la version actuelle du document afin d’inclure uniquement les versions actuelles des BAT en attente de votre approbation.

Cela s’avère utile, par exemple, si vous avez été invité à approuver des bons à tirer qui comportent plusieurs versions. Lorsque vous exécutez le rapport Approbation de BAT avec le filtre Is Current Document Version , il répertorie uniquement la version actuelle de chaque BAT en attente de votre approbation, omettant les versions antérieures sur lesquelles vous n’avez plus besoin de travailler.

Pour plus d’informations, voir [Rapport d’approbation de BAT pour omettre les versions précédentes du BAT](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-proof-approval-report.md).

