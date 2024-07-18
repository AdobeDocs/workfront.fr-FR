---
title: mises à jour du projet pendant la période de la version 22.3
description: mises à jour du projet pendant la période de la version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 0876d4d47aad701d5ffadc88868217ebae7e4790
workflow-type: tm+mt
source-wordcount: '1538'
ht-degree: 1%

---

# Améliorations apportées aux projets (version 22.3)

Cette page décrit toutes les améliorations apportées aux projets avec la version 22.3 de l’environnement Aperçu. Ces améliorations ont été apportées à l’environnement de production au cours de la semaine du 11 juillet 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.3, consultez la [présentation de la version 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Délégation de travail en absence du bureau

Désormais, vous pouvez temporairement déléguer les tâches et les problèmes qui vous sont assignés à d’autres utilisateurs lorsque vous envisagez de quitter le bureau pendant une courte période. Ainsi, votre absence ne devient pas un obstacle à la réalisation de vos travaux.

Avant cette amélioration, vous ne pouviez déléguer que les approbations.

Voici quelques-unes des fonctionnalités que nous avons ajoutées avec cette mise à jour :

* Un paramètre dans la zone Tâches et problèmes Préférences de la configuration pour l’administrateur système ou groupe permettant d’activer la délégation dans votre environnement.

* Nouvelle option pour &quot;Déléguer les tâches et les problèmes&quot; dans la zone Accueil pour les utilisateurs disposant d’une licence de révision ou supérieure afin de déléguer leurs tâches.

* Indication dans la page d’accueil et dans la zone Affectations des en-têtes de tâche et d’émission que les éléments sont délégués à d’autres.

* Notifications d’événements dans la zone Configuration et Notifications électroniques dans le profil utilisateur pour contrôler les notifications par e-mail sur le travail délégué


>[!NOTE]
>
>Seuls les utilisateurs disposant d’une licence de révision ou supérieure peuvent déléguer leur travail à d’autres utilisateurs. Le travail peut être délégué à n’importe quel utilisateur, quel que soit son niveau d’accès. Les utilisateurs délégués reçoivent les mêmes autorisations que les personnes désignées sur les éléments délégués. Si ces autorisations sont inférieures à la configuration du niveau d’accès d’un utilisateur, il se peut que les utilisateurs délégués ne puissent pas exécuter certaines des activités sur les tâches et problèmes qui leur sont délégués.


Pour plus d’informations, voir [Délégation de tâche et présentation des problèmes](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Nouvelle expérience lors de la conversion d’un problème en tâche

Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface pour convertir un problème en tâche.

Cette mise à jour inclut :

* Interface utilisateur mise à jour qui correspond au reste de la nouvelle expérience Workfront.

* Accès pour convertir un problème en tâches depuis une liste ou un rapport.

* Les formulaires personnalisés par défaut définis dans la zone Paramètres des tâches du projet de destination ont été ajoutés à la nouvelle tâche.


Pour plus d’informations, voir [Convertir un problème en une tâche dans Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nouvelle expérience lors de la conversion d’un problème en projet sans modèle

Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface pour convertir un problème en projet sans utiliser de modèle.

Outre une interface utilisateur mise à jour qui correspond au reste de la nouvelle expérience Workfront, nous avons également ajouté la possibilité de convertir un problème en projets vierges à partir d’une liste ou d’un rapport.

Pour plus d’informations, voir [Convertir un problème en projet dans Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Balisage intelligent dans le flux de mise à jour

Nous avons amélioré le balisage des utilisateurs dans le flux de mise à jour lorsque vous créez une mise à jour ou que vous répondez à une mise à jour existante. Désormais, lorsque vous marquez un utilisateur pour l’inclure dans une mise à jour, en plus de son nom et de son avatar, nous affichons également son rôle de Principal et son email. Cela permet de distinguer plusieurs utilisateurs portant des noms similaires ou identiques.

Pour plus d’informations, consultez [Baliser d’autres personnes sur les mises à jour](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nouvelle syntaxe pour les calculs dans les champs personnalisés

Pour vous préparer aux améliorations à venir qui vous aideront à ajouter des calculs aux formulaires personnalisés, nous avons normalisé la syntaxe des champs référencés que vous ajoutez à un calcul. Il est facile d’utiliser cette nouvelle syntaxe car le système la saisit pour vous lorsque vous commencez à saisir le nom d’un champ, puis vous la sélectionnez.

## Conserver des informations précises lorsque deux utilisateurs ayant un rôle commun sont impliqués dans un processus d’approbation

Afin d’assurer l’exactitude de vos données pour la validation du travail, nous avons apporté une modification à l’enregistrement des informations d’approbation sur un élément lorsqu’un processus d’approbation multirôle est associé à l’élément.

Certains processus d’approbation nécessitent l’approbation de deux rôles différents, et deux approbateurs différents peuvent avoir l’un de ces rôles en commun. Maintenant, lorsque cela se produit, une fois les décisions d’approbation prises, Workfront enregistre chaque approbateur et leur rôle respectif associé au processus d’approbation.

Avant cette modification, les deux approbations étaient enregistrées pour le deuxième utilisateur, car il partageait l’un des rôles d’approbation avec le premier approbateur. Dans ce cas, le second approbateur remplaçait les informations du premier approbateur.

Pour plus d’informations sur les processus d’approbation dans Workfront, consultez la [présentation des processus d’approbation](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Les heures d’affectation ne seront plus supprimées lors de la modification des affectations.

>[!NOTE]
>
>Cette fonctionnalité était initialement prévue avec la version 22.2. Il a été publié en production le 21 avril 2022.


Pour garantir l’exactitude de vos données, nous avons apporté une modification afin de conserver les heures d’affectation et de conserver les heures planifiées de la tâche inchangées lors de la modification des affectations sur la tâche.

Les modifications suivantes ont été apportées aux tâches avec un type de durée simple :

* Les heures planifiées sont conservées lors de la suppression de tous les cessionnaires.

* Les affectations d’affectation individuelles sont conservées lors du remplacement des utilisateurs et des rôles.

* Les affectations d’affectation individuelles sont conservées sur le rôle lors de la suppression de l’utilisateur. (Supprimée de la version. Désormais, les heures planifiées seront définies sur 0 après la suppression de tous les cessionnaires.)


Pour plus d’informations sur les heures planifiées, consultez la [présentation des heures planifiées](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Améliorations des panoramas

Les améliorations suivantes ont été apportées aux panoramas Adobe Workfront :

* Options de filtrage : vous pouvez désormais filtrer par date d’échéance ou statut sur un panorama. Le filtre a également été mis à jour avec des sections réductibles pour séparer les options.

* Panorama d’archives : vous pouvez désormais archiver un panorama lorsque vous vous trouvez dans le panorama, au lieu d’avoir à accéder au tableau de bord des panoramas.

* Ajouter une équipe à un panorama : lorsque vous recherchez des membres, vous pouvez ajouter une équipe entière. Le choix d’une équipe ajoute tous les membres de l’équipe au tableau.

* Zones de dépôt dans les colonnes : lorsque vous faites glisser et déposez une carte d’une colonne de panorama à une autre, une &quot;zone de dépôt&quot; grise indique désormais où la carte sera placée. Auparavant, il n’existait pas d’indicateur visuel de l’emplacement de la carte.

* Cartes connectées : vous pouvez désormais ajouter des cartes connectées à des tâches et des problèmes Workfront. La mise à jour du nom, de la description ou de la personne désignée dans la carte ou la tâche met à jour les mêmes champs dans l’autre emplacement.

* Champ d’état sur toutes les cartes : un champ d’état et un bouton Marquer comme terminé ont été ajoutés aux cartes ad hoc et connectées. Lorsque vous cliquez sur Marquer comme terminé, l’état passe automatiquement à Terminé.

* Convertir une carte ad hoc en carte connectée : vous avez désormais la possibilité de convertir une carte ad hoc en carte connectée à partir des détails de la carte.

* Déconnecter la carte connectée : la déconnexion d’une carte connectée rompt la connexion à l’objet Workfront. La carte reste une carte ad hoc sur le panorama et l’objet Workfront n’est pas affecté.

* Mappage de l’état dans les colonnes : les nouveaux paramètres et stratégies de colonne vous permettent de définir un état, une personne désignée ou une balise appliqué aux cartes déplacées dans cette colonne. En outre, les noms de colonne par défaut d’un nouveau panorama ont été modifiés en Colonne 1, Colonne 2 et Colonne 3.

* Indicateur de mise à jour des champs : un indicateur s’affiche maintenant lorsque vous enregistrez une carte pour confirmer que vos mises à jour ont été enregistrées.


Pour plus d’informations, voir [Prise en main des panoramas dans Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Partage de dossiers uniquement aux cinq premiers niveaux d’une hiérarchie de dossiers

Afin d’optimiser les performances pour les utilisateurs partageant des dossiers, nous limitons actuellement le partage aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet.

Chaque dossier au sixième niveau ou au-dessous hérite de ses configurations de partage à partir du dossier situé directement au-dessus.

Pour plus d’informations sur le partage de dossiers, voir [Partage d’un dossier de document de niveau supérieur](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Campagnes Workfront (Beta) : une nouvelle façon de gérer votre travail

>[!NOTE]
>
>Cette fonctionnalité devrait être supprimée de l’aperçu le 9 janvier 2023. Pour plus d&#39;informations, consultez la [page de présentation des versions 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Cette fonctionnalité ne sera pas incluse dans la version de production 22.3. Il sera publié en production avec une version ultérieure.


>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement en version bêta et est actuellement en cours de construction. Nous continuerons à ajouter des fonctionnalités pour le workflow de Campaign avec les prochaines versions. La participation au programme bêta des campagnes Workfront est volontaire.

Nous introduisons un nouvel objet dans Adobe Workfront qui a le potentiel de modifier la façon dont vous gérez le travail.

Les campagnes Workfront permettent d’organiser dans un nouveau conteneur de travail des projets issus de différents portefeuilles et programmes. Ce nouveau conteneur va évoluer dans les prochaines versions afin d’inclure éventuellement tous les objets de travail actuellement gérés dans des silos distincts.

Les fonctionnalités suivantes sont incluses dans cette version :

* Un nouvel objet Workfront appelé Campaign

* Nouvelle zone Campagnes (Beta) dans le menu principal

* Liste des campagnes dans la zone Campagnes

* Page Détails d’une campagne qui affiche des informations supplémentaires sur une campagne

* Possibilité d’ajouter des projets à une campagne

* Possibilité de modifier des informations sur une campagne

* Possibilité de renommer l’objet Campaign à partir du modèle de mise en page

  Les administrateurs système et groupe Workfront peuvent ajouter la zone Campagnes (Beta) dans le menu principal d’un modèle de mise en page. Elle est ainsi disponible pour tous les utilisateurs affectés au modèle. Une fois disponible, n’importe qui dans Workfront peut créer une campagne.




