---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 21 de l’API
description: Adobe Workfront a publié la verison 21 de l’API le vendredi 23 octobre 2025. La version 21 de l’API présente les changements suivants par rapport à la version 20.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 7166a6b51a45b744a33df697c2bc8080427908a8
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 79%

---

# Nouveautés de la version 21 de l’API

>[!IMPORTANT]
>
>Cette modification de version de l’API comprend une modification avec rupture qui peut affecter vos appels API existants. Cela est dû au fait que l’API version 21 utilise la version 2 des abonnements aux événements.
>
> Pour les champs à sélection multiple, la version 2 des abonnements aux événements envoie toujours sous la forme d’un tableau. La version 1 a envoyé un tableau si plusieurs valeurs ont été sélectionnées. Si une seule valeur a été sélectionnée, une chaîne a été envoyée.

Adobe Workfront a publié la verison 21 de l’API le vendredi 23 octobre 2025. La version 21 de l’API présente les changements suivants par rapport à la version 20.

## Ressources ajoutées

### OriginalRequest (ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>entryDate</li>
          <li>ID</li>
          <li>requestID</li>
          <li>requestName</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>ID</li>
          <li>objCode</li>
        </ul>
      </td>
 </tbody>
</table>

<!--

### StaffingPlanTemplate (SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
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

-->

## Ressources supprimées

### AssignmentBillingRole (ASBLRL)

L&#39;objet AssignmentBillingRole et tous ses champs ont été supprimés.

## Ressources modifiées

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
            <p><b>coreAction</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
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
            <p><b>action</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
         </li>
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
            <p><b>coreAction</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Pièce jointe d’annonce (ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
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
            <p><b>realWorkRequiredDouble</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Assignment (ASSGN)

Un objet Affectation représente le lien entre un élément de travail et l&#39;utilisateur, l&#39;équipe ou le groupe affecté à ce travail.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>Supprimés</p>
              </li>
            </ul>
         </li>
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
            <p><b>catObjCode</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Équipe)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Équipe)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Customer (CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (Désactiver l'utilisation d'une applet Java pour les calculs de chronologie)
            </p>
            <p>Ajouté(e)(s)</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Document (DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>Ajouté(e)(s)</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder

L’objet DocumentFolder a ajouté l’indicateur `RESTORABLE`.

### Hour (HOUR)

Un objet Hour représente une heure enregistrée par un utilisateur ou une utilisatrice sur une feuille de temps.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>getTerejectionCommentmporaryCloudURL</b>
            </p>
            <p>Ajout du programme de validation <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### OpTask (OPTASK)

Un objet OpTask est généralement appelé un Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de centre d’assistance. Les ordres de modification, les requêtes et les bugs sont également des problèmes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>realWorkRequiredDouble</b>
            </p>
            <p>Ajouté(e)(s)</p>
              </li>
            </ul>
         </li>
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
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (Texte enrichi lexical)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Cumul sur une seule ligne)</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Ajouté(e)(s)</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs par défaut</td>
      <td>
        <ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Ajouté(e)(s)</p>
           </li>
           </ul>
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
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>Ajouté(e)(s)</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>devise</b>
            </p>
            <p>Ajouté(e)(s)</p>
              </li>
            </ul>
         </li>
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
            <p><b>realWorkRequiredDouble</b>
            </p>
            <p>Ajouté(e)(s)</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Un objet QueueDef représente une file d’attente, à savoir un projet qui a été publié dans la zone Centre d’assistance pour permettre aux utilisateurs et utilisatrices d’y envoyer des problèmes.

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
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Modifier les informations de contact)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>helpDeskProjects</b>
            </p>
            <p>Ajouté(e)(s)</p>
            </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Taux (RATE)

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
            <p><b>localBillingPerHour</b>
            </p>
            <p>Supprimés</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>Supprimés</p>
              </li>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Rôle (ROLE)

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
            <p><b>Remplacer la devise</b>
            </p>
            <p>Supprimés</p>
              </li>
          <li>
            <p><b>Remplacer le taux de coût</b>
            </p>
            <p>Supprimés</p>
              </li>
          <li>
            <p><b>Remplacer le taux de facturation</b>
            </p>
            <p>Supprimés</p>
              </li>
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
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un objet ScoreCardQuestion représente une question qui a été ajoutée à une carte de performance. Ces questions sont généralement définies par la personne gestionnaire du portfolio et leurs réponses lui permettent de comprendre dans quelle mesure un projet s’aligne sur les objectifs du portfolio.<table>
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
            <p>Ajout de la valeur possible suivante :</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Cumul sur une seule ligne)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### StaffingPlan

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

<!--

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

### Tâche (TASK)

Un objet Task représente un élément de travail qui doit être exécuté comme une étape vers la réalisation d’un objectif final (achèvement d’un projet).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>realWorkRequiredDouble</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Equipe

L’objet Équipe a ajouté les indicateurs `DATA_EXTENDIBLE` et `SHARABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de référence</td>
      <td>
        <ul>
          <li>
            <p><b>category</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### TemplateAssignment

L&#39;objet TemplateAssignment a ajouté l&#39;indicateur `ATTRIBUTE_ATTACHABLE`.

### Timesheet (TSHET)

Un objet Timesheet représente une feuille de temps virtuelle qui permet aux utilisateurs et utilisatrices de saisir les heures effectives travaillées pour les tâches, les projets et les types d’heures supplémentaires.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs principaux</td>
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

### Work (WORK)

Un objet Work est une interface commune dont Task et OpTask héritent tous deux et qui partage le code commun entre les deux.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>realWorkRequiredDouble</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>Ajouté(e)(s)</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


