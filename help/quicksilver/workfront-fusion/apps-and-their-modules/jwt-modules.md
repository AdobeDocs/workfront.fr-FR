---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules JWT
description: La variable [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] L’application fournit un module qui crée des jetons JWT en fonction de l’algorithme fourni.
author: Becky
feature: Workfront Fusion
source-git-commit: 121aef2ee55597fee2e2adc8250dd0651ea86f17
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# [!UICONTROL JWT] module

La variable [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] L’application fournit un module qui crée des jetons JWT en fonction de l’algorithme fourni.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Exigences de licence actuelles : non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail, [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de l’[!UICONTROL Select] ou de l’[!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Module JWT et ses champs

### Génération de JWT

Ce module génère un jeton JWT en fonction de l’algorithme sélectionné.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algorithme]</td> 
   <td> <p>Sélectionnez l’algorithme avec lequel vous souhaitez générer le JWT.</p> <ul>
   <li><b>HS256</b>: HMAC utilisant l’algorithme de hachage SHA-256</li>
   <li><b>HS384</b>: HMAC utilisant l’algorithme de hachage SHA-384</li>
   <li><b>HS512</b>: HMAC utilisant l’algorithme de hachage SHA-512</li>
   <li><b>RS256</b>: RSASSA-PKCS1-v1_5 utilisant l’algorithme de hachage SHA-256</li>
   <li><b>RS384</b>: RSASSA-PKCS1-v1_5 utilisant l’algorithme de hachage SHA-384</li>
   <li><b>RS512</b>: RSASSA-PKCS1-v1_5 utilisant l’algorithme de hachage SHA-512</li>
   <li><b>PS256</b>: RSASSA-PSS utilisant l’algorithme de hachage SHA-256 (seul noeud ^6.12.0 OU &gt;=8.0.0)</li>
   <li><b>PS384</b>: RSASSA-PSS utilisant l’algorithme de hachage SHA-384 (seul noeud ^6.12.0 OU &gt;=8.0.0)</li>
   <li><b>PS512</b>: RSASSA-PSS utilisant l’algorithme de hachage SHA-512 (seul noeud ^6.12.0 OU &gt;=8.0.0)</li>
   <li><b>ES256</b>: ECDSA utilisant la courbe P-256 et l’algorithme de hachage SHA-256</li>
   <li><b>ES384</b>: ECDSA utilisant la courbe P-384 et l’algorithme de hachage SHA-384</li>
   <li><b>ES512</b>: ECDSA utilisant la courbe P-521 et l’algorithme de hachage SHA-512</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload] </td> 
   <td> <p>Pour chaque élément de charge utile à ajouter, cliquez sur <b>Ajouter un élément</b> et saisissez la clé et la valeur de l’élément.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Options] </td> 
   <td> <p>Pour chaque élément d’option à ajouter, cliquez sur <b>Ajouter un élément</b> et saisissez la clé et la valeur de l’élément.</p> <p>Les clés disponibles sont les suivantes :
   <ul>
   <li><b>algorithme</b>: (par défaut : RS256)</li>
   <li><b>expiresIn</b>: exprimé en secondes ou chaîne décrivant une période (par exemple, 2 jours, 10h, 7j). Une valeur numérique est interprétée comme un nombre de secondes. Si vous utilisez une chaîne, veillez à indiquer les unités horaires (jours, heures, etc.), sinon l’unité de millisecondes est utilisée par défaut (120 équivaut à 120 ms).</li>
   <li><b>notBefore</b>: exprimé en secondes ou chaîne décrivant une période (par exemple, 2 jours, 10h, 7j). Une valeur numérique est interprétée comme un nombre de secondes. Si vous utilisez une chaîne, veillez à indiquer les unités horaires (jours, heures, etc.), sinon l’unité de millisecondes est utilisée par défaut (120 équivaut à 120 ms).
</li>
   <li><b>audience</b></li>
   <li><b>issuer</b></li>
   <li><b>jwtid</b></li>
   <li><b>subject</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>header</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>: Si <code>true</code>, la fonction sign modifie directement l’objet de charge utile. Cela s’avère utile si vous avez besoin d’une référence brute à la payload une fois que des revendications lui ont été appliquées, mais avant qu’elle ne soit codée dans un jeton.</li>
   <li><b>allowInsecureKeySzes</b>: Si <code>true</code>, permet l’utilisation de clés privées avec un module inférieur à 2048 pour RSA.</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>: Si <code>true</code>, autorise les clés asymétriques qui ne correspondent pas à l’algorithme spécifié. Cette option est uniquement destinée à une compatibilité ascendante et doit être évitée.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>


