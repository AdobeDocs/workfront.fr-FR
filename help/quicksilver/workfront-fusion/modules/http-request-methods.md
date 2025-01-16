---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Méthodes de requête HTTP dans  [!DNL Adobe Workfront Fusion]
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 83%

---

# Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Méthodes de requête HTTP](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/http-request-methods.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Lorsque vous configurez un appel API dans un module, vous devez remplir le champ de la méthode de requête HTTP.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Méthodes HTTP

Utilisez l’une des méthodes HTTP suivantes.

* **[!UICONTROL GET]** : récupère les données d’un serveur web en fonction de vos paramètres. [!UICONTROL GET] demande une représentation de la ressource spécifiée et reçoit un message de réponse [!UICONTROL 200 OK] avec le contenu demandé en cas de succès.
* **[!UICONTROL POST]** : envoie des données à un serveur web en fonction de vos paramètres. Les requêtes [!UICONTROL POST] comprennent des actions telles que le chargement d’un fichier. L’envoi de plusieurs requêtes [!UICONTROL POST] peut avoir un résultat différent de celui d’une seule requête [!UICONTROL POST], il convient donc de faire preuve de prudence et de ne pas envoyer involontairement plusieurs requêtes [!UICONTROL POST]. Si une requête [!UICONTROL POST] réussit, vous recevez un message de réponse [!UICONTROL 200 OK].
* **[!UICONTROL PUT]** : envoie des données à un emplacement du serveur web en fonction de vos paramètres. Les requêtes [!UICONTROL PUT] comprennent des actions telles que le chargement d’un fichier. La différence entre [!UICONTROL PUT] et [!UICONTROL POST] est que PUT est idempotent, ce qui signifie que le résultat d’une seule requête [!UICONTROL PUT] réussie est le même que celui de plusieurs requêtes [!UICONTROL PUT] identiques. Si une requête PUT réussit, vous recevez un message de réponse 200 (généralement 201 ou 204).
* **[!UICONTROL PATCH]** : (non disponible pour certains modules d’appel API) applique des modifications partielles à une ressource sur un serveur web en fonction de vos paramètres. [!UICONTROL PATCH] n’est pas idempotent, ce qui signifie que le résultat de plusieurs requêtes [!UICONTROL PATCH] pourrait avoir des conséquences inattendues. Si une requête [!UICONTROL PATCH] réussit, vous recevrez un message de réponse 200 (généralement 204).
* **[!UICONTROL DELETE]** : supprime la ressource spécifiée du serveur web en fonction de vos paramètres (si la ressource existe). Si une requête [!UICONTROL DELETE] réussit, vous recevez un message de réponse 200 OK.
