---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Méthodes de requête HTTP dans  [!DNL Adobe Workfront Fusion]
description: Lorsque vous configurez un appel API dans un module, vous devez renseigner le champ correspondant à la méthode de requête HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 28%

---

# Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]

Lorsque vous configurez un appel API dans un module, vous devez renseigner le champ correspondant à la méthode de requête HTTP.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## Méthodes HTTP

Utilisez l’une des méthodes HTTP suivantes.

* **[!UICONTROL GET]** : récupère des données d’un serveur web en fonction de vos paramètres. [!UICONTROL GET] demande une représentation de la ressource spécifiée et reçoit un message de réponse [!UICONTROL 200 OK] avec le contenu demandé en cas de réussite.
* **[!UICONTROL POST]** : envoie des données à un serveur web en fonction de vos paramètres. Les requêtes [!UICONTROL POST] incluent des actions telles que le téléchargement d’un fichier. Plusieurs [!UICONTROL POST] peuvent donner un résultat différent d&#39;un seul [!UICONTROL POST], soyez donc prudent lorsque vous envoyez involontairement plusieurs [!UICONTROL POST]. Si un [!UICONTROL POST] réussit, vous recevez un message de réponse [!UICONTROL 200 OK].
* **[!UICONTROL PUT]** : envoie des données vers un emplacement du serveur web en fonction de vos paramètres. Les requêtes [!UICONTROL PUT] incluent des actions telles que le téléchargement d’un fichier. La différence entre un [!UICONTROL PUT] et un [!UICONTROL POST] réside dans le fait que le PUT est idempotent, ce qui signifie que le résultat d’un seul [!UICONTROL PUT] réussi est le même que pour de nombreux [!UICONTROL PUT] identiques. Si un PUT réussit, vous recevez un message de réponse 200 (généralement 201 ou 204).
* **[!UICONTROL PATCH]** : (non disponible pour certains modules d’appel API) applique des modifications partielles à une ressource sur un serveur web en fonction de vos paramètres. [!UICONTROL PATCH] n’est pas idempotent, ce qui signifie que le résultat de plusieurs [!UICONTROL PATCH] peut avoir des conséquences imprévues. Si un [!UICONTROL PATCH] réussit, vous recevrez un message de réponse 200 (généralement 204).
* **[!UICONTROL DELETE]** : supprime la ressource spécifiée du serveur web en fonction de vos paramètres (si la ressource existe). Si un [!UICONTROL DELETE] réussit, vous recevez un message de réponse 200 OK.
