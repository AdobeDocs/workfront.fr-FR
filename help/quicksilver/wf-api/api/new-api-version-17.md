---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 17 de l’API
description: Adobe Workfront a publié la version 17 de l’API le 6 avril 2022. La versions 17 de l’API comprend les modifications suivantes par rapport à la version 16.
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 99%

---

# Nouveautés de la version 17 de l’API

Adobe Workfront a publié la verison 17 de l’API le 12 octobre 2023. La versions 17 de l’API comprend les modifications suivantes par rapport à la version 16.

## Ressources ajoutées

<!--

### Booking (BOOKNG)

-->

### ExternalDocument (EXTDOC)

Un objet ExternalDocument est un document ou une autre ressource numérique qui se trouve chez un fournisseur de stockage de documents externe à Workfront. Ces ressources peuvent être liées à Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>poste</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>path</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>poste</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>path</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>value</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs par défaut</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Requêtes</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Opérations</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>
        <ul>
          <li><p><b>customer</b></p></li>
          <li><p><b>utilisateur</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## Ressources supprimées

Aucune ressource n’a été supprimée pour l’API version 17.

## Ressources modifiées

Les ressources suivantes ont été modifiées pour l’API version 17.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Baseline (BLIN)

Les niveaux de référence sont des instantanés de ce à quoi ressemblaient les performances d’un projet à un moment donné dans le temps. Elles stockent des informations clés sur le projet, telles que les dates clés et la progression, ainsi que les valeurs des coûts et des revenus.

L’objet Baseline a supprimé l’indicateur **INLINE_EDITABLE**.

### BillingRecord (BILL)

Un objet BillingRecord enregistre les revenus, les heures ou les dépenses qui peuvent être facturées. Ces informations peuvent être utilisées pour créer des factures dans un système comptable externe.

L’objet BillingRecord a supprimé l’indicateur **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Entreprise (CMPY)

Un objet Company représente une organisation composée d’un ensemble de personnes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Supprimés</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### CustomerPreferences (CUSTPR)

Un objet CustomerPreferences représente l’ensemble des préférences définies par un client ou une cliente pour son instance de Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
            <p>Ajout de la valeur possible « config.defaultToNewHomeDescription » (customer:config.defaultToNewHome)&gt;/p?<p>Cela permet à une organisation de faire de la nouvelle expérience d’accueil la nouvelle expérience par défaut de ses utilisateurs et utilisatrices.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

Un objet DocumentVersion représente une version spécifique d’un fichier (comme du contenu écrit, des images ou d’autres formes d’informations).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Ajout de la valeur possible « Frame.io »" (FRAMEIO)</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>Ajout de la valeur possible « enum.filetype.site » (site)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate (EXRATE)

Un objet ExchangeRate représente un taux d’exchange de devise configuré dans Workfront. Les objets ExchangeRate ne sont pas dynamiques.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés :
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>Ajout.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Expense (EXPNS)

Les dépenses représentent les coûts non liés à la main-d’œuvre qui peuvent être engagés pendant la durée de vie d’un projet.

L’objet Expense a supprimé l’indicateur **INLINE_EDITABLE**.

### Groupe (GROUP)

Un objet Group représente un ensemble d’utilisateurs et utilisatrices et d’équipes. Les groupes représentent souvent la structure des services.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Supprimés</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Hour (HOUR)

Un objet Hour représente une heure enregistrée par un utilisateur ou une utilisatrice sur une feuille de temps.

L’objet Hour a supprimé l’indicateur **INLINE_EDITABLE**.

### Iteration (ITRN)

Un objet Iteration représente une seule itération Agile. Les itérations sont des périodes discrètes utilisées pour planifier et compléter des histoires Agile.

L’objet Iteration a supprimé l’indicateur **INLINE_EDITABLE**.


### JournalEntry (JRNLE)

L’objet JournalEntry peut être configuré pour enregistrer des informations sur des champs d’objet spécifiques chaque fois que ces champs sont modifiés. Lorsqu’un champ est configuré pour être enregistré dans le cadre de l’objet JournalEntry, une entrée de journal correspondante est créée chaque fois que ce champ est modifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>Ajout d’un approbateur ou d’une approbatrice (AAA)</li>
              <li>Ajout d’un réviseur ou d’une réviseuse (AAR)</li>
              <li>Suppression du réviseur ou de la réviseuse (ARR)</li>
              <li>Suppression de l’approbateur ou de l’approbatrice (ARA)</li>
              <li>Décision approuvée (ADA)</li>
              <li>Décision approuvée avec des modifications (ADC)</li>
              <li>La décision doit être retravaillée (ADN)</li>
              <li>Décision révoquée (MARC)</li>
              <li>Modification de l’approbateur ou de l’approbatrice (AAC)</li>
              <li>Modification du réviseur ou de la réviseuse (ARC)</li>
              <li>Révision terminée (RDC)</li>
              <li>Révision révoquée (RDR)</li>
              <li>Publier (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban Board (KNBNBD)

Un panorama Kanban est utilisé pour suivre les tâches dans un environnement agile.

L’objet Panorama Kanban a supprimé l’indicateur **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

Un objet LinkedFolder représente un dossier lié à un fournisseur de documents externe, tel que Google Drive ou Dropbox.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Ajout de la valeur possible Frame.io (FRAMEIO)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / Problème (OPTASK)

Un objet OpTask est généralement appelé Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de centre d’assistance. Les ordres de modification, les requêtes et les bugs sont également des problèmes.

L’objet Problème a supprimé l’indicateur **INLINE_EDITABLE**.

### Projet (PROJ)

Les projets sont des éléments de travail dans Workfront et sont un bloc de création essentiel de la façon dont Workfront aide les personnes à travailler. Un objet Projet représente un groupe de tâches avec un objectif commun et spécifique.

L’objet Projet a supprimé l’indicateur **INLINE_EDITABLE**.

### ProjectUser (PRTU)

Un objet ProjectUser représente une personne associée à un projet spécifique.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Taux (RATE)

Un objet Rate représente un taux de facturation dans Workfront.

L’objet Rate a supprimé l’indicateur **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>Les actions suivantes ont été ajoutées pour prendre en charge la fonctionnalité Carte tarifaire :
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>L’action <b>setRatesForRole</b> a été modifiée pour ajouter les champs suivants :
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risque (RISK)

Un objet Risk représente un événement possible qui peut empêcher un projet de se terminer dans les délais ou dans le respect un budget. Lors de la phase de planification, des risques sont ajoutés aux projets pour identifier les obstacles potentiels avant l’approbation d’un travail.

L&#39;objet Risk a retiré l’indicateur **INLINE_EDITABLE**.

### Rôle/Fonction (ROLE)

Un objet Rôle (fonction) représente une capacité fonctionnelle ou un ensemble de compétences qu’un utilisateur ou une utilisateur peut remplir, tel que Designer ou Chef ou Cheffe de produits.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Supprimés</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tâche (TASK)

Un objet Task représente un élément de travail qui doit être exécuté comme une étape vers la réalisation d’un objectif final (achèvement d’un projet).

L’objet Task a supprimé l’indicateur **INLINE_EDITABLE**.

### Team (TEAMOB)

Un objet Team est un ensemble d’utilisateurs et d’utilisatrices pouvant être affectés à un élément de travail.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Supprimés</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TeamMember (TEAMMB)

Un objet TeamMember est une personne associée à une équipe spécifique.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser (TMTU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Timesheet (TSHET)

Un objet Timesheet représente une feuille de temps virtuelle qui permet aux utilisateurs et utilisatrices de saisir les heures effectives travaillées pour les tâches, les projets et les types d’heures supplémentaires.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>Supprimés</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Update (UPDATE)

Les éléments de travail dans Workfront peuvent être mis à jour afin de tenir les utilisateurs et utilisatrices informés du statut actuel. Un objet Update représente l’une de ces mises à jour. Les mises à jour peuvent être saisies par les utilisateurs et utilisatrices ou créées par le système Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Ajout des valeurs suivantes :</p>
            <ul>
              <li>Ajout d’un approbateur ou d’une approbatrice (assetapprovalAddApprover)</li>
              <li>Ajout d’un réviseur ou d’une réviseuse (assetapprovalAddReviewer)</li>
              <li>Suppression de l’approbateur ou de l’approbatrice (assetapprovalRemoveApprover)</li>
              <li>Suppression du réviseur ou de la réviseuse (assetapprovalRemoveReviewer)</li>
              <li>Décision approuvée (assetapprovalDecisionApproval)</li>
              <li>La décision doit être retravaillée (assetapprovalDecisionNeedsWork)</li>
              <li>Décision approuvée avec des modifications (assetapprovalDecisionApprovalChanges)</li>
              <li>Décision révoquée (assetapprovalDecisionRevoked)</li>
              <li>Modification de l’approbateur ou de l’approbatrice (assetapprovalApproverChanged)</li>
              <li>Modification du réviseur ou de la réviseuse (assetapprovalReviewerChanged)</li>
              <li>Révision terminée (assetapprovalReviewerDecisionComplete)</li>
              <li>Révision révoquée (assetapprovalReviewerDecisionRevoked)</li>
              <li>Erreur d’envoi de document externe (externalDocumentSendError)</li>
              <li>Version du document publiée (documentVersionPublish)</li>
              <li>Workflow du dossier lié (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Utilisateur ou utilisatrice (USER)

Un objet User représente une personne disposant d’un compte dans Workfront qui peut se connecter et interagir avec le système.

L’objet User a supprimé l’indicateur **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>Ce champ a été ajouté. Il s’agit d’un nombre compris entre 0 et 1 qui représente le pourcentage de temps qu’un utilisateur ou une utilisatrice peut consacrer chaque jour à travailler sur le projet (hors heures supplémentaires). Une valeur de 1 signifie que l’utilisateur ou l’utilisatrice peut passer 100 % de son temps à travailler sur un projet.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserGroups (USRGPS)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserNote (USRNOT)

Un objet UserNote est une notification.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Ajout des valeurs suivantes :</p>
            <ul>
              <li>Le document a besoin de votre approbation (AAA).</li>
              <li>Le document a besoin d’être examiné (AAR).</li>
              <li>Le document n’a plus besoin de votre approbation (ARA).</li>
              <li>Le document n’a plus besoin d’être examiné (ARR).</li>
              <li>Le document a besoin de l’approbation de (utilisateur ou utilisatrice) (ATA).</li>
              <li>Le document a besoin d’être examiné par (utilisateur ou utilisatrice) (ATR).</li>
              <li>Le document n’a plus besoin de l’approbation de (utilisateur ou utilisatrice) (RTA).</li>
              <li>Le document n’a plus besoin d’être examiné par (utilisateur ou utilisatrice) (RTR).</li>
              <li>Document approuvé (ADA)</li>
              <li>Document approuvé avec des modifications (ADC)</li>
              <li>Le document a besoin d’être retravaillé (ADN).</li>
              <li>(Utilisateur ou utilisatrice) a marqué (document) comme approuvé. Votre approbation n’est plus nécessaire. (AAN)</li>
              <li>(Utilisateur ou utilisatrice) a marqué (document) comme approuvé avec des modifications. Votre approbation n’est plus nécessaire. (ACN)</li>
              <li>(Utilisateur ou utilisatrice) a marqué (document) comme devant être retravaillé. Votre approbation n’est plus nécessaire. (AWN)</li>
              <li>Le document a besoin d’être examiné maintenant plutôt que d’être approuvé (AAC).</li>
              <li>Le document a besoin d’être approuvé maintenant plutôt que d’être examiné (ADN).</li>
              <li>Document examiné (RDC)</li>
              <li>Document examiné (TRC)</li>
              <li>(Utilisateur ou utilisatrice) a examiné (document) et l’a signalé comme terminé. Votre examen n’est plus nécessaire. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole (USRROL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
