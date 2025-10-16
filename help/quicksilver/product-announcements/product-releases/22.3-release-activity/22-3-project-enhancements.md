---
title: Mises à jour du projet pendant la période de la version 22.3
description: Mises à jour du projet pendant la période de la version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1535'
ht-degree: 99%

---

# 22.3 Améliorations apportées au projet

Cette page décrit toutes les améliorations apportées au projet par la version 22.3 de l’environnement de prévisualisation. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 juillet 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.3, voir [Vue d’ensemble de la version 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Délégation du travail lors d’absences du bureau

Vous pouvez déléguer les tâches et les problèmes qui vous sont affectés à d’autres personnes lorsque vous prévoyez de vous absenter du bureau pour une brève période. Cela permet de s’assurer que votre absence ne constitue pas un obstacle à la réalisation du travail.

Avant cette amélioration, vous ne pouviez que déléguer des approbations.

Voici quelques-unes des fonctionnalités ajoutées lors de cette mise à jour :

* Paramètre de la zone Préférences de tâches et de problèmes de la Configuration pour l’administrateur ou l’administratrice du système ou de groupes permettant d’activer la délégation dans votre environnement.

* Nouvelle option pour « Déléguer des tâches et des problèmes » dans la zone d’accueil pour les personnes disposant d’une licence Révision ou supérieure pour déléguer leurs éléments de travail.

* Indication dans l’accueil et dans la zone Affectations des en-têtes de tâches et de problèmes que des éléments sont délégués à d’autres personnes.

* Notifications d’événement dans la zone Configuration et Notifications par e-mail dans le profil de l’utilisateur ou de l’utilisatrice pour contrôler les notifications par e-mail concernant le travail délégué.


>[!NOTE]
>
>Seules les personnes disposant d’une licence Révision ou supérieure peuvent déléguer leur travail à d’autres personnes. Le travail peut être délégué à n’importe quelle personne, quel que soit son niveau d’accès. Les personnes déléguées reçoivent les mêmes autorisations que les personnes cessionnaires sur les éléments délégués. Si ces autorisations sont inférieures à la configuration du niveau d’accès d’une personne, les personnes déléguées peuvent être empêchées d’effectuer certaines des activités relatives aux tâches et aux problèmes qui leur sont délégués.


Pour plus d’informations, voir [Vue d’ensemble des tâches et des problèmes délégués](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nouvelle expérience lors de la conversion d’un problème en tâche

Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface de conversion d’un problème en tâche.

Cette mise à jour comprend ce qui suit :

* Interface d’utilisation actualisée qui s’harmonise avec le reste de la nouvelle expérience Workfront.

* Accès pour convertir un problème en tâche à partir d’une liste ou d’un rapport.

* Les formulaires personnalisés par défaut définis dans la zone Paramètres des tâches du projet de destination sont ajoutés à la nouvelle tâche.


Pour plus d’informations, voir [Convertir un événement en tâche](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nouvelle expérience lors de la conversion d’un problème en projet sans modèle

Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface permettant de convertir un problème en projet sans utiliser de modèle.

En plus d’une interface utilisateur mise à jour qui correspond au reste de la nouvelle expérience Workfront, nous avons également ajouté la possibilité de convertir un problème en projets vierges à partir d’une liste ou d’un rapport.

Pour plus d’informations, voir [Convertir un problème en projet dans Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Balises intelligentes dans le flux de mises à jour

Nous avons amélioré la façon de taguer des personnes dans le flux de mises à jour lorsque vous créez une mise à jour ou répondez à une mise à jour existante. Désormais, lorsque vous taguez une personne pour l’inclure dans une mise à jour, en plus de son nom et de son avatar, nous affichons également son rôle principal et son e-mail. Cela permet de distinguer plusieurs utilisateurs portant des noms similaires ou identiques.

Pour plus d’informations, voir [Taguer d’autres personnes sur les mises à jour](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nouvelle syntaxe pour les calculs dans les champs personnalisés

Pour préparer les futures améliorations qui vous permettront d’ajouter des calculs aux formulaires personnalisés, nous avons normalisé la syntaxe des champs référencés que vous ajoutez à un calcul. Il est facile d’utiliser cette nouvelle syntaxe, car le système la saisit pour vous lorsque vous commencez à taper le nom d’un champ et que vous le sélectionnez.

## Conserver des informations précises lorsque deux personnes ayant un rôle commun sont impliquées dans un processus d’approbation.

Afin de garantir l’exactitude des données relatives à l’approbation du travail, nous avons modifié la manière dont les informations d’approbation sont enregistrées sur un élément lorsqu’un processus d’approbation nécessitant plusieurs rôles est associé à cet élément.

Certains processus d’approbation requièrent l’approbation de deux rôles différents, et deux personnes différentes chargées de l’approbation peuvent avoir l’un de ces rôles en commun. Lorsque cela se produit, après que les décisions d’approbation ont été prises, Workfront enregistre chaque personne chargée de l’approbation et son rôle respectif associé au processus d’approbation.

Avant cette modification, les deux approbations étaient enregistrées pour la deuxième personne parce qu’elle partageait l’un des rôles d’approbation avec la première. Dans ce cas, la deuxième personne approbatrice écrasait les informations de la première.

Pour plus d’informations sur les processus d’approbation dans Workfront, voir [Vue d’ensemble du processus d’approbation](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Les heures d’affectation ne seront plus supprimées lors de la modification des affectations.

>[!NOTE]
>
>Cette fonctionnalité était initialement prévue pour la version 22.2. Elle a été mise en production le 21 avril 2022.


Pour garantir l’exactitude de vos données, nous avons apporté une modification afin de préserver les heures d’attribution et de maintenir inchangé le nombre d’heures prévues pour la tâche lorsque des changements sont apportés aux affectations de la tâche.

Les changements suivants ont été apportés aux tâches avec un type de durée simple :

* Le nombre d’heures prévues est conservé lors de la suppression de toutes les personnes cessionnaires.

* Les attributions d’affectations individuelles sont conservées lors du remplacement des utilisateurs et utilisatrices et des rôles.

* Les attributions d’affectations individuelles sont conservées sur le rôle lors de la suppression de l’utilisateur ou de l’utilisatrice. (Retiré de la version. Désormais, le nombre d’heures prévues sera défini sur 0 après la suppression de toutes les personnes cessionnaires).


Pour plus d’informations sur le nombre d’heures prévues, voir [Vue d’ensemble du nombre d’heures prévues](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Améliorations des panoramas

Les améliorations suivantes ont été apportées aux panoramas Adobe Workfront :

* Options de filtrage - Vous pouvez désormais filtrer par date d’échéance ou par statut sur un panorama. Le filtre a également été mis à jour avec des sections rétractables pour séparer les options.

* Archiver le panorama - Vous pouvez maintenant archiver un panorama pendant que vous êtes dans le panorama, au lieu d’avoir à aller dans le tableau de bord des panoramas.

* Ajouter une équipe à un panorama - Lorsque vous recherchez des personnes membres, vous pouvez ajouter une équipe entière. Le choix d’une équipe ajoute toutes les personnes membres de l’équipe au panorama.

* Zones de dépôt dans les colonnes - Lorsque l’on fait glisser une carte d’une colonne du tableau à une autre, une « zone de dépôt » grise indique désormais l’endroit où la carte sera placée. Auparavant, il ny’avait pas d’indicateur visuel de l’emplacement de la carte.

* Cartes connectées - Vous pouvez désormais ajouter des cartes connectées aux tâches et aux problèmes de Workfront. La mise à jour du nom, de la description ou de la personne cessionnaire dans la carte ou la tâche mettra à jour les mêmes champs dans l’autre emplacement.

* Champ de statut sur toutes les cartes - Un champ de statut et un bouton Marquer comme terminé ont été ajoutés aux cartes ad hoc et connectées. Lorsque vous cliquez sur Marquer comme terminé, le statut devient automatiquement Terminé.

* Convertir une carte ad hoc en carte connectée - Vous avez désormais la possibilité de convertir une carte ad hoc en carte connectée à partir des détails de la carte.

* Déconnecter une carte connectée - La déconnexion d’une carte connectée rompt la connexion avec l’objet Workfront. La carte reste une carte ad hoc sur le panorama et l’objet Workfront n’est pas affecté.

* Mappage des statuts dans les colonnes - Les nouveaux paramètres et politiques des colonnes vous permettent de définir un statut, une personne cessionnaire ou une balise s’appliquant aux cartes déplacées dans cette colonne. En outre, les noms de colonnes par défaut sur un nouveau panorama ont été modifiés en Colonne 1, Colonne 2 et Colonne 3.

* Indicateur de mise à jour des champs - Un indicateur s’affiche désormais lorsque vous enregistrez une carte, afin de confirmer que vos mises à jour ont été enregistrées.


Pour plus d’informations, voir [Commencer avec les panoramas dans Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Partager des dossiers uniquement dans les cinq premiers niveaux d’une hiérarchie de dossiers

Pour garantir les meilleures performances aux utilisateurs et utilisatrices qui partagent des dossiers, nous limitons actuellement le partage aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet.

Chaque dossier du sixième niveau ou d’un niveau inférieur hérite ses configurations de partage du dossier qui lui est directement supérieur.

Pour plus d’informations sur le partage de dossiers, voir [Partager un dossier de documents de premier niveau](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campagnes Workfront (version Beta) : une nouvelle façon de gérer votre travail

>[!NOTE]
>
>Il est prévu que cette fonctionnalité soit supprimée de l’environnement de prévisualisation le 9 janvier 2023. Pour plus d’informations, voir la [page de vue d’ensemble de la version 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Cette fonctionnalité ne sera pas incluse dans la version de production 22.3. Elle sera publiée en production avec une version future.


>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement en version Beta et est actuellement en cours de construction. Nous continuerons à ajouter des fonctionnalités pour le workflow Campagnes avec les prochaines versions. La participation au programme Beta de Campagnes de Workfront se fait sur une base volontaire.

Nous introduisons un nouvel objet dans Adobe Workfront qui a le potentiel de modifier la façon dont vous gérez le travail.

Les campagnes Workfront vous permettent d’organiser des projets provenant de différents portfolios et programmes dans un nouveau conteneur de travail. Ce nouveau conteneur évoluera dans les prochaines versions pour éventuellement inclure tous les objets de travail actuellement gérés dans des silos distincts.

Les fonctionnalités suivantes sont incluses dans cette version :

* Nouvel objet Workfront appelé « Campagnes »

* Nouvelle zone « Campagnes » (Beta) dans le menu principal

* Liste des campagnes dans la zone « Campagnes »

* Page « Détails d’une campagne » qui affiche des informations supplémentaires sur une campagne.

* Possibilité d’ajouter des projets à une campagne

* Possibilité de modifier des informations sur une campagne

* Possibilité de renommer l’objet Campagne à partir du modèle de mise en page

  Les personnes chargées de l’administration du système et des groupes Workfront peuvent ajouter la zone « Campagnes » (Beta) dans le menu principal d’un modèle de mise en page. Elle est ainsi disponible pour l’ensemble des utilisateurs et des utilisatrices à qui le modèle est affecté. Une fois disponible, n’importe quelle personne dans Workfront peut créer une campagne.




