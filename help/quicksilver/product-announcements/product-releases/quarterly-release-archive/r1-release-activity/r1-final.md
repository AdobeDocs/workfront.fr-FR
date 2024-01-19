---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Final
description: Activité Version 2018.3
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---

# R1 Final

La fonctionnalité suivante n’est actuellement pas disponible dans la version bêta ou d’aperçu, mais est actuellement disponible dans l’environnement de production dans R1 :

## Décisions d’approbation pour les bons à tirer de la zone de travail My Work Area (Workfront)

Désormais, lorsqu’un utilisateur vous ajoute à un BAT et lui accorde le rôle d’approbateur ou de réviseur et d’approbateur (soit à partir de l’application BATHQ autonome, soit à l’aide d’un workflow automatisé dans Workfront ), la demande de validation s’affiche dans l’onglet Approbations de votre zone de travail Mes tâches. Vous pouvez ensuite afficher le BAT et prendre une décision d’approbation sur le BAT directement depuis Workfront.

Pour plus d’informations sur l’ajout d’utilisateurs à un BAT à l’aide d’Automated Workflow, voir [Partage d’un BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Partage d’un BAT dans Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

Pour plus d’informations sur la façon de prendre des décisions d’approbation à partir de la zone Mon travail, voir [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## Rapport sur les approbations de la vérification dans la zone de travail Mes (Workfront)

Vous pouvez maintenant créer un rapport basé sur l’objet Validation de BAT. Ce rapport vous permet de rendre compte des validations de BAT effectuées par les utilisateurs dans les zones Mon travail où des décisions n’ont pas encore été prises.

Les rapports de validation des BAT contiennent les informations suivantes :

* Document soumis à approbation
* Nom de l’approbateur
* Version du BAT
* ID de l&#39;épreuve
* Date de création du BAT

Vous accédez à cette validation lors de la création d&#39;un rapport basé sur un objet, comme décrit dans la section [Création d’un rapport personnalisé](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour plus d’informations sur le rapport d’objet Approbations de BAT, voir [Présentation des objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) dans [Présentation des objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Générer automatiquement une nouvelle version d’un BAT de document à l’aide de la fonction glisser-déposer (Workfront)

Lorsque vous utilisez la méthode glisser-déposer pour ajouter une nouvelle version d’un document nécessitant une vérification, un BAT est généré automatiquement. Le BAT dispose des mêmes options et workflows que le BAT d’origine ou la version précédente.

Auparavant, lorsque vous ajoutiez une nouvelle version du document, le BAT n’était pas généré automatiquement sur la nouvelle version et vous deviez générer à nouveau le BAT pour la nouvelle version.

Lorsque vous utilisez le menu Plus de documents pour charger une nouvelle version, un BAT n’est pas généré automatiquement.

Pour plus d’informations, voir la section

## Activation de l’accès direct à BAT par tous les utilisateurs de la vérification de performance à partir de l’interface de Workfront (Workfront)

Vous pouvez maintenant permettre à tous les utilisateurs de la vérification de votre système d’accéder en toute transparence à votre compte BATHQ Premium directement depuis l’interface de Workfront. Lorsque cette option est activée, tous les utilisateurs de l’authentification voient une icône BATHQ dans la barre de navigation globale qui les dirige vers le site BATHQ.

Cette option n’est pas activée par défaut. Pour activer cette option, contactez le support technique de Workfront et demandez cet accès pour tous les utilisateurs de vérification de performance de votre système.

Pour plus d’informations, voir [Accès au BAT Workfront à partir d’Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) in  [Accès au BAT Workfront à partir d’Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Avant cette modification, seul l’administrateur de Workfront pouvait accéder directement au site BAT depuis l’interface de Workfront.

## Nouvelle option pour la connexion sécurisée TLS pour le courrier sortant (Workfront)

Lorsque vous choisissez de gérer votre communication Workfront à l’aide de votre propre serveur de messagerie, vous pouvez maintenant activer votre messagerie sortante pour utiliser une connexion sécurisée TLS.

Avant cette amélioration, vous ne pouviez activer la messagerie sortante que par le biais d’une connexion sécurisée SSL.

Pour plus d’informations sur la configuration de votre messagerie sortante, voir .

## Nouveau champ pour la gestion des emails dans l’environnement de test de prévisualisation

Workfront désactive désormais toutes les communications par courrier électronique à partir de l’environnement Preview Sandbox et de l’environnement d’actualisation personnalisée. Si vous souhaitez recevoir des notifications par courrier électronique de la part des environnements de prévisualisation Sandbox ou d’actualisation personnalisée, vous devez activer cette fonctionnalité dans vos paramètres utilisateur.

Pour plus d’informations, voir les informations suivantes :

* [Environnement Adobe Workfront Preview Sandbox](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) in [Environnement Adobe Workfront Preview Sandbox](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* &quot;Réception d’emails à partir de l’environnement de test d’actualisation personnalisée&quot; dans [Environnement Sandbox d’actualisation personnalisée d’Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook pour Office 365 (Workfront)

Le module complémentaire Workfront pour Outlook 365 est désormais disponible. 

Pour plus d’informations sur l’utilisation du module complémentaire, voir [Utilisation du module complémentaire Workfront avec Outlook pour Office 365.](https://support.workfront.com/hc/en-us/sections/205046167)

## Recherche dans l’application mobile (Workfront)

Vous pouvez désormais rechercher des objets dans l’application mobile, comme vous le faites dans l’application web. La nouvelle fonctionnalité de recherche recherche recherche d’abord les éléments de la liste Éléments récents, ainsi que les objets qui ont été précédemment téléchargés sur votre périphérique mobile. La liste des éléments récents est la même que celle que vous voyez dans l’application web.

>[!NOTE]
>
>Cette fonctionnalité sera disponible la première semaine de mai 2017.

Pour plus d’informations sur l’application mobile, voir la section &quot;Recherche dans Mobile&quot; dans  

## Aide améliorée dans l’application mobile : Tutorials (Workfront)

À compter de la version mobile d’avril, de nouveaux écrans de tutoriels vous guideront tout au long de votre expérience mobile. Lorsque vous vous connectez à l’application mobile pour la première fois et que vous utilisez une fonctionnalité pour la première fois, un bref tutoriel s’affiche, expliquant le fonctionnement de cette fonctionnalité. Le tutoriel ne s’affiche qu’une seule fois, la première fois que vous utilisez une fonction spécifique.

Pour plus d’informations sur l’application mobile, voir .

## Recherche dans les documents PDF (ProofHQ)

Vous pouvez désormais effectuer des recherches dans des documents PDF, des documents de bureau et des pages web statiques.

Pour plus d’informations, voir  [Recherche de contenu dans un BAT](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## Mise à jour de la barre de navigation globale (ProofHQ)

Les comptes ProofHQ Premium intégrés à Workfront voient maintenant les améliorations suivantes apportées à la barre de navigation globale dans ProofHQ :

* Nouvelle image de profil utilisateur 
* Aspect mis à jour

## Inclure des informations supplémentaires dans les vues personnalisées (ProofHQ)

Vous pouvez désormais inclure les informations supplémentaires suivantes dans les vues personnalisées :

* **Données au niveau des destinataires**\
  Vous pouvez configurer des vues personnalisées afin d’inclure les colonnes suivantes relatives aux données au niveau du destinataire : Rôle, Position, Alertes par e-mail, Mon délai, Date d’ajout au bon à tirer et Recherche de destinataire.\
  Pour plus d’informations, voir [Créer et gérer des vues personnalisées dans le BAT Workfront](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Données de vérification**\
  Vous pouvez configurer des vues personnalisées afin d’inclure les colonnes suivantes relatives aux données de vérification : Nombre de commentaires (toutes versions), Taille sur disque, Type de BAT, Nombre de fichiers par version, Données de pièce jointe du commentaire (taille sur le disque, nom de fichier) et Filtrage par sous-dossier.\
  Pour plus d’informations, voir [Créer et gérer des vues personnalisées dans le BAT Workfront](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **Données d’étape liées aux workflows automatisés**\
  Vous pouvez configurer des vues personnalisées afin d’inclure les colonnes suivantes relatives à des étapes individuelles des processus automatisés : état SOCD, échéances d’évaluation, nom d’étape actif, nom d’étape suivant, nom d’étape et modèle.\
  Pour plus d’informations, voir [Créer et gérer des vues personnalisées dans le BAT Workfront](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Améliorations des rapports de vérification (anciennement Analytics) (ProofHQ)

La fonctionnalité de création de rapports (anciennement appelée Analytics) contient les améliorations suivantes :

* Nouveaux types de rapports par défaut :

   * Délai d’exécution de la preuve
   * Pourcentage d&#39;approbation en retard
   * Première activité de preuve
   * Nombre de commentaires et de réponses

* Imprimer les rapports
* Aspect mis à jour

## Affichage de la fonctionnalité BATHQ dans l’environnement d’aperçu (BATHQ)

Les fonctionnalités publiées sur BATHQ seront d’abord disponibles pour le test dans l’environnement Aperçu avant la publication dans l’environnement de production.

Ce nouveau workflow de publication de la fonctionnalité Aperçu avant production vous permettra d’être mieux préparé aux futures mises à jour de votre environnement de production BATHQ.

Pour plus d’informations sur l’environnement d’aperçu de BATHQ, voir [Aperçu de l’environnement de test Sandbox - BAT Workfront](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
