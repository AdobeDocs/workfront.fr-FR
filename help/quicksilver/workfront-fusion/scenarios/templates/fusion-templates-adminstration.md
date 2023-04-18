---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administration des modèles de fusion Adobe Workfront
description: Si vous êtes administrateur, vous êtes autorisé à afficher, modifier, renommer, publier, approuver et supprimer les modèles créés par d’autres utilisateurs. Vous pouvez effectuer ces actions à partir du [!UICONTROL Modèles] dans la [!DNL Adobe Workfront Fusion Administration] zone.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: bcca026e193e66cfb92ab9a0fb1aaf1eeb6892fb
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Administration des modèles

Si vous êtes administrateur, vous êtes autorisé à afficher, modifier, renommer, publier, approuver et supprimer les modèles créés par d’autres utilisateurs. Vous pouvez effectuer ces actions à partir du [!UICONTROL Modèles] dans la [!DNL Adobe Workfront Fusion Administration] zone.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un administrateur Workfront Fusion pour votre entreprise.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Affichage [!DNL Workfront Fusion] modèles en tant qu’administrateur

Pour afficher un tableau de tous les modèles créés et de leur statut :

1. Cliquez sur **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir la [!UICONTROL Administration] zone.
1. Cliquez sur **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.

Trois colonnes sont liées à l’état de publication des modèles. Une coche dans une colonne indique les éléments suivants :

* **[!UICONTROL Publié]**: Ces modèles sont actuellement visibles dans la variable [!UICONTROL Modèles d’équipe] dans l’interface utilisateur.
* **[!UICONTROL Validation demandée]**: Ces modèles attendent votre approbation. Ils sont actuellement visibles dans la variable [!UICONTROL Modèles d’équipe] dans l’interface utilisateur.
* **[!UICONTROL Approuvé]**: Ces modèles ont été approuvés. Ils sont actuellement visibles dans la variable [!UICONTROL Modèles publics] dans l’interface utilisateur standard.

>[!NOTE]
>
>Modèles avec coche dans les [!UICONTROL Validation demandée] et dans la variable [!UICONTROL Approuvé] ont déjà été approuvées et rendues publiques, mais une version plus récente d&#39;entre elles attend votre approbation.

## Modifier [!DNL Workfront Fusion] modèles en tant qu’administrateur

1. Cliquez sur **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir la [!UICONTROL Administration] zone.
1. Cliquez sur **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.
1. Cliquez sur **[!UICONTROL Détail]** à droite du modèle que vous souhaitez modifier.

Vous pouvez désormais modifier le modèle, comme vous le faites pour modifier un modèle en tant qu’utilisateur non administrateur. Toutefois, dans la variable [!UICONTROL Options] dans le coin supérieur droit, il existe une option supplémentaire : le diagramme du SVG qui vous fournit le code du SVG. En outre, le processus de publication est le même que pour un utilisateur standard. Pour plus d’informations, reportez-vous à la section Publication et partage de modèles .

Pour plus d’informations sur les options de modèle spécifiques que vous pouvez modifier, voir [Création de modèles dans [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Pour plus d’informations sur la publication de modèles, voir [Publier et partager [!DNL Adobe Workfront Fusion] templates](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Approuver ou refuser [!DNL Workfront Fusion] templates

La validation d’un modèle le rend visible dans la variable [!UICONTROL Modèles publics] et disponibles pour tous les utilisateurs. La désapprobation d’un modèle le supprime de la fonction [!UICONTROL Modèles publics] et la rend disponible uniquement pour l’équipe qui l’a créé.

1. Cliquez sur **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir la [!UICONTROL Administration] zone.
1. Cliquez sur **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.
1. Si vous souhaitez valider un modèle, cliquez sur **[!UICONTROL Approuver]** à droite du modèle.
1. Si vous souhaitez désapprouver un modèle, cliquez sur **[!UICONTROL Désapprouver]** à droite du modèle.

>[!NOTE]
>
>Si vous validez le modèle précédemment validé puis édité, votre seconde validation remplacera le modèle d&#39;origine.

## Cloner un scénario en tant que modèle

En tant qu’administrateur, vous avez la possibilité de cloner un scénario en tant que modèle.

Pour plus d’informations sur le clonage d’un scénario en tant que modèle, voir [Création d’un modèle à partir d’un scénario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Création de modèles dans [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
