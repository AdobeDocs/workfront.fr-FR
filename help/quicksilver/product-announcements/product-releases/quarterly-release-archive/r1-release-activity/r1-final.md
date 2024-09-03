---
content-type: release-notes
navigation-topic: product-releases-archive
title: Version R1 finale
description: Activité Version 2018.3
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 100%

---

# Version R1 finale

La fonctionnalité suivante n’est actuellement pas disponible dans la version bêta ou préliminaire, mais est actuellement disponible dans l’environnement de production dans R1 :

## Prendre des décisions d’approbation pour les épreuves à partir de la zone Mon travail (Workfront)

Désormais, lorsqu’un utilisateur ou une utilisatrice vous ajoute à une épreuve et lui accorde le rôle de personne approbatrice ou de personne approbatrice et chargée de la révision (soit à partir de l’application ProofHQ autonome, soit à l’aide d’un workflow automatisé dans Workfront), la demande d’approbation s’affiche dans l’onglet Approbations de votre zone de travail Mon travail. Vous pouvez ensuite afficher l’épreuve et prendre une décision d’approbation sur l’épreuve directement à partir de Workfront.

Pour plus d’informations sur l’ajout d’utilisateurs et d’utilisatrices à une épreuve à l’aide d’un workflow automatisé, voir [Partager une épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) dans [Partager une épreuve dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

Pour plus d’informations sur la façon de prendre des décisions d’approbation depuis la zone Mon travail, voir [Approuver du travail](../../../../review-and-approve-work/manage-approvals/approving-work.md) dans [Approuver du travail](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Créer un rapport sur les approbations de relecture dans la zone Mon travail (Workfront)

Vous pouvez désormais créer un rapport basé sur l’objet Approbation d’épreuve. Ce rapport vous permet de créer un rapport sur les approbations d’épreuve des zones Mon travail des utilisateurs et utilisatrices où des décisions n’ont pas encore été prises.

Les rapports d’approbation d’épreuve contiennent les informations suivantes :

* Document soumis à approbation
* Nom de la personne chargée de l’approbation
* Version de l’épreuve
* ID de l&#39;épreuve
* Date de création de l’épreuve

Vous accédez à cette approbation lors de la création d’un rapport basé sur un objet, comme décrit dans la section [Créer un rapport personnalisé](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur le rapport d’objet Approbations d’épreuves, voir la section [Comprendre les objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) dans [Comprendre les objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Générer automatiquement une nouvelle version d’une épreuve de document à l’aide de la fonction glisser-déposer (Workfront)

Lorsque vous utilisez la méthode glisser-déposer pour ajouter une nouvelle version d’un document nécessitant une relecture, une épreuve est générée automatiquement. L’épreuve dispose des mêmes options et workflows que l’épreuve d’origine ou la version précédente.

Auparavant, lorsque vous ajoutiez une nouvelle version du document, l’épreuve n’était pas générée automatiquement sur la nouvelle version et vous deviez générer à nouveau l’épreuve pour la nouvelle version.

Lorsque vous utilisez le menu Plus des documents pour charger une nouvelle version, une épreuve n’est pas générée automatiquement.

Pour plus d’informations, voir la section dans

## Activer l’accès direct à ProofHQ pour toutes les personnes de la relecture à partir de l’interface de Workfront (Workfront)

Vous pouvez désormais permettre à tous les utilisateurs et utilisatrices de relecture de votre système d’accéder en toute transparence à votre compte ProofHQ Premium directement depuis l’interface de Workfront. Lorsque cette option est activée, tous les utilisateurs et utilisatrices de relecture voient une icône ProofHQ dans la barre de navigation globale qui les dirige vers le site ProofHQ.

Cette option n’est pas activée par défaut. Pour activer cette option, contactez l’assistance technique de Workfront et demandez cet accès pour tous les utilisateurs et utilisatrices de relecture de votre système.

Pour plus d’informations, voir [Accéder à Workfront Proof à partir d’Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) dans [Accéder à Workfront Proof à partir d’Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Avant cette modification, seulement l’administrateur ou l’administratrice de Workfront pouvait accéder directement au site ProofHQ depuis l’interface de Workfront.

## Nouvelle option pour la connexion sécurisée TLS pour le courrier sortant (Workfront)

Lorsque vous choisissez de gérer votre communication Workfront à l’aide de votre propre serveur de messagerie, vous pouvez maintenant activer votre messagerie sortante pour utiliser une connexion sécurisée TLS.

Avant cette amélioration, vous ne pouviez activer la messagerie sortante que par le biais d’une connexion sécurisée SSL.

Pour plus d’informations sur la configuration de votre messagerie sortante, voir .

## Nouveau champ pour la gestion des e-mails dans l’environnement de prévisualisation de sandbox

Workfront désactive désormais toutes les communications par e-mail depuis l’environnement de prévisualisation de sandbox et l’environnement à actualisation personnalisée. Si vous souhaitez recevoir des notifications par e-mail depuis des environnements de prévisualisation de sandbox ou à actualisation personnalisée, vous devez activer cette fonctionnalité dans vos paramètres d’utilisateur ou d’utilisatrice.

Pour plus d’informations, consultez ce qui suit :

* [Environnement de prévisualisation de sandbox Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) dans [Environnement de prévisualisation de sandbox Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* « Recevoir des e-mails du sandbox à actualisation personnalisée » dans [Environnement de sandbox à actualisation personnalisée Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook pour Office 365 (Workfront)

Le module complémentaire Workfront pour Outlook 365 est désormais disponible. 

Pour plus d’informations sur l’utilisation du module complémentaire, voir [Utiliser le module complémentaire Workfront avec Outlook pour Office 365.](https://support.workfront.com/hc/fr-fr/sections/205046167)

## Rechercher dans l’application mobile (Workfront)

Vous pouvez désormais rechercher des objets dans l’application mobile, comme dans l’application web. La nouvelle fonctionnalité de recherche recherche d’abord les éléments de la liste Éléments récents, ainsi que les objets qui ont été précédemment téléchargés sur votre équipement mobile. La liste des éléments récents est la même que celle que vous voyez dans l’application web.

>[!NOTE]
>
>Cette fonctionnalité est disponible depuis la première semaine de mai 2017.

Pour plus d’informations sur l’application mobile, voir la section Recherche mobile dans

## Aide améliorée dans l’application mobile : tutoriels (Workfront)

À compter de la version mobile d’avril, de nouveaux écrans de tutoriels vous guideront tout au long de votre expérience mobile. Lorsque vous vous connectez à l’application mobile pour la première fois et que vous utilisez une fonctionnalité pour la première fois, un bref tutoriel s’affiche, expliquant son fonctionnement. Le tutoriel ne s’affiche qu’une seule fois, la première fois que vous utilisez une fonction spécifique.

Pour plus d’informations sur l’application mobile, voir .

## Recherche dans les documents PDF (ProofHQ)

Vous pouvez désormais effectuer des recherches dans des documents PDF, des documents Office et des pages web statiques.

Pour plus d’informations, voir [Rechercher du contenu dans une épreuve](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Mise à jour de la barre de navigation globale (ProofHQ)

Les comptes ProofHQ Premium intégrés à Workfront voient maintenant les améliorations suivantes apportées à la barre de navigation globale dans ProofHQ :

* Nouvelle image de profil utilisateur
* Aspect mis à jour

## Inclure des informations supplémentaires dans les vues personnalisées (ProofHQ)

Vous pouvez désormais inclure les informations supplémentaires suivantes dans les vues personnalisées :

* **Données au niveau des personnes destinataires**\
  Vous pouvez configurer des vues personnalisées afin d’inclure les colonnes suivantes relatives aux données au niveau des personnes destinataires : Rôle, Position, Alertes par e-mail, Mon délai, Date d’ajout à l’épreuve et Recherche de personne destinataire.\
  Pour plus d’informations, voir [Créer et gérer les vues personnalisées dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Données de relecture**\
  Vous pouvez configurer des vues personnalisées afin d’inclure les colonnes suivantes relatives aux données de relecture : Nombre de commentaires (toutes versions), Taille sur disque, Type d’épreuve, Nombre de fichiers par version, Données de pièce jointe du commentaire (taille sur le disque, nom de fichier) et Filtrage par sous-dossier.\
  Pour plus d’informations, voir [Créer et gérer les vues personnalisées dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Données d’étape liées aux workflows automatisés**\
  Vous pouvez configurer des vues personnalisées afin d’inclure les colonnes suivantes relatives aux étapes individuelles des workflows automatisés : Statut SOCD, Échéances d’étapes, Nom d’étape actif, Nom d’étape suivant, Nom d’étape et Modèle.\
  Pour plus d’informations, voir [Créer et gérer les vues personnalisées dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Améliorations des rapports de relecture (anciennement Analytics) (ProofHQ)

La fonctionnalité de création de rapports (anciennement Analytics) contient les améliorations suivantes :

* Nouveaux types de rapports par défaut :

   * Délai d’exécution de l’épreuve
   * Pourcentage d’approbation en retard
   * Heure de la première activité d’épreuve
   * Nombre de commentaires et de réponses

* Impression des rapports
* Aspect mis à jour

## Afficher la fonctionnalité ProofHQ dans l’environnement de prévisualisation (ProofHQ)

Les fonctionnalités liées à ProofHQ seront d’abord disponibles pour le test dans l’environnement de prévisualisation avant leur publication dans l’environnement de production.

Ce nouveau workflow de prévisualisation des fonctionnalités avant leur production permet de mieux vous préparer aux futures mises à jour de votre environnement de production ProofHQ.

Pour plus d’informations sur l’environnement de prévisualisation de ProofHQ, voir [Prévisualiser l’environnement de test Sandbox - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
