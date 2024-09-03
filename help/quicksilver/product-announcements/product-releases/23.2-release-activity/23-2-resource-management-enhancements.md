---
title: 23.2 Améliorations de la gestion des ressources
description: 23.2 Améliorations de la gestion des ressources
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 100%

---

# 23.2 Améliorations de la gestion des ressources

Cette page décrit toutes les améliorations apportées à la gestion des ressources avec la version 23.2 de l’environnement de Prévisualisation. Ces améliorations seront mises à disposition dans l’environnement de production avec la version 23.2.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication 23.2, voir l’article [Vue d’ensemble de la version 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Présentation du champ Durée du travail pour calculer précisément la capacité de l’utilisateur ou l’utilisatrice

>[!NOTE]
>
>Version de prévisualisation : 16 février 2023 ; version de production prévue : 2 mars 2023

Pour permettre aux gestionnaires de ressources de calculer précisément la disponibilité de leurs utilisateurs et utilisatrices et de tenir compte du temps que ceux-ci consacrent à des tâches réelles liées au projet, nous proposons le concept de temps de travail dans Adobe Workfront.

Vous pouvez définir la valeur du champ Temps de travail pour chaque utilisateur ou utilisatrice lorsque vous créez ou modifiez son profil. Pour plus d’informations, voir la section [Modifier le profil d’un utilisateur ou d’une utilisatrice](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Le champ Temps de travail correspond au pourcentage de temps, en équivalent temps complet (FTE), que l’utilisateur ou l’utilisatrice peut consacrer à un travail réel, sans compter les frais généraux. Le temps de travail doit être un nombre décimal, d’une valeur comprise entre 0 et 1. Par exemple, une disponibilité de 20 % pour le travail effectif serait de 0,2.

La valeur par défaut de ce champ est 1, ce qui indique que la personne consacre la totalité de son équivalent temps complet au travail réel lié au projet.

Suite à cette mise à jour, Workfront calcule la disponibilité de l’utilisateur ou l’utilisatrice à l’aide des formules ci-dessous, en fonction de votre sélection dans la zone des préférences de la gestion des ressources :

* Planning par défaut :
* Capacité de l’utilisateur ou l’utilisatrice = [(Heures du planning - Exceptions du planning) * ETC - Congés] * Durée de travail
* Planning de l’utilisateur ou l’utilisatrice :
* Capacité de l’utilisateur ou l’utilisatrice = (Heures du planning - Exceptions au planning - Congés) * Temps de travail.

Pour plus d’informations, voir la section [Configurer les préférences de [!UICONTROL gestion des ressources]](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3415608/){target=_blank}
