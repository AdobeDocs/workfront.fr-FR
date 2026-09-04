---
title: Améliorations des documents du quatrième trimestre de 2026
description: Améliorations des documents du quatrième trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 1b37b57f764d1579629e019c2025c809530124ea
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 3%

---

# Améliorations des documents du quatrième trimestre de 2026

Cette page décrit les améliorations apportées aux documents avec la version du quatrième trimestre 2026 dans l’environnement de Prévisualisation. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du quatrième trimestre 2026, voir [présentation de la version du quatrième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## System Administrators full access to approval templates

>[!NOTE]
>
>Preview: September 4, 2026
>Production fast release: September 4, 2026
>Production for everyone: September 4, 2026
>[!BADGE Off schedule]{type=Neutral}

System Administrators can now view, edit, delete, and bulk-delete every approval template in the account, regardless of who created or shared it. Previously, System Administrators were subject to the same sharing rules as other users, and could only see or manage templates they created or that were shared with them.

For more information, see [Manage approval templates](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md).

-->

<!--

## Frame comment visibility in Workfront

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When an approval workflow is created for a document, users can leave comments and make annotations in the Frame.io viewer. These comments are not displayed in the Workfront Comments panel, but you can view them in the Frame.io viewer.

Now, the Comments panel in Workfront displays a message letting you know when new comments are available in Frame.io.

For more information, see [Add an update to a document](/help/quicksilver/documents/managing-documents/add-update-documents.md).

-->

## Accès direct aux épreuves à partir des liens des e-mails de validation

>[!NOTE]
>
>Aperçu : S.O.
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Lorsqu’un BAT est joint à un document, le lien « Accéder à la révision » dans les e-mails d’approbation ouvre désormais directement la visionneuse d’épreuves, afin que les réviseurs et les approbateurs puissent commencer leur révision immédiatement. Si un document ne comporte pas d’épreuve, le lien continue d’ouvrir la section Validations du document, comme auparavant.

## Ajouter des équipes aux approbations d’objets à l’aide de l’espace de stockage dans le cloud Adobe

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais ajouter une équipe Workfront en tant qu’approbateur ou réviseur sur un modèle d’approbation ou d’approbation de document, au lieu d’ajouter chaque personne individuellement :

* Objets sur l’espace de stockage Adobe dans le cloud : Workfront ajoute chaque membre actif de l’équipe individuellement, de sorte que la liste des approbateurs reflète toujours les personnes qui font actuellement partie de l’équipe.
* Objets utilisant le stockage Workfront hérité : l’équipe est ajoutée par défaut en tant que participant unique, mais vous pouvez désormais choisir d’ajouter chaque membre de l’équipe en tant que participant individuel.
* Dans les modèles d’approbation, Workfront stocke une référence à l’équipe et la développe en membres actifs lorsque vous appliquez le modèle à un document, et non lorsque vous enregistrez le modèle.

Pour plus d’informations, voir :

* [Créer un workflow d’approbation dans la zone Nouveaux documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Créer un workflow d’approbation dans la zone des documents hérités](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Créer un modèle de workflow d’approbation pour les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

## Définir un espace de travail Frame.io sur des modèles de projet

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Si votre entreprise utilise l’espace de stockage cloud Adobe et que vous disposez d’une licence Enterprise Frame.io, vous pouvez désormais choisir un espace de travail Frame.io dans la section Détails du projet sur un modèle de projet. Les projets créés à partir du modèle utilisent automatiquement l&#39;espace de travail défini sur le modèle, de sorte que les projets sont acheminés vers l&#39;espace de travail Frame.io souhaité sans aucune action supplémentaire nécessaire lors de la création du projet.

Le nouveau champ répertorie les espaces de travail Frame.io auxquels vous êtes autorisé à affecter des projets. Le champ reste modifiable sur le modèle à tout moment ; les modifications ne s’appliquent qu’aux projets créés après la mise à jour, de sorte que les projets existants conservent leur espace de travail d’origine.

Une fois qu’un projet est créé à partir du modèle, son champ d’espace de travail Frame.io est en lecture seule et contient des liens vers l’espace de travail dans Frame.io.

Si vous ne disposez pas d’une licence d’entreprise Frame.io, les projets continuent d’accéder à l’espace de travail par défaut pour Workfront.

Pour plus d’informations, voir [Modifier les modèles de projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) et [Gérer les informations dans la zone Présentation du projet](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md).

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

## Message personnalisé dans l’objet de l’e-mail

>[!NOTE]
>
>Aperçu : S.O.
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Lorsque vous définissez un message personnalisé lors de l’approbation d’un document, ce message apparaît désormais également dans l’objet de l’e-mail de demande d’approbation, avec en tête la date d’échéance à laquelle le message est défini. Cela permet aux réviseurs et aux réviseuses de voir ce qui nécessite une attention et à quel moment directement depuis leur boîte de réception, sans ouvrir l’e-mail.

Pour plus d’informations, voir [Créer un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Panneau Versions repensées dans la zone des nouveaux documents

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Si votre entreprise utilise l’espace de stockage dans le cloud d’Adobe, le panneau Versions dans la nouvelle zone Documents présente une nouvelle conception :

* Les versions sont libellées V1, V2, etc. afin d’assurer la cohérence avec Frame.io.
* Chaque version affiche son statut d’approbation, tel que « Approuvé » ou « Retiré », directement dans la liste.
* Le panneau ne répertorie désormais que l’historique des versions ; il n’y a plus d’entrée « dernier fichier » distincte en haut.

Auparavant, les versions étaient horodatées au lieu d’être numérotées.

Pour plus d’informations, consultez [Gérer les versions des documents](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Panneau Approbations repensées dans la zone des nouveaux documents

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Si votre entreprise utilise l’espace de stockage Adobe dans le cloud, le panneau Approbations de la zone des nouveaux documents affiche désormais l’historique des validations pour toutes les versions :

* Le panneau répertorie le workflow d’approbation pour chaque version qui en comporte une, et pas seulement la version actuelle.
* Les workflows retirés restent dans la liste, de sorte que vous pouvez toujours consulter leurs décisions antérieures.
* Développez une version pour afficher ses étapes, les décisions des approbateurs, les règles de décision et les dates d’échéance sans quitter le panneau.

Auparavant, le panneau Approbations affichait uniquement le workflow de la version actuelle.

Pour plus d’informations, voir [Créer un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Joindre des images aux commentaires sur les objets d’espace de stockage dans le cloud Adobe

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 30 juillet 2026
>Production pour tous : 30 juillet 2026
>[!BADGE Hors planning]{type=Neutral}

Les entreprises qui utilisent le stockage dans le cloud Adobe dans le cadre de la révision et de l’approbation unifiées peuvent désormais joindre des fichiers image directement aux commentaires, ce qui permet de conserver les commentaires, le contexte et les visuels d’assistance dans un seul fil de commentaires traçable. Cela comble une lacune précédente où seules les organisations disposant d’un stockage Workfront hérité pouvaient joindre des images aux commentaires.

Tous les formats d’image de type média sont désormais pris en charge pour les organisations de stockage dans le cloud Adobe. (Les commentaires d’objet hérités continuent à prendre en charge les fichiers .jpg, .gif et .png uniquement.) Les fichiers autres que les images ne sont pas pris en charge dans les commentaires pour les objets de stockage cloud hérités ou Adobe.

Pour plus d’informations, voir [Mettre à jour le travail](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Liaison de ressources de Experience Manager Assets à l’espace de stockage dans le cloud Adobe

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Si votre entreprise utilise l’espace de stockage Adobe, vous pouvez lier des ressources individuelles de Experience Manager Assets à n’importe quel objet Workfront prenant en charge les documents. Le contenu lié reste automatiquement synchronisé : les modifications apportées dans Experience Manager Assets apparaissent dans Workfront et vous pouvez extraire de nouvelles versions de ressources sans quitter Workfront.

La liaison est optimisée par le gestionnaire d’accès. Vous obtenez ainsi également des Recherche optimisée par l&#39;IA, des suggestions intelligentes, une analyse de résumés de campagne, etc. lors de la sélection de contenu.

Pour plus d’informations, voir [Lier du contenu de Experience Manager Assets avec l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md).

<!--

## Approval workflow templates are private by default

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Approval templates are now private by default. Previously, every approval requester could see every template in the system, which made template lists long and hard to navigate. Now, a template is visible only to the user who created it, unless the creator shares it.

For more information, see:

* [Share a template](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md#share-a-template) in Manage approval templates
* [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

-->

