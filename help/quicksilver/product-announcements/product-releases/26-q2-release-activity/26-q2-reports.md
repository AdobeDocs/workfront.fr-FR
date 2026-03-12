---
title: Améliorations des rapports pour le deuxième trimestre 2026
description: Améliorations des rapports pour le deuxième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
source-git-commit: ed4b03429a479797854a0cae08f9191a25eebc13
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 14%

---

# Améliorations des rapports pour le deuxième trimestre 2026

Cette page décrit les améliorations apportées aux rapports avec la version du deuxième trimestre 2026 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du deuxième trimestre 2026, consultez la section [Vue d’ensemble de la version du deuxième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Nouvelles options d’authentification pour la connexion à Data Connect

>[!NOTE]
>
>Aperçu : 12 mars 2026
>Version rapide de production : vendredi 12 mars 2026
>Production pour tous : vendredi 16 avril 2026

Vous pouvez désormais vous authentifier auprès de Data Connect à l’aide de clés RSA ou de connexions PAT (Programmatic Access Tokens), ajoutant ainsi des alternatives plus sécurisées et flexibles aux informations d’identification traditionnelles de nom d’utilisateur/mot de passe.

Ces nouvelles options permettent aux entreprises de maintenir des connexions stables à partir de Power BI, Tableau et d’autres outils de BI tiers sans recourir à des méthodes de connexion basées sur l’utilisateur.

>[!IMPORTANT]
>
>En juin 2026, les informations d’identification de nom d’utilisateur/mot de passe seront requises pour utiliser l’authentification multifacteur (MFA). Nous vous recommandons de passer à l’authentification RSA ou PAT pour les comptes utilisateur de service utilisés pour charger des données de Data Connect dans des outils de visualisation, des processeurs de données et des scripts tiers qui ne fonctionneront pas avec MFA dans le processus d’authentification.

## Libellés de champ personnalisés affichés lors de la création de rapports

>[!NOTE]
>
>Aperçu : 26 février 2026
>Version rapide de production : vendredi 12 mars 2026
>Production pour tous : vendredi 16 avril 2026

Le libellé du champ personnalisé s’affiche désormais avant le nom du champ et l’objet dans les outils de création de rapports, ce qui vous permet de localiser plus facilement les champs. Les libellés des champs s’affichent également lors de la définition de filtres, de vues et de regroupements dans des listes.

Le libellé du champ personnalisé est destiné à l’interface système, tandis que le nom du champ est fréquemment utilisé à des fins d’API et de stockage back-end, et peut ne pas être aussi utile lors de la localisation d’un champ.

Pour plus d’informations, voir [Créer un rapport personnalisé](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Dossiers de rapports partageables

>[!NOTE]
>
>Aperçu : 26 février 2026
>Version rapide de production : vendredi 12 mars 2026
>Production pour tous : vendredi 16 avril 2026

Vous pouvez désormais organiser et partager des rapports à l’aide de dossiers de rapports partageables. Cette nouvelle fonctionnalité permet aux équipes qui gèrent d’importants volumes de rapports de maintenir un contrôle d’accès évolutif et cohérent :

* **Créer des structures de dossiers organisées** : les administrateurs système peuvent créer des dossiers de niveau supérieur, tandis que les utilisateurs disposant d’un accès de gestion peuvent créer des sous-dossiers jusqu’à 4 niveaux de profondeur.
* **Contrôles d’autorisation granulaires** : partagez des dossiers avec deux niveaux d’autorisation :
   * Afficher : les utilisateurs peuvent ouvrir des rapports et partager des dossiers
   * Gérer : les utilisateurs peuvent modifier les détails du dossier, ajouter/supprimer des éléments et recevoir automatiquement un accès de gestion à tous les rapports du dossier
* **Autorisations héritées** : cascade d’autorisations des dossiers parents vers tous les sous-dossiers et rapports de l’arborescence de dossiers
* **Expérience de liste améliorée** : lorsque vous activez les dossiers à partager, vous avez accès à l’expérience de liste améliorée. Pour plus d’informations, voir [Utilisation de listes améliorées](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


Pour plus d’informations, voir [Utilisation de dossiers de rapports partageables](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

## Amélioration des libellés de date pour les regroupements de graphiques dans les tableaux de bord Zone de travail

>[!NOTE]
>
>Aperçu : 26 février 2026
>Version rapide de production : vendredi 12 mars 2026
>Production pour tous : vendredi 16 avril 2026

>[!NOTE]
>
>Les tableaux de bord de la zone de travail sont actuellement en version bêta.

Les graphiques qui regroupent les données par date affichent désormais des libellés de date plus clairs et plus lisibles. Grâce à cette mise à jour, les libellés de date s’ajustent dynamiquement en fonction de l’option Regrouper par sélectionnée (par jour, semaine, mois ou année, par exemple), ce qui facilite la lecture et l’interprétation des graphiques en un coup d’œil :

<table> <tbody> <tr> <td>Jour</td> <td>Affiche la date complète. Exemple : 3/12/2026</td> </tr> <tr> <td>Semaine</td> <td>Affiche une date de début de semaine formatée. Exemple : 8 Mars 2026</td> </tr> <tr> <td>Mois</td> <td>Affiche le mois et l’année. Exemple mars 2026</td> </tr> <tr> <td>Année</td> <td>Affiche l’année uniquement. Exemple : 2026</td> </tr> </tbody> </table>

Auparavant, les regroupements de graphiques affichaient toujours la date de début de la période sélectionnée au format numérique.
