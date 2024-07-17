---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Obtenir des jetons OAuth2
description: Obtenir des jetons OAuth2
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 7%

---


# Obtenir des jetons OAuth2

## Obtention de jetons OAuth2

Renvoie le jeton d’actualisation OAuth2 et le jeton d’accès pour un utilisateur authentifié. Il est appelé une fois lorsque l’utilisateur a configuré un fournisseur de documents. Les appels suivants sont effectués pour obtenir un jeton d’accès mis à jour.

**URL**

POST /any/url

L’URL est configurable et correspond à la valeur de l’URL Point d’entrée du jeton sur la page de configuration de l’intégration personnalisée.

### Paramètres de requête

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Nom</th>
   <th>Requis</th>
   <th>Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>oui</td>
   <td><p>Les valeurs comprennent "authorization_code" ou "refresh_token". La valeur spécifiée indique lequel des deux paramètres sera transmis à cet appel API : code ou refresh_token.</p></td>
  </tr>
  <tr>
   <td>code</td>
   <td>dépend</td>
   <td><p>Code d’autorisation envoyé à Adobe Workfront juste après que l’utilisateur a cliqué sur le bouton "Accorder". Cela n’est nécessaire que lorsque le type d’octroi est "authorization_code". Le code d’autorisation doit être de courte durée, expirant généralement en 10 minutes ou moins.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>dépend</td>
   <td><p>Cela n’est nécessaire que lors d’appels ultérieurs pour récupérer un nouveau jeton d’accès, étant donné que le jeton d’accès précédent a expiré. Lors de l’envoi de cette valeur, définissez le paramètre grant_type sur "refresh_token".</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>oui</td>
   <td>Identifiant du client configuré dans Workfront pour cette intégration personnalisée.</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>oui</td>
   <td> Secret client configuré dans Workfront pour cette intégration personnalisée.</td>
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
   <th>Type </th>
   <th>Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>Chaîne</td>
   <td><p>Jeton utilisé pour effectuer des appels API autorisés pour le compte de l’utilisateur. Cet délai doit expirer pour empêcher les appels d’API non autorisés.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>Chaîne</td>
   <td><p>Jeton de longue durée utilisé pour récupérer un nouveau jeton d’accès en appelant cette méthode d’API.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>long</td>
   <td><p>(facultatif) La durée (en secondes) précédant l’expiration de access_token, généralement 3 600.</p></td>
  </tr>
 </tbody>
</table>

**Exemple**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## Réponse

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
