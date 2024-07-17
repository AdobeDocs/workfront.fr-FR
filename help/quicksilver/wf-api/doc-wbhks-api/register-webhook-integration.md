---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Enregistrer une intégration de webhook
description: Enregistrer une intégration de webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 14%

---


# Enregistrer une intégration de webhook

Les administrateurs Adobe Workfront peuvent ajouter une intégration webhook personnalisée pour leur entreprise en accédant à Configuration > Documents > Intégrations personnalisées dans Workfront. Sur la page Intégration personnalisée de Configuration, les administrateurs peuvent afficher une liste des intégrations Webhook de document existantes. Depuis cette page, les intégrations peuvent être ajoutées, modifiées, activées et désactivées.

Pour ajouter une intégration, cliquez sur **Ajouter une intégration personnalisée**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## Champs disponibles

Lors de l’ajout d’une intégration, l’administrateur saisit les valeurs des champs suivants.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nom de champ</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nom</td> 
   <td>Nom de cette intégration.</td> 
  </tr> 
  <tr> 
   <td>URL API de base</td> 
   <td> <p>Emplacement de l’API de rappel. Lors d’appels au système externe, Workfront ajoute simplement le nom du point de terminaison à cette adresse. Par exemple, si l’administrateur a saisi l’URL de l’API de base " https://www.mycompany.com/api/v1", Workfront utilise l’URL suivante pour obtenir les métadonnées d’un document : https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Paramètres de requête</td> 
   <td> <p>Les valeurs optionnelles à ajouter à la chaîne de requête de chaque appel API. Par exemple, access_type </p> </td> 
  </tr> 
  <tr> 
   <td>Type d'authentification</td> 
   <td>OAuth2 ou ApiKey</td> 
  </tr> 
  <tr> 
   <td>URL d'authentification</td> 
   <td> <p>(OAuth2 uniquement) URL complète utilisée pour l’authentification de l’utilisateur. Workfront accède aux utilisateurs à cette adresse dans le cadre du processus d’approvisionnement OAuth. Remarque : Workfront ajoute un paramètre "state" à la chaîne de requête. Le fournisseur doit transmettre cette information à Workfront en l’ajoutant à l’URI de redirection Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>URL de jeton de point d’entrée</td> 
   <td> <p>(OAuth2 uniquement) URL complète de l’API utilisée pour récupérer les jetons OAuth2. Il est hébergé par le fournisseur webhook ou le fournisseur de document externe</p> </td> 
  </tr> 
  <tr> 
   <td>ID client</td> 
   <td>(OAuth2 uniquement) ID client OAuth2 pour cette intégration</td> 
  </tr> 
  <tr> 
   <td>Clé secrète client</td> 
   <td> <p>(OAuth2 uniquement) Secret client OAuth2 pour cette intégration</p> </td> 
  </tr> 
  <tr> 
   <td>URI de redirection Workfront</td> 
   <td>(OAuth2 uniquement) Il s’agit d’un champ en lecture seule généré par Workfront. Cette valeur est utilisée pour enregistrer cette intégration auprès du fournisseur de documents externe. Remarque : Comme décrit ci-dessus pour l’URL d’authentification, le fournisseur doit ajouter le paramètre "state" et sa valeur à la chaîne de requête lors de l’exécution de la redirection.</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>(ApiKey uniquement) Utilisé pour effectuer des appels API autorisés au fournisseur webhook. Clé API émise par le fournisseur webhook.</p> </td> 
  </tr> 
 </tbody> 
</table>
