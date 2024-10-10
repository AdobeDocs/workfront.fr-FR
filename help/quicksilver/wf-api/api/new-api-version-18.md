---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 18 de l’API
description: Adobe Workfront a publié la version 18 de l’API le 6 avril 2022. La version 18 de l’API présente les changements suivants par rapport à la version 17.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 100%

---

# Nouveautés de la version 18 de l’API

Adobe Workfront a publié la version 18 de l’API le 8 avril 2024. La version 18 de l’API présente les changements suivants par rapport à la version 17.

## Ressources ajoutées

Aucune ressource n’a été ajoutée pour la version 18 de l’API.

## Ressources supprimées

Aucune ressource n’a été supprimée pour la version 18 de l’API.

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
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
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
            <p><b>action</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
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
            <p><b>coreAction</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
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
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AwaitApproval (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Opérations</td>
      <td>
        <ul>
          <li>
            <p>Ajout des opérations suivantes :
            </p>
            <ul>
              <li>
                <p><b>ADD</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Baseline (BLIN)

Les niveaux de référence sont des instantanés de ce à quoi ressemblaient les performances d’un projet à un moment donné dans le temps. Elles stockent des informations clés sur le projet, telles que les dates clés, la progression, et les valeurs de coût et de revenu.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BaselineTask (BSTSK)

Les références sont des instantanés de ce à quoi ressemblaient les performances d’un projet à un moment donné dans le temps. Elles stockent des informations clés sur le projet, telles que les dates clés et la progression, ainsi que les valeurs des coûts et des revenus. Lorsque vous créez une référence, les informations de tâche sont également capturées sur les tâches de base de cette référence.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Category (CTGY)

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
            <p><b>catObjCode</b> :
            </p>
            <p>Ajout des valeurs possibles suivantes :
            <ul>
              <li>
                <p><code>NLBRCY</code> (Catégorie de ressources non liée à la main-d’œuvre)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Heure)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Carte tarifaire)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b> :
            </p>
            <p>Ajout des valeurs possibles suivantes :
            <ul>
              <li>
                <p><code>NLBRCY</code> (Catégorie de ressources non liée à la main-d’œuvre)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Heure)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Carte tarifaire)
                </p>
              </li>
             </ul>
             </p>
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
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b> :
            </p>
            <p>Ajout du paramètre suivant :
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b> :
            </p>
            <p>Ajouté. Cette nouvelle action utilise les paramètres suivants :
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### FinancialData (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decisions.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
              </li>
            </ul>
          </li>
        </ul>
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
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b> :
            </p>
            <p>Ajout des champs suivants :
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b> :
            </p>
            <p>Ajout des champs suivants :
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Project (PROJ)

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
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>createProjectWithOverride</b>
            </p>
             <p>Ajouté.
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ProjectUserRole (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout du champ suivant :
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p>Ajout du champ suivant :
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
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
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de dépenses)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher les finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de dépenses)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier les finances générales)</p>
              </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Rate (RATE)

Un objet Rate représente un taux de facturation dans Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>Ajout des indicateurs suivants :
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DYNAMIC
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>Ajouté.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>Ajouté.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Task (TASK)

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
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>convertToProject</b>
            </p>
             <p>Ajout du champ suivant :
             <ul><li><code>copyCategories</code></li></ul>
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Template (TMPL)

Un objet Template représente un modèle de projet. Les projets peuvent être créés à partir de modèles pour gagner du temps. Un modèle contient une équipe et des tâches qui seront copiées dans tout projet créé à partir du modèle.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TemplateTask (TTSK)

Un objet TemplateTask représente une tâche qui fait partie d’un modèle. Les tâches de modèle deviennent des tâches dans le projet où le modèle est utilisé.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole (TTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout du champ suivant :
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p>Ajout du champ suivant :
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Timesheet (TSHET)

Un objet Timesheet représente une feuille de temps virtuelle qui permet aux utilisateurs et utilisatrices de saisir les heures effectives travaillées pour les tâches, les projets et les types d’heures supplémentaires.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p>Suppression du champ suivant :
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
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
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
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
            <p><b>recentUpdatesObjIDs</b>
            </p>
            <p>Ajouté.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

Un objet UserPrefValue représente une préférence utilisateur ou utilisatrice.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>value</b>
            </p>
            <p>Ajout du programme de validation <code>MAX_LENGTH</code></p>
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
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

