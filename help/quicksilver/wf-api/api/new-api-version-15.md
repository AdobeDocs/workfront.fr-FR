---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 15
description: Adobe Workfront a publié l’API version 14 le 14 juin 2022. L’API version 15 comprend les modifications suivantes à partir de la version 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 2%

---

# Nouveautés de l’API version 15

Adobe Workfront a publié l’API version 15 le 14 juin 2022. L’API version 15 comprend les modifications suivantes à partir de la version 14.

## Ressources ajoutées

* [Initiative (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [UserApproval (USRAPV)](#UserAppr)

### Initiative (INITIV)

L’objet Initiative crée des estimations dans le planificateur de scénarios de Workfront pour le type et le nombre de rôles de tâche, les coûts fixes et l’avantage planifié.

Pour plus d’informations sur les initiatives, voir [Présentation des initiatives dans le planificateur de scénarios](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>C'est un objet interne.</p>
          </li>
          <li>
            <p><b>durée</b>
            </p>
            <p>Durée entre endDate et startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>Date d’achèvement prévue de l’initiative.</p>
          </li>
          <li>
            <p><b>entryByID</b>
            </p>
            <p>Identifiant associé à l’utilisateur qui a envoyé la demande.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>ID associé à l’action.</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>ID associé à l’initiative.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>Date de la dernière publication de l’initiative dans le planificateur de scénario Workfront.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>Nom de l’initiative</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>ID du plan associé à l’initiative.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>Nom du plan associé à l’initiative.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>Identifiant du projet associé à l’initiative.</p>
          </li>
          <li>
            <p><b>scénarioID</b>
            </p>
            <p>Identifiant du scénario dans le planificateur de scénario Workfront associé à l’initiative.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>Date de début prévue de l’initiative.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td >
        <ul>
          <li>
            <p><b>client</b>
            </p>
          </li>
          <li>
            <p><b>entryBy</b>
            </p>
          </li>
          <li>
            <p><b>projet</b>
            </p>
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
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Opérations</td>
      <td>
        <ul>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>RAPPORT </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

L’objet IssueDef représente un ensemble de données concernant le format des problèmes. Cet objet peut être associé à des projets ou des modèles et affecte les problèmes ajoutés à ce projet ou modèle.

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
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

Dans certains cas, il est possible de lier des tâches Workfront directement à des objets d’un produit logiciel externe. L’objet ObjectIntegration représente ce lien.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>C'est un objet interne.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>Date et heure auxquelles l’intégration ObjectIntegration a été saisie dans le système Workfront.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>Identifiant Workfront unique de l’objet ObjectIntegration spécifique.</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>Le logiciel externe avec lequel l’objet ObjectIntegration crée un lien. Les valeurs possibles sont les suivantes :</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>Objet dans Workfront auquel ObjectIntegration est associé.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>Code d’objet de l’objet dans Workfront auquel ObjectIntegration est associé.</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td >
        <ul>
          <li>
            <p><b>client</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

L’objet TaskDef représente un ensemble de données concernant le format des tâches. Cet objet peut être associé à des projets ou des modèles et affecte les tâches ajoutées à ce projet ou modèle.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcScheduleHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories
</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserApproval (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestsDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td >
        <ul>
          <li>
            <p><b>approbateur</b>
            </p>
          </li>
          <li>
            <p><b>client</b>
            </p>
          </li>
          <li>
            <p><b>demandeur</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs par défaut</td>
      <td >
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>valider</b>
            </p>
          </li>
          <li>
            <p><b>rejeter</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Opérations</td>
      <td>
        <ul>
          <li>
            <p><b>AJOUTER</b>
            </p>
          </li>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>RAPPORT</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Ressources supprimées

Aucune ressource n’a été supprimée pour l’API version 15.

## Ressources modifiées

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSRUL)](#AccessRu)

* [Validation (APPROBATION)](#Approval)

* [Catégorie (CTGY)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [CustomerPreferences (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Groupe (GROUP)](#Group)

* [JournalEntry (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [OpTask / Problème (OPTASK)](#OpTask)

* [Paramètre (PARAM)](#Paramete)

* [Portfolio (PORT)](#Portfoli)

* [Programme (PRGM)](#Program)

* [Projet (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Tâche (TÂCHE)](#Task)

* [Modèle (TMPL)](#Template)

* [Feuille de calcul (TSHET)](#Timeshee)

* [Vue (UIVIEW)](#View)

* [Mise à jour (MISE À JOUR)](#Update)

* [Utilisateur (USER)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Travail (WORK)](#Work)

### AccessLevel (ACSLVL)

Un objet AccessLevel est associé à des utilisateurs et décrit le jeu d’autorisations AccessLevel qui déterminent ce à quoi l’utilisateur peut accéder.

Pour plus d’informations sur les niveaux d’accès, voir [Niveaux d’accès](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>VTMAWMG (Afficher les équipes associées à mes groupes)</p>
              </li>
              <li>
                <p>VALLTM (Afficher toutes les équipes)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions (ALVPER)

Un objet AccessLevelPermissions représente une autorisation spécifique d’accès, de création ou de modification d’un objet Workfront. Ces autorisations peuvent ensuite être associées à un niveau d’accès.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Si un utilisateur n’a pas accès à un objet Workfront dont il a besoin, il peut demander l’accès à cet objet. L’objet AccessRequest représente cette requête.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>action</b> (string)</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (string)</p>
            <p>Ajout de la valeur possible suivante :</p>
            <ul>
              <li>
                <p>WDL</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Un objet AccessRule représente un jeu de règles dans les niveaux d’accès personnalisés qui détermine comment les utilisateurs peuvent partager les projets qu’ils créent.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Validation (APPROBATION)

Un élément de travail donné, tel qu’une tâche, un document ou une feuille de temps, peut exiger qu’un superviseur ou un autre utilisateur signe l’élément de travail. Un objet Approval représente l’action de déconnexion d’un élément de travail.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td >
        <ul>
          <li>
            <p><b>initiative</b>
            </p>
            <p>Ajout de .</p>
            <p>L’objet Initiative crée des estimations dans le planificateur de scénarios de Workfront pour le type et le nombre de rôles de tâche, les coûts fixes et l’avantage planifié. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Ajout de .</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Ajout de .</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">Ajout de .</p>
            <p>Dans certains cas, il est possible de lier des tâches Workfront directement à des objets d’un produit logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Catégorie (CTGY)

Un objet Category est un formulaire personnalisé.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b> (string)</p>
            <p>Ajout de la valeur possible suivante :</p>
            <ul>
              <li>
                <p>GROUP (Groupe)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Ajout de .</p>
            <p style="font-weight: normal;">Ce paramètre est un tableau d’objets possibles auxquels le formulaire personnalisé peut être joint. Il a été ajouté pour prendre en charge la possibilité de joindre un formulaire personnalisé à plusieurs types d’objets.</p>
            <p>Valeurs possibles : </p>
            <p>CMPY, PORT, PRGM, PROJ, TÂCHE, OPTASK, UTILISATEUR, DOCU, EXPNS, ITRN, BILL, GROUPE</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Ajout de .</p>
            <p style="font-weight: normal;">Ce paramètre est un tableau d’objets possibles auxquels le formulaire personnalisé peut être joint. Il a été ajouté pour prendre en charge la possibilité de joindre un formulaire personnalisé à plusieurs types d’objets.</p>
            <p>Valeurs possibles : </p>
            <p>CMPY, PORT, PRGM, PROJ, TÂCHE, OPTASK, UTILISATEUR, DOCU, EXPNS, ITRN, BILL, GROUPE</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>Ajout de .</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>Ajout de .</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Ajout de .</p>
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
            <p>Ajout des valeurs suivantes :</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (Intégration (API Graph) SharePoint activée)</p>
                <p>Cette valeur prend en charge l’intégration SharePoint mise à jour.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Autoriser les utilisateurs à créer des projets sans utiliser de modèle)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

Les documents peuvent être organisés en dossiers. Vous pouvez créer des dossiers personnels dans votre zone Documents personnels. L’objet DocumentFolder représente l’un de ces dossiers.

L’objet DocumentFolder a ajouté l’indicateur . `SHARABLE`.

### DocumentVersion (DOCV)

Un objet DocumentVersion représente une version spécifique d’un fichier (comme du matériel écrit, des images ou d’autres formes d’informations).

Pour plus d’informations sur les versions de document, voir [Télécharger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

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
            <p>Ajout de la valeur suivante : </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (API Graph))</p>
                <p>Cette valeur prend en charge l’intégration SharePoint mise à jour.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Groupe (GROUP)

Un objet Group représente un ensemble d’utilisateurs et d’équipes. Les groupes représentent souvent la structure du Ministère.

Pour plus d’informations sur les groupes, voir Groupes et équipes.

L’objet Group a ajouté l’indicateur . `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <p>Les champs suivants ont été ajoutés :</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Une catégorie est un formulaire personnalisé. Ce paramètre a été ajouté pour prendre en charge la possibilité d’ajouter des Forms personnalisées aux objets de groupe. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Il s’agit d’un paramètre booléen dont la valeur est true si un objet est actif et false dans le cas contraire. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td >
        <p>Les champs suivants ont été ajoutés :</p>
        <ul>
          <li>
            <p><b>approbateur</b>
            </p>
          </li>
          <li>
            <p><b>client</b>
            </p>
          </li>
          <li>
            <p><b>demandeur</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <p>Les champs suivants ont été ajoutés :</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>Dans certains cas, il est possible de lier des tâches Workfront directement à des objets d’un produit logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs par défaut</td>
      <td >
        <p>Le champ suivant a été ajouté :</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Il s’agit d’un paramètre booléen dont la valeur est true si un objet est actif et false dans le cas contraire. Les objets définis sur Actif s’affichent dans des menus déroulants et des champs de type avant et peuvent être associés à d’autres objets.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <p>Les champs suivants ont été ajoutés :</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>Cette action recalcule les expressions dans les champs de formulaire personnalisés.</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

L’objet JournalEntry peut être configuré pour consigner des informations sur des champs d’objet spécifiques chaque fois que ces champs sont modifiés. Lorsqu’un champ est configuré pour être consigné dans le cadre de l’objet d’entrée de journal, une entrée de journal correspondante est créée chaque fois que ce champ est modifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>Ajout de la valeur suivante : </p>
        <ul>
          <li>
            <p>DW (Téléchargement)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

Un objet LinkedFolder représente un dossier lié à un fournisseur de documents externe, tel que Google Drive ou Dropbox.

Pour plus d’informations sur les dossiers liés, voir Lier des documents à partir d’applications externes.

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
            <p>Ajout de la valeur suivante : </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (API Graph))</p>
                <p>Cette valeur prend en charge l’intégration SharePoint mise à jour.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask / Problème (OPTASK)

Un objet OpTask est généralement appelé Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de service d’assistance. Modifier les commandes, les requêtes et les bogues sont également des problèmes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <p>Les actions suivantes ont été ajoutées :</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>L’action suivante a été modifiée :</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>Champ ajouté <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Paramètre (PARAM)

Un objet de paramètre est un champ personnalisé.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <p>Le champ suivant a été ajouté :</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>Les champs suivants ont été modifiés :</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Ajout de la valeur possible <code>WIDGET </code>(Widget) </p>
            <p>Cette valeur prend en charge l’utilisation d’images dans les formulaires personnalisés.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Ajout de la valeur possible <code>WIDGET </code>(Widget)</p>
            <p>Cette valeur prend en charge l’utilisation d’images dans les formulaires personnalisés.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (PORT)

Un objet de Portfolio est un ensemble de projets qui rivalisent pour les mêmes ressources, généralement de l’argent ou des personnes pour les compléter.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Programme (PRGM)

Un objet de programme est un sous-ensemble de projets d’un portfolio, où des projets similaires peuvent être regroupés.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Projet (PROJ)

Les projets sont des éléments de travail dans Workfront et sont une composante essentielle de la façon dont Workfront aide les personnes à travailler. Un objet Projet représente un groupe de tâches avec un objectif commun et spécifique.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td >
        <ul>
          <li>
            <p><b>initiative</b>
            </p>
            <p>L’objet Initiative crée des estimations dans le planificateur de scénarios de Workfront pour le type et le nombre de rôles de tâche, les coûts fixes et l’avantage planifié. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>Dans certains cas, il est possible de lier des tâches Workfront directement à des objets d’un produit logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Un objet QueueDef représente une file d’attente, qui est un projet qui a été publié dans la zone Aide Desk pour permettre aux utilisateurs de lui envoyer des problèmes.

Pour plus d’informations sur les files d’attente de requête, voir [Création d’une file d’attente de requête](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Éditer les équipes sur lesquelles je travaille)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Éditer les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un objet ScoreCardQuestion représente une question qui a été ajoutée à une Fiche d’évaluation. Ces questions sont généralement définies par le responsable du Portfolio et leurs réponses permettent au responsable de comprendre dans quelle mesure un projet s’aligne sur les objectifs du portefeuille.

Pour plus d’informations sur les questions de la Fiche d’évaluation, voir [Création d’une Fiche d’évaluation](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Ajout de la valeur possible <code>WIDGET </code>(Widget)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tâche (TÂCHE)

Un objet Task représente un élément de travail qui doit être exécuté comme une étape vers l’atteinte d’un objectif final (achèvement d’un projet).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>Dans certains cas, il est possible de lier des tâches Workfront directement à des objets d’un produit logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Modèle (TMPL)

Un objet Template représente un modèle pour un projet. Les projets peuvent être créés à partir de modèles pour gagner du temps. Un modèle contient une équipe et des tâches qui seront copiées dans tout projet créé à partir du modèle.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
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
      <td role="rowheader">Champs principaux</td>
      <td>
        <p>Le champ suivant a été supprimé :</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Vue (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>Les valeurs possibles suivantes ont été supprimées :</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (Mise en page Quatre colonnes)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Mises à jour)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Mises à jour)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (En train de travailler sur)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (Données personnalisées)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (Mettre à jour les données personnalisées)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (Mise à jour statut)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Mise à jour statut)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Mise à jour statut)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Mise à jour statut)</p>
              </li>
              <li>
                <p><code>DLIST</code> (Liste détaillée)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (Section de liste détaillée)</p>
              </li>
            </ul>
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
            <p><b>updateType</b>
            </p>
            <p>Ajout de la valeur possible <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Utilisateur (USER)

Un objet User représente une personne disposant d’un compte dans Workfront qui peut se connecter et interagir avec le système.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
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
            <p><b>eventType</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>DUP </code>(Demande de BAT d’un document)</p>
              </li>
              <li>
                <p><code>DUV </code>(Permet d’afficher un document)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Travail (WORK)

Un objet de travail est une interface commune dont Task et OpTask héritent tous deux et partagent le code commun entre les deux.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>Dans certains cas, il est possible de lier des tâches Workfront directement à des objets d’un produit logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
