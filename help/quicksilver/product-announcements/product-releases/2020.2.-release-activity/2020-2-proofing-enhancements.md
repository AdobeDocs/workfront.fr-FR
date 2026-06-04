---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 Améliorations de la relecture
description: Cette page décrit toutes les améliorations de relecture apportées à la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
TQID: https://experienceleague.adobe.com/Z86GWBBVdj1DPENzHS7wKI1ViRGFzov8L3sNtss4iJU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 100%

---

# 2020.2 Améliorations de la relecture

Cette page décrit toutes les améliorations de relecture apportées à la version 2020.2 de l’environnement de production. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 mai 2020.

Pour obtenir la liste de toutes les modifications disponibles avec la version 2020.2, consultez l’article [Présentation de la version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Le domaine de relecture passe de proofhq.com à workfront.com.

>[!NOTE]
>
>Cette fonctionnalité a été initialement communiquée dans le cadre de la version 2020.1, mais a été retirée de la version avant sa mise en production.

Si votre pare-feu ou votre serveur de messagerie est configuré pour autoriser l’accès uniquement à des fournisseurs spécifiques, vous devez ajouter l’URL supplémentaire suivante à votre liste autorisée pour vous assurer que les utilisateurs et utilisatrices de votre entreprise peuvent afficher les épreuves dans Workfront, à la fois dans la visionneuse de relecture du navigateur et dans la visionneuse de relecture sur ordinateur :

&#42;.workfront.com

L’URL &#42;proofhq.com est également requise.

Pour plus d’informations sur la mise à jour de votre liste autorisée, voir [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Cette mise à jour s’applique uniquement à la relecture dans Workfront ; elle ne s’applique pas lors de l’utilisation de l’application autonome Workfront Proof.

## Les commentaires de relecture des personnes invitées apparaissent dans la zone Mises à jour.

Pour simplifier la collaboration sur les épreuves, les commentaires des personnes invitées apparaissent dans la zone Mises à jour.

Auparavant, les commentaires des épreuves des personnes invitées n’étaient disponibles que dans l’épreuve.
