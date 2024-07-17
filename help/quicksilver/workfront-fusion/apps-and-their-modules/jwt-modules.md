---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules JWT
description: L’application  [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] fournit un module qui crée des jetons JWT en fonction de l’algorithme fourni.
author: Becky
feature: Workfront Fusion
exl-id: 1c09967e-a236-404f-bf3e-9de66118e77b
source-git-commit: 2fbf38c3c35761c52416966fb6a4ab032190e04b
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 23%

---

# Module [!UICONTROL JWT]

L’application [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] fournit un module qui crée des jetons JWT en fonction de l’algorithme fourni.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <li><b>HS256</b> : HMAC à l’aide de l’algorithme de hachage SHA-256</li>
   <li><b>HS384</b> : HMAC à l’aide de l’algorithme de hachage SHA-384</li>
   <li><b>HS512</b> : HMAC à l’aide de l’algorithme de hachage SHA-512</li>
   <li><b>RS256</b> : RSASSA-PKCS1-v1_5 à l’aide de l’algorithme de hachage SHA-256</li>
   <li><b>RS384</b> : RSASSA-PKCS1-v1_5 à l’aide de l’algorithme de hachage SHA-384</li>
   <li><b>RS512</b> : RSASSA-PKCS1-v1_5 à l’aide de l’algorithme de hachage SHA-512</li>
   <li><b>PS256</b> : RSASSA-PSS à l’aide de l’algorithme de hachage SHA-256 (seul noeud ^6.12.0 OR &gt;=8.0.0)</li>
   <li><b>PS384</b> : RSASSA-PSS à l’aide de l’algorithme de hachage SHA-384 (seul noeud ^6.12.0 OR &gt;=8.0.0)</li>
   <li><b>PS512</b> : RSASSA-PSS à l’aide de l’algorithme de hachage SHA-512 (seul noeud ^6.12.0 OR &gt;=8.0.0)</li>
   <li><b>ES256</b> : ECDSA utilisant la courbe P-256 et l’algorithme de hachage SHA-256</li>
   <li><b>ES384</b> : ECDSA utilisant la courbe P-384 et l’algorithme de hachage SHA-384</li>
   <li><b>ES512</b> : ECDSA utilisant la courbe P-521 et l’algorithme de hachage SHA-512</li>
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
   <li><b>algorithme</b> : (par défaut : RS256)</li>
   <li><b>expiresIn</b> : exprimé en secondes ou chaîne décrivant une période (par exemple, 2 jours, 10h, 7d). Une valeur numérique est interprétée comme un nombre de secondes. Si vous utilisez une chaîne, veillez à indiquer les unités horaires (jours, heures, etc.), sinon l’unité de millisecondes est utilisée par défaut (120 équivaut à 120 ms).</li>
   <li><b>notBefore</b> : exprimé en secondes ou chaîne décrivant une période (par exemple, 2 jours, 10h, 7d). Une valeur numérique est interprétée comme un nombre de secondes. Si vous utilisez une chaîne, veillez à indiquer les unités horaires (jours, heures, etc.), sinon l’unité de millisecondes est utilisée par défaut (120 équivaut à 120 ms).
</li>
   <li><b>audience</b></li>
   <li><b>issuer</b></li>
   <li><b>jwtid</b></li>
   <li><b>subject</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>header</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b> : si <code>true</code>, la fonction sign modifie directement l’objet de la payload. Cela s’avère utile si vous avez besoin d’une référence brute à la payload une fois que des revendications lui ont été appliquées, mais avant qu’elle ne soit codée dans un jeton.</li>
   <li><b>allowInsecureKeySzes</b> : si <code>true</code>, autorise l’utilisation de clés privées avec un module inférieur à 2048 pour RSA.</li>
   <li><b>allowInvalidAsymetricKeyTypes</b> : si <code>true</code>, autorise des clés asymétriques qui ne correspondent pas à l’algorithme spécifié. Cette option est uniquement destinée à une compatibilité ascendante et doit être évitée.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>
