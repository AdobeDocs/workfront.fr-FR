---
content-type: api
navigation-topic: general-api
title: Contrôle de version de l’abonnement aux événements
description: API d’abonnement aux événements
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: 0b8c327f5ab541358649474b405b881dac06c1aa
workflow-type: tm+mt
source-wordcount: '1124'
ht-degree: 2%

---

# Contrôle de version de l’abonnement aux événements

Workfront propose deux versions d’abonnements aux événements. Cet article décrit les différences entre eux.

La nouvelle version ne constitue pas une modification de l’API Workfront, mais plutôt une modification de la fonctionnalité d’abonnement aux événements.

La possibilité de mettre à niveau ou de rétrograder des abonnements aux événements garantit que lorsque des modifications sont apportées à la structure des événements, les abonnements existants ne sont pas rompus, ce qui vous permet de tester et de mettre à niveau vers la nouvelle version sans interruption de votre abonnement aux événements.

Pour plus d’informations sur les points d’entrée utilisés pour mettre à niveau ou rétrograder des abonnements aux événements, consultez [Contrôle de version des abonnements aux événements](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) dans l’article API d’abonnement aux événements.

>[!IMPORTANT]
>
>Les versions suivantes affecteront le contrôle de version des abonnements aux événements :
>
>* **Version 25.2** (10 avril 2025) : tous les nouveaux abonnements créés après la version 25.2 sont créés en tant que version 2.
>* Version **25.3** (17 juillet 2025) : les abonnements ne peuvent plus être rétrogradés à la version 1 après la version 25.3.

## Modifications entre les versions 1 et 2

Les modifications suivantes ont été apportées aux abonnements aux événements version 2


### Modifications générales


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>Champs concernés</b></p> </th> 
   <th> <p><b>Version 1 (comportement précédent)</b></p> </th> 
   <th> <p><b>Version 2 (Modifier)</b></p> </th> 
   <th> <p><b>Action corrective</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Valeurs de paramètre</p> </td> 
   <td> <p>Pour tout objet créé à partir d’un modèle qui incluait un formulaire personnalisé, un événement <code>CREATE</code> a été envoyé, puis un <code>UPDATE</code> a été envoyé avec les valeurs de paramètre (y compris les champs calculés et leurs valeurs).    </p> </td> 
   <td> <p>Seul un événement <code>CREATE</code> est envoyé, qui contient les valeurs de paramètre, y compris les champs calculés.</p> </td> 
   <td> <p>Si vous disposez d’un filtre sur les événements de <code>UPDATE</code> avec des valeurs de paramètre (y compris les champs personnalisés calculés) et que vous prévoyez de le recevoir après un événement de <code>CREATE</code> d’objet qui inclut des valeurs de paramètre, vous ne recevez plus cet événement de <code>UPDATE</code>. Si vous souhaitez voir les valeurs de paramètre lors de la création d’objet, vous devez créer un abonnement <code>CREATE</code> supplémentaire.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Champs de type Sélection multiple</p> </td> 
   <td> <p>Pour tout type d’événement contenant une modification sur un champ de type à sélection multiple, si le champ ne contenait qu’une seule valeur, il était converti en et envoyé sous la forme d’une chaîne. Sinon, elle serait envoyée sous la forme d’un tableau. </p><p>Exemples :</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> est converti et envoyé en tant que <code>myMultiSelectField: "oneValue"</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> est envoyé en tant que <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Quel que soit le nombre de valeurs dans le tableau, il sera envoyé en tant que tableau. </p><p>Exemples :</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> est envoyé en tant que <code>myMultiSelectField: ["oneValue"]</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> est envoyé en tant que <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Si vous disposez d’un abonnement avec un filtre sur un champ à sélection multiple et la valeur sous la forme d’une chaîne, vous devez créer un abonnement avec le même filtre qui possède la valeur sous la forme d’un tableau. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Modifications spécifiques à l’objet

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>Code objet</b> </th> 
   <th> <b>Champs concernés</b> </th> 
   <th> <b>Version 1 (Comportement précédent)</b></th> 
   <th> <b>Version 2 (Modifier)</b> </th> 
   <th> <b>Action corrective</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>Lorsque cet objet a été mis à jour, l’événement <code>UPDATE</code> a parfois indiqué de manière incorrecte que les champs affectés passaient de <code>null</code> à <code>ID value</code>.</td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour les champs concernés.</td> 
   <td>Aucun. Si vous disposez d’un filtre sur les champs concernés, vous ne recevez un événement <code>UPDATE</code> que si ces champs ont réellement changé, et non si une autre valeur a été modifiée.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>Lorsqu’une valeur de paramètre a été mise à jour sur cet objet, l’événement <code>UPDATE</code> a incorrectement affiché le changement de champ affecté de <code>null</code> à <code>object id</code>. </td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour les champs concernés.</td> 
   <td>Aucun. Si vous disposez d’un filtre sur les champs concernés, vous ne recevez un événement <code>UPDATE</code> que si ces champs ont réellement changé, et non si une autre valeur a été modifiée.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>Lorsqu’un document a été supprimé, l’événement <code>DELETE</code> affichait incorrectement le champ affecté sous la forme d’un tableau vide à l’état « before ».    </td> 
   <td>L’événement <code>DELETE</code> affiche correctement le champ affecté à l’état « before ».</td> 
   <td>Aucun. L’événement <code>DELETE</code> sera toujours envoyé, mais affichez désormais les données correctes pour le champ affecté. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>Lorsque cet objet a été mis à jour, deux événements <code>UPDATE</code> ont été envoyés. Le premier événement n’incluait pas les champs concernés, alors que le second l’a fait.</td> 
   <td>Toutes les mises à jour des champs, y compris les champs concernés, sont présentes dans un seul événement <code>UPDATE</code> et aucun second événement inutile n’est envoyé.     </td> 
   <td>Aucun. Si les champs concernés appliquent un filtre, les événements sont diffusés dans le premier événement. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">EXPNS</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Lorsqu'une valeur de paramètre a été mise à jour sur une dépense, l'événement <code>UPDATE</code> affichait incorrectement topReferenceObjCode modifié de <code>EXPNS</code> en <code>PROJ</code>, et <code>referenceObjectName</code> modifié de <code>null</code> en <code>string value of project name</code>.      </td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour les champs concernés.</td> 
   <td>Aucun. Si vous disposez d’un filtre sur les champs concernés, vous ne recevez un événement <code>UPDATE</code> que si ces champs ont réellement changé, et non si une autre valeur a été modifiée.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Lorsqu'un objet Expense a été supprimé, un événement de <code>UPDATE</code> a été envoyé, modifiant les champs concernés en les rendant nuls avant l'envoi de l'événement de <code>DELETE</code>.    </td> 
   <td>L’événement <code>UPDATE</code> supplémentaire n’est pas envoyé. L’événement <code>DELETE</code> contient des valeurs correctes pour les champs concernés à l’état « avant ». </td> 
   <td>Si vous disposez d’un filtre pour les champs concernés par les événements <code>UPDATE</code> et que vous prévoyez de le recevoir lorsque l’objet est supprimé, vous ne recevez plus cet événement <code>UPDATE</code>. Si vous souhaitez afficher ces champs lors de la suppression de l’objet , vous devez créer un abonnement <code>DELETE</code> supplémentaire.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">HOUR</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>Lorsque cet objet a été supprimé, l’événement <code>DELETE</code> affichait incorrectement les champs affectés tels qu’<code>null</code> dans l’état « before ». </td> 
   <td>L’événement <code>DELETE</code> affiche correctement les champs concernés à l’état « before ».</td> 
   <td>Aucun. L’événement <code>DELETE</code> est toujours envoyé, mais affiche désormais les données correctes pour les champs concernés. </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Lorsqu’une valeur de paramètre a été mise à jour sur cet objet, l’événement <code>UPDATE</code> a incorrectement affiché le changement de champ affecté de <code>null</code> à <code>ID value</code>. </td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour le champ concerné.</td> 
   <td>Aucun. Si vous disposez d’un filtre sur le champ affecté, vous ne recevez un événement <code>UPDATE</code> que si ce champ a réellement changé, et non si une autre valeur de paramètre a changé.
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>Lorsque cet objet a été mis à jour, l’événement <code>UPDATE</code> a parfois indiqué de manière incorrecte que les champs affectés passaient de <code>null</code> à <code>ID value</code>.</td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour les champs concernés.    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>Lorsqu’une valeur de paramètre a été mise à jour sur cet objet, l’événement <code>UPDATE</code> a incorrectement affiché le changement de champ affecté de <code>null</code> à <code>ID value</code>. </td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour le champ concerné.</td> 
   <td>Aucun. Si vous disposez d’un filtre sur le champ affecté, vous ne recevez un événement <code>UPDATE</code> que si ce champ a réellement changé, et non si une autre valeur de paramètre a changé.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Lorsque cet objet a été mis à jour, l’événement <code>UPDATE</code> a parfois indiqué de manière incorrecte que les champs affectés passaient de <code>null</code> à <code>ID value</code>.</td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour le champ concerné.</td> 
   <td>Aucun. Si vous disposez d’un filtre sur le champ affecté, vous ne recevez un événement <code>UPDATE</code> que si ce champ a réellement changé, et non si une autre valeur de paramètre a changé.
  </tr> 
  <tr> 
   <th rowspan="2">TASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Lorsqu’une valeur de paramètre a été mise à jour sur cet objet, l’événement <code>UPDATE</code> a incorrectement affiché le changement de champ affecté de <code>null</code> à <code>ID value</code>. </td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour le champ concerné.</td> 
   <td>Aucun. Si vous disposez d’un filtre sur le champ affecté, vous ne recevez un événement <code>UPDATE</code> que si ce champ a réellement changé, et non si une autre valeur de paramètre a changé.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Lorsque cet objet a été mis à jour, l’événement <code>UPDATE</code> a parfois indiqué de manière incorrecte que les champs affectés passaient de <code>null</code> à <code>ID value</code>.</td> 
   <td>Tous les événements <code>UPDATE</code> affichent la valeur correcte pour le champ concerné.</td> 
   <td>Aucun. Si vous disposez d’un filtre sur le champ affecté, vous ne recevez un événement <code>UPDATE</code> que si ce champ a réellement changé, et non si une autre valeur de paramètre a changé.
 </tbody> 
</table>
