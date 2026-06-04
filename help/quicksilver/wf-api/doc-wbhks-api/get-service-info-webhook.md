---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtenir des informations sur le service
description: Obtenir des informations sur le service
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
TQID: https://experienceleague.adobe.com/PIZ-dlAj-cj41-DJ9roBu1GXYsEOule5Jhgh6-jR6hc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 266
ht-degree: 100%

---

# Obtenir des informations sur le service (pas encore implémenté)

>[!NOTE]
>
>La date de publication de cette fonctionnalité n’a pas encore été déterminée.

Renvoie des informations sur le service, telles que ses caractéristiques et ses capacités. Adobe Workfront utilisera ces informations pour personnaliser l’interface utilisateur de Workfront. Par exemple, si la mise en œuvre du webhook contient des actions personnalisées, le fichier JSON doit énumérer ces opérations dans le fichier JSON. Les utilisateurs et utilisatrices pourront alors invoquer ces actions à partir de Workfront.

**URL**

GET /serviceInfo

## Paramètres de requête

Aucun. En outre, les appels à ce point d’entrée ne doivent pas nécessiter d’authentification.

## Réponse

Fichier JSON contenant des informations sur ce service.

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
   <td>Version du webhook mise en œuvre par ce service. Il s’agit du numéro de version indiqué au début de la présente spécification.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Chaîne </td> 
   <td>Numéro de version interne de ce service. Ce numéro est déterminé par le fournisseur du service du webhook et n’est utilisé qu’à titre d’information.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher </td> 
   <td>Chaîne </td> 
   <td>Nom de l’entreprise qui fournit l’implémentation du webhook.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Chaîne </td> 
   <td>Liste contenant les points d’entrée de l’API mis en œuvre par ce service. Ceci peut être utilisé pour s’assurer que l’interface d’utilisation dans Workfront reflète les capacités offertes par le fournisseur du webhook. Chaque élément de la liste doit inclure le nom du point d’entrée (tel que « search »).</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Chaîne</td> 
   <td>  <p>Liste contenant les opérations personnalisées implémentées par ce webhook. Chaque élément de la liste comprend un nom et un nom d’affichage. Le nom d’affichage apparaît dans le menu déroulant « Actions sur le document » dans Workfront. En cliquant sur l’élément de la liste déroulante, l’action est déclenchée en appelant le point d’entrée /customAction du webhook.</p></td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** `https://www.acme.com/api/serviceInfo`

returns

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
