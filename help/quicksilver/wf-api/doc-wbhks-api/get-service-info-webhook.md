---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtention d’informations sur le service
description: Obtention d’informations sur le service
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 4%

---


# Obtention d’informations sur le service (pas encore mis en oeuvre)

>[!NOTE]
>
>La date de publication de cette fonctionnalité n’a pas encore été fixée.

Renvoie des informations sur le service, telles que les fonctionnalités. Adobe Workfront utilisera ces informations pour personnaliser l’interface utilisateur dans Workfront. Par exemple, si l’implémentation du webhook contient des actions personnalisées, le fichier JSON doit répertorier ces opérations dans le fichier JSON. Les utilisateurs pourront alors appeler ces actions à partir de Workfront.

**URL**

GET /serviceInfo

## Paramètres de requête

Aucun. En outre, les appels à ce point de terminaison ne doivent pas nécessiter d’authentification.

## réponse

JSON contenant des informations sur ce service

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom</th> 
   <th>Type </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>Chaîne </td> 
   <td>Version du webhook implémentée par ce service. Il s’agit du numéro de version répertorié en haut de cette spécification.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Chaîne </td> 
   <td>Numéro de version interne de ce service. Ce nombre est déterminé par le fournisseur de services webhook et utilisé à des fins d’information uniquement.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher </td> 
   <td>Chaîne </td> 
   <td>Nom de la société qui fournit l’implémentation du webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Chaîne </td> 
   <td>Liste contenant les points de terminaison de l’API implémentés par ce service. Cela peut être utilisé pour s’assurer que l’interface utilisateur de Workfront reflète les fonctionnalités offertes par le fournisseur webhook. Chaque élément de la liste doit inclure le nom du point de terminaison (par exemple, "recherche").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Chaîne</td> 
   <td>  <p>Liste contenant les opérations personnalisées implémentées par ce webhook. Chaque élément de liste comprend un nom et un nom d’affichage. Le nom d’affichage s’affiche dans la liste déroulante "Actions de document" dans Workfront. Cliquez sur l’élément dans la liste déroulante pour appeler l’action dans le webhook en appelant le point de terminaison /customAction .</p></td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** `https://www.acme.com/api/serviceInfo`

renvoie

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
