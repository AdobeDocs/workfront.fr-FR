---
title: Améliorations des rapports du troisième trimestre 2025
description: Améliorations apportées aux projets au troisième trimestre 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 15%

---

# Améliorations des rapports du troisième trimestre 2025

Cette page décrit toutes les améliorations apportées aux rapports avec la version du troisième trimestre 2025 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du troisième trimestre 2025, consultez la [Vue d’ensemble de la version du troisième trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Amélioration De La Sécurité De La Diffusion Des Rapports

* Prévisualisation : vendredi 26 juin 2025
* Production : déploiement échelonné du 26 juin 2025 au 9 juillet 2025

Nous avons amélioré la diffusion de rapports planifiés pour nous assurer que les notifications Workfront sont envoyées uniquement aux domaines d’e-mail approuvés dans la place sur la liste autorisée.

Auparavant, si votre organisation avait défini une limitation sur les domaines d’e-mail auxquels les notifications Workfront étaient ajoutées, nous effectuions une vérification de la liste autorisée lorsque des e-mails étaient ajoutés.

Désormais, nous effectuons également une vérification lors de l’envoi de l’e-mail pour nous assurer que l’adresse e-mail saisie est conforme à la place sur la liste autorisée e-mail. Cette vérification améliorée s’applique à la fois aux adresses e-mail associées aux utilisateurs et aux e-mails ad hoc ajoutés à la liste des destinataires du rapport.

Pour plus d’informations, voir [Planification de la diffusion automatique des rapports](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


## Les caractères génériques utilisateur ne renvoient plus de résultats avec une valeur nulle lors du filtrage

>[!NOTE]
>
>* Aperçu : 30 avril 2025
>* Version rapide de production : 15 mai 2025
>* Production pour tous les clients : 17 juillet 2025

Nous avons mis à jour le comportement du caractère générique utilisateur pour exclure la valeur nulle lors du filtrage d’un rapport. Cette modification permet au filtre de produire des résultats plus précis, plutôt que de renvoyer des résultats qui ne sont pas correctement configurés par un utilisateur (résultat nul).

Auparavant, lorsqu’un caractère générique utilisateur générait une valeur nulle, un rapport affichait tous les enregistrements qui avaient également une valeur nulle.

Cette modification s’applique aux filtres génériques suivants :

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
