---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Exécution d’une action personnalisée
description: Exécution d’une action personnalisée
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 3%

---


# Exécution d’une action personnalisée (non encore implémentée)

Ce point de terminaison permet à un utilisateur Adobe Workfront (ou à un événement de workflow automatisé) d’effectuer une action dans le système externe. Le point d’entrée /customAction accepte un paramètre &quot;name&quot;, qui permet au fournisseur webhook d’implémenter plusieurs opérations personnalisées.

Le fournisseur de webhook enregistre des actions personnalisées avec Workfront en incluant les actions dans la réponse /serviceInfo sous customActions. Workfront charge cette liste lors de la configuration ou de l’actualisation du fournisseur webhook sous Configuration > Documents > Intégrations personnalisées.

Les utilisateurs peuvent déclencher l’action personnalisée en sélectionnant la section située sous &quot;Actions de document&quot;.

**URL**

GET /customAction

## Paramètres de requête

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>name</p> </td> 
   <td> <p>Identifiant spécifiant le type d’action à effectuer. Cette valeur correspond à l’une des valeurs customAction répertoriées par le point d’entrée /serviceInfo .</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>Identifiant du document de travail pour lequel l’action est en cours d’exécution.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> Identifiant de version de document du plan de travail pour lequel l’action est effectuée.</td> 
  </tr> 
 </tbody> 
</table>

 

## réponse

Chaîne JSON indiquant la réussite ou l’échec, comme indiqué dans la section Gestion des erreurs ci-dessous. En cas d’échec (c.-à-d. status = &quot;failure&quot;), Workfront affiche le message d’erreur fourni à l’utilisateur.

**Exemple:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

response

```
{
status: "success"
}
```
