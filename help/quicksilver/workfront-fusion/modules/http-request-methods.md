---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]
description: Lorsque vous configurez un appel API dans un module, vous devez renseigner le champ correspondant à la méthode de requête HTTP.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]

Lorsque vous configurez un appel API dans un module, vous devez renseigner le champ correspondant à la méthode de requête HTTP.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Méthodes HTTP

Utilisez l’une des méthodes HTTP suivantes.

* **[!UICONTROL GET]**: Récupère les données d’un serveur web en fonction de vos paramètres. [!UICONTROL GET] demande une représentation de la ressource spécifiée et reçoit une [!UICONTROL 200 OK] message de réponse avec le contenu demandé en cas de réussite.
* **[!UICONTROL POST]**: Envoie des données à un serveur web en fonction de vos paramètres. [!UICONTROL POST] les requêtes incluent des actions telles que le téléchargement d’un fichier. Multiple [!UICONTROL POST]s peut entraîner un résultat différent d’un seul [!UICONTROL POST], soyez donc prudent lorsque vous envoyez involontairement plusieurs [!UICONTROL POST]s. Si une [!UICONTROL POST] a réussi, vous recevez un événement [!UICONTROL 200 OK] message de réponse.
* **[!UICONTROL PUT]**: Envoie les données à un emplacement du serveur web en fonction de vos paramètres. [!UICONTROL PUT] les requêtes incluent des actions telles que le téléchargement d’un fichier. La différence entre un [!UICONTROL PUT] et [!UICONTROL POST] est que le PUT est idempotent, ce qui signifie que le résultat d’un seul succès [!UICONTROL PUT] est identique à plusieurs identiques [!UICONTROL PUT]s. Si un PUT réussit, vous recevez un message de réponse 200 (généralement 201 ou 204).
* **[!UICONTROL PATCH]**: (Non disponible pour certains modules d’appel API) Applique des modifications partielles à une ressource sur un serveur web en fonction de vos paramètres. [!UICONTROL PATCH] n’est pas idempotent, ce qui signifie que le résultat de plusieurs [!UICONTROL PATCH]Nous pourrions avoir des conséquences inattendues. Si une [!UICONTROL PATCH] est réussie, vous recevrez un message de réponse 200 (généralement 204).
* **[!UICONTROL DELETE]**: Supprime la ressource spécifiée du serveur web en fonction de vos paramètres (si la ressource existe). Si une [!UICONTROL DELETE] est réussie, vous recevez un message de réponse 200 OK.
