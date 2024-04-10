---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de l’API version 18
description: Adobe Workfront a publié la version 18 de l’API le 6 avril 2022. La version 18 de l’API présente les modifications suivantes par rapport à la version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Nouveautés de l’API version 18

Adobe Workfront a publié la version 18 de l’API le 8 avril 2024. La version 18 de l’API présente les modifications suivantes par rapport à la version 15.

## Ressources ajoutées

Aucune ressource n’a été ajoutée pour l’API version 18.

## Ressources supprimées

Aucune ressource n’a été supprimée pour l’API version 18

## Ressources modifiées

### AccessLevelPermissions (ALVPER)

Un objet AccessLevelPermissions représente une autorisation spécifique d&#39;accès, de création ou de modification d&#39;un objet Workfront. Ces autorisations peuvent ensuite être associées à un niveau d’accès.

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
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Demande d&#39;accès (ACSREQ)

Si un utilisateur n’a pas accès à un objet dans Workfront dont il a besoin, il peut demander l’accès à cet objet. L&#39;objet AccessRequest représente cette demande.

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
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Règle d’accès (ACSRUL)

Un objet AccessRule représente un ensemble de règles dans les niveaux d&#39;accès personnalisés qui détermine comment les utilisateurs peuvent partager les projets qu&#39;ils créent.

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
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approbation (APPROBATION)

Un élément de travail donné, tel qu’une tâche, un document ou une feuille de temps, peut nécessiter l’approbation d’un superviseur ou d’un autre utilisateur sur l’élément de travail. Un objet d&#39;approbation représente l&#39;action d&#39;approbation d&#39;un élément de travail.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>realNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### En attente d’approbation (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Opérations</td>
      <td>
        <ul>
          <li>
            <p>Ajout des opérations suivantes :
            </p>
            <ul>
              <li>
                <p><b>AJOUTER</b>
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

### Ligne de base (BLIN)

Les références sont des instantanés de la performance d’un projet à un moment donné dans le temps. Ils stockent des informations clés sur le projet, telles que les dates clés, l’avancement, les coûts et les valeurs de chiffre d’affaires.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>realNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tâche de ligne de base (BSTSK)

Les références sont des instantanés de la performance d’un projet à un moment donné dans le temps. Ils stockent des informations clés sur le projet, telles que les dates clés, l’avancement, les coûts et les valeurs de chiffre d’affaires. Lorsque vous créez une planification, les informations sur la tâche sont également capturées sur les tâches planifiées de cette planification.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>realNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Catégorie (CTY)

Un objet Catégorie est un formulaire personnalisé.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>:
            </p>
            <p>Ajout des valeurs possibles suivantes :
            <ul>
              <li>
                <p><code>NLBRCY</code> (Catégorie de ressources non liées à la main-d’œuvre)
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
            <p><b>objTypes</b>:
            </p>
            <p>Ajout des valeurs possibles suivantes :
            <ul>
              <li>
                <p><code>NLBRCY</code> (Catégorie de ressources non liées à la main-d’œuvre)
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

Un objet Document représente un fichier (tel qu&#39;un document écrit, des images ou d&#39;autres formes d&#39;informations).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>Ajout du paramètre suivant :
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>:
            </p>
            <p>Ajouté. Cette nouvelle action utilise les paramètres suivants :
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

### Données financières (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>realNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
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
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>realNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Entrée de journal (JRNLE)

L&#39;objet JournalEntry peut être configuré pour enregistrer des informations sur des champs d&#39;objet spécifiques chaque fois que ces champs sont modifiés. Lorsqu’un champ est configuré pour être enregistré dans l’objet Entrée du journal, une entrée du journal correspondante sera créée chaque fois que ce champ sera modifié.

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
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opens)</p>
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

Un objet OpTask est communément appelé événement. Un événement est un élément de travail qui indique généralement qu’il existe un problème empêchant l’achèvement d’une tâche ou d’un projet. Un événement peut également être une demande du Help Desk. Les ordres de modification, les demandes et les bogues sont également des problèmes.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>Ajout des champs suivants :
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>Ajout des champs suivants :
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

### Projet (PROJ)

Les projets sont des éléments de travail dans Workfront et constituent un élément essentiel de la manière dont Workfront aide les utilisateurs à travailler. Un objet Project représente un groupe de tâches ayant un objectif commun et spécifique.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>realNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
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
            <p>Ajout du champ suivant :
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
            <p>Ajout du champ suivant :
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

Un objet QueueDef représente une file d&#39;attente, qui est un projet qui a été publié dans la zone du Help Desk pour permettre aux utilisateurs d&#39;y soumettre des problèmes.

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
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Afficher les taux de coûts)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Afficher les taux de facturation)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Afficher finances générales)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Modifier les taux de coûts)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Modifier les taux de facturation)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Modifier finances générales)</p>
              </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Taux (TAUX)

Un objet Rate représente un taux de facturation dans Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>Ajout des indicateurs suivants :
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DYNAMIQUE
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


### Tâche (TÂCHE)

Un objet Tâche représente un élément de travail qui doit être effectué en tant qu’étape vers l’objectif final (terminer un projet).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>realNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
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
             <p>Ajout du champ suivant :
             <ul><li><code>copyCategories</code></li></ul>
            </p>
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
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TâcheModèle (TSK)

Un objet TemplateTask représente une tâche qui fait partie d&#39;un modèle. Les tâches de modèles deviennent des tâches dans le projet dans lequel le modèle est utilisé.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole (ÉQUIPE)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout du champ suivant :
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
            <p>Ajout du champ suivant :
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

### Feuille de temps (TSHET)

Un objet de feuille de temps représente une carte de présence virtuelle qui permet aux utilisateurs de saisir les heures réellement travaillées pour les tâches, les projets et les types d&#39;heures de frais généraux.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p>Suppression du champ suivant :
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

### Mettre à jour (MISE À JOUR)

Les éléments de travail dans Workfront peuvent être mis à jour pour tenir les utilisateurs informés du statut actuel. Un objet Update représente l&#39;une de ces mises à jour. Les mises à jour peuvent être saisies par les utilisateurs ou créées par le système Workfront.

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
            <p>Ajout des valeurs possibles suivantes :</p>
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

Un objet UserPrefValue représente une préférence utilisateur.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>valeur</b>
            </p>
            <p>Ajout du programme de validation <code>MAX_LENGTH</code></p>
      </td>
    </tr>
  </tbody>
</table>

### Travail (TRAVAIL)

Un objet de travail est une interface commune dont les propriétés Task et OpTask héritent et qui partage un code commun.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Ajout des champs suivants :
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>realNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>coûtDépenseNonFacturablePrévu</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

