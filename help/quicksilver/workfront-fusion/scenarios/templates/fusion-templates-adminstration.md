---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administration des modèles Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 8163f9f12bb27bbc8adfde34fc1e1f0f8c8be7f9
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 88%

---

# Administration des modèles [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans les articles suivants :
>
>* [Approuver ou refuser des modèles pour l&#39;onglet Public](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/approve-templates.html)
>* [Modifier les modèles](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/manage-templates-admin/edit-templates.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Si vous êtes administrateur ou administratrice, vous avez l’autorisation d’afficher, de modifier, de renommer, de publier, d’approuver et de supprimer les modèles créés par d’autres personnes. Vous pouvez effectuer ces actions à partir de la page [!UICONTROL Modèles] dans la zone [!DNL Adobe Workfront Fusion Administration].

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigence de produit hérité : votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez être administrateur ou administratrice Workfront Fusion pour votre entreprise.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Afficher les modèles [!DNL Workfront Fusion] en tant qu’administrateur ou administratrice [!DNL Workfront Fusion]

Pour afficher un tableau de tous les modèles créés et de leur statut :

1. Cliquez sur **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir la zone [!UICONTROL Administration].

   >[!NOTE]
   >
   >La zone Administration n’est visible que par les administrateurs et administratrices de Workfront Fusion.

1. Cliquez sur **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.

Trois colonnes sont liées au statut de publication des modèles. Une coche dans une colonne indique les éléments suivants :

* **[!UICONTROL Publié]** : ces modèles sont actuellement visibles dans l’onglet [!UICONTROL Modèles d’équipe] dans l’interface utilisateur.
* **[!UICONTROL Approbation demandée]** : ces modèles attendent votre approbation. Ils sont actuellement visibles dans l’onglet [!UICONTROL Modèles d’équipe] dans l’interface utilisateur.
* **[!UICONTROL Approuvé]** : ces modèles ont été approuvés. Ils sont actuellement visibles dans l’onglet [!UICONTROL Modèles publics] dans l’interface utilisateur standard.

>[!NOTE]
>
>Les modèles avec des coches dans la colonne [!UICONTROL Approbation demandée] et dans la colonne [!UICONTROL Approuvé] ont déjà été approuvés et rendus publics, mais une version plus récente attend votre approbation.

## Modifier les modèles [!DNL Workfront Fusion] en tant qu’administrateur et administratrice

1. Cliquez sur **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir la zone [!UICONTROL Administration].
1. Cliquez sur **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.
1. Cliquez sur **[!UICONTROL Détail]** à droite du modèle à modifier.

Vous pouvez désormais modifier le modèle, comme vous le faites pour modifier un modèle en tant qu’utilisateur ou utilisatrice hors administration. Toutefois, dans les [!UICONTROL Options] dans le coin supérieur droit, il existe une option supplémentaire : le diagramme SVG qui vous fournit le code SVG. En outre, le processus de publication est le même que pour un utilisateur ou une utilisatrice standard. Pour plus d’informations, reportez-vous à la section Publication et partage de modèles.

Pour plus d’informations sur les options de modèle spécifiques que vous pouvez modifier, voir [Créer des modèles dans  [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Pour plus d’informations sur la publication de modèles, voir [Publier et partager des modèles  [!DNL Adobe Workfront Fusion] ](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Approuver ou refuser des modèles [!DNL Workfront Fusion]

L’approbation d’un modèle le rend visible dans l’onglet [!UICONTROL Modèles publics] et disponibles pour tous les utilisateurs et utilisatrices. La désapprobation d’un modèle le supprime de l’onglet [!UICONTROL Modèles publics] et le rend disponible uniquement pour l’équipe qui l’a créé.

1. Cliquez sur **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir la zone [!UICONTROL Administration].
1. Cliquez sur **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.
1. Pour valider un modèle, cliquez sur **[!UICONTROL Approuver]** à droite du modèle.
1. Pour rejeter un modèle, cliquez sur **[!UICONTROL Refuser]** à droite du modèle.

>[!NOTE]
>
>Si vous validez un modèle précédemment approuvé puis modifié, votre seconde approbation remplacera le modèle d’origine.

## Cloner un scénario en tant que modèle

En tant qu’administrateur ou administratrice, vous pouvez cloner un scénario en tant que modèle.

Pour plus d’informations sur le clonage d’un scénario en tant que modèle, consultez la section [Créer un modèle à partir d’un scénario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) dans [Créer des modèles dans  [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
