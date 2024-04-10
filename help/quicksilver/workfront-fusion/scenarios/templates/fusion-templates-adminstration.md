---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Administration des modèles Adobe Workfront Fusion
description: Si vous êtes administrateur, vous avez l’autorisation d’afficher, de modifier, de renommer, de publier, d’approuver et de supprimer les modèles créés par d’autres personnes. Vous pouvez effectuer ces actions à partir du [!UICONTROL Modèles] dans le [!DNL Adobe Workfront Fusion Administration] zone.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: 2b67b5fb951b5ae7867144c444411ebd1c299e75
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Administration des modèles

Si vous êtes administrateur, vous avez l’autorisation d’afficher, de modifier, de renommer, de publier, d’approuver et de supprimer les modèles créés par d’autres personnes. Vous pouvez effectuer ces actions à partir du [!UICONTROL Modèles] dans le [!DNL Adobe Workfront Fusion Administration] zone.

## Exigences d’accès

Pour exécuter les étapes de cet article, vous devez disposer des droits d’accès suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Exigence de licence actuelle : Non [!DNL Workfront Fusion] exigence de licence.</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail], [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Configuration requise actuelle du produit : si vous disposez de [!UICONTROL Select] ou de [!UICONTROL Prime] [!DNL Adobe Workfront] Planifier, votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans [!UICONTROL Ultimate]. [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigence de produit héritée : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès*</td> 
   <td> <p>Vous devez être un administrateur Workfront Fusion pour votre organisation.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour savoir quel plan, type de licence ou accès vous avez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Vue [!DNL Workfront Fusion] modèles en tant que [!DNL Workfront Fusion] administrateur

Pour afficher un tableau de tous les modèles créés et de leurs statuts :

1. Clic **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir le [!UICONTROL Administration] zone.

   >[!NOTE]
   >
   >La zone Administration n’est visible que par les administrateurs de Workfront Fusion.

1. Clic **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.

Trois colonnes sont associées au statut de publication des modèles. Une coche dans une colonne indique ce qui suit :

* **[!UICONTROL Publié]**: ces modèles sont actuellement visibles dans le [!UICONTROL Modèles d’équipe] dans l’interface utilisateur.
* **[!UICONTROL Approbation demandée]**: ces modèles sont en attente de votre approbation. Ils sont actuellement visibles dans [!UICONTROL Modèles d’équipe] dans l’interface utilisateur.
* **[!UICONTROL Approuvé]**: ces modèles ont été approuvés. Ils sont actuellement visibles dans [!UICONTROL Modèles publics] dans l’interface utilisateur standard.

>[!NOTE]
>
>Modèles avec la coche dans le [!UICONTROL Approbation demandée] et dans la colonne [!UICONTROL Approuvé] colonnes ont déjà été approuvées et rendues publiques, mais une version plus récente d’entre elles est en attente de votre approbation.

## Modifier [!DNL Workfront Fusion] modèles en tant qu’administrateur

1. Clic **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir le [!UICONTROL Administration] zone.
1. Clic **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.
1. Clic **[!UICONTROL Détail]** à droite du modèle que vous souhaitez modifier.

Vous pouvez désormais modifier le modèle, comme vous le feriez pour un utilisateur non administrateur. Cependant, dans le [!UICONTROL Options] dans le coin supérieur droit se trouve une option supplémentaire : le diagramme de SVG qui vous fournit le code du SVG. En outre, le processus de publication est le même que dans le cas d’un utilisateur standard. Pour plus d’informations, consultez la section Publication et partage de modèles .

Pour plus d’informations sur les options de modèle spécifiques que vous pouvez modifier, voir [Création de modèles dans [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Pour plus d’informations sur la publication de modèles, voir [Publier et partager [!DNL Adobe Workfront Fusion] modèles](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Approuver ou désapprouver [!DNL Workfront Fusion] modèles

La validation d’un modèle le rend visible dans le [!UICONTROL Modèles publics] et disponible pour tous les utilisateurs. La désapprobation d’un modèle le supprime de la liste [!UICONTROL Modèles publics] et le rend disponible uniquement pour l’équipe qui l’a créé.

1. Clic **[!UICONTROL Administration]** dans le panneau de navigation de gauche pour ouvrir le [!UICONTROL Administration] zone.
1. Clic **[!UICONTROL Modèles]** dans le panneau de navigation de gauche.
1. Pour valider un modèle, cliquez sur **[!UICONTROL Approuver]** à droite du modèle.
1. Pour désapprouver un modèle, cliquez sur **[!UICONTROL Désapprouver]** à droite du modèle.

>[!NOTE]
>
>Si vous approuvez le modèle qui a été précédemment approuvé puis modifié, votre seconde approbation remplacera le modèle d’origine.

## Clonage d’un scénario en tant que modèle

En tant qu’administrateur, vous avez la possibilité de cloner un scénario en tant que modèle.

Pour obtenir des instructions sur le clonage d’un scénario en tant que modèle, voir [Création d’un modèle à partir d’un scénario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) dans [Création de modèles dans [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
