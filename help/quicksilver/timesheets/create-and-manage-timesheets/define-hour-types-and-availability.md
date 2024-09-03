---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Définition des types d’heures et de la disponibilité
description: Un type d’heure est une étiquette qui vous permet de classer les heures saisies par catégorie. Selon les exigences de votre organisation en matière de rapports sur les heures, il peut s’agir d’un élément essentiel de la consignation des heures.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: bfaf566e556882078875649549c0dfadacd800b8
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 52%

---

# Définition des types d’heures et de la disponibilité

Un type d’heure est une étiquette qui vous permet de classer les heures saisies par catégorie. Selon les exigences de votre organisation en matière de rapports sur les heures, il peut s’agir d’un élément essentiel de la consignation des heures.

Il existe deux ensembles de types d’heures dans Adobe Workfront :

* **Heures générales :** les heures qui ne sont pas associées à un projet, telles que les congés maladie ou les heures d’administration. Vous ne pouvez consigner les heures générales que sur la feuille de temps.
* **Heures spécifiques à un projet :** heures consignées sur les projets, les tâches et les problèmes. Vous pouvez enregistrer des heures spécifiques à un projet à partir de n’importe quel emplacement où vous pouvez consigner des heures.

Lors de la consignation des heures dans Workfront, les types d’heures spécifiques au projet qui sont disponibles dépendent des options de configuration définies au niveau du système, du projet et de l’utilisateur ou de l’utilisatrice. (Les types d’heures suivants, spécifiques au projet, sont toujours disponibles par défaut : Heures du projet, Heures de la tâche et Heures du problème.)

Les types d’heures disponibles à sélectionner lors de la durée de journalisation (sur les projets, les tâches et les problèmes) sont déterminés d’abord par les types d’heures rendus disponibles à l’échelle du système par l’administrateur système, puis par les types d’heures sélectionnés au niveau du projet et de l’utilisateur.

Après avoir configuré les types d’heures appropriés, vous pouvez consigner les heures à partir de plusieurs endroits dans Workfront, comme décrit dans [Consigner les heures](../../timesheets/create-and-manage-timesheets/log-time.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès d’administrateur ou administratrice système pour définir les types d’heures à l’échelle du système et pour modifier tous les utilisateurs et utilisatrices</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Accès en gestion au projet pour définir les types d’heures sur un projet</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître votre plan ou votre type de licence, contactez l’administration de Workfront.

+++

## Définition de la disponibilité au niveau du système

L’administrateur ou l’administratrice système détermine les types d’heures spécifiques à un projet qui sont mis à la disposition de l’ensemble du système, comme décrit dans la section [Gérer les types d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Définition de la disponibilité au niveau du projet {#define-availability-at-the-project-level}

La personne propriétaire du projet détermine si tous les types d’heures définis au niveau du système sont disponibles sur le projet (et les tâches et problèmes au sein du projet), ou si seul un sous-ensemble de ces types d’heures est disponible.

1. Accédez au projet dans lequel vous souhaitez déterminer la disponibilité des types d’heures.
1. Cliquez sur le menu **Plus** en regard du nom de la tâche, puis cliquez sur **Modifier**.

1. Cliquez sur **Modifier le projet**.
1. Dans la section **Paramètres**, localisez l’option **Filtrer les types d’heures**.

1. Sélectionnez **Non** pour rendre tous les types d’heures spécifiques au projet disponibles dans le projet.

   Ou

   Sélectionnez **Oui** pour n’afficher qu’un sous-ensemble des types d’heures spécifiques au projet, puis sélectionnez les types d’heures à rendre disponibles. (Maintenez la touche Maj enfoncée pour sélectionner plusieurs types d’heures.)

   Si vous sélectionnez cette option, seuls les types d’heures que vous avez sélectionnés seront disponibles lors de l’enregistrement des heures sur le projet (ou sur les tâches et les problèmes au sein du projet). Si vous sélectionnez cette option et que vous ne sélectionnez aucun type d’heure, le projet n’affiche que les types d’heure généraux.

   Les mêmes sélections doivent être effectuées au niveau de la personne individuelle pour que l’utilisateur ou l’utilisatrice puisse voir ces options de type d’heure sur le projet.

   Lorsque le type d’heure par défaut de l’utilisateur et un type d’heure filtré de projet correspondent, ce type d’heure est sélectionné par défaut lors de l’heure de journalisation.

1. Cliquez sur **Enregistrer les modifications**.

## Définition de la disponibilité au niveau de l’utilisateur

Vous pouvez consigner des heures pour un type d’heure donné sur des projets, des tâches et des problèmes uniquement si ce type d’heure a été rendu disponible au niveau du système, au niveau du projet et au niveau de l’utilisateur ou de l’utilisatrice.

Si vous rendez un type d’heure disponible au niveau de l’utilisateur ou de l’utilisatrice comme décrit dans cette section, mais que vous ne voyez pas ce type d’heure lorsque vous consignez des heures sur un projet, une tâche ou un problème, c’est que ce type d’heure n’a pas été rendu disponible sur le projet (comme décrit dans [Définir la disponibilité au niveau du projet](#define-availability-at-the-project-level)).

Pour définir les types d’heure disponibles pour un utilisateur ou une utilisatrice, procédez comme suit :

1. Cliquez sur l’icône **Menu princiapl** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur votre avatar d’utilisateur ou d’utilisatrice dans le coin supérieur gauche.
1. Cliquez sur le menu **Plus** en regard du nom d’utilisateur ou d’utilisatrice, puis cliquez sur **Modifier**.

1. Seul un administrateur ou une administratrice système peut modifier les autres utilisateurs et utilisatrices. Si vous disposez d’une licence de plan, vous pouvez modifier les types d’heures sur votre propre profil.
1. Dans la section **Planification des ressources**, dans le menu déroulant **Types d’heures disponibles**, effectuez l’une des opérations suivantes, en fonction des types d’heures que vous souhaitez rendre disponibles lors de la consignation de temps pour un projet, une tâche ou un problème :

   * **Pour rendre tous les types d’heure disponibles pour l’utilisateur :** sélectionnez tous les types d’heure.\
     Si vous ne sélectionnez aucun type d’heure, cela revient techniquement à sélectionner tous les types d’heures. Cependant, dans ce cas, tous les types d’heure ne sont disponibles pour l’utilisateur que pour les projets, tâches et problèmes pour lesquels **Non** est sélectionné dans l’option **Filtrer les types d’heure** lors de la modification du projet, comme décrit dans la section [Définir la disponibilité au niveau du projet](#define-availability-at-the-project-level).
   * **Pour ne mettre à la disposition de l’utilisateur ou de l’utilisatrice qu’un sous-ensemble de types d’heures :** sélectionnez uniquement les types d’heures que vous souhaitez rendre disponibles.

     Pour que les types d’heures que vous sélectionnez au niveau de l’utilisateur soient disponibles sur les projets, les tâches et les problèmes, ces mêmes types d’heures doivent également être sélectionnés dans l’option **Filtrer les types d’heures** lors de la modification du projet, comme décrit dans la section [Définir la disponibilité au niveau du projet](#define-availability-at-the-project-level).

1. (Facultatif) Dans le menu déroulant **Type d’heure par défaut**, sélectionnez un type d’heure.

   Lorsque le type d’heure par défaut de l’utilisateur et un type d’heure filtré de projet correspondent, ce type d’heure est sélectionné par défaut lors de l’heure de journalisation.

1. Cliquez sur **Enregistrer les modifications**.

   Désormais, lorsque vous consignez le temps pour un projet, une tâche ou un problème, les types d’heures que vous sélectionnez sont disponibles si ces mêmes types d’heures ont été rendus disponibles au niveau du projet.


## Fonctionnement des types d’heures au niveau de l’utilisateur ou de l’utilisatrice et au niveau du projet

La liste suivante décrit les types d’heure qui s’affichent sur un objet après avoir personnalisé et filtré les types d’heure au niveau de l’utilisateur et du projet lorsque vous définissez l’heure de connexion sur l’objet :

* Après avoir personnalisé le type d’heure par défaut pour l’utilisateur et les types d’heures de projet filtrés, le menu déroulant Type d’heure affiche l’un des types d’heures suivants :

   * Lorsque l’utilisateur a un type d’heure par défaut sur son profil et que le projet a le même type d’heure filtrée, ce type d’heure s’affiche comme valeur par défaut sélectionnée lors de l’heure de connexion. Le projet, la tâche ou l’heure de publication s’affichent sous la forme d’options supplémentaires.

   * Lorsque l’utilisateur ne dispose pas d’un type d’heure par défaut et que le projet comporte des types d’heure filtrés, le type d’heure par défaut lors de la journalisation est Projet, Tâche ou Heure de publication, mais les types d’heure filtrés du projet s’affichent également sous forme d’options supplémentaires.

   * Lorsque l’utilisateur ne dispose pas d’un type d’heure par défaut et que le projet ne comporte aucun type d’heure filtré, seuls les types Projet, Tâche ou Heure de publication s’affichent par défaut, selon l’objet sur lequel vous connectez le temps.

   * Lorsque l’utilisateur possède un type d’heure par défaut et que le projet ne comporte aucun type d’heure filtré, le projet, la tâche ou l’option Problème s’affiche par défaut lors de la connexion de l’heure aux objets, et aucun autre type d’heure n’est disponible en tant qu’options, y compris le type d’heure par défaut de l’utilisateur.

* Une fois que vous avez personnalisé les types d’heures et défini les types d’heures disponibles pour votre utilisateur ou utilisatrice ou filtré les types d’heures pour un projet, les scénarios suivants se produisent :

   * Lorsque vous avez sélectionné tous les types d’heure pour le champ Type d’heure disponible dans le profil de votre utilisateur et que les types d’heure du projet ne sont pas filtrés, tous les types d’heure disponibles s’affichent lorsque vous enregistrez l’heure.
   * Lorsque vous avez sélectionné uniquement un sous-ensemble de types d’heure pour le champ Type d’heure disponible dans le profil de votre utilisateur et que les types d’heure du projet ne sont pas filtrés, seuls les types d’heure de l’utilisateur s’affichent lorsque vous enregistrez l’heure.
   * Lorsque vous avez sélectionné tous les types d’heure pour le champ Type d’heure disponible dans le profil de votre utilisateur et que les types d’heure du projet sont filtrés, seuls les types d’heure du projet et les types d’heure par défaut tels que Heure du projet, Heure de la tâche, Heure de la publication dépendent de l’objet.
   * Lorsque vous avez sélectionné uniquement un sous-ensemble de types d’heure pour le champ Type d’heure disponible dans le profil de votre utilisateur et que les types d’heure du projet sont filtrés, vous ne verrez que les types d’heure communs à l’utilisateur et au projet. Si aucun type d’heure n’est commun à l’utilisateur ou à l’utilisatrice et au projet, seuls les types d’heures par défaut s’affichent (durée du projet, durée de la tâche, heure du problème).

>[!TIP]
>
>   Si vous sélectionnez un type d’heure différent du type d’heure par défaut pour un objet, le type d’heure sélectionné persiste. La prochaine fois que vous consignerez des heures pour le même objet, le type d’heure sera automatiquement celui que vous avez sélectionné la dernière fois.

