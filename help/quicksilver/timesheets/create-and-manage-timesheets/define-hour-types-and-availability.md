---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Définir les types d'heures et la disponibilité
description: Un type d’heure est une étiquette qui vous permet de classer les heures saisies par catégorie. Selon les exigences de votre organisation en matière de rapports sur les heures, il peut s’agir d’un élément essentiel de la consignation des heures.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 28%

---

# Définir les types d&#39;heures et la disponibilité

<!--Audited: 6/2025-->

Un type d’heure est une étiquette qui vous permet de classer les heures saisies par catégorie. Selon les exigences de création de rapports de votre entreprise pour les heures, cela peut être une partie essentielle du temps de connexion.

Il existe 2 ensembles de types d’heures dans Adobe Workfront :

* **Heures générales** : heures qui ne sont pas associées à un projet, comme les congés maladie ou l’administration. Vous pouvez uniquement consigner des heures générales sur la feuille de temps.
* **Heures spécifiques au projet** : heures enregistrées sur les projets, tâches et événements. Vous pouvez consigner les heures spécifiques à un projet à partir de n’importe quel emplacement où vous pouvez consigner les heures.

Lors de la consignation des heures dans Workfront, les types d’heures spécifiques au projet qui sont disponibles dépendent des options de configuration définies au niveau du système, du projet et de l’utilisateur ou de l’utilisatrice. (Les types d’heures suivants, spécifiques au projet, sont toujours disponibles par défaut : Heures du projet, Heures de la tâche et Heures du problème.)

Les types d’heures disponibles à sélectionner lors de la journalisation du temps (sur les projets, tâches et événements) sont déterminés d’abord par les types d’heures rendus disponibles à l’échelle du système par l’administrateur système, puis par les types d’heures sélectionnés au niveau du projet et de l’utilisateur.

Une fois les types d’heures appropriés configurés, vous pouvez consigner le temps à partir de plusieurs emplacements dans Workfront. Pour plus d’informations, voir la section [Consigner le temps](../../timesheets/create-and-manage-timesheets/log-time.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard</p> 
   <p>Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès d’administrateur ou administratrice système pour définir les types d’heures à l’échelle du système et pour modifier tous les utilisateurs et utilisatrices</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Accès en gestion au projet pour définir les types d’heures sur un projet</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Définir la disponibilité au niveau du système

L’administrateur système détermine les types d’heures spécifiques au projet qui sont disponibles dans tout le système. Pour plus d’informations, voir [Gérer les types d’heures](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Définir la disponibilité au niveau du projet {#define-availability-at-the-project-level}

La personne propriétaire du projet détermine si tous les types d’heures définis au niveau du système sont disponibles sur le projet (et les tâches et problèmes au sein du projet), ou si seul un sous-ensemble de ces types d’heures est disponible.

{{step1-to-projects}}

1. Sur la page **Projets**, sélectionnez le projet pour lequel vous souhaitez déterminer la disponibilité des types d’heures.
1. Cliquez sur l’icône **Plus** ![Icône Plus](assets/more-icon.png) en regard du nom du projet dans l’en-tête, puis cliquez sur **Modifier**. Le panneau **Modifier le projet** s’ouvre.

1. Dans la section **Paramètres du projet**, recherchez le paramètre **Filtrer les types d’heures**.

1. Sélectionnez **Non** pour que tous les types d’heures spécifiques au projet soient disponibles dans le projet.

   Ou

   Sélectionnez **Oui** pour rendre disponible uniquement un sous-ensemble des types d’heures spécifiques au projet, puis sélectionnez les **types d’heures** à rendre disponibles. Vous pouvez sélectionner plusieurs types d’heures.

   >[!NOTE]
   >
   >   Tenez compte des points suivants :
   >   
   >   * Si vous sélectionnez **Oui**, seuls les types d’heures que vous sélectionnez sont disponibles pour la sélection lors de la journalisation des heures dans le projet (ou pour les tâches et événements au sein du projet).
   >   
   >   * Si vous sélectionnez **Oui** et ne sélectionnez aucun type d&#39;heures, le projet affiche uniquement les types d&#39;heures généraux.
   >
   >   * Les mêmes sélections doivent être effectuées au niveau de la personne individuelle pour que l’utilisateur ou l’utilisatrice puisse voir ces options de type d’heure sur le projet.
   >
   >   * Lorsque le Type d’heure par défaut de l’utilisateur et un Type d’heure filtré du projet correspondent, ce type d’heure est sélectionné par défaut lors de la journalisation de l’heure.

1. Cliquer sur **Enregistrer**.

## Définir la disponibilité au niveau de l&#39;utilisateur

Vous pouvez saisir des heures pour un type d&#39;heure donné dans des projets, des tâches et des événements uniquement si ce type d&#39;heure a été mis à disposition au niveau du système, du projet et de l&#39;utilisateur.

Si vous rendez un type d&#39;heures disponible au niveau de l&#39;utilisateur comme décrit dans cette section, mais que vous ne le voyez pas lors de la journalisation du temps sur un projet, une tâche ou un événement, ce type d&#39;heures n&#39;a pas été rendu disponible sur le projet. Pour plus d’informations, consultez la section suivante de cet article : [Définir la disponibilité au niveau du projet](#define-availability-at-the-project-level).

Pour définir les types d’heure disponibles pour un utilisateur ou une utilisatrice, procédez comme suit :

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur votre avatar en haut à gauche.

   Ou

   Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/adobe-main-menu.png) dans le coin supérieur droit, le cas échéant, puis cliquez sur **Profil Workfront**.

1. Cliquez sur l’icône **Plus** ![Plus](assets/more-icon.png) en regard du nom d’utilisateur, puis cliquez sur **Modifier**. La zone **Modifier la personne** s’ouvre.

   >[!IMPORTANT]
   >
   >Seul un administrateur ou une administratrice système peut modifier les autres utilisateurs et utilisatrices. Si vous disposez d’une licence de plan, vous pouvez modifier les types d’heures sur votre propre profil.


1. Dans la section **Planification des ressources**, dans le menu déroulant **Types d’heures disponibles**, effectuez l’une des opérations suivantes, en fonction des types d’heures que vous souhaitez rendre disponibles lors de la consignation de temps pour un projet, une tâche ou un problème :

   * **Pour rendre tous les types d’heures disponibles pour l’utilisateur :** sélectionnez tous les types d’heures.\
     Si vous ne sélectionnez aucun type d’heure, cela revient techniquement à sélectionner tous les types d’heures. Cependant, dans ce cas, tous les types d&#39;heures ne sont disponibles pour l&#39;utilisateur que pour les projets, tâches et événements pour lesquels **Non** est sélectionné dans l&#39;option **Filtrer les types d&#39;heures** lors de la modification du projet, comme décrit dans [Définir la disponibilité au niveau du projet](#define-availability-at-the-project-level).
   * **Pour ne mettre à la disposition de l’utilisateur ou de l’utilisatrice qu’un sous-ensemble de types d’heures :** sélectionnez uniquement les types d’heures que vous souhaitez rendre disponibles.

     Pour que les types d’heures sélectionnés au niveau utilisateur soient disponibles pour les projets, les tâches et les événements, ces mêmes types d’heures doivent également être sélectionnés dans l’option **Filtrer les types d’heures** lors de la modification du projet, comme décrit dans [Définir la disponibilité au niveau du projet](#define-availability-at-the-project-level).

1. (Facultatif) Dans le menu déroulant **Type d’heure par défaut**, sélectionnez un type d’heure. Lorsque le type d’heure par défaut de l’utilisateur et un type d’heure filtré de projet correspondent, ce type d’heure est sélectionné par défaut lors de la journalisation de l’heure.

1. Cliquez sur Enregistrer les modifications. **&#x200B;**&#x200B;Désormais, lorsque vous consignez des heures pour un projet, une tâche ou un événement, les types d’heures que vous sélectionnez sont disponibles si ces mêmes types d’heures ont été rendus disponibles au niveau du projet.

## Fonctionnement des types d’heures au niveau de l’utilisateur ou de l’utilisatrice et au niveau du projet

La liste suivante décrit les types d&#39;heures qui s&#39;affichent sur un objet après avoir personnalisé et filtré les types d&#39;heures au niveau de l&#39;utilisateur et au niveau du projet lorsque vous enregistrez des heures sur l&#39;objet :

* Après avoir personnalisé le type d’heures par défaut pour l’utilisateur et les types d’heures du projet filtré, le menu déroulant Type d’heures affiche l’un des types d’heures suivants :

   * Lorsque l’utilisateur possède un Type d’heure par défaut sur son profil et que le projet a le même Type d’heure filtré, ce Type d’heure s’affiche comme la valeur par défaut sélectionnée lors de la journalisation du temps ; les heures de projet, de tâche ou d’événement s’affichent en tant qu’options supplémentaires.

   * Lorsque l’utilisateur ne dispose pas d’un type d’heures par défaut et que le projet a des types d’heures filtrés, le type d’heures par défaut lors de la journalisation du temps est Projet, Tâche ou Événement, mais les types d’heures filtrés du projet s’affichent également sous forme d’options supplémentaires.

   * Lorsque l’utilisateur ne dispose pas d’un type d’heure par défaut et que le projet ne comporte aucun type d’heure filtré, seuls les types d’heures Projet, Tâche ou Événement s’affichent par défaut en fonction de l’objet auquel vous connectez du temps.

   * Lorsque l’utilisateur dispose d’un type d’heure par défaut et que le projet ne comporte aucun type d’heure filtré, les heures du projet, de la tâche ou de l’événement sont affichées par défaut lors de la journalisation du temps sur les objets, et aucun autre type d’heure n’est disponible sous forme d’options, y compris le type d’heure par défaut de l’utilisateur.

* Une fois que vous avez personnalisé les types d’heures et défini les types d’heures disponibles pour votre utilisateur ou utilisatrice ou filtré les types d’heures pour un projet, les scénarios suivants se produisent :

   * Lorsque vous avez sélectionné tous les types d’heures pour le champ Type d’heures disponible dans le profil de votre utilisateur et que les types d’heures du projet ne sont pas filtrés, tous les types d’heures disponibles s’affichent lorsque vous consignez du temps.
   * Lorsque vous avez sélectionné uniquement un sous-ensemble de types d’heures pour le champ Type d’heures disponible dans le profil de votre utilisateur et que les types d’heures du projet ne sont pas filtrés, seuls les types d’heures de l’utilisateur s’affichent lorsque vous consignez du temps.
   * Lorsque vous avez sélectionné tous les types d’heures pour le champ Type d’heure disponible dans le profil de votre utilisateur et que les types d’heures du projet sont filtrés, seuls les types d’heures du projet et les types d’heures par défaut tels que Heure du projet, Heure de la tâche, Heure de l’événement sont affichés, selon l’objet.
   * Lorsque vous avez sélectionné uniquement un sous-ensemble de types d’heures pour le champ Type d’heures disponible dans le profil de votre utilisateur et que les types d’heures du projet sont filtrés, seuls les types d’heures communs à l’utilisateur et au projet s’affichent. Si aucun type d’heure n’est commun à l’utilisateur ou à l’utilisatrice et au projet, seuls les types d’heures par défaut s’affichent (durée du projet, durée de la tâche, heure du problème).

>[!TIP]
>
>   Si vous sélectionnez un autre type d&#39;heures que le type d&#39;heures par défaut pour un objet, le type d&#39;heures devient contigu. La prochaine fois que vous consignerez des heures pour le même objet, le type d’heure sera automatiquement celui que vous avez sélectionné la dernière fois.

