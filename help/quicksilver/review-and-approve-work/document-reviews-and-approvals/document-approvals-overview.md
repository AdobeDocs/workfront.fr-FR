---
product-area: documents
navigation-topic: approvals
title: Aperçu de la révision et de l’approbation unifiées
description: En savoir plus sur la révision et l’approbation unifiées optimisées par Workfront et Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
source-git-commit: d35e6c33479ed051aaa87b07ddf38811fffc0cc0
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# Aperçu de la révision et de l’approbation unifiées

La révision et l’approbation unifiées optimisées par Workfront et Frame.io permettent aux coordinateurs de projet de gérer les projets et de planifier le travail dans Workfront, tandis que les créatifs, les spécialistes marketing et les parties prenantes peuvent réviser et approuver les ressources dans Frame.io.

## Exigences d’intégration

* Workfront et Frame.io doivent être déployés sur la même organisation Identity Management system (IMS).

* Les utilisateurs ne peuvent appartenir qu’à une seule instance Workfront au sein de l’organisation IMS.

* L’instance Workfront doit être activée sur l’expérience unifiée Adobe et le stockage d’entreprise Adobe.

* L’intégration doit être configurée par Adobe Professional Services.


## Basé sur le stockage d’entreprise Adobe

La révision et l’approbation unifiées reposent sur le stockage d’entreprise d’Adobe, une solution de stockage dans le cloud qui sert de référentiel central pour les ressources de l’ensemble des produits d’entreprise d’Adobe, y compris Workfront et Frame.io. <!--, and Creative Cloud.-->

Les principaux avantages du stockage d’entreprise dans Adobe sont les suivants :

* Couche de stockage unifiée pour les ressources de création et de gestion de travail
* Autorisations centralisées avec le système Adobe Identity Management (IMS) pour un contrôle d’accès sécurisé
* Visibilité de bout en bout des ressources dans Workfront et Frame.io <!--, and Creative Cloud apps -->
* Stockage évolutif et gestion des quotas pour les besoins de l&#39;entreprise

Pour plus d’informations, consultez [Présentation du stockage d’entreprise ](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Révision et approbation unifiées

Grâce à la révision et à l’approbation unifiées, vous pouvez :

* Créer et gérer des révisions et des approbations directement depuis Workfront
* Suivre le statut des révisions et des validations en temps réel
* Centraliser les commentaires et les approbations au même endroit
* Vérifiez que toutes les parties prenantes ont accès aux dernières versions des ressources
* Utiliser les réviseurs d’IA pour automatiser les révisions de conformité de la marque
* et plus...

Pour plus d’informations, voir [Approbations de documents unifiés : index des articles](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Utilisation de la visionneuse Frame.io

Utilisez la visionneuse Frame.io pour réviser et approuver des ressources. La visionneuse Frame.io fournit

* Outils de balisage et de commentaires
* Historique et comparaison des versions
* Commentaires horodatés pour les révisions vidéo
* Accès mobile pour les révisions et les approbations en cours de route

Pour plus d’informations, voir [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Limites de révision vidéo

Les demandes d’épreuves vidéo sont plafonnées à 10 % du nombre total de licences d’utilisation payantes de Workfront d’une entreprise (standard et light). Cette limite est appliquée au niveau de l’organisation.

Les administrateurs et administratrices de Workfront reçoivent des notifications lorsque l’utilisation atteint 80 % et 100 % de la limite.

Cette limite ne s’applique pas aux clients Frame.io Enterprise.

#### Types de fichiers pris en charge dans la visionneuse Frame.io

La visionneuse Frame.io prend en charge tous les types courants de vidéos, d’images, d’audio, de PDF et de MS® Office. Pour obtenir la liste détaillée des fichiers pris en charge, voir [Types de fichiers pris en charge sur Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Accès et licences pour la visionneuse Frame.io

La visionneuse Frame.io est la visionneuse par défaut pour tous les workflows de révision et d’approbation Workfront. Il est automatiquement inclus pour tous les utilisateurs de Workfront disposant d’une licence payante. Aucune licence Frame.io supplémentaire n&#39;est requise pour utiliser la visionneuse Frame.io pour les révisions et les approbations.

Si votre entreprise souhaite tirer parti des fonctionnalités Frame.io supplémentaires disponibles avec cette intégration, telles que le chargement direct de ressources vers des projets dans Frame.io, vous pouvez acheter une licence d’entreprise Frame.io. Contactez votre représentant de compte Adobe pour planifier une démonstration et explorer les avantages de la solution Frame.io complète.

La fonctionnalité de relecture de Workfront n&#39;est pas disponible avec cette intégration.

## Gestion de projet puissante dans Workfront

Les coordinateurs de projet peuvent tirer parti des puissantes fonctionnalités de gestion de projet de Workfront pour planifier, suivre et gérer le travail.

Pour plus d’informations sur la gestion des projets dans Workfront, voir [Projets : index d’article](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Structure appliquée et conventions de nommage

Étant donné que la révision et l’approbation unifiées sont créées à l’aide du stockage d’entreprise Adobe, il existe une structure appliquée et des conventions de nommage à connaître lors de la gestion des projets et des documents.

* Les noms d’objet doivent être uniques et ne peuvent pas être dupliqués
* Le stockage d’entreprise Adobe nécessite des noms uniques pour les objets homologue avec le même parent dans l’arborescence hiérarchique
* Les documents ne peuvent pas porter le même nom s&#39;ils appartiennent au même projet
* Les noms de document ne peuvent pas contenir les caractères spéciaux suivants : \ / : * ? « | &lt; >
* Les noms de document sont limités à 255 caractères maximum

Compte tenu de ces limitations, Workfront renomme automatiquement les objets ou les documents selon les besoins afin d’éviter les conflits.

### Partage et autorisations

Dans le cadre de l’intégration, les autorisations utilisateur sont contrôlées dans Workfront et descendent vers Frame.io. Cela signifie que vous ne pouvez pas inviter un utilisateur à un projet dans Frame.io ni modifier les autorisations utilisateur dans Frame.io. Ces actions doivent être effectuées via la fenêtre modale Partage de projet dans Workfront.

Le tableau suivant montre comment les autorisations Workfront sont mappées aux autorisations Frame.io :

<table>
<tr>
<th>Autorisation utilisateur Workfront</th>
<th>Autorisation utilisateur Frame.io</th>
</tr>
<tr>
<td>Gérer</td>
<td>Modifier et partager</td>
</tr>
<tr>
<td>Contribuer</td>
<td>Modifier et partager</td>
</tr>
<tr>
<td>Afficher</td>
<td>Commentaire uniquement</td>
</tr>
</table>



### Gestion des documents dans Workfront

Les documents chargés vers Workfront sont stockés dans le stockage d’entreprise d’Adobe et sont accessibles dans Workfront et Frame.io. Lorsque vous chargez un document vers une tâche ou un événement dans Workfront, un dossier généré par le système est créé dans le stockage d’entreprise Adobe et hérite des autorisations de la tâche ou de l’événement. Tous les documents chargés vers cette tâche ou cet événement sont stockés dans ce dossier et y héritent des autorisations. Pour plus d’informations sur les documents dans Workfront, voir [Présentation de la zone des nouveaux documents](/help/quicksilver/documents/managing-documents/documents-area.md) et [Autorisations d’objet et présentation du niveau d’accès pour le modèle de stockage d’entreprise Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Limites de l’expérience du document

Les fonctionnalités suivantes du document ne sont pas incluses :

<!--* External document providers-->
* Accès à la relecture dans Workfront
* Visionneuse de documents dans Workfront
* Documents favoris
* Demander des documents










<!--
# Unified Approvals overview

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Unified Approvals, previously referred to as New Document Approvals, is a holistic redesign of the existing approvals process that is currently in development for Adobe Workfront. Currently available in limited release, it is designed to be a practical and effective solution for businesses requiring comprehensive stakeholder engagement and version-specific document approvals. Its thoughtful design and purposeful new features facilitate collaboration, role clarity, and version control in the approval process, enhancing efficiency and accountability.

## Key differences from Proofing and legacy document approvals

**Differences from Proofing**

* Document approval participants display in the document Summary, not the proofing workflow tab.
* Unified Approvals are not supported in the current reporting tool. 

    You can join the new Canvas Dashboards beta to [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md), or you can use the Document approval metrics widget available in new Home and Canvas Dashboards provides the following details about Unified Approvals:

    * Approvals by decision
    * Average approval time
    * Pending approvals
    * Overdue approvals

**Differences from Legacy document approvals**

With Unified Approvals, you can

* Add reviewers in addition to approvers
* Designate an entire Workfront team as either reviewers or approvers
* Set a deadline for the review or approval
* Create and resuse approval templates
* Utilize new versions 
* View multiple key performance indicators for your approvals in Workfront Home widgets
* Use Canvas Dashboards to view reporting details about Unified Approvals

## Using Unified Approvals

For users looking to create or manage document approvals, see the articles listed in [Set up and manage unified approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/set-up-and-manage-doc-asset-approvals-toc.md)

For users looking to review or approve documents for which they have received a request, see the articles listed in [Approve and review documents: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-documents-toc.md).



-->