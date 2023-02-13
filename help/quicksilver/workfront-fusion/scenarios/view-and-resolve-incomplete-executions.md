---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]
description: Le [!UICONTROL Exécutions incomplètes] stocke les exécutions de scénario qui n’ont pas été finalisées en raison d’une erreur. Chaque exécution incomplète stockée peut être résolue manuellement ou automatiquement.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]

Le [!UICONTROL Exécutions incomplètes] stocke les exécutions de scénario qui n’ont pas été finalisées en raison d’une erreur. Chaque exécution incomplète stockée peut être résolue manuellement ou automatiquement.

>[!NOTE]
>
>Par défaut, le stockage des exécutions incomplètes est désactivé. Pour l’activer, activez l’option [!UICONTROL Autoriser le stockage d’exécutions incomplètes] dans les paramètres avancés du scénario.
>
>Pour plus d’informations sur les paramètres de scénario, voir [Le panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p><p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Affichage des exécutions incomplètes

Si un module rencontre une erreur lors de son fonctionnement, une nouvelle exécution incomplète est ajoutée au dossier Exécutions incomplètes . Chaque exécution incomplète contient le plan directeur du scénario et tous les lots pouvant être mappés dans le module en échec. La liste des exécutions incomplètes peut être ouverte en cliquant sur le [!UICONTROL Exécutions incomplètes] sur la page détails du scénario :

![](assets/incomplete-executions-tab-350x102.png)

Pour plus d’informations, voir [Erreurs résultant en exécutions incomplètes](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>La taille limite actuelle du dossier d’exécutions incomplètes non résolues par organisation est de 500 Mo. Si votre entreprise dépasse cette limite, l’erreur suivante peut s’afficher :
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Pour plus d’informations, voir [Perte de données](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [Le panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Résoudre les exécutions incomplètes

Lorsqu’une nouvelle exécution incomplète est stockée, vous pouvez la résoudre comme suit :

1. Cliquez sur le bouton **[!UICONTROL Exécutions incomplètes]** .
1. Recherchez l’exécution incomplète que vous souhaitez résoudre, puis cliquez sur **[!UICONTROL Détail]**.


   Si vous souhaitez consulter le journal de toutes les opérations du module avant de tenter de résoudre l’exécution incomplète, vous pouvez résoudre l’exécution incomplète à partir de la variable [!UICONTROL Histoire] folder:

1. Cliquez sur le bouton **[!UICONTROL Histoire]** .
1. Recherchez le journal d’exécution en échec du scénario, puis cliquez sur **[!UICONTROL Détails]**.
1. Ouvrez le journal du module, où toutes les opérations du module sont affichées.
1. Recherchez l’opération ayant échoué et cliquez sur **[!UICONTROL Résoudre]**:

   ![](assets/resolve-btn-350x188.png)

## Options relatives aux exécutions incomplètes

Les options suivantes du [!UICONTROL Paramètres du scénario] détermine si et comment les exécutions incomplètes sont stockées :

* Autoriser le stockage d’exécutions incomplètes
* Traitement séquentiel
* Perte de données

Pour plus d’informations sur ces options, voir [Le panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Erreurs résultant en exécutions incomplètes

Il existe plusieurs catégories d&#39;erreurs qui se traduisent par le stockage d&#39;exécutions incomplètes. Il peut s’agir :

* Erreurs de validation provenant de données incomplètes ou erronées, principalement en raison d’un élément manquant attendu pour traiter correctement toutes les données transitant par un module.
* Erreurs survenant lors de l’indisponibilité de la destination finale en raison d’un échec temporaire ou à long terme de la connexion (par exemple, lors de la connexion à un serveur de messagerie ou FTP distant).

Si une erreur se produit sur le premier module du scénario, l’exécution s’arrête immédiatement et aucune exécution incomplète n’est stockée.

Si une erreur se produit sur un autre module et qu’aucun itinéraire de gestionnaire d’erreur n’est associé, l’un des événements suivants se produit :

* Si le type d’erreur est `ConnectionError`, `RateLimitError`, `OutOfSpaceError` ou `ModuleTimeoutError`, un enregistrement d’exécution incomplet avec reprise automatique est stocké.
* Si le type d’erreur est `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`ou `MaxResultsExceededError`, un enregistrement d’exécution incomplet sans reprise automatique est stocké.
* Si le type d&#39;erreur est autre que ci-dessus, l&#39;exécution échoue.
