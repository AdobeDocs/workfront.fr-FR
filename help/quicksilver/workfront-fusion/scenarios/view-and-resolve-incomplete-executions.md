---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Afficher et résoudre les exécutions incomplètes dans  [!DNL Adobe Workfront Fusion]
description: Le dossier [!UICONTROL Exécutions incomplètes] stocke les exécutions de scénario qui n’ont pas été finalisées correctement en raison d’une erreur. Chaque exécution incomplète stockée peut être résolue manuellement ou automatiquement.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 53582d36ef2256f6073705ce3eabe8cd61c9b2cc
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 96%

---

# Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]

Le dossier [!UICONTROL Exécutions incomplètes] stocke les exécutions de scénario qui n’ont pas été finalisées correctement en raison d’une erreur. Chaque exécution incomplète stockée peut être résolue manuellement ou automatiquement.

>[!NOTE]
>
>Par défaut, le stockage des exécutions incomplètes est désactivé. Pour l’activer, activez l’option [!UICONTROL Autoriser le stockage d’exécutions incomplètes] dans les paramètres avancés du scénario.
>
>Pour plus d’informations sur les paramètres de scénario, voir [Panneau des paramètres de scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Afficher les exécutions incomplètes

Si un module rencontre une erreur lors de son fonctionnement, une nouvelle exécution incomplète est ajoutée au dossier Exécutions incomplètes. Chaque exécution incomplète contient le plan directeur du scénario et tous les lots pouvant être mappés dans le module qui a échoué. Vous pouvez ouvrir la liste des exécutions incomplètes en cliquant sur l’onglet [!UICONTROL Exécutions incomplètes] de la page des détails du scénario.

<!--

![](assets/incomplete-executions-tab-350x102.png)

-->

Pour plus d’informations, voir [Erreurs aboutissant à des exécutions incomplètes](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>La taille limite actuelle du dossier d’exécutions incomplètes non résolues par organisation est de 500 Mo. Si votre entreprise dépasse cette limite, l’erreur suivante peut s’afficher :
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Pour plus d’informations, voir [Activer la perte de données](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) dans [Panneau des paramètres de scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Résoudre les exécutions incomplètes

Lorsqu’une nouvelle exécution incomplète est stockée, vous pouvez la résoudre comme suit :

1. Cliquez sur l’onglet **[!UICONTROL Exécutions incomplètes]**.
1. Recherchez l’exécution incomplète que vous souhaitez résoudre, puis cliquez sur **[!UICONTROL Détail]**.


   Si vous souhaitez consulter le journal de toutes les opérations du module avant de tenter de résoudre l’exécution incomplète, vous pouvez résoudre l’exécution incomplète à partir du dossier [!UICONTROL Historique] :

1. Cliquez sur l’onglet **[!UICONTROL Historique]**.
1. Recherchez le journal d’exécution en échec du scénario, puis cliquez sur **[!UICONTROL Détails]**.
1. Ouvrez le journal du module, où toutes les opérations du module sont affichées.
1. Recherchez l’opération ayant échoué et cliquez sur **[!UICONTROL Résoudre]** :

   ![](assets/resolve-btn-350x188.png)

## Options relatives aux exécutions incomplètes

Les options suivantes dans le panneau [!UICONTROL Paramètres du scénario] déterminent si et comment les exécutions incomplètes sont stockées :

* Autoriser le stockage d’exécutions incomplètes
* Traitement séquentiel
* Activer la perte de données

Pour plus d’informations sur ces options, voir [Panneau des paramètres de scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Erreurs entraînant des exécutions incomplètes

Il existe plusieurs catégories d’erreurs qui entraînent le stockage d’exécutions incomplètes. Ces erreurs peuvent inclure les suivantes :

* Des erreurs de validation dues à des données incomplètes ou erronées. Le plus souvent, cela est dû à un élément manquant qui est nécessaire pour traiter avec succès toutes les données passant par un module.
* Des erreurs dues à l’indisponibilité de la destination finale en raison d’un échec temporaire ou à long terme de la connexion (par exemple, lors de la connexion à un serveur de messagerie ou FTP distant).

Si une erreur se produit sur le premier module du scénario, l’exécution s’arrête immédiatement et aucune exécution incomplète n’est stockée.

Si une erreur se produit sur un autre module et qu’aucun itinéraire de gestionnaire d’erreur n’est associé, alors l’un des événements suivants se produit :

* Si le type d’erreur est `ConnectionError`, `RateLimitError`, `OutOfSpaceError` ou `ModuleTimeoutError`, un enregistrement d’exécution incomplète avec reprise automatique est stocké.
* Si le type d’erreur est `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`, ou `MaxResultsExceededError`, un enregistrement d’exécution incomplète sans reprise automatique est stocké.
* Si le type d’erreur est autre que ci-dessus, l’exécution échoue.
