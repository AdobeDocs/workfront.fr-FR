---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurer les éléments supprimés
description: Si vous êtes administrateur ou administratrice de Workfront, vous pouvez restaurer des projets, tâches, problèmes, documents et modèles dans Adobe Workfront s’ils ont été supprimés au cours des 30 derniers jours. Au bout de 30 jours, ces éléments sont supprimés définitivement et ne peuvent pas être restaurés.
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 99%

---

# Restaurer les éléments supprimés

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Si vous êtes administrateur ou administratrice de Workfront, vous pouvez restaurer des projets, tâches, problèmes, documents et modèles dans Adobe Workfront s’ils ont été supprimés au cours des 30 derniers jours. Au bout de 30 jours, ces éléments sont supprimés définitivement et ne peuvent pas être restaurés.

Lorsque vous restaurez un objet, tous ses objets et champs enfant sont également restaurés. Par exemple, si vous restaurez un projet, tous les tâches, problèmes, documents, heures, notes, affectations et données personnalisées du projet seront également restaurés.

Une personne chargée de l’administration de groupes peut également restaurer ces objets pour un groupe qu’elle gère.

>[!IMPORTANT]
>
>* Si vous supprimez un rapport, un tableau de bord, un utilisateur ou une utilisatrice, un groupe, une équipe ou une itération, cet élément ne peut pas être restauré.
>* Dans un groupe, lorsqu’une personne autre que l’administrateur ou administratrice du groupes charge un document directement dans la zone Documents d’un objet, seulement un administrateur ou une administratrice Workfront peut restaurer le document.
>
>* Si vous déplacez une tâche ou un problème et que vous choisissez de ne pas déplacer également les documents joints à la tâche ou au problème, les documents sont supprimés et placés dans la corbeille pendant 30 jours. Un administrateur ou une administratrice peut les restaurer et ils sont rattachés à la tâche déplacée ou au problème déplacé. Si la tâche ou le problème a été supprimé depuis son déplacement, les documents sont restaurés dans la zone Documents de la page de l’utilisateur ou de l’utilisatrice de l’administrateur ou de l’administratrice qui les restaure.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>Ou</p>
       <p>Actuel : formule</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informations récupérées lorsque vous restaurez un projet, une tâche ou un problème.

Lorsque vous restaurez un projet, une tâche ou un problème, les informations associées suivantes sont récupérées avec cet élément :

* Commentaires et réponses dans la zone Mises à jour
* Approbations
* Affectations
* Formulaires personnalisés
* Configuration de la file d’attente
* Dossiers commerciaux, notamment cartes de score, objectifs et risques
* Équipes de projet
* Dates
* Problèmes
* Tâches
* Sous-tâches
* Statuts
* Informations financières :

   * Enregistrements de facturation
   * Taux de facturation
   * Frais

* Informations concernant la chronologie :

   * Tâches antérieures
   * Contraintes de tâche
   * Type de durée

* Niveaux de référence

  Les références de tâches sont récupérées lorsque vous restaurez leur projet ou tâche parent, mais pas lorsque vous restaurez des tâches supprimées individuellement.

* Heures (et identifiants d’heure)

  Le fait que les heures soient restaurées ou non sur l’élément supprimé dépend des paramètres choisis lors de la configuration des préférences pour les feuilles de temps et les heures. Pour plus d’informations, voir [Configurer l’effet sur les heures lorsqu’un objet est supprimé et restauré](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* URL de l’élément

  Une fois restauré, l’URL de l’élément reste la même. Si des personnes ont créé des signets de navigateur pour l’élément, ils restent valides.

* Accès et autorisations

  Les personnes qui avaient accès à l’élément avant qu’il ne soit supprimé récupèrent l’accès après sa restauration.

* Documents (y compris les documents relus)

  Tenez compte des points suivants lors de la restauration de documents et de versions de document :

   * Les documents qui ont été supprimés individuellement peuvent être restaurés individuellement.

     Les documents qui ont été supprimés avec leur projet, tâche ou problème parent sont récupérés lorsque vous restaurez le parent, mais vous ne pouvez pas les restaurer individuellement.

   * Toutes les versions d’un document ou d’une épreuve de document sont restaurées lorsque le document est restauré.\
     Les versions individuelles d’un document ou d’une épreuve de document qui ont été supprimées individuellement ne peuvent pas être récupérées.

## Informations qui ne sont pas récupérées lorsque vous restaurez un projet, une tâche ou un problème

Lorsque vous restaurez un projet, une tâche ou un problème, les informations associées suivantes ne seront pas récupérées avec celui-ci :

* Mentions J’aime
* Parrainages
* Envoi de l’adresse e-mail dans une file d’attente des demandes
* Favoris

  Un projet, une tâche ou un problème que vous avez ajouté au menu Favoris avant de le supprimer n’apparaît pas à nouveau dans le menu Favoris après sa restauration.

* Objets de résolution

  Un objet de résolution est un problème converti configuré avec l’option **Conserver le problème d’origine et lier sa résolution à ce** &lt;**project** or **task)**>. Si vous supprimez le projet ou la tâche parent, le problème n’est plus identifié comme un objet de résolution, car il n’existe plus de lien le reliant au projet ou à la tâche. Si vous restaurez le parent, le lien ne sera pas restauré.

  Pour plus d’informations sur la manière dont un administrateur ou une administratrice Workfront ou de groupes configure les problèmes pour qu’ils correspondent à l’objet de résolution lors de la conversion, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) et [Configurer les préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  Pour plus d’informations sur la conversion de problèmes, voir [Vue d’ensemble des problèmes de conversion dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Restaurer des éléments

{{step-1-to-setup}}

1. Cliquez sur **Corbeille** > **Récemment supprimés**.
1. Cliquez sur l’onglet **Projets**, **Tâches**, **Problèmes**, **Modèles** ou **Documents** selon le type d’élément à restaurer.

   Les éléments sont triés par la colonne **Date de suppression** par défaut.

1. Sélectionnez jusqu’à 10 éléments à restaurer.

   Si vous supprimez une tâche enfant, elle s’affiche dans la liste.

   Si vous supprimez une tâche parent, seule la tâche parent s’affiche dans la liste. Mais toutes les tâches enfants sont restaurées lorsque vous restaurez une tâche parent.

1. Cliquez sur **Restaurer** pour restaurer les éléments sélectionnés à leur emplacement d’origine.
1. (Facultatif) Pour afficher rapidement l’élément restauré, suivez les étapes dans [Afficher l’élément restauré](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Pour plus d’informations sur ce qui se passe après la restauration d’un élément, voir la section [Que se passe-t-il après la restauration des éléments ?](#what-happens-after-you-restore-items) dans cet article.

## Que se passe-t-il après la restauration des éléments ? {#what-happens-after-you-restore-items}

* Lorsque vous restaurez des tâches et des sous-tâches, elles s’affichent dans l’ordre dans lequel elles étaient avant d’être supprimées.

  Cependant, si l’ordre des autres tâches change pendant la suppression de la tâche, la tâche peut être restaurée au bas de la liste des tâches ou sous-tâches.

* Après avoir restauré un élément :

   * Un message s’affiche pour vous indiquer si vous avez réussi.

     Vous recevez également une notification par e-mail. Si vous avez restauré plusieurs éléments, l’e-mail les répertorie.

   * Un commentaire s’affiche dans la zone Mises à jour du projet, de la tâche ou du problème, ainsi que dans celle de l’objet parent.

     Cela ne se produit pas lorsque vous restaurez un document ou un modèle.

## Épreuves restaurées

Lorsqu’une personne restaure un document comportant une épreuve, la page Activités de relecture de l’épreuve peut afficher le nom de la première personne active dans l’administration Workfront répertoriée pour l’instance de votre organisation (par ordre d’identifiant de profil) au lieu de la personne qui a restauré l’épreuve.
