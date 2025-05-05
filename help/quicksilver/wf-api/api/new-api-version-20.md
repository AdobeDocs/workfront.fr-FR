---
content-type: api
navigation-topic: api-navigation-topic
title: Nouveautés de la version 20 de l’API
description: Adobe Workfront a publié la version 20 de l’API le jeudi 6 avril 2022. La version 20 de l’API présente les changements suivants par rapport à la version 19.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 61%

---

# Nouveautés de la version 20 de l’API

Adobe Workfront a publié la version 20 de l’API le lundi 4 mai 2025. La version 20 de l’API présente les changements suivants par rapport à la version 19.

## Ressources ajoutées

Aucune ressource n’a été ajoutée pour la version 20 de l’API.

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## Ressources supprimées

Aucune ressource n’a été supprimée pour l’API version 20.

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
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
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
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>realBenefits</li>
              <li>realBillableExpenseCost</li>
              <li>actualCost</li>
              <li>realExpenseCost</li>
              <li>realLaborCost</li>
              <li>realNonBillableExpenseCost</li>
              <li>revenu réel</li>
              <li>realRiskCost</li>
              <li>realValue</li>
              <li>billingRevenue</li>
              <li>budget</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>FixedCost</li>
              <li>FixedRevenue</li>
              <li>PlannedBenefits</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coût prévu</li>
              <li>coûtDépensePrévu</li>
              <li>coût prévu de la main-d'œuvre</li>
              <li>coûtDépenseNonFacturablePrévu</li>
              <li>coûtRisquePrévu</li>
              <li>valeur planifiée</li>
              <li>remainingCost</li>
              <li>chiffre d’affaires restant</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>ressourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>revenu réel</li>
          <li>coût prévu</li>
          <li>revenu prévu</li>
          </ul>
          </li>
          <li><p><b>durée planifiée</b></p> <p>Ajout des indicateurs <code>DYNAMIC</code>, <code>LAZY_READ</code> et <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Ajout de l’indicateur <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Ajout de la valeur possible <code>URH</code> (Utilisateur et rôle par heure) </li>
          <li><p><b>revenueType</b></p> <p>Ajout des valeurs possibles <code>URH</code> (Utilisateur et rôle par heure), <code>URC</code> (Utilisateur et rôle par heure avec plafond) et <code>URF</code> (Utilisateur et rôle par heure plus fixe)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
          <p>Les champs suivants ont été ajoutés :</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Assignment (ASSGN)

Un objet Affectation représente le lien entre un élément de travail et l&#39;utilisateur, l&#39;équipe ou le groupe affecté à ce travail.

L’objet Affectation a ajouté les indicateurs `ATTRIBUTE_ATTACHABLE` et `DOMAIN_EXTENDABLE`.


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### Avatar

Un objet Avatar est une photo d’utilisateur.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p><b>attachmentObjectCode</b>
            </p>
             <p>Ajouté(e)(s)</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs principaux</td>
      <td>
        <ul>
          <li>
            <p><b>attachmentObjectCode</b>
            </p>
             <p>Ajouté(e)(s)</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Opérations</td>
      <td>
        <ul>
          <li>
            <p><b>COPIER</b>
            </p>
             <p>Ajouté(e)(s)</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
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
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>realBillableExpenseCost</li>
              <li>actualCost</li>
              <li>realNonBillableExpenseCost</li>
              <li>budget</li>
              <li>eac</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coût prévu</li>
              <li>coûtDépenseNonFacturablePrévu</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>coût prévu</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Ajout de l’indicateur <code>CURRENCY</code></li>
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
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>realBillableExpenseCost</li>
              <li>actualCost</li>
              <li>realNonBillableExpenseCost</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coût prévu</li>
              <li>coûtDépenseNonFacturablePrévu</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>coût prévu</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Ajout de l’indicateur <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BillingRecord (BILL)

Un objet BillingRecord enregistre les revenus, les heures ou les dépenses qui peuvent être facturées. Ces informations peuvent être utilisées pour créer des factures dans un système comptable externe.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>montant</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>Ajouté(e)(s)</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

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
            <p><b>configurations</b>
            </p>
             <p>Ajouté(e)(s)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Entreprise (CMPY)

Un objet Company représente une organisation composée d’un ensemble de personnes.

L’objet Company a ajouté l’indicateur `SHARABLE`.

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
             <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (single assignmentschedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissue)</p></li>
            </ul>
          </li>
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
      <td>
           <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>taux</li>
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
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>realBillableExpenseCost</li>
              <li>realExpenseCost</li>
              <li>realFixedRevenue</li>
              <li>realLaborCost</li>
              <li>realLaborCostHours</li>
              <li>realLaborRevenue</li>
              <li>realNonBillableExpenseCost</li>
              <li>FixedCost</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coûtDépensePrévu</li>
              <li>revenuFixePrévu</li>
              <li>coût prévu de la main-d'œuvre</li>
              <li>planningHeuresCoûtMainD'Œuvre</li>
              <li>revenuMainD'œuvre prévu</li>
              <li>coûtDépenseNonFacturablePrévu</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceDépenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

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
            <p><b>devise</b>
            </p>
             <p>Ajouté(e)(s)</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>Ajouté(e)(s)</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask (OPTASK)

Un objet OpTask est généralement appelé un Problème. Un problème est un élément de travail qui indique généralement qu’un problème empêche la réalisation d’une tâche ou d’un projet. Il peut également s’agir d’une demande de centre d’assistance. Les ordres de modification, les requêtes et les bugs sont également des problèmes.

L&#39;objet OpTask a ajouté l&#39;indicateur DOMAIN_EXTENDABLE

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualCost</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
              <li>actualCost</li>
          </ul>
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
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (Recherche interne)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (Recherche interne à sélection multiple)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio (PORT)

Un objet Portfolio est un ensemble de projets qui rivalisent pour les mêmes ressources, généralement de l’argent ou des personnes pour les mener à bien.

L’objet Portfolio a ajouté l’indicateur `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>aligné</li>
              <li>budget</li>
              <li>currency</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>rsi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Programme (PRGM)

Un objet de programme est un sous-ensemble de projets d’un portfolio, où des projets similaires peuvent être regroupés.

L’objet Program a ajouté l’indicateur `DOMAIN_EXTENDABLE`.

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
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>realBenefits</li>
              <li>realBillableExpenseCost</li>
              <li>actualCost</li>
              <li>realExpenseCost</li>
              <li>realLaborCost</li>
              <li>realNonBillableExpenseCost</li>
              <li>revenu réel</li>
              <li>realRiskCost</li>
              <li>realValue</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>billingRevenue</li>
              <li>budget</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>eac</li>
              <li>FixedCost</li>
              <li>FixedRevenue</li>
              <li>PlannedBenefits</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coût prévu</li>
              <li>coûtDépensePrévu</li>
              <li>coût prévu de la main-d'œuvre</li>
              <li>coûtDépenseNonFacturablePrévu</li>
              <li>revenu prévu</li>
              <li>coûtRisquePrévu</li>
              <li>valeur planifiée</li>
              <li>remainingCost</li>
              <li>chiffre d’affaires restant</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>ressourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>revenu réel</li>
          <li>coût prévu</li>
          <li>revenu prévu</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Ajout de l’indicateur <code>CURRENCY</code></li>
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
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Supprimer des données personnalisées)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Ajout de sous-projets)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Taux (RATE)

Un objet Rate représente un taux de facturation dans Workfront.

L’objet Rate a ajouté l’indicateur `ATTRIBUTE_ATTACHABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>Les champs suivants ont été ajoutés :
          <ul>
          <li>currency</li>
          <li>verrouillé</li>
          <li>type</li>
          <li>value</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Rôle (ROLE)

Un objet Rôle (fonction) représente une capacité fonctionnelle ou un ensemble de compétences qu’un utilisateur ou une utilisateur peut remplir, tel que Designer ou Chef ou Cheffe de produits.

L&#39;objet Role a ajouté l&#39;indicateur `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
        <ul>
          <li>
          <p>Les champs suivants ont été ajoutés :
          <ul>
          <li>billingRates</li>
          <li>costRates</li>
          </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
             <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Un objet ScoreCardQuestion représente une question qui a été ajoutée à une carte de performance. Ces questions sont généralement définies par la personne gestionnaire du portfolio et leurs réponses lui permettent de comprendre dans quelle mesure un projet s’aligne sur les objectifs du portfolio.

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
             <p>Ajout des valeurs possibles suivantes :</p>
             <ul>
              <li><p><code>INTRNL</code> (Recherche interne)</p></li>
              <li><p><code>MULTINTRNL</code> (Recherche interne à sélection multiple)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tâche (TASK)

Un objet Task représente un élément de travail qui doit être exécuté comme une étape vers la réalisation d’un objectif final (achèvement d’un projet).

L’objet Task a ajouté l’indicateur `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>realBillableExpenseCost</li>
              <li>actualCost</li>
              <li>realExpenseCost</li>
              <li>realLaborCost</li>
              <li>realNonBillableExpenseCost</li>
              <li>revenu réel</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coût prévu/li&gt;
              <li>coûtDépensePrévu</li>
              <li>coût prévu de la main-d'œuvre</li>
              <li>coûtDépenseNonFacturablePrévu</li>
              <li>revenu prévu</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>revenu réel</li>
          <li>coût prévu</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Ajout des valeurs possibles suivantes :<ul><li><code>URH</code> (Utilisateur et rôle par heure)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Ajout des valeurs possibles suivantes :<ul><li><code>URH</code> (Utilisateur et rôle par heure)</li><li><code>URC</code> (Utilisateur et rôle par heure avec plafond)</li><li><code>URF</code> (Utilisateur et rôle par heure plus fixe)</li></ul></li>
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
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>budget</li>
              <li>FixedCost</li>
              <li>FixedRevenue</li>
              <li>PlannedBenefits</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coût prévu</li>
              <li>coûtDépensePrévu</li>
              <li>coût prévu de la main-d'œuvre</li>
              <li>coûtDépenseNonFacturablePrévu</li>
              <li>revenu prévu</li>
              <li>coûtRisquePrévu</li>
              <li>workRequired</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>coût prévu</li>
          <li>revenu prévu</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
          <p>Les champs suivants ont été ajoutés :</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateTask (TTSK)

Un objet TemplateTask représente une tâche qui fait partie d’un modèle. Les tâches de modèle deviennent des tâches dans le projet où le modèle est utilisé.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>billingAmount</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coût prévu/li&gt;
              <li>coûtDépensePrévu</li>
              <li>coût prévu de la main-d'œuvre</li>
              <li>coûtDépenseNonFacturablePrévu</li>
              <li>revenu prévu</li>
              <li>revenueType</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>coût prévu</li>
          <li>revenu prévu</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Ajout des valeurs possibles suivantes :<ul><li><code>URH</code> (Utilisateur et rôle par heure)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Ajout des valeurs possibles suivantes :<ul><li><code>URH</code> (Utilisateur et rôle par heure)</li><li><code>URC</code> (Utilisateur et rôle par heure avec plafond)</li><li><code>URF</code> (Utilisateur et rôle par heure plus fixe)</li></ul></li>
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
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>Supprimés</p>
          </li>
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
                <p><code>externalFolderMetadataError</code> (enum.updatetypeenum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Utilisateur ou utilisatrice (USER)

Un objet User représente une personne disposant d’un compte dans Workfront qui peut se connecter et interagir avec le système.

L’objet utilisateur a ajouté les champs `ATTRIBUTE_ATTACHABLE` et `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Champs directs</td>
      <td>
        <ul>
          <li>
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Champs de collection</td>
      <td>
          <p>Les champs suivants ont été ajoutés :</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
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
            <p>Les champs suivants ont ajouté l’indicateur <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>realBillableExpenseCost</li>
              <li>actualCost</li>
              <li>realExpenseCost</li>
              <li>realLaborCost</li>
              <li>realNonBillableExpenseCost</li>
              <li>revenu réel</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>coût prévu</li>
              <li>coûtDépensePrévu</li>
              <li>coût prévu de la main-d'œuvre</li>
              <li>coûtDépenseNonFacturablePrévu</li>
              <li>revenu prévu</li>
            </ul>
          </li>
          <li>
          <p>Le type des champs suivants a été modifié de <code>double</code> en <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>revenu réel</li>
          <li>coût prévu</li>
          <li>revenu prévu</li>
          </ul>
          </li>
          <li><p><b>durée planifiée</b></p> <p>Ajout des indicateurs <code>DYNAMIC</code>, <code>LAZY_READ</code> et <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Ajout de l’indicateur <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Ajout de la valeur possible <code>URH</code> (Utilisateur et rôle par heure) </li>
          <li><p><b>revenueType</b></p> <p>Ajout des valeurs possibles <code>URH</code> (Utilisateur et rôle par heure), <code>URC</code> (Utilisateur et rôle par heure avec plafond) et <code>URF</code> (Utilisateur et rôle par heure plus fixe)</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



