---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 15 de l’API
description: Adobe Workfront a publié l’API version 14 le 14 juin 2022. La version 15 de l’API présente les changements suivants par rapport à la version 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2286'
ht-degree: 100%

---

# Nouveautés de la version 15 de l’API

Adobe Workfront a publié l’API version 15 le 14 juin 2022. La version 15 de l’API présente les changements suivants par rapport à la version 14.

## Ressources ajoutées

* [Initiative (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [UserApproval (USRAPV)](#UserAppr)

### Initiative (INITIV)

L’objet Initiative crée des estimations dans le planificateur de scénarios Workfront pour le type et le nombre de fonctions, les coûts fixes et le bénéfice prévu.

Pour plus d’informations sur les initiatives, voir [Vue d’ensemble des initiatives dans le planificateur de scénarios](../../scenario-planner/initiatives-overview.md).

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
            <p>Il s’agit d’un objet interne.</p>
          </li>
          <li>
            <p><b>duration</b>
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
            <p>Identifiant associé à l’utilisateur ou l’utilisatrice qui a envoyé la demande.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>Identifiant associé à l’action</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>Identifiant associé à l’initiative.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>Date de la dernière publication de l’initiative dans le planificateur de scénarios Workfront.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>Nom de l’initiative</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>Identifiant du plan associé à l’initiative.</p>
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
            <p><b>scenarioID</b>
            </p>
            <p>Identifiant du scénario dans le planificateur de scénarios Workfront associé à l’initiative.</p>
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
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>enteredBy</b>
            </p>
          </li>
          <li>
            <p><b>project</b>
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
            <p><b>REPORT </b>
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

Dans certains cas, il est possible de lier des éléments de travail Workfront directement aux objets d’un logiciel externe. L’objet ObjectIntegration représente ce lien.

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
            <p>Il s’agit d’un objet interne.</p>
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
            <p>Logiciel externe avec lequel l’objet ObjectIntegration crée un lien. Les valeurs possibles sont les suivantes :</p>
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
            <p><b>customer</b>
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
            <p><b>autoCalcPlannedHours</b>
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
            <p><b>defaultApprovalProcess</b>
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
            <p><b>objectCategories</b>
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
            <p><b>requestedDate</b>
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
            <p><b>approver</b>
            </p>
          </li>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
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
            <p><b>approve</b>
            </p>
          </li>
          <li>
            <p><b>reject</b>
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
            <p><b>ADD</b>
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
            <p><b>REPORT</b>
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

Aucune ressource n’a été supprimée pour l’API version 15.

## Ressources modifiées

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSRUL)](#AccessRu)

* [Approval (APPROVAL)](#Approval)

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

* [Tâche (TASK)](#Task)

* [Modèle (TMPL)](#Template)

* [Timesheet (TSHET)](#Timeshee)

* [View (UIVIEW)](#View)

* [Update (UPDATE)](#Update)

* [Utilisateur ou utilisatrice (USER)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Work (WORK)](#Work)

### AccessLevel (ACSLVL)

Un objet AccessLevel est associé à des personnes et décrit le jeu d’autorisations AccessLevelPermissions qui déterminent ce à quoi la personne peut accéder.

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
            <p>Ajout des valeurs possibles suivantes :</p>
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
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Si une personne n’a pas accès à un objet Workfront dont elle a besoin, elle peut demander l’accès à cet objet. L’objet AccessRequest représente cette requête.

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
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (string)</p>
            <p>Ajout de la valeur possible suivante :</p>
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

Un objet AccessRule représente un jeu de règles dans les niveaux d’accès personnalisés qui détermine comment les personnes peuvent partager les projets qu’elles créent.

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
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approval (APPROVAL)

Un élément de travail donné, tel qu’une tâche, un document ou une feuille de temps, peut exiger qu’une personne en charge de la supervision ou une autre personne valide l’élément de travail. Un objet Approbation représente l’action de validation d’un élément de travail.

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
            <p>Ajout.</p>
            <p>L’objet Initiative crée des estimations dans le planificateur de scénarios Workfront pour le type et le nombre de fonctions, les coûts fixes et le bénéfice prévu. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Ajout.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Ajout.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations</b>
            </p>
            <p style="font-weight: normal;">Ajout.</p>
            <p>Dans certains cas, il est possible de lier des éléments de travail Workfront directement aux objets d’un logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
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
            <p>Ajout de la valeur possible suivante :</p>
            <ul>
              <li>
                <p>GROUP (Groupe)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Ajout.</p>
            <p style="font-weight: normal;">Ce paramètre est un tableau d’objets possibles auxquels le formulaire personnalisé peut être joint. Il a été ajouté pour prendre en charge la possibilité de joindre un formulaire personnalisé à plusieurs types d’objets.</p>
            <p>Valeurs possibles : </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
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
            <p>Ajout.</p>
            <p style="font-weight: normal;">Ce paramètre est un tableau d’objets possibles auxquels le formulaire personnalisé peut être joint. Il a été ajouté pour prendre en charge la possibilité de joindre un formulaire personnalisé à plusieurs types d’objets.</p>
            <p>Valeurs possibles : </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
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
            <p>Ajout.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>Ajout.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Ajout.</p>
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
            <p>Ajout des valeurs suivantes :</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (Intégration (API Graph) SharePoint activée)</p>
                <p>Cette valeur prend en charge l’intégration SharePoint mise à jour.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Autoriser les utilisateurs et utilisatrices à créer des projets sans utiliser de modèle)</p>
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

Les documents peuvent être organisés en dossiers. Vous pouvez créer des dossiers personnels dans votre zone personnelle Documents. L’objet DocumentFolder représente l’un de ces dossiers.

L’objet DocumentFolder a ajouté l’indicateur `SHARABLE`.

### DocumentVersion (DOCV)

Un objet DocumentVersion représente une version spécifique d’un fichier (comme du contenu écrit, des images ou d’autres formes d’informations).

Pour plus d’informations sur les versions de documents, voir [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

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
            <p>Ajout de la valeur suivante : </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> ((API Graph) SharePoint)</p>
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

Un objet Group représente un ensemble d’utilisateurs et utilisatrices et d’équipes. Les groupes représentent souvent la structure des services.

Pour plus d’informations sur les groupes, voir Groupes et équipes.

L’objet Group a ajouté l’indicateur `DATA_EXTENDIBLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <p>Les champs suivants ont été ajoutés :</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Une catégorie est un formulaire personnalisé. Ce paramètre a été ajouté pour prendre en charge la possibilité d’ajouter des formulairess personnalisés aux objets Group. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Il s’agit d’un paramètre booléen qui a la valeur true si un objet est actif et false s’il ne l’est pas. Les objets définis comme actifs apparaissent dans les menus déroulants et les champs de saisie et peuvent être attachés à d’autres objets.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td >
        <p>Les champs suivants ont été ajoutés :</p>
        <ul>
          <li>
            <p><b>approver</b>
            </p>
          </li>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
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
        <p>Les champs suivants ont été ajoutés :</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>Dans certains cas, il est possible de lier des éléments de travail Workfront directement aux objets d’un logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs par défaut</td>
      <td >
        <p>Le champ suivant a été ajouté :</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Il s’agit d’un paramètre booléen qui a la valeur true si un objet est actif et false s’il ne l’est pas. Les objets définis comme actifs apparaissent dans les menus déroulants et les champs de saisie et peuvent être attachés à d’autres objets.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <p>Les champs suivants ont été ajoutés :</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>Cette action recalcule les expressions dans les champs des formulaires personnalisés.</p>
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

L’objet JournalEntry peut être configuré pour enregistrer des informations sur des champs d’objet spécifiques chaque fois que ces champs sont modifiés. Lorsqu’un champ est configuré pour être enregistré dans le cadre de l’objet JournalEntry, une entrée de journal correspondante est créée chaque fois que ce champ est modifié.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>Ajout de la valeur suivante : </p>
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
            <p>Ajout de la valeur suivante : </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> ((API Graph) SharePoint)</p>
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

Un objet OpTask est généralement appelé Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de centre d’assistance. Les ordres de modification, les requêtes et les bugs sont également des problèmes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <p>Les actions suivantes ont été ajoutées :</p>
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
        <p>L’action suivante a été modifiée :</p>
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
        <p>Le champ suivant a été ajouté :</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>Les champs suivants ont été modifiés :</p>
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

Un objet Portfolio est un ensemble de projets qui rivalisent pour les mêmes ressources, généralement de l’argent ou des personnes pour les mener à bien.

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

Les projets sont des éléments de travail dans Workfront et sont un bloc de création essentiel de la façon dont Workfront aide les personnes à travailler. Un objet Projet représente un groupe de tâches avec un objectif commun et spécifique.

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
            <p>L’objet Initiative crée des estimations dans le planificateur de scénarios Workfront pour le type et le nombre de fonctions, les coûts fixes et le bénéfice prévu. </p>
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
            <p>Dans certains cas, il est possible de lier des éléments de travail Workfront directement aux objets d’un logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Un objet QueueDef représente une file d’attente, qui est un projet qui a été publié dans la zone Centre d’assistance pour permettre aux utilisateurs et utilisatrices de lui soumettre des problèmes.

Pour plus d’informations sur les files d’attente des demandes, voir [Créer une file d’attente des demandes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Modifier les équipes auxquelles j’appartiens)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Modifier les équipes dans les groupes que je gère (administrateurs et administratrices de groupes uniquement))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un objet ScoreCardQuestion représente une question qui a été ajoutée à une carte de performance. Ces questions sont généralement définies par la personne gestionnaire du portfolio et leurs réponses lui permettent de comprendre dans quelle mesure un projet s’aligne sur les objectifs du portfolio.

Pour plus d’informations sur les questions relatives aux cartes de performance, voir [Créer une carte de performance](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

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

### Tâche (TASK)

Un objet Task représente un élément de travail qui doit être exécuté comme une étape vers la réalisation d’un objectif final (achèvement d’un projet).

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
            <p>Dans certains cas, il est possible de lier des éléments de travail Workfront directement aux objets d’un logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Modèle (TMPL)

Un objet Template représente un modèle de projet. Les projets peuvent être créés à partir de modèles pour gagner du temps. Un modèle contient une équipe et des tâches qui seront copiées dans tout projet créé à partir du modèle.

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

### Timesheet (TSHET)

Un objet Timesheet représente une feuille de temps virtuelle qui permet aux utilisateurs et utilisatrices de saisir les heures effectives travaillées pour les tâches, les projets et les types d’heures supplémentaires.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <p>Le champ suivant a été supprimé :</p>
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

### View (UIVIEW)

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
            <p>Les valeurs possibles suivantes ont été supprimées :</p>
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
                <p><code>STATUS_UPDATE</code> (Mise à jour du statut)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Mise à jour du statut)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Mise à jour du statut)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Mise à jour du statut)</p>
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
            <p><b>updateType</b>
            </p>
            <p>Ajout de la valeur possible <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Utilisateur ou utilisatrice (USER)

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
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>DUP </code>(a demandé que vous relisiez un document)</p>
              </li>
              <li>
                <p><code>DUV </code>(vous autorise à afficher un document)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Work (WORK)

Un objet Work est une interface commune dont Task et OpTask héritent tous deux et qui partage le code commun entre les deux.

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
            <p>Dans certains cas, il est possible de lier des éléments de travail Workfront directement aux objets d’un logiciel externe. L’objet ObjectIntegration représente ce lien.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
