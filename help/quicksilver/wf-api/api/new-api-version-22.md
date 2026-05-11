---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 22 de l’API
description: Adobe Workfront a publié la version 22 de l’API le 11 mai 2026. La version 22 de l’API présente les modifications suivantes par rapport à la version 21.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 54%

---

# Nouveautés de la version 22 de l’API

Adobe Workfront a publié la version 22 de l’API le 8 mai 2026. La version 22 de l’API présente les modifications suivantes par rapport à la version 21.

## Ressources ajoutées

Les ressources suivantes ont été ajoutées pour l’API version 22.

### ReportShareableFolder (RPSHFD)

Vous pouvez utiliser des dossiers de rapports partageables pour organiser les rapports et partager ces dossiers avec d’autres utilisateurs. Cette fonctionnalité est conçue pour les équipes qui gèrent d’importants volumes de rapports et ont besoin d’un contrôle d’accès évolutif et cohérent.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Champs par défaut</td>
      <td>
        <ul>
          <li>name</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">Opérations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>SUPPRIMER</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## Ressources supprimées

Les ressources suivantes ont été supprimées de l’API version 22.

### UserLocation (USRLOC)

Cet objet a été supprimé.

## Ressources modifiées

Les ressources suivantes ont été modifiées pour l’API version 22.

### AccessLevel (ACSLVL)

Un objet AccessLevel est associé à des personnes et décrit le jeu d’autorisations AccessLevelPermissions qui déterminent ce à quoi la personne peut accéder.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Le champ suivant a été modifié avec des modifications de valeurs possibles. Pour plus d’informations, consultez la documentation destinée aux développeurs et développeuses.
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
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
      <td>Les champs suivants ont été modifiés avec des modifications de valeurs possibles. Pour plus d’informations, consultez la documentation destinée aux développeurs et développeuses.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>Le champ suivant a été modifié avec des modifications de valeurs possibles. Pour plus d’informations, consultez la documentation destinée aux développeurs et développeuses.
        <ul>
          <li><b>action</b></li>
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
      <td>Les champs suivants ont été modifiés avec des modifications de valeurs possibles. Pour plus d’informations, consultez la documentation destinée aux développeurs et développeuses.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>Le champ suivant a été ajouté.
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Entreprise (CMPY)

Un objet Company représente une organisation composée d’un ensemble de personnes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmProjectID</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

L’objet CustomEnum permet de convertir les codes de statut en texte lisible par une personne.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>Ajouté(e)(s)
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Requêtes</td>
      <td>Ajouté(e)(s)
        <ul>
          <li><p><b>assignmentStatuses</b></p></li>
          <li><p><b>bookingStatuses</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### Customer (CUST)

Un objet Customer représente une organisation qui utilise une instance de Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Le champ suivant a été modifié.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Ajout des valeurs possibles suivantes.</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> (Statuts de la réservation)</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> (Statuts d'affectation)</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
         <ul>
         <li><b>isLegacyCustomerEsmStorageEnabled</b></li>
         <li><b>isLegacyCustomerSystemFileMigrationEnabled</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomerSystemFileMigrationDate</b></li>
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
      <td>Le champ suivant a été modifié.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Ajout des valeurs possibles suivantes pour la prise en charge de Enterprise Storage Management :</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>


### Document (DOCU)

Un objet Document représente un fichier (tel qu’un support écrit, des images ou d’autres formes d’informations).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>L’action suivante a été modifiée.
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>objID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder (DOCFDR)

Les documents peuvent être organisés en dossiers. Vous pouvez créer des dossiers personnels dans votre zone personnelle Documents. L’objet DocumentFolder représente l’un de ces dossiers.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
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
      <td>Le champ suivant a été ajouté pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      Le champ suivant a été modifié.
        <ul>
          <li><b>version</b><p>Suppression du programme de validation « OBLIGATOIRE ».</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>L’action suivante a été ajoutée.
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Opérations</td>
      <td>L'opération suivante a été ajoutée.
        <ul>
          <li><p><b>EDIT</b></p>
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
      <td>Les champs suivants ont été ajoutés.
        <ul>
          <li><b>portfolioID</b></li>
          <li><b>programID
          </b></li>
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
      <td>Les champs suivants ont été modifiés.
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Ajout des valeurs possibles suivantes.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Déplacer le dossier)</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>indicateurs</b>
            </p>
            <p>Ajout des valeurs possibles suivantes.</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.journalentryflagenum.iscontactinfoentry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalField (JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été modifiés.
        <ul>
          <li>
            <p><b>action</b>
            </p>
            <p>Ajout des valeurs possibles suivantes.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Déplacer le dossier)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask (OPTASK)

Un objet OpTask est généralement appelé Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de centre d’assistance. Les ordres de modification, les requêtes et les bugs sont également des problèmes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li><b>realWorkRequired</b><p>Ajout des indicateurs suivants :
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de recherche</td>
      <td>
        <ul>
          <li><b>travailRéel</b><p>Type modifié de <code>null</code> en <code>double</code>.</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest(ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Opérations</td>
      <td>Les opérations suivantes ont été ajoutées.
        <ul>
          <li><p><b>COUNT</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>REPORT</b></p>
          <li><p><b>SEARCH</b></p>
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
      <td>Les champs suivants ont été ajoutés.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### ParameterGroup (PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### PortalSection (PTLSEC)

Un objet PortalSection est un rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Le champ suivant a été ajouté.
        <ul>
          <li><b>reportShareFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>Le champ suivant a été ajouté.
        <ul>
          <li><b>reportShareableFolder</b></li>
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
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
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
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      Le champ suivant a été modifié.
        <ul>
          <li><b>portfolioID</b><p>Ajout du programme de validation « OBLIGATOIRE ».</li>
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
      <td>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef (QUED)

Un objet QueueDef représente une définition de file d’attente des demandes dans Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été modifiés avec des modifications de valeurs possibles. Pour plus d’informations, consultez la documentation destinée aux développeurs et développeuses.
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Rapport planifié (SCHREP)

Un objet ScheduledReport représente un rapport qui a été configuré pour être diffusé.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>Le champ suivant a été modifié avec des modifications importantes des valeurs possibles. Pour plus d’informations, consultez la documentation destinée aux développeurs et développeuses.
        <ul>
          <li><b>format</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tâche (TASK)

Un objet Tâche représente un élément de travail qui doit être terminé pour atteindre un objectif final (terminer un projet).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>Ajouté(e)(s)</p></li>
          <li><p><b>realWorkRequired</b></p><p>Ajout des indicateurs <code>AUTO_LOAD</code> et <code>DYNAMIC</code>.</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>
        <ul>
          <li>
            <p><b>convertedOpTask</b>
            </p>
            <p>Ajouté(e)(s)</p>
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
      <td role="rowheader">Champs directs</td>
      <td>Les champs suivants ont été ajoutés pour prendre en charge la gestion du stockage d’entreprise.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>Le champ suivant a été modifié.
        <ul>
          <li>
            <p><b>action</b>
            </p>
            <p>Ajout de la valeur possible suivante.</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
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
      <td role="rowheader">Champs directs</td>
      <td>Le champ suivant a été ajouté.
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>Le champ suivant a été supprimé.
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





