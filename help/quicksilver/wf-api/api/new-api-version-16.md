---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 16 de l’API
description: Adobe Workfront a publié la version 16 de l’API le jeudi 6 avril 2022. La version 16 de l’API comprend les modifications suivantes par rapport à la version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 26%

---

# Nouveautés de la version 16 de l’API

Adobe Workfront a publié la version 16 de l’API le vendredi 6 avril 2023. La version 16 de l’API comprend les modifications suivantes par rapport à la version 15.

## Ressources ajoutées

Aucune ressource n’a été ajoutée pour la version 16 de l’API.

## Ressources supprimées

Aucune ressource n’a été supprimée pour la version 16 de l’API.

## Ressources modifiées

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Approval (APPROVAL)](#approval-approval)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [Heure (HEURE)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [Remarque (REMARQUE)](#note-note)
* [OpTask / Problème (OPTASK)](#note-note)
* [Project (PROJ)](#project-proj)
* [Rate (RATE)](#rate-rate)
* [RichTextNote (RHRETE)](#richtextnote-rhnote)
* [Rôle/Rôle de tâche (RÔLE)](#role--job-role-role)
* [Task (TASK)](#task-task)
* [Timesheet (TSHET)](#timesheet-tshet)
* [UIFilter / Filter (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Regroupement (UIGB)](#uigroupby--grouping-uigb)
* [UIView / View (UIVW)](#uiview--view-uivw)
* [Utilisateur (USER)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

### Approval (APPROVAL)

Un élément de travail donné, tel qu’une tâche, un document ou une feuille de temps, peut exiger qu’un superviseur ou une superviseuse, ou un autre utilisateur ou une autre utilisatrice, valide l’élément de travail. Un objet Approval représente l’action de validation d’un élément de travail.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Ce champ a été ajouté et indique le nombre de minutes de travail par jour que vous devez effectuer. Il a le format <code>YYYY-MM-DD: (number of minutes)</code> et prend en compte le fuseau horaire.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Attribution (ASSGN)

Un objet d’affectation représente la connexion entre un élément de travail et l’utilisateur, l’équipe ou le groupe affecté pour y travailler.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Ce champ a été ajouté et indique le nombre de minutes de travail par jour que vous devez effectuer. Il a le format <code>YYYY-MM-DD: (number of minutes)</code> et prend en compte le fuseau horaire.</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>Ce champ a été ajouté et est une valeur booléenne qui indique si l’affectation est liée ou non. Si les minutes de l’affectation par jour ont été modifiées dans l’équilibreur de charge de travail, l’affectation a été tronquée.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

L’objet CustomEnum permet de convertir des codes d’état en texte lisible.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
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
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>Cette action renvoie une valeur booléenne qui indique si le client a désactivé l’option permettant de mettre à niveau automatiquement les titulaires de licence du contributeur.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

Un objet ExternalSection est une page Web externe qui est incorporée dans un rapport Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>Ceci a été ajouté et calcule l’URL d’un iFrame incorporé dans un rapport.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>Ceci a été ajouté et calcule les URL des iFrames incorporées dans un rapport.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Heure (HEURE)

Un objet Hour représente une heure consignée par un utilisateur sur une feuille de temps.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>Ajouté. Ce paramètre est utilisé pour identifier les heures créées avec <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Remarque (REMARQUE)

Un objet Remarque est un commentaire ou une mise à jour effectué sur un objet Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>attachmentDocuments</b>
            </p>
            <p>Ce champ a été ajouté et représente une liste de documents joints au commentaire.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / Problème (OPTASK)

Un objet OpTask est généralement appelé un Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de service d’assistance. Les ordres de modification, les demandes et les bogues sont également des problèmes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Ce champ a été ajouté et indique le nombre de minutes de travail par jour que vous devez effectuer. Il a le format <code>YYYY-MM-DD: (number of minutes)</code> et prend en compte le fuseau horaire.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Cette action a ajouté le champ <code>teamIDs</code> pour prendre en charge la fonctionnalité d’affectation de plusieurs équipes à une tâche ou un problème.</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Project (PROJ)

Les projets sont des éléments de travail dans Workfront et sont un bloc de création essentiel de la façon dont Workfront aide les personnes à travailler. Un objet Project représente un groupe de tâches avec un objectif commun et spécifique.

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
            <p>Ce champ a été ajouté et représente la somme de toutes les heures budgétées du projet.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Rate (RATE)

Un objet Rate représente un taux de facturation dans Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>Ces paramètres ont été déplacés vers l’objet Rate à partir de l’objet Role , de sorte que les objets Role et User puissent avoir plusieurs valeurs (pour des périodes distinctes).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Ces paramètres représentent l’identifiant et le code d’objet de l’objet auquel le taux est associé.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>Cette action a été ajoutée et joint des objets Rate à l’objet donné. Ce point de terminaison fonctionne pour tous les objets de rate Attachable.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHRETE)

Un objet RichTextNote est un commentaire ou une mise à jour effectué sur un objet Workfront, qui comprend du texte enrichi tel que du texte en gras ou en italique.

L’objet RichTextNote a supprimé l’indicateur `REPORTABLE`.

### Rôle/Rôle de tâche (RÔLE)

Un objet Rôle (rôle de tâche) représente une capacité fonctionnelle ou un ensemble de compétences qu’un utilisateur peut remplir, tel que Designer ou Gestionnaire de produits.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
           <li>
            <p><b>rates</b>
            </p>
            <p>Ceci a été ajouté et représente les objets Rate associés à ce rôle.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Task (TASK)

Un objet Task représente un élément de travail qui doit être exécuté en tant qu’étape vers la réalisation d’un objectif final (achèvement d’un projet).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Ce champ a été ajouté et indique le nombre de minutes de travail par jour que vous devez effectuer. Il a le format <code>YYYY-MM-DD: (number of minutes)</code> et prend en compte le fuseau horaire.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Cette action a ajouté le champ <code>teamIDs</code> pour prendre en charge la fonctionnalité d’affectation de plusieurs équipes à une tâche ou un problème.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Timesheet (TSHET)

Un objet Timesheet représente une feuille de temps virtuelle qui permet aux utilisateurs et utilisatrices de saisir les heures effectives travaillées pour les heures de tâches, projets et types de frais.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>Ce paramètre a supprimé l’indicateur <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Ce paramètre a supprimé l’indicateur <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Ce paramètre a été ajouté et stocke la durée des feuilles de temps en jours, indépendamment des modifications apportées à "Heures équivalentes pour le Workday complet".  Par exemple, si la valeur Horaires équivalents est définie sur 6 et qu’un jour est consigné, la valeur Horaires équivalents est changée sur 8 heures, <code>totalDays</code> a toujours la valeur 1.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filter (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>Cette action a été ajoutée et utilise une carte de requête de filtre et ajoute la jointure <code>allowingnull</code> pour les champs nuls.</p>
         </li>
         <li>
            <p><b> disableSystemWideVisibility
</b>
            </p>
            <p><b> enableSystemWideVisibility </b>
            </p>
            <p>Ces actions permettent de partager des filtres, des vues et des regroupements à l’échelle du système.</p><p>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Mise à disposition de filtres, de vues ou de groupes pour tous les utilisateurs</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Regroupement (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b> disableSystemWideVisibility
</b>
            </p>
            <p><b> enableSystemWideVisibility </b>
            </p>
            <p>Ces actions permettent de partager des filtres, des vues et des regroupements à l’échelle du système.</p><p>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Mise à disposition de filtres, de vues ou de groupes pour tous les utilisateurs</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / View (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b> disableSystemWideVisibility
</b>
            </p>
            <p><b> enableSystemWideVisibility </b>
            </p>
            <p>Ces actions permettent de partager des filtres, des vues et des regroupements à l’échelle du système.</p><p>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Mise à disposition de filtres, de vues ou de groupes pour tous les utilisateurs</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Utilisateur (USER)

Un objet User représente une personne disposant d’un compte dans Workfront qui peut se connecter et interagir avec le système.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
           <li>
            <p><b>rates</b>
            </p>
            <p>Ceci a été ajouté et représente les objets Rate associés à cet utilisateur.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

Un objet UserNote est une notification.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Requêtes</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>Ajout de la valeur possible suivante :
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Work (WORK)

Un objet Work est une interface commune dont Task et OpTask héritent tous deux, et partage le code commun entre les deux.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Ce champ a été ajouté et indique le nombre de minutes de travail par jour que vous devez effectuer. Il a le format <code>YYYY-MM-DD: (number of minutes)</code> et prend en compte le fuseau horaire.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
