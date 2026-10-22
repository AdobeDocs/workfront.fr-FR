---
title: Présentation de la version du premier trimestre 2027
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du premier trimestre 2027. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 18e1d35b98b8c1afc6f9c1b14dba73d160b7e420
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 30%
---

# Présentation de la version du premier trimestre 2027

Cette page fournit des informations sur les fonctionnalités incluses dans la version du premier trimestre 2027 prévue pour janvier 2027.

Les améliorations apportées à cette page sont disponibles dans l’environnement de Prévisualisation. Cette page sera mise à jour avec des améliorations supplémentaires à mesure que la version du premier trimestre 2027 approche de sa mise en production prévue.

>[!IMPORTANT]
>
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>2026.11 (12 novembre 2026)</li><li>2026.12 (17 décembre 2026)</li><li>2027.01 (21 janvier 2027)</li></ul> | <ul><li>2027.01 (21 janvier 2027)</li></ul> |
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux projets](#project-enhancements)


### Améliorations apportées aux projets

<table>
    <tbody>
        <tr>
            <td><strong>Fonctionnalité</strong>
            </td>
            <td><strong>Aperçu</strong></td>
            <td><strong>Version rapide</strong></td>
            <td><strong>Tous les trimestres</strong></td>
        </tr>
        <tr>
            <td>
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">Épingler les threads en haut des mises à jour</a></p>
                <p>Vous pouvez désormais épingler les threads les plus importants en haut de la zone des Mises à jour sur un projet, une tâche, un problème ou une demande afin que les informations clés restent visibles pour votre équipe.</p>
            </td>
            <td><p>15 Octobre 2026</p></td>
            <td><p>12 Novembre 2026</p></td>
            <td><p>21 janvier 2027</p></td>
        </tr>
    </tbody>
</table>

## Notes de mise à jour pour d’autres zones

* [Activité de version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).
* [Activité de publication d’Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

Les éléments suivants n’ont pas été modifiés à ce stade de la publication :

* Planificateur de scénarios
* Épreuve
* Objectifs

## Annonces

### Obsolescence des champs de taux de facturation et de coût hérités dans les vues de liste de fonctions

Au fil du temps, nous avons mis en place des fonctionnalités améliorées de gestion des taux et des expériences dédiées aux fonctions qui offrent une approche plus complète et évolutive de la gestion des informations sur les taux. Par conséquent, l’administration des taux se dirige vers ces expériences dédiées plutôt que vers des workflows de gestion basés sur des listes.

Avec la version de janvier 2027, les champs hérités **Facturation par heure** et **Coût par heure** ne seront plus disponibles dans l’API Workfront ou dans les vues de liste des fonctions, y compris les configurations de filtrage/affichage/regroupement (références directes et colonnes calculées du mode texte).

En remplacement dans les rapports , vous pouvez utiliser le code de mode texte recommandé (utilisez `costRates` ou `billingRates` selon les besoins) :

    «
    displayname=Test
    listdelimiter=&lt;br>
    listmethod=nested(costRates).lists
    type=iterate
    valueexpression=CONCAT({startDate}, » -  »,{endDate}, »:  »,{value})
    valueformat=HTML
    « 

Pour gérer et examiner les taux de fonctions, utilisez les expériences de gestion des taux dédiées :

* Accédez aux taux de fonctions et gérez-les directement à partir de la page Fonction > Taux .
* Utilisez les rapports de taux pour examiner, analyser et générer des rapports sur les informations de taux dans les différentes fonctions.

Aucune action n’est requise pour préparer la modification. Cependant, les administrateurs qui affichent actuellement les champs **Facturation par heure** et **Coût par heure** dans les vues Liste des fonctions doivent mettre à jour leurs workflows pour utiliser les expériences de gestion de taux recommandées décrites ci-dessus.

Pour plus d’informations sur les taux de fonctions, voir [Créer et gérer des fonctions](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

-->

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).
