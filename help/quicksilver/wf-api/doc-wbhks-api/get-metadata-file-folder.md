---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtenir des métadonnées pour un fichier ou un dossier
description: Obtenir des métadonnées pour un fichier ou un dossier
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
TQID: https://experienceleague.adobe.com/H04UQeyhGw-FdXDwaRZs5PSXnN-YErVptHWn-78INYo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 90%

---

# Obtenir des métadonnées pour un fichier ou un dossier

Renvoie les métadonnées du fichier ou du dossier spécifié.

**URL**

GET /metadata?id=[ID de document ou de dossier]

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
   <td>ID</td> 
   <td>L’identifiant du fichier ou du dossier, tel que référencé par le fournisseur webhook. Ceci est différent de l’ID de document Adobe Workfront. Pour obtenir les métadonnées du répertoire racine, utilisez la valeur « / ».
   <p>Remarque : la longueur maximale de l’ID est de 255 caractères.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Réponse

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom </th> 
   <th>Type </th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Chaîne </td> 
   <td>Nom du document ou du dossier</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>Chaîne </td> 
   <td>Indique si cet élément est un fichier ou un dossier (« fichier » ou « dossier »).</td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td>Chaîne </td> 
   <td>ID du fichier ou du dossier.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Chaîne </td> 
   <td> <p>Chemin de l’URL utilisé par une personne pour visualiser le document dans une fenêtre de navigateur. L’URL peut être hébergée soit par le fournisseur de documents ou le fournisseur de stockage externe natif.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Chaîne </td> 
   <td> <p>Le chemin d’URL utilisé par une personne pour télécharger le document dans une fenêtre de navigateur. L’URL peut être hébergée soit par le fournisseur de documents ou le fournisseur de stockage externe natif.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Chaîne </td> 
   <td>Type MIME du fichier. (facultatif)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Chaîne </td> 
   <td>Dernière modification de ce fichier (date et heure au format RFC 3339)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Long</td> 
   <td> Taille du fichier en octets. (facultatif)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booléen</td> 
   <td> Indique si ce fichier ou dossier est en lecture seule pour l’utilisateur authentifié. (facultatif) </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"My Document",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z",<br>size: "32554694"<br>}</pre>

>[!NOTE]
>
>La gestion des erreurs doit être cohérente pour tous les appels API. Voir la section « Gestion des erreurs » ci-dessous pour plus de détails.
