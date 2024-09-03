---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Effectuer une action personnalisée
description: Effectuer une action personnalisée
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 100%

---


# Exécuter une action personnalisée (pas encore implémentée)

Ce point d’entrée permet à un utilisateur ou une utilisatrice Adobe Workfront (ou à un événement de workflow automatisé) d’effectuer une action dans le système externe. Le point d’entrée /customAction accepte un paramètre « nom », qui permet au fournisseur du webhook de mettre en œuvre plusieurs opérations personnalisées.

Le fournisseur du webhook enregistre les actions personnalisées avec Workfront en incluant les actions dans la réponse /serviceInfo dans customActions. Workfront charge cette liste lors de la configuration ou de l’actualisation du fournisseur du webhook dans Configuration > Documents > Intégrations personnalisées.

Les utilisateurs et utilisatrices peuvent déclencher l’action personnalisée en sélectionnant la section dans « Actions sur le document ».

**URL**

GET /customAction

## Paramètres de requête

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>name</p> </td> 
   <td> <p>Identifiant spécifiant le type d’action à effectuer. Cette valeur correspond à l’une des valeurs customAction répertoriées par le point d’entrée /serviceInfo.</p> </td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td>Identifiant du document Workfront pour lequel l’action est effectuée.</td> 
  </tr> 
  <tr> 
   <td>documentVersionId</td> 
   <td>Identifiant de la version du document Workfront pour lequel l’action est effectuée.</td> 
  </tr> 
 </tbody> 
</table>

 

## Réponse

Chaîne JSON indiquant le succès ou l’échec, tel que spécifié dans la section Gestion des erreurs ci-dessous. En cas d’échec (c’est-à-dire si le statut = «échec »), Workfront affichera le message d’erreur envoyé à l’utilisateur ou l’utilisatrice.

**Exemple :**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

response

```
{
status: "success"
}
```
