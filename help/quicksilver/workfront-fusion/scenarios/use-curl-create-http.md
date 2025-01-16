---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Utiliser cURL pour ajouter un module HTTP
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 17%

---

# Utiliser cURL pour ajouter un module HTTP

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Utilisez cURL pour ajouter un module HTTP](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/use-curl-create-http.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Vous pouvez coller une requête cURL dans votre scénario, puis Fusion crée un module HTTP configuré à partir de la requête cURL.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Formule Adobe Workfront</td>  
      <td>Tous</td>  
    </tr>  
    <tr>  
      <td>Licence Adobe Workfront</td>  
      <td>
        Nouveau : Standard<br>
        Ou <br>
        En cours : Travail ou version ultérieure
      </td>  
    </tr>  
    <tr>  
      <td>Licence Adobe Workfront Fusion</td>  
      <td> 
        Actuel : aucune exigence de licence Workfront Fusion.<br>
        Ou <br>
        Hérité : Tous
      </td>  
    </tr>  
    <tr>  
      <td>Produit</td>  
      <td> 
        Nouveau : sélectionnez ou Prime Workfront Plan : votre entreprise doit acheter Adobe Workfront Fusion.<br>
        Plan Ultimate Workfront : Workfront Fusion est inclus.<br>
        Ou <br>
        Actuel : votre entreprise doit acheter Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Création d’un module HTTP à partir d’une requête cURL


Pour créer un module HTTP à l’aide de cURL :

1. Créez le texte de la requête cURL en dehors de Fusion, par exemple dans un éditeur de texte.
1. Copiez la requête cURL dans le presse-papiers.
1. Cliquez sur l’onglet **[!UICONTROL Scénario]** dans le panneau de gauche.
1. Sélectionnez le scénario dans lequel vous souhaitez créer le module.
1. Cliquez n’importe où sur le scénario pour accéder à l’éditeur de scénarios.
1. Cliquez avec le bouton droit sur un espace blanc dans l’éditeur de scénarios et sélectionnez **Coller**.

   Ou

   Appuyez sur Ctrl + V (Windows) ou Cmd + V (Mac).


   Un module HTML est créé.
1. Faites glisser le module pour le connecter à votre scénario.

## Dépannage

Si votre cURL n’est pas collée dans votre scénario, vérifiez les paramètres de votre navigateur pour vous assurer que le collage à partir du presse-papiers est activé.


