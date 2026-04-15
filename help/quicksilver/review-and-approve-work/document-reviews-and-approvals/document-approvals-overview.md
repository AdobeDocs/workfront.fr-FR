---
product-area: documents
navigation-topic: approvals
title: Aperçu de la révision et de l’approbation unifiées
description: En savoir plus sur la révision et l’approbation unifiées optimisées par Workfront et Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453d4862883e299fea46b3dfe94548375bfc4209
workflow-type: tm+mt
source-wordcount: '3846'
ht-degree: 0%

---


# Aperçu de la révision et de l’approbation unifiées

La révision et l’approbation unifiées rassemblent Adobe Workfront et Adobe Frame.io dans une expérience unique et profondément connectée, réduisant ainsi les écarts entre la gestion marketing, la révision créative et la diffusion de contenu.
Les coordinateurs de projet gèrent le travail dans Workfront pendant que les créatifs, les spécialistes marketing et les parties prenantes examinent et approuvent les ressources dans la visionneuse Frame.io de qualité professionnelle, le tout sans déplacer les fichiers entre des outils déconnectés.

![Diagramme présentant le workflow de révision et d’approbation unifié, avec les coordinateurs de projet gérant le travail dans Workfront et les réviseurs et approbateurs fournissant des commentaires et prenant des décisions dans la visionneuse Frame.io.](assets/Unified-Review-Approvals-Image.png)


## Exigences d’intégration

* L’instance Workfront doit être activée sur l’expérience unifiée Adobe.


## Basé sur le stockage d’entreprise Adobe

La révision et l’approbation unifiées reposent sur le stockage d’entreprise d’Adobe, une solution de stockage dans le cloud qui sert de référentiel central pour les ressources de l’ensemble des produits d’entreprise d’Adobe, y compris Workfront et Frame.io. <!--, and Creative Cloud.-->

Les principaux avantages du stockage d’entreprise dans Adobe sont les suivants :

* Couche de stockage unifiée pour les ressources de création et de gestion de travail
* Autorisations centralisées avec le système Adobe Identity Management (IMS) pour un contrôle d’accès sécurisé
* Visibilité de bout en bout des ressources dans Workfront et Frame.io <!--, and Creative Cloud apps -->
* Stockage évolutif et gestion des quotas pour les besoins de l&#39;entreprise

Pour plus d’informations, consultez [Présentation du stockage d’entreprise &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md).

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

* Les programmes et les projets ne peuvent pas porter le même nom s&#39;ils appartiennent au même portefeuille.
* Les documents ne peuvent pas porter le même nom s&#39;ils appartiennent au même projet.
* Les noms d&#39;objet ne peuvent pas contenir les caractères spéciaux suivants : \ / : * ? « | &lt; >
* Les noms d’objet sont limités à 255 caractères maximum.

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

## Prise en main de la révision et de l’approbation unifiées

Pour commencer à utiliser la révision et l’approbation unifiées, voir [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

## Questions fréquentes

### Prise en main de la révision et de l’approbation unifiées

+++ Développez pour afficher les questions fréquentes sur la prise en main de la révision et de l’approbation unifiées.

**En quoi consistent la révision et l’approbation unifiées ?**

La révision et l’approbation unifiées sont une intégration native entre Adobe Workfront et Adobe Frame.io qui réunit la gestion du travail et la révision créative dans un seul système connecté. Les coordinateurs de projet planifient et effectuent le suivi du travail dans Workfront, tandis que les réviseurs et les approbateurs utilisent la visionneuse Frame.io de qualité professionnelle pour fournir des commentaires, marquer les ressources et prendre des décisions d’approbation, sans basculer entre des outils distincts ou déplacer manuellement les fichiers.

La révision et l’approbation sont au centre de chaque opération de contenu. C’est là que convergent le travail créatif, la contribution des parties prenantes et les décisions d’entreprise. Lorsque ce processus est distribué à travers des outils déconnectés (threads d’e-mail, messages de conversation, balises de capture d’écran), les conséquences s’aggravent : temps de mise sur le marché plus lent, commentaires perdus, confusion des versions et temps passé à gérer les fichiers au lieu de créer du contenu.

L’examen et l’approbation unifiés permettent de résoudre ce problème en remplaçant le patchwork d’outils d’examen déconnectés par un système moderne, une source unique de vérité qui vit là où le travail se fait déjà.

**Quelles sont les exigences à respecter pour utiliser cette intégration ?**

Pour utiliser la révision et l’approbation unifiées, les conditions suivantes doivent être remplies :

* Workfront et Frame.io doivent être déployés sur la même organisation Adobe Identity Management System (IMS).

* Les utilisateurs ne peuvent appartenir qu’à une seule instance Workfront au sein de l’organisation IMS.

* L’instance Workfront doit être activée sur l’expérience unifiée Adobe et le stockage d’entreprise Adobe.

* Les clients Workfront doivent disposer d’un SKU V2 (cela peut nécessiter un événement de contrat ; contactez votre représentant de compte Adobe).

**Ai-je besoin d’une licence Frame.io pour utiliser cette intégration ?**

Non. La visionneuse Frame.io est automatiquement incluse pour tous les utilisateurs de Workfront disposant d’une licence payante, sans frais supplémentaires. Vous n’avez pas besoin d’une licence Frame.io distincte pour réviser et approuver des ressources via Workfront.

Si votre entreprise souhaite accéder à d’autres fonctionnalités de Frame.io, telles que le chargement direct de ressources vers des projets dans Frame.io, vous pouvez acheter une licence d’entreprise Frame.io. Contactez votre représentant de compte Adobe pour en savoir plus.

**Cela remplace-t-il Workfront Proof ?**

Oui. Lorsque la révision et l’approbation unifiées sont activées, la visionneuse Frame.io devient la principale surface de révision dans Workfront, remplaçant Workfront Proof.

Les clients existants conserveront l’accès à la fonctionnalité de vérification linguistique de Workfront pour tous les projets créés avant l’activation de l’intégration.

**Comment puis-je accéder à la révision et à l’approbation unifiées ?**

**Que dois-je faire pour obtenir l’accès ?**

Pour accéder à la révision et à l’approbation unifiées, votre organisation doit utiliser un SKU Workfront V2. Si vous n’utilisez pas actuellement de SKU V2, un événement de contrat avec Adobe sera nécessaire. Pour démarrer :

* Contactez votre représentant de compte Adobe pour confirmer si votre plan Workfront actuel prend en charge la révision et l’approbation unifiées.

* Si une mise à niveau du SKU est nécessaire, votre représentant de compte vous guidera tout au long du processus de passation de contrats.

* Une fois que votre compte utilise le bon SKU, Adobe Professional Services configure l’intégration pour votre organisation.

   * Si vous ne savez pas qui est votre représentant de compte Adobe, vous pouvez contacter par le biais du portail d’assistance Adobe ou consulter Experience League pour connaître les options de contact.

+++

### Comment fonctionnent la révision et l’approbation unifiées

+++ Développez pour afficher les questions fréquentes sur le fonctionnement de la révision et de l’approbation unifiées.

**Comment fonctionne le workflow de révision et d’approbation ?**

Le workflow suit les étapes générales suivantes :

1. Un coordinateur de projet crée un projet dans Workfront et charge ou lie des ressources.

1. Lorsqu’un actif est prêt à être révisé, le coordinateur crée un workflow d’approbation, soit une approbation à usage unique, soit l’application d’un modèle d’approbation réutilisable.

1. Les réviseurs et approbateurs affectés sont avertis par e-mail et peuvent ouvrir la ressource directement dans la visionneuse Frame.io.

1. Les réviseurs et réviseuses peuvent ajouter des commentaires et des balises. Les approbateurs doivent prendre une décision formelle.

1. Le coordinateur suit le statut en temps réel depuis Workfront.

**Quelle est la différence entre un réviseur et un approbateur ?**

Les réviseurs et réviseuses peuvent ajouter des commentaires et marquer des ressources dans la visionneuse Frame.io. Lorsqu’ils ont terminé, ils marquent leur révision comme terminée. Toutefois, leur action n’est pas nécessaire pour que le workflow d’approbation progresse.

Les approbateurs doivent prendre l&#39;une des décisions suivantes pour faire avancer le workflow d&#39;approbation :

* **Approuver** : la ressource est prête à être utilisée en l’état.

* **Travail nécessaire** : la ressource a besoin d’être modifiée et doit être envoyée à nouveau en tant que nouvelle version pour approbation.

**Quels types de workflows d’approbation puis-je créer ?**

* **Approbations à usage unique** : vous pouvez créer une approbation à usage unique directement sur un document d’un projet, d’une tâche ou d’un événement. Vous attribuez des réviseurs et des approbateurs, définissez des échéances et configurez plusieurs étapes si nécessaire. Les rappels par e-mail automatisés sont envoyés 72 heures avant, 24 heures avant et à l’échéance.

* **Modèles d’approbation** : vous pouvez créer des modèles réutilisables dans la configuration de Workfront. Un modèle définit les réviseurs et réviseuses, les approbateurs et un délai d’achèvement relatif. Vous pouvez créer plusieurs étapes si nécessaire. Une fois qu’un modèle est appliqué à une ressource, l’échéance est calculée automatiquement.

**Comment les utilisateurs externes participent-ils aux révisions ?**

Les utilisateurs Workfront externes sont avertis par e-mail lorsqu’une révision ou une approbation leur est affectée. Ils seront invités à créer une connexion Frame.io pour accéder à la visionneuse et participer au processus de révision.

**Comment effectuer le suivi de la progression de la révision et de l’approbation ?**

Les coordinateurs de projet peuvent surveiller toutes les approbations en cours de route de plusieurs manières :

* Le widget Mes approbations de la zone d’accueil de Workfront fournit un résumé en temps réel des approbations en attente et en retard.

* Le widget Mesures d’approbation du document affiche les temps d’approbation moyens et les répartitions de décision.

* Vous pouvez créer des tableaux de bord de rapports personnalisés dans les tableaux de bord de zone de travail pour une visibilité plus approfondie des activités de révision et d’approbation.

+++


### Révision et approbation des ressources et des vidéos

+++ Développez pour afficher les questions fréquentes sur la révision et l’approbation des ressources et des vidéos.

**Existe-t-il des limites aux révisions vidéo ?**

Oui. Les demandes d’épreuves vidéo sont plafonnées à 10 % du nombre total de licences utilisateur payantes Workfront de votre entreprise (standard et light). Cette limite s’applique au niveau de l’organisation.

Les administrateurs de Workfront recevront des notifications in-app lorsque l’utilisation atteindra 80 % et 100 % de la limite.

Cette limite ne s’applique pas aux clients Frame.io Enterprise. Si votre entreprise examine régulièrement d’importants volumes de contenu vidéo, contactez votre représentant de compte Adobe pour en savoir plus sur les licences Frame.io Enterprise.

**Un même utilisateur peut-il apparaître à plusieurs étapes d’un workflow d’approbation ?**

Oui. Un utilisateur peut être affecté à plusieurs étapes au sein du même workflow d’approbation.

**Puis-je ajouter des étapes pour créer un workflow d’approbation à plusieurs étapes ?**

Oui. Les workflows d’approbation à plusieurs étapes sont pris en charge, ce qui vous permet d’acheminer les ressources au cours d’exercices séquentiels de révision et d’approbation avec différents participants à chaque étape.

<!--
**Can I modify the trigger for a later stage---for example, based on all approved versus the due date ending?**

Stages in a multi-stage approval workflow proceed sequentially based on all required decisions being made in the current stage. When all assigned approvers in a stage have made their decisions, the next stage begins and the previous stage is locked. There is no option to trigger a stage based on the due date ending. If the "One decision required" toggle is enabled on a stage, the first approver decision completes that stage and advances the workflow.

**Can I remove the due date from an approval?**

Yes. Due dates are optional for both single-use approvals and approval templates. When creating a single-use approval, you can leave the deadline field empty. For approval templates, the relative completion timeframe is also optional.

**Can I change the default due date on new approval templates?**

Yes. When creating or editing an approval template, the timeframe (or "Workdays until due date" for multi-stage templates) can be adjusted per stage or left empty. The deadline is calculated automatically from this timeframe when the template is applied to an asset, so updating the template changes the default for all future approvals that use it.

**What happens when the deadline is reached for a review stage?**

For both single-stage and multi-stage reviews, automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. However, reaching the deadline does not automatically reject the asset, lock the stage, or advance the workflow. Approvers and reviewers can still make decisions or complete their review after the deadline has passed. In a multi-stage workflow, each stage has its own independent deadline, and stages still advance based on all required decisions being made---not based on the deadline.
-->

**Les modèles d’approbation peuvent-ils inclure des groupes ou des équipes, ou uniquement des utilisateurs individuels ?**

Actuellement, les modèles d’approbation prennent en charge les utilisateurs individuels et les équipes.

**Les approbateurs sont-ils avertis par e-mail lorsqu’ils ont quelque chose à réviser ?**

Oui. Les approbateurs et les réviseurs reçoivent des notifications par e-mail lorsqu’ils sont affectés à une révision ou une approbation. Les e-mails de rappel automatisés sont également envoyés 72 heures avant l’échéance, 24 heures avant l’échéance et à l’échéance elle-même.

La possibilité de personnaliser les messages de notification par e-mail n’est pas actuellement disponible, mais elle figure sur la feuille de route du produit.

<!--
**Can I change the notification frequency for a unified approver or reviewer (for example, all comments, replies to my comments, or daily summaries)?**

No. Notification frequency settings such as receiving all comments, only replies to your comments, or daily digest summaries are not currently available for unified review and approval. The system sends email notifications automatically when a user is assigned as a reviewer or approver, and automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. The ability to customize notification messages and frequency is on the product roadmap.
-->

**Puis-je garder une étape de révision privée des autres participants ?**

Il n’existe actuellement aucune fonctionnalité d’étape privée. Pour que la révision reste privée pour les autres participants, il est recommandé de créer une copie distincte de la ressource spécifiquement pour ce groupe de révision. Les commentaires ne sont actuellement pas segmentés par groupe de participants dans une seule ressource.

Notez que l’historique des versions, y compris les versions antérieures et actuelles, est toujours visible par toute personne autorisée à afficher cette ressource.

**Les commentaires peuvent-ils être marqués comme résolus ?**

Oui. Les commentaires peuvent être marqués comme résolus dans la visionneuse Frame.io.

**Quels outils de balisage et d’annotation sont disponibles dans la visionneuse Frame.io ?**

La visionneuse Frame.io comprend un ensemble complet d&#39;outils de balisage visuel, notamment le dessin à main levée et les formes standard telles que les cercles, les flèches et les carrés. Dans le cas des ressources vidéo, les commentaires sont horodatés avec une précision d’image exacte. Le retour est donc toujours lié au moment exact dans l’élément et pas seulement à un horodatage général.

**Les commentaires ajoutés dans la visionneuse Frame.io apparaîtront-ils dans le projet Workfront ?**

Les commentaires et les annotations restent dans la visionneuse Frame.io afin de conserver leur contexte complet, y compris les horodatages et les balises visuelles. Cela peut évoluer dans les prochaines versions.

**Est-il possible d’ajouter des commentaires sur une version téléchargée d’une ressource (par exemple, un PDF) ?**

Cette fonctionnalité n’est actuellement pas prise en charge, mais elle est fréquemment demandée et est en cours d’examen pour une version ultérieure.

**Puis-je examiner plusieurs ressources ensemble en tant que groupe ?**

Les options de révision en bloc améliorées seront bientôt disponibles. En attendant, les ressources de différents types de fichiers, tels qu’une vidéo et un document Word, peuvent être incluses ensemble dans une révision de ressources groupée.

**La révision et l’approbation unifiées concernent-elles uniquement les vidéos ou prennent-elles en charge d’autres types de fichiers ?**

La révision et l’approbation unifiées sont conçues pour tous les types de ressources, et pas seulement pour la vidéo. La visionneuse Frame.io a été considérablement mise à jour pour prendre en charge les images, les documents, les fichiers PDF et d’autres formats de fichiers courants en plus de la vidéo.

Pour obtenir la liste complète des types de fichiers pris en charge, consultez la documentation sur les types de fichiers pris en charge par Frame.io sur Experience League.

**Puis-je partager des ressources en externe avec des parties prenantes qui n’ont pas accès à Workfront ?**

Oui. Assets peut être partagé en externe. Les utilisateurs externes sont avertis par e-mail et seront invités à créer une connexion Frame.io pour accéder à la visionneuse et participer à la révision.

<!--
**Before unified review and approval, is a reviewer just directed to a proof?**

Yes. In the legacy proofing workflow (prior to unified review and approval), when a user was assigned as a reviewer they were directed to the Workfront Proof viewer (ProofHQ) to review the proof. With unified review and approval, reviewers are instead directed to the Frame.io viewer, which replaces the Workfront Proof viewer as the primary review surface.

**When I upload a document and not a proof, a proof gets generated. Will a proof always be generated?**

No. With unified review and approval enabled and Adobe enterprise storage active, uploading a document does not automatically generate a proof. Documents are stored in Adobe enterprise storage and are reviewed using the Frame.io viewer. A proof is only generated if you explicitly create one using the legacy proofing workflow. The Frame.io viewer serves as the primary review surface, so a separate proof is not needed for standard review and approval workflows.

**What is the difference between uploading a document and a proof after the 26.2 release?**

With unified review and approval enabled, uploading a document stores it in Adobe enterprise storage and makes it available for review in the Frame.io viewer. A unified approval workflow can be created directly on the document. Uploading a proof, by contrast, uses the legacy Workfront Proof viewer (ProofHQ) and its own proofing workflow. Both options are available for projects created before the integration was enabled, but the Frame.io viewer is the primary review surface going forward. The key difference is that a document uses the unified approval workflow and Frame.io viewer, while a proof uses the legacy proofing workflow and viewer.

**Reviews under My Approvals only show a "Complete my review" button and no link to the proofing viewer or the document. Is this intended?**

For unified review and approval, the My Approvals widget provides an "Open review" button that opens the asset in the Frame.io viewer, as well as action buttons to approve, request changes, or complete a review. Reviewers can complete their review directly from the widget. If you are only seeing a "Complete my review" button without a link to the viewer, this may reflect the reviewer role behavior---reviewers are not required to open the asset to mark their review as complete, though they can choose to open it in the Frame.io viewer to provide feedback before completing.

**Before unified review and approval, if a user is both an approver in a document approval and a reviewer/approver on a proof, both show up in the proof window. How do these work together?**

When using unified approvals alongside legacy proofing on the same document, the two workflows operate independently. Document approval participants are shown in the Document Summary panel, while proof participants are shown in the proofing workflow. The SOCD (Sent, Opened, Comment, Decision) indicators in the document list are proofing-related and do not reflect the unified approval decision status. These two workflows do not automatically sync---a decision made in one does not carry over to the other.

**If you upload a new version, the document approval users do not get repopulated. Is that intended?**

Yes. When a new version is uploaded, previous approval participants are not automatically repopulated. The previous version's approval process is closed and any outstanding approvals are marked as "Withdrawn." The document owner must manually add participants to the new version's approval workflow. An "Add all" button is available to quickly repopulate all participants from the previous version, and you can also selectively add previous participants or add new ones.
-->

+++

### Gestion du stockage et des fichiers

+++ Développez pour afficher les questions fréquentes sur la gestion du stockage et des fichiers.

**Qu’est-ce que le stockage d’entreprise d’Adobe et en quoi est-il lié à cette intégration ?**

Le stockage d’entreprise Adobe est la couche de stockage commune qui connecte Workfront, Frame.io et Adobe Creative Cloud. Assets se trouve au même endroit et est accessible via plusieurs outils sans transfert manuel de fichiers. Les créatifs peuvent travailler sur place et les réviseurs voient toujours la dernière version.

Les principaux avantages du stockage d’entreprise dans Adobe sont les suivants :

* Une couche de stockage unique pour toutes les ressources de travail en cours dans Workfront et Frame.io

* Contrôle d’accès centralisé géré via le système Adobe Identity Management (IMS)

* Visibilité de bout en bout des ressources : aucune dérive de version, aucune perte de métadonnées

* Gestion évolutive du stockage au niveau de l’entreprise

**Existe-t-il des exigences de dénomination ou de structure pour les fichiers et les projets ?**

Oui. Comme l’intégration utilise le stockage d’entreprise d’Adobe, les conventions suivantes s’appliquent :

* Les programmes et les projets ne peuvent pas porter le même nom s&#39;ils appartiennent au même portefeuille.

* Les noms de document doivent être uniques dans le même parent de la hiérarchie des dossiers.

* Les documents d&#39;un même projet ne peuvent pas partager un nom.

* Les noms de programmes, portfolios, projets, modèles, tâches, événements, documents et dossiers de documents ne peuvent pas contenir les caractères spéciaux suivants : `\ / : * ? " | < >` et sont limités à 255 caractères.

Workfront renomme automatiquement les objets ou les documents selon les besoins pour éviter les conflits.

**Quels types de fichiers sont pris en charge dans la visionneuse Frame.io ?**

La visionneuse Frame.io prend en charge plus de 40 formats de fichiers, y compris tous les types courants de fichiers vidéo, image, audio, PDF et Microsoft Office. La prise en charge vidéo inclut la lecture native pour les formats professionnels tels que ProRes, H.265 et DNxHD, avec prise en charge de fichiers allant jusqu’à 500 Go.

Frame.io a été conçu spécifiquement pour la révision créative, ce qui signifie qu’il gère l’ensemble des types de ressources avec lesquels les équipes marketing et créatives travaillent.

+++

### Autorisations et accès

+++ Développez pour afficher les questions fréquentes sur les autorisations et l’accès.

**Comment les autorisations utilisateur sont-elles gérées ?**

Les autorisations utilisateur sont définies et contrôlées dans Workfront et sont automatiquement transmises à Frame.io. Vous ne pouvez pas inviter d’utilisateurs ni modifier les autorisations directement dans Frame.io pour cette intégration. Toute la gestion des accès doit être effectuée à l’aide de la fenêtre modale de partage de projet dans Workfront.

Le tableau ci-dessous montre comment les autorisations Workfront sont mappées aux autorisations Frame.io :

<table>
  <thead>
    <tr>
      <th>Autorisation Workfront</th>
      <th>Autorisation Frame.io</th>
    </tr>
  </thead>
  <tbody>
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
  </tbody>
</table>

+++


### Intégrations et fonctionnalités avancées

+++ Développez pour afficher les questions fréquentes sur les intégrations et les fonctionnalités avancées.

**Quel est l’impact sur les intégrations de plug-ins Creative Cloud existantes avec Adobe Express et GenStudio ?**

Des intégrations prenant en charge l’expérience de visionneuse Frame.io sont actuellement en cours de développement pour Adobe Express et GenStudio Performance Marketing. Les nouvelles intégrations seront créées sur le même système de révision et d’approbation unifié, de sorte qu’elles exploitent la visionneuse Frame.io pour une expérience de révision cohérente sur les trois produits.

**Frame.io est-il intégré à Workfront ou les utilisateurs accèdent-ils à une autre interface ?**

Les utilisateurs peuvent lancer la visionneuse Frame.io directement depuis Workfront. Toutes les activités de révision et d’approbation ont lieu dans la visionneuse Frame.io et sont automatiquement resynchronisées avec Workfront.

**Puis-je envoyer des ressources approuvées à Adobe Experience Manager (AEM) ?**

Oui. Une fois qu’une ressource a terminé le cycle de révision et d’approbation, vous pouvez la transférer vers Adobe Experience Manager Assets pour stockage final et distribution. Cela connecte Workfront pour la gestion du travail, Frame.io pour la révision et AEM pour la gestion des ressources numériques dans un supply chain de contenu unifié.

Pour plus d’informations, voir [Utilisation de Adobe Experience Manager avec l’intégration Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

**Comment la révision et l’approbation unifiées s’intègrent-elles à Adobe GenStudio ?**

La révision et l’approbation unifiées sont un composant fondamental d’Adobe GenStudio : Adobe offre une vision plus large d’un supply chain de contenu connecté. GenStudio connecte Workfront, Frame.io, Creative Cloud, Adobe Express, Adobe Experience Manager Assets et GenStudio for Performance Marketing en un workflow unifié, du brief de campaign à la diffusion de contenu.

Au sein de cet écosystème, la révision et l’approbation servent de point de transfert critique entre la création et la diffusion. C’est là que le travail créatif rencontre les commentaires des parties prenantes, que la qualité est validée et que le contenu est autorisé à être publié. Lorsque cette remise est rapide, visible et fiable, elle libère de la vitesse dans l’ensemble de la supply chain de contenu. L’IA peut accélérer la création, l’automatisation peut gérer la distribution, mais un goulot d’étranglement en révision limite les gains des deux côtés. La connexion de Workfront et Frame.io supprime ce goulot d’étranglement.

**Qu’est-ce que la fonctionnalité IA Reviewer ?**

La révision et l’approbation unifiées comprennent une fonctionnalité d’IA Reviewer qui automatise les contrôles de conformité de la marque dans le cadre du processus de révision. Le réviseur AI peut évaluer les ressources par rapport aux directives de la marque et signaler les problèmes potentiels avant que les réviseurs humains ne soient engagés, ce qui permet aux équipes de détecter les problèmes plus tôt et d’avancer plus rapidement.

Pour plus d’informations sur la configuration et l’utilisation d’AI Reviewer, consultez la documentation de Workfront sur Experience League.

+++

### Contrats, SKU et stockage

+++ Développez pour afficher les questions fréquentes sur les contrats, les SKU et le stockage.

**Quand la révision et l’approbation unifiées seront-elles disponibles pour moi ?**

La révision et l’approbation unifiées sont maintenant disponibles. Access nécessite une mise à niveau vers un SKU Workfront V2. Si votre contrat a été signé avant la disponibilité des SKU V2, vous pouvez y accéder de deux façons :

* Lors du renouvellement : l’accès sera activé à la prochaine date de renouvellement de votre contrat.

* Réengagement anticipé : votre équipe de compte Adobe peut vous réengager plus tôt pour ajouter les nouveaux droits de SKU tout en conservant la date de fin de votre contrat existant. Il n&#39;y a pas d&#39;augmentation de prix lorsque vous passez à un forfait équivalent.

Contactez votre représentant de compte Adobe pour déterminer le meilleur chemin d’accès pour votre organisation.

<!--
**Before we sign the contract, what changes will we see in Workfront?**

Before signing the V2 SKU contract, your Workfront instance will continue to operate using the existing document and proofing experience. No unified review and approval features---such as the Frame.io viewer, Adobe enterprise storage, or multi-stage approval templates---will be available until the V2 SKU is contracted and Adobe Professional Services configures the integration for your organization.
-->

**La mise à niveau vers le SKU V2 m’offre-t-elle plus de stockage ?**

Oui. Avec le SKU V2, chaque utilisateur sous licence reçoit 60 Go de stockage, contre 30 Go dans la version précédente.

**Comment choisir entre le stockage d’entreprise Adobe et le stockage Workfront hérité ?**

Le stockage d’entreprise active l’expérience de la visionneuse Frame.io et est requis pour une révision et une approbation unifiées. Le stockage hérité continue d’utiliser la visionneuse Workfront Proof (ProofHQ) par défaut.

Si votre entreprise propose une combinaison de workflows simples et de workflows de relecture plus complexes, vous pouvez donner la priorité aux workflows à migrer en premier.

Le stockage d’entreprise vous offre la possibilité de déployer la nouvelle expérience de manière incrémentielle, en commençant par les workflows qui en bénéficieront le plus.

**Comment les licences Frame.io sont-elles gérées ?**

Après avoir signé le SKU V2, tous les utilisateurs de Workfront auront accès à la visionneuse Frame.io pour les workflows de révision et d’approbation. Aucune licence Entreprise Frame.io distincte n’est requise pour cela.

Si votre entreprise a besoin de fonctionnalités supplémentaires de Frame.io Enterprise telles que

* Filigranage avancé (dynamique et criminalistique)
* Gestion des droits numériques avec suppression automatique des ressources
* Informations d’identification de contenu pour le contenu généré par l’IA
* Métadonnées de création personnalisées
* Intégrations de la caméra au cloud
* Votre propre espace de travail pour le travail créatif en cours

vous pouvez travailler avec l’équipe de votre compte Adobe pour déterminer le nombre approprié de licences Frame.io Enterprise. Toutes les licences sont gérées via Adobe Admin Console.

+++

### Sandbox et déploiement

+++ Développez pour afficher les questions fréquentes sur le sandbox et le déploiement.

**Puis-je tester la révision et l’approbation unifiées dans un environnement sandbox ?**

Partiellement. Les workflows d’approbation peuvent être testés dans un environnement sandbox Workfront. Toutefois, l’expérience de la visionneuse Frame.io n’est pas disponible dans le sandbox. Le test de la surface de révision elle-même nécessite un environnement de production.

Pour limiter l’exposition lors du déploiement, vous pouvez activer la révision et l’approbation unifiées pour un groupe spécifique dans votre environnement de production Workfront. Vous pouvez ainsi exécuter un pilote ciblé avec un plus petit ensemble d’utilisateurs avant d’effectuer un déploiement plus large.

<!--
**How should we test future quarterly releases involving unified review and approval if the Frame.io viewer is not available in sandbox?**

Because the Frame.io viewer experience is not available in the Workfront sandbox environment, testing future quarterly releases should be done using a controlled pilot group in your production environment. You can enable unified review and approval for a specific group within your Workfront production instance, allowing a smaller set of users to validate new features as they release. Approval workflow configuration and template setup can still be tested in sandbox, but the full review experience---including the Frame.io viewer---must be validated in production.
-->

+++

### Épreuves interactives et HTML

+++ Développez pour afficher les questions fréquentes sur les épreuves interactives et HTML.

**La révision et l’approbation unifiées prennent-elles en charge les épreuves interactives ou les URL HTML ?**

Les fichiers Zip HTML sont actuellement pris en charge pour la révision interactive. La prise en charge des URL HTML (révision des URL web en direct) est prévue pour le 3e trimestre.

Consultez les notes de mise à jour de Workfront sur Experience League pour connaître les mises à jour.

+++

### Fusion et automatisation

+++ Développez pour afficher les questions fréquentes sur Fusion et l’automatisation.

**Ai-je besoin de Workfront Fusion pour utiliser la révision et l’approbation unifiées ?**

Non. La révision et l’approbation unifiées sont une intégration de produit native qui ne nécessite pas Fusion. Le workflow est directement intégré à Workfront.

**Les connecteurs Fusion seront-ils disponibles pour une révision et une approbation unifiées ?**

Oui. Les actions de fusion pour l’examen et l’approbation unifiés sont actuellement en cours d’élaboration et devraient être disponibles au 3e trimestre. Consultez les notes de mise à jour de Workfront sur Experience League pour connaître les mises à jour dès qu’elles sont disponibles.

**Fusion peut-il être utilisé pour déclencher automatiquement une révision lorsqu’un document est chargé ?**

Oui. Ce type d’automatisation est possible à l’aide des Webhooks Workfront en combinaison avec Fusion.

**Comment les workflows Fusion existants créés sur Workfront Proof seront-ils affectés ?**

L’impact varie en fonction de la conception de chaque workflow. En général :

* **Modifier ou mettre à jour** : les workflows pour lesquels l’action liée à l’épreuve existante a un équivalent direct dans les approbations unifiées peuvent être mis à jour pour utiliser la nouvelle action.

* **Reconstruire** : les workflows pour lesquels les étapes sous-jacentes ont considérablement changé ou pour lesquels de nouvelles fonctionnalités sont disponibles peuvent être reconstruits à partir de zéro.

Une image plus claire apparaîtra une fois que les API Fusion pour les approbations unifiées seront disponibles. Il est recommandé d’auditer vos workflows Fusion existants et de les évaluer par rapport aux nouvelles fonctionnalités d’approbations unifiées à ce moment-là.

+++






