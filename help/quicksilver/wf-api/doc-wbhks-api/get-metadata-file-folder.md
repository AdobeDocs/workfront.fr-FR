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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 100%

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
   <th>Nom</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td>L’ID du fichier ou du dossier, tel qu’il est référencé par le fournisseur du webhook. Différent de l’ID de document Adobe Workfront. Pour obtenir les métadonnées du répertoire racine, utilisez la valeur « / ».
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
   <th>Nom</th> 
   <th>Type</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title</td> 
   <td>Chaîne</td> 
   <td>Nom du document ou du dossier</td> 
  </tr> 
  <tr> 
   <td>kind</td> 
   <td>Chaîne</td> 
   <td>Indique si cet élément est un fichier ou un dossier (« fichier » ou « dossier »).</td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td>Chaîne</td> 
   <td>ID du fichier ou du dossier.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Chaîne</td> 
   <td> <p>Chemin de l’URL utilisé par une personne pour visualiser le document dans une fenêtre de navigateur. L’URL peut être hébergée soit par le fournisseur de documents ou le fournisseur de stockage externe natif.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Chaîne</td> 
   <td> <p>Le chemin d’URL utilisé par une personne pour télécharger le document dans une fenêtre de navigateur. L’URL peut être hébergée soit par le fournisseur de documents ou le fournisseur de stockage externe natif.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Chaîne</td> 
   <td>Type MIME du fichier. (facultatif)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Chaîne</td> 
   <td>Dernière modification de ce fichier (date et heure au format RFC 3339)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Long</td> 
   <td>Taille du fichier en octets. (facultatif)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Booléen</td> 
   <td> Indique si ce fichier ou ce dossier est en lecture seule pour la personne authentifiée.(facultatif) </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"My Document",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z",<br>size: "32554694"<br>}</pre>

>[!NOTE]
>
>La gestion des erreurs doit être cohérente pour tous les appels API. Voir la section « Gestion des erreurs » ci-dessous pour plus de détails.
