---
product-area: betas
navigation-topic: new-commenting-exprience-beta
title: Nouvelle activité de mise à jour d’une expérience de commentaire
description: Examinez l’activité de publication hebdomadaire pour découvrir la nouvelle expérience de commentaires d’Adobe Workfront.
author: Alina
feature: Product Announcements
role: User, Admin
exl-id: 276b28f0-3955-4a0e-aa31-604b291f2f14
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '2223'
ht-degree: 2%

---

# Nouvelle activité de mise à jour d’une expérience de commentaire

<!--take the badge out when it comes to production GA for everyone-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
* <span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> -->


>[!IMPORTANT]
>
>Les informations de cet article font référence aux fonctionnalités publiées pendant la phase bêta pour la nouvelle expérience de commentaire.
>
>Le programme bêta pour la nouvelle expérience de commentaires a commencé en avril 2023 et s&#39;est terminé en octobre 2023.
>
>Les fonctionnalités publiées pendant la période bêta ont été mises à la disposition de tous les clients à partir de la version du quatrième trimestre 2023 (octobre 2023) et le programme bêta a été fermé.
> 
><br>Pour plus d’informations, voir les articles suivants : </br>
>
>* Pour plus d’informations sur les fonctionnalités publiées pendant la nouvelle période bêta de l’expérience, voir [Nouvelle expérience de commentaire](../../betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>* Pour plus d’informations sur les fonctionnalités publiées pour l’expérience de commentaires après la fermeture du nouveau programme bêta d’expérience de commentaires, consultez la page d’aperçu de la version actuelle du produit.

<!--
 This page contains information about the release timeline for the new commenting experience which is currently ongoing in Adobe Workfront. 

For general information on the new commenting experience, including a list of features that are currently available or in research, see [New commenting experience](../new-commenting-experience-beta/unified-commenting-experience.md). 


>[!IMPORTANT]
>
>The new commenting experience launched in Beta with the 23.2 release. For information about the original release, see [23.2 Release overview](../../product-releases/23.2-release-activity/23-2-release-overview.md). 
>
>Features that are released to the Workfront objects that support the beta commenting experience are also released to the Updates section of the following objects as the only commenting experience: 
>* Goals
>* Cards in the Boards area. 

-->

## Nouvelle chronologie de la mise à jour des commentaires

La nouvelle expérience de commentaire apporte une nouvelle conception à la section Mises à jour des objets Workfront.

Pour plus d’informations sur les objets Workfront qui affichent la section Mises à jour, voir [Présentation de la section Mises à jour](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

Vous trouverez ci-dessous une chronologie planifiée avec des jalons clés pour la publication de la nouvelle expérience de commentaire dans l’environnement de production. Outre les jalons ci-dessous, nous continuerons à améliorer l’expérience de commentaires grâce à des améliorations plus modestes.

Pour plus d’informations sur les fonctionnalités publiées pendant la période bêta et leur date de publication, voir la section [Fonctionnalités publiées pendant la période bêta](#features-released-during-the-beta-period) dans cet article.

Pour plus d’informations sur les fonctionnalités publiées pour la nouvelle expérience de commentaires après la fin de la période bêta, consultez la page de présentation de la version actuelle.

Voici un calendrier planifié de la publication de la nouvelle expérience de commentaires :

* Avec la version 23.2 (6 avril 2023) :
   * Lancement de l’expérience de commentaires bêta pour les problèmes
   * Publication de la nouvelle expérience de commentaire pour les objectifs (comme seule expérience)
* Avec la version 23.3 (20 juillet 2023) :
   * Lancez la version bêta des commentaires pour les projets, les tâches et les documents.
   * Publication de la nouvelle expérience de commentaires pour les cartes dans la zone Panoramas (comme seule expérience)
* Au cours de la version du quatrième trimestre 2023 (version limitée, disponible uniquement pour les clients qui choisissent la version rapide) :
   * Libérez la nouvelle expérience de commentaires pour les modèles, les tâches de modèle, les programmes, les portefeuilles, les équipes, les utilisateurs et les feuilles de temps (comme seule expérience).
   * Mettez à jour l’expérience de commentaire bêta pour que les projets, les tâches, les problèmes et les documents deviennent l’option par défaut. Le libellé &quot;Beta&quot; est supprimé.
* Avec la version du quatrième trimestre 2023 (23.10) (26 octobre 2023)
   * Libérez la nouvelle expérience de commentaires pour les modèles, les tâches de modèle, les programmes, les portefeuilles, les équipes, les utilisateurs et les feuilles de temps (la seule expérience) à tous les clients.
   * Faites de la nouvelle expérience de commentaire pour les projets, les tâches, les problèmes et les documents l’option par défaut.

  >[!IMPORTANT]
  >
  >    Cela mettra fin à l’étape bêta de la nouvelle expérience de commentaire.

   * Publiez toutes les fonctionnalités relatives aux commentaires à partir de cette date dans les versions mensuelles et trimestrielles actuelles.
* Fin 2023 :
   * Conservez l’expérience héritée de commentaires comme option secondaire pour les objets suivants : projets, tâches, problèmes et documents. La nouvelle expérience de commentaire est l’option par défaut pour tous les utilisateurs.

  >[!NOTE]
  >
  >    Les itérations conserveront l’expérience héritée de commentaires. La nouvelle expérience de commentaire ne sera pas disponible pour les itérations.

* Premier trimestre 2024 (janvier 2024) :

   * Supprimez l’option permettant de revenir au flux de commentaires hérité et de faire du nouveau flux de commentaires la seule expérience pour tous les objets, à l’exception des itérations.

## Fonctionnalités publiées pendant la période bêta

Les fonctionnalités documentées dans cette section sont désormais disponibles pour tous les clients et dans tous les environnements.

Les fonctionnalités suivantes ont été ajoutées à l’expérience de commentaires au cours de la phase bêta, entre la version 23.2 (6 avril 2023) et la version du quatrième trimestre 2023 (26 octobre 2023).

Les informations suivantes font référence à l’activité de publication chaque semaine, en commençant par la mise à jour la plus récente.

### Semaine du 16 octobre 2023

#### Ajoutez les informations &quot;au nom de &lt; nom d’utilisateur >&quot; lors de l’ajout de commentaires lors de la connexion en tant qu’autre utilisateur.

Lors de la reconception de l’expérience de commentaire, nous avons supprimé l’indicateur &quot;au nom de &lt; nom d’utilisateur >&quot; lorsqu’un administrateur Workfront ou de groupe ajoutait des commentaires lorsqu’il était connecté en tant qu’autre utilisateur. Ces informations ont maintenant été restaurées.

Aperçu et production pour tous les clients : 19 octobre 2023.

### Semaine du 11 septembre 2023

#### La nouvelle expérience de commentaires capture les informations à partir du 1er janvier 2019.

>[!NOTE]
>
>Cette limitation a été supprimée après le 28 novembre 2023. Pour plus d’informations, voir [Présentation de la version du premier trimestre 2024](../../product-releases/24-q1-release-activity/24-q1-release-overview.md).


Les projets, tâches, problèmes et documents affichent désormais les mises à jour à partir du 1er janvier 2019. Avant cette amélioration, la nouvelle expérience de commentaires capturait uniquement les mises à jour de juin 2022 pour ces objets.

Pour plus d’informations, voir [Nouvelle expérience de commentaire](../new-commenting-experience-beta/unified-commenting-experience.md).

Aperçu et production pour tous les clients : 11 septembre 2023.

### Semaine du 21 août 2023

#### Modifier le format d’horodatage dans l’onglet Commentaires

Nous avons mis à jour le format d’horodatage des commentaires des utilisateurs dans l’onglet Commentaires du nouveau flux de commentaires. Dans le cadre de cette modification, les commentaires de l’année en cours n’affichent plus l’année dans l’horodatage. Le survol d’un horodatage affiche la date complète, y compris l’année.

Les modifications n’ont aucune incidence sur les mises à jour du système dans l’onglet Activité du système .

Aperçu et production pour tous les clients : 24 août 2023

### Semaine du 14 août 2023

[Visionnez une démonstration vidéo de toutes les fonctionnalités publiées au cours de la semaine du 14 août 2023](https://video.tv.adobe.com/v/3422912/){target=_blank}

#### Nouvelle expérience de commentaire pour des objets supplémentaires

<!--
[!BADGE In production for Fast Release ]{type=Positive}
-->

La nouvelle expérience de commentaire sera disponible pour les objets suivants, peu après la version 23.3 de Production : tâches de modèle, modèles, feuilles de temps, équipes, utilisateurs, programmes, portefeuilles.

Il s’agit de la seule expérience de commentaire pour ces objets, car l’expérience de commentaire héritée est supprimée lorsque vous y accédez.

Pour plus d’informations, voir [Nouvelle expérience de commentaire](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

Version d’aperçu : 17 août 2023

Version de production pour une version rapide : avec la version 23.8 (31 août 2023)

Version de production pour tous les clients : avec la version 23.10 (octobre 2023)

#### Nouvelle mise à jour de la conception du nouveau flux de commentaires

<!--
[!BADGE In production for Fast Release ]{type=Positive}
-->

Nous avons repensé le nouveau flux de commentaires pour lui donner un aspect plus actualisé. Voici quelques améliorations :

* Le contenu du flux de commentaires est centré sur la page, plutôt que sur toute la largeur de la page.

* L’icône de menu Plus est déplacée dans le coin supérieur droit du commentaire, plutôt que près du bouton J’aime.

* Les boutons J’aime et Répondre sont maintenant positionnés les uns à côté des autres.

* Le bouton Temps journal a été déplacé dans le coin supérieur droit de la zone de commentaire.

* L’invite Ajouter une réponse a été ajoutée pour inviter les utilisateurs à ajouter une réponse à une réponse existante.

* Il existe une ligne de séparation entre chaque thread de commentaire

Pour plus d’informations, voir [Onglet Mises à jour - Aperçu](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

Version d’aperçu : 17 août 2023

Production pour une version rapide : avec la version 23.8 (31 août 2023)

Production pour une version trimestrielle : avec la version 23.10 (octobre 2023)

#### La nouvelle expérience de commentaire est l’expérience par défaut pour les projets, les tâches, les problèmes et les documents.

<!--
[!BADGE In production for Fast Release ]{type=Positive}
-->

Nous faisons de la nouvelle expérience de commentaire l’expérience par défaut pour les objets suivants : projets, tâches, problèmes et documents.  L’expérience de commentaire héritée restera une option alternative lors de l’accès à ces objets.

Pour prendre en charge cette modification, nous avons également renommé la bascule &quot;Commentaires bêta&quot; en &quot;Nouveau commentaire&quot;.

Pour plus d’informations, voir [Nouvelle expérience de commentaire](../new-commenting-experience-beta/unified-commenting-experience.md).

Version d’aperçu : 17 août 2023

Production pour une version rapide : avec la version 23.8 (31 août 2023)

Production pour une version trimestrielle : avec la version 23.10 (octobre 2023)

#### Améliorations des avatars lors du balisage des utilisateurs dans une mise à jour

Pour vous donner une meilleure visibilité sur les utilisateurs balisés dans une mise à jour, nous affichons désormais les noms des utilisateurs (jusqu’à deux utilisateurs) qui sont balisés dans une mise à jour. Pour plus d’informations, voir [Balisage des autres dans les mises à jour](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

Version d’aperçu : 17 août 2023

Production pour une version rapide : avec la version 23.8 (31 août 2023)

Production pour tous les clients : avec la version 23.10 (octobre 2023)

### Semaine du 7 août 2023

#### Ajout d’émoticônes à une mise à jour

Vous pouvez désormais ajouter des émoticônes à un commentaire à l’aide d’une option de barre d’outils de texte enrichi dans la nouvelle expérience de commentaire.

Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). La documentation sera mise à jour au moment de la publication.

Aperçu et production : 10 août 2023

### Semaine du 10 juillet 2023

#### Balisage automatique de tous les participants au thread

Un propriétaire de commentaire est désormais balisé automatiquement dans un thread. Avant cette mise à jour, seuls les utilisateurs qui avaient été balisés en utilisant les balises &quot;@name&quot; ou en les ajoutant à la section &quot;Baliser les personnes ou les équipes&quot; affichée dans la liste des utilisateurs balisés. Vous pouvez ainsi supprimer le propriétaire d’un commentaire du thread, si nécessaire, même s’il n’a pas été balisé manuellement auparavant.

Version d’aperçu : 12 juillet 2023

Version de production : 13 juillet 2023

### Semaine du 3 juillet 2023

#### Nouvelle interface pour l’heure de journalisation

Nous avons repensé l’interface pour le temps de connexion à partir de la zone Mises à jour dans la nouvelle expérience de commentaires.

Pour plus d’informations, voir [Temps de connexion](../../../timesheets/create-and-manage-timesheets/log-time.md).

Version d’aperçu : 5 juillet 2023

Version de production : avec la version 23.3 (juillet 2023)

### Semaine du 26 juin 2023

#### Contenu des commentaires sous une nouvelle réponse

Vous avez désormais la possibilité de copier le contenu d’un commentaire et de l’ajouter comme nouveau guillemet à une réponse dans le même thread lors de l’utilisation de la nouvelle expérience de commentaire.

Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Aperçu : 28 juin 2023

Version de production : 29 juin 2023

### Semaine du 12 juin 2023

#### Nouvelle expérience de commentaire pour les cartes dans la zone Panoramas

La nouvelle expérience de commentaires est désormais disponible pour les cartes dans la zone Panoramas . Il s’agit de la seule expérience disponible pour les cartes. Pour plus d’informations, voir [Présentation de la version 23.3](../../product-releases/23.3-release-activity/23-3-release-overview.md).

Aperçu : 15 juin 2023

Mise à jour de la production pour l’inclusion anticipée : 22 juin 2023

Production pour tous les clients : avec la version 23.3 (juillet 2023)

#### Ajouter des guillemets de bloc à un commentaire

Vous pouvez désormais ajouter des guillemets de bloc à un commentaire à l’aide d’une option de barre d’outils de texte enrichi dans la nouvelle expérience bêta de commentaires.

Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Aperçu : 14 juin 2023

Production : 15 juin 2023

#### Amélioration de l’expérience lors de la modification de commentaires

Vous pouvez désormais utiliser les raccourcis clavier suivants lors de la modification de commentaires :

* Ctrl + Z (CMD + Z pour Mac) pour annuler une modification.

* Ctrl + Y (CMD + Y pour Mac) pour rétablir la modification

Avant ces améliorations, vous ne pouviez pas annuler ou rétablir des modifications lors de la modification d’un commentaire. Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Aperçu : 13 juin 2023

Production : 13 juin 2023

<!--I used the date when I found them in Prod. Not sure when these released, but it could have been before this date-->

### Semaine du 29 mai 2023

#### Nouvelle expérience de commentaires bêta pour les projets, tâches et documents

La nouvelle expérience de commentaires bêta est désormais disponible pour les projets, les tâches et les documents. Avant cette mise à jour, l’expérience de commentaires bêta n’était disponible que pour les problèmes et les objectifs.

Aperçu : 1er juin 2023

Production : avec la version 23.3 (juillet 2023)

>[!NOTE]
>
>Toutes les fonctionnalités publiées pour la nouvelle expérience de commentaires bêta à partir du 1er juin 2023 seront disponibles dans Production pour les projets, les tâches et les documents après la version 23.3 de production. Pour plus d’informations, voir [Présentation de la version 23.3](../../../product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

#### Nouvelle apparence de la balise &quot;modifiée&quot; après modification d’un commentaire

Lors de la modification d’un commentaire dans la nouvelle expérience bêta de commentaires, une balise &quot;modifiée&quot; est ajoutée au commentaire. Cette balise a désormais un nouvel aspect de celle qui a été publiée à l’origine. Les horodatages du commentaire sont ceux du commentaire d’origine. Il ne s’agit pas des horodatages de date et d’heure du moment où la modification a été effectuée.  Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Aperçu : 31 mai 2023

Production : 1er juin 2023

#### Les commentaires des objets enfants s’affichent dans un objet parent.

Lors de l’activation de l’expérience bêta de commentaires, les commentaires associés à un objet enfant sont désormais cumulés à l’objet parent. Par exemple, les commentaires des documents s’affichent maintenant sur le problème où les documents sont joints. Pour plus d’informations, voir [Mise à jour de la section - Aperçu](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

Aperçu : 1er juin 2023

Production : 1er juin 2023

#### Temps de connexion à la nouvelle expérience bêta de commentaires

Vous pouvez consigner le temps nécessaire aux problèmes, aux tâches et aux projets dans la zone Mises à jour lors de l’utilisation de la nouvelle expérience de commentaires bêta. Pour plus d’informations, voir [Temps de connexion](../../../timesheets/create-and-manage-timesheets/log-time.md).

Aperçu : 1er juin 2023

Production : avec la version 23.3 (juillet 2023)

### Semaine du 15 mai 2023

#### Amélioration de l’expérience lors de l’ajout d’hyperliens aux commentaires

Vous pouvez désormais ajouter des liens hypertextes aux commentaires à l’aide des raccourcis clavier suivants :

* Ctrl + V (CMD + V pour Mac) colle un lien au-dessus du texte sélectionné
* CTRL + K (CMD + K pour Mac) ouvre la zone Ajouter des liens .

Avant ces améliorations, vous ne pouviez ajouter des liens hypertexte qu’en cliquant sur l’icône de lien dans la barre d’outils Texte enrichi. Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Aperçu : 17 mai 2023

Production : 18 mai 2023

### Semaine du 1er mai 2023

#### Les images sont supprimées de la zone Documents lorsque des pièces jointes sont supprimées de commentaires ou lorsque des commentaires contenant une pièce jointe sont supprimés.

Nous sommes en train de modifier le fonctionnement des pièces jointes lors de la suppression ou de la modification d’un commentaire contenant une pièce jointe. Désormais, lorsque vous modifiez un commentaire et supprimez la pièce jointe, ou lorsque vous supprimez un commentaire contenant une pièce jointe, la pièce jointe est également supprimée de votre zone Documents. Avant cette modification, dans l’expérience de commentaire précédente, les pièces jointes étaient conservées dans votre zone Documents. Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Disponible pour les problèmes de commentaires sur l’expérience bêta et pour les objectifs Workfront, par défaut, aux dates suivantes :

* Aperçu et production : 4 mai 2023


### 27 avril 2023

La mise à jour de maintenance suivante a été publiée pour les commentaires de problème bêta et pour les objectifs :

Modifier les images jointes lors de la modification d’un commentaire. Pour plus d’informations, voir la section &quot;Mise à jour de maintenance le 27 avril&quot; de l’article <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">Mises à jour en avril 2023</a>.

### 20 avril 2023

La mise à jour de maintenance suivante a été publiée pour les commentaires de problème bêta et pour les objectifs :

Conserver les images sous format brouillon lors de l’abandon d’une mise à jour pour les objectifs et les problèmes liés à l’expérience bêta de commentaires. Pour plus d’informations, voir la section &quot;Mise à jour de maintenance le 20 avril&quot; de l’article <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">Mises à jour en avril 2023</a>.

### 17 avril 2023

La mise à jour de maintenance suivante a été publiée pour les commentaires de problème bêta et pour les objectifs :

Afficher les nouveaux commentaires en dehors de la zone d’écran visible dans la section Mises à jour des problèmes (nouvelle expérience de commentaires bêta) et Objectifs. Pour plus d’informations, reportez-vous à la section &quot;Mise à jour de maintenance le 17 avril&quot; de l’article .  <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">Mises à jour en avril 2023</a>.


### Semaine du 6 avril 2023

Nouvelle expérience bêta de commentaires lancée pour les problèmes.
Les mêmes fonctionnalités que celles publiées pour la version bêta des commentaires pour les objets Workfront sont publiées en même temps pour les objectifs pour tous les utilisateurs ayant accès aux objectifs de Workfront. Pour plus d’informations, voir [Présentation de la version 23.2](../../product-releases/23.2-release-activity/23-2-release-overview.md).
