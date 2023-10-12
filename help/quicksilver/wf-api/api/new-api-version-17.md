---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 17
description: Adobe Workfront a publié l’API version 17 le 6 avril 2022. L’API version 17 comprend les modifications suivantes à partir de la version 15.
author: Becky
feature: Workfront API
source-git-commit: e0b040b062796a1d1b1e0c029ca0ef71b77ed54a
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 3%

---

# Nouveautés de l’API version 17

Adobe Workfront a publié l’API version 17 le 12 octobre 2023. L’API version 17 comprend les modifications suivantes à partir de la version 16.

## Ressources ajoutées

<!--

### Booking (BOOKNG)

-->

### ExternalDocument (EXTDOC)

Un objet ExternalDocument est un document ou une autre ressource numérique qui se trouve dans un fournisseur de stockage de documents externe à Workfront. Ces ressources peuvent être liées à et depuis Workfront.

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
          <li><p><b>client</b></p></li>
          <li><p><b>user</b></p></li>
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

Aucune ressource n’a été supprimée pour l’API version 17.

## Ressources modifiées

Les ressources suivantes ont été modifiées pour l’API version 17.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Ligne de base (BLIN)

Les lignes de base sont des instantanés de ce à quoi ressemblaient les performances d’un projet à un moment donné dans le temps. Ils stockent des informations clés sur le projet, telles que les dates clés, l’avancement, les coûts et les valeurs de recettes.

L’objet Baseline a supprimé l’indicateur **INLINE_EDITABLE**.

### BillingRecord (BILL)

Un objet BillingRecord enregistre les recettes, les heures ou les dépenses qui peuvent être facturées. Ces informations peuvent être utilisées pour créer des factures dans un système comptable externe.

L’objet BillingRecord a supprimé l’indicateur **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Société (CMPY)

Un objet Société représente une organisation composée d’un ensemble de personnes.

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
            <p>Supprimé</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### CustomerPreferences (CUSTPR)

Un objet CustomerPreferences représente l’ensemble des préférences définies par un client pour son instance de Workfront.

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
            <p>Ajout de la valeur possible "config.defaultToNewHomeDescription" (customer:config.defaultToNewHome)&gt;/p?<p>Cela permet à une entreprise de faire de la nouvelle expérience d’accueil la nouvelle expérience par défaut pour ses utilisateurs.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

Un objet DocumentVersion représente une version spécifique d’un fichier (comme du matériel écrit, des images ou d’autres formes d’informations).

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
            <p>Ajout de la valeur possible "Frame.io" (FRAMEIO)</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>Ajout de la valeur possible "enum.filetype.site" (site)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate (EXRATE)

Un objet ExchangeRate représente un taux de change de devise configuré dans Workfront. Les objets ExchangeRate ne sont pas dynamiques.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés :
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
          <p>Ajout de .</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Dépenses (EXPNS)

Les dépenses représentent les frais non liés au travail qui pourraient être engagés pendant la durée de vie d&#39;un projet.

L’objet Frais a supprimé l’indicateur **INLINE_EDITABLE**.

### Groupe (GROUP)

Un objet Group représente un ensemble d’utilisateurs et d’équipes. Les groupes représentent souvent la structure du Ministère.

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
            <p>Supprimé</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Heure (HEURE)

Un objet Hour représente une heure consignée par un utilisateur sur une feuille de temps.

L’objet Heure a supprimé l’indicateur **INLINE_EDITABLE**.

### Itération (ITRN)

Un objet Itération représente une seule itération Agile. Les itérations sont des périodes discrètes utilisées pour planifier et compléter des histoires Agile.

L’objet Itération a supprimé l’indicateur **INLINE_EDITABLE**.


### JournalEntry (JRNLE)

L’objet JournalEntry peut être configuré pour consigner des informations sur des champs d’objet spécifiques chaque fois que ces champs sont modifiés. Lorsqu’un champ est configuré pour être consigné dans le cadre de l’objet d’entrée de journal, une entrée de journal correspondante est créée chaque fois que ce champ est modifié.

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
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>Ajout de l’approbateur (AAA)</li>
              <li>Ajout d’un réviseur (AAR)</li>
              <li>Suppression du réviseur (ARR)</li>
              <li>Approbateur supprimé (ARA)</li>
              <li>Décision approuvée (ADA)</li>
              <li>Décision approuvée avec modifications (ADC)</li>
              <li>Les besoins de décision fonctionnent (ADN)</li>
              <li>Décision révoquée (MARC)</li>
              <li>Approbateur modifié (AAC)</li>
              <li>Réviseur modifié (ARC)</li>
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

Un panorama Kanban est utilisé pour effectuer le suivi des tâches dans un environnement agile.

L’objet Kanban Board a supprimé l’indicateur **INLINE_EDITABLE**.


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
            <p>Ajout de la valeur possible "Frame.io (FRAMEIO)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / Problème (OPTASK)

Un objet OpTask est généralement appelé Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de service d’assistance. Modifier les commandes, les requêtes et les bogues sont également des problèmes.

L’objet Problème a supprimé l’indicateur **INLINE_EDITABLE**.

### Projet (PROJ)

Les projets sont des éléments de travail dans Workfront et sont une composante essentielle de la façon dont Workfront aide les personnes à travailler. Un objet Projet représente un groupe de tâches avec un objectif commun et spécifique.

L’objet Projet a supprimé l’indicateur **INLINE_EDITABLE**.

### ProjectUser (PRTU)

Un objet ProjectUser représente un utilisateur associé à un projet spécifique.

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
            <p>Ajout de .</p>
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
            <p>Ajout de .</p>
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

### Rate (RATE)

Un objet Rate représente un taux de facturation dans Workfront.

L’objet Rate a supprimé l’indicateur. **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>Les actions suivantes ont été ajoutées pour prendre en charge la fonctionnalité Carte de taux :
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>La variable <b>setRatesForRole</b> L’action a été modifiée pour ajouter les champs suivants :
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risque (RISQUE)

Un objet Risk représente un événement possible qui peut empêcher la fin d’un projet à temps ou dans les limites du budget. Lors de la phase de planification, des risques sont ajoutés aux projets pour identifier les obstacles potentiels avant l’approbation des travaux.

L&#39;objet Risk a retiré l&#39;indicateur **INLINE_EDITABLE**.

### Rôle/Rôle de tâche (RÔLE)

Un objet Rôle (rôle de tâche) représente une capacité fonctionnelle ou un ensemble de compétences qu’un utilisateur peut remplir, tel que Designer ou Gestionnaire de produits.

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
            <p>Supprimé</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tâche (TÂCHE)

Un objet Task représente un élément de travail qui doit être exécuté comme une étape vers l’atteinte d’un objectif final (achèvement d’un projet).

L’objet Task a supprimé l’indicateur **INLINE_EDITABLE**.

### Équipe (TEAMOB)

Un objet Équipe est un ensemble d’utilisateurs pouvant être affectés à un élément de travail.

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
            <p>Supprimé</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TeamMember (TEAMMB)

Un objet TeamMember est un utilisateur associé à une équipe spécifique.

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
            <p>Ajout de .</p>
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
            <p>Ajout de .</p>
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
            <p>Ajout de .</p>
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
            <p>Ajout de .</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Feuille de calcul (TSHET)

Un objet de feuille de temps représente une feuille de temps virtuelle qui permet aux utilisateurs de saisir les heures réelles travaillées pour les tâches, les projets et les types d’heures de surcharge.

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
            <p>Supprimé</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Mise à jour (MISE À JOUR)

Les éléments de travail dans Workfront peuvent être mis à jour afin de tenir les utilisateurs informés de l’état actuel. Un objet Update représente l’une de ces mises à jour. Les mises à jour peuvent être saisies par les utilisateurs ou créées par le système Workfront.

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
            <p>Ajout des valeurs suivantes :</p>
            <ul>
              <li>Ajout de l’approbateur (assetapprovalAddApprover)</li>
              <li>Ajout d’un réviseur (assetapprovalAddReviewer)</li>
              <li>Approbateur supprimé (assetapprovalRemoveApprover)</li>
              <li>Suppression du réviseur (assetapprovalRemoveReviewer)</li>
              <li>Décision approuvée (assetapprovalDecisionApproval)</li>
              <li>La décision doit fonctionner (assetapprovalDecisionNeedsWork)</li>
              <li>Décision approuvée avec modifications (assetapprovalDecisionApprovalChanges)</li>
              <li>Décision révoquée (assetapprovalDecisionRevoked)</li>
              <li>Approbateur modifié (assetapprovalApproverChanged)</li>
              <li>Réviseur modifié (assetapprovalReviewerChanged)</li>
              <li>Révision terminée (assetapprovalReviewerDecisionComplete)</li>
              <li>Révision révoquée (assetapprovalReviewerDecisionRevoked)</li>
              <li>Erreur d'envoi de document externe (externalDocumentSendError)</li>
              <li>Version du document publiée (documentVersionPublish)</li>
              <li>Workflow du dossier lié (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Utilisateur (USER)

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
            <p>Ce champ a été ajouté. Il s’agit d’un nombre compris entre 0 et 1 qui représente le pourcentage de temps qu’un utilisateur peut consacrer chaque jour à des tâches de projet (sans frais généraux). Une valeur de 1 signifie que l’utilisateur peut passer 100 % de son temps à travailler sur un projet.</p>
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
            <p>Ajout de .</p>
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
            <p>Ajout de .</p>
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
            <p>Ajout des valeurs suivantes :</p>
            <ul>
              <li>Le document nécessite votre approbation (AAA)</li>
              <li>Le document nécessite votre révision (AAR).</li>
              <li>Document n’a plus besoin de votre approbation (ARA)</li>
              <li>Document n’a plus besoin de votre révision (ARR)</li>
              <li>Approbation requise du document (ATA) par l’utilisateur</li>
              <li>Examen des besoins du document (utilisateur) (ATR)</li>
              <li>Document n’a plus besoin de la validation (RTA) de l’utilisateur</li>
              <li>Le document n’a plus besoin de révision (RTR) (utilisateur).</li>
              <li>Document approuvé (ADA)</li>
              <li>Document approuvé avec modifications (ADC)</li>
              <li>Travail sur les documents nécessaires (ADN)</li>
              <li>(Utilisateur) a marqué (document) comme approuvé. Votre approbation n’est plus nécessaire. (AAN)</li>
              <li>(Utilisateur) a marqué (document) comme approuvé avec les modifications. Votre approbation n’est plus nécessaire. (ACN)</li>
              <li>(Utilisateur) a marqué (document) comme le travail nécessaire. Votre approbation n’est plus nécessaire. (AWN)</li>
              <li>Le document a besoin de votre révision maintenant plutôt que de votre approbation (AAC).</li>
              <li>Le document a besoin de votre approbation maintenant plutôt que d'une révision (ADN).</li>
              <li>Document révisé (RDC)</li>
              <li>Document révisé (TRC)</li>
              <li>(Utilisateur) a examiné (document) comme terminé. Votre examen n’est plus nécessaire. (TRN)</li>
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
            <p>Ajout de .</p>
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
            <p>Ajout de .</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
