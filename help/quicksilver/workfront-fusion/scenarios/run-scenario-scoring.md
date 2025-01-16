---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exécuter l’expert en notation de scénario dans Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 144c8dbd-a3e9-4267-b3db-0768dac8f384
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 19%

---

# Exécuter l’expert en notation de scénario dans Adobe Workfront Fusion

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Exécuter l’expert en notation de scénario](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/run-scenario-scoring.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

L’expert en notation de scénario peut vous aider à vous assurer que votre scénario est configuré de manière à suivre les bonnes pratiques. Il vérifie votre scénario et fournit des recommandations pour sa structure et son organisation.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

Exécuter l’expert en notation de scénario

1. Cliquez sur l’onglet **[!UICONTROL Scénario]** dans le panneau de gauche.
1. Sélectionnez le scénario dans lequel vous souhaitez exécuter l’expert en notation de scénario.
1. Cliquez n’importe où sur le scénario pour accéder à l’éditeur de scénarios.
1. Cliquez sur l’icône d’expert en notation de scénario ![expert en notation de scénario](assets/scoring-expert-icon.png) en bas de l’écran.

   Le panneau d’experts en notation de scénario s’ouvre.
1. Cliquez sur **Évaluer**.

L’expert en notation de scénario renvoie une note sur 10 et indique les vérifications qui ont réussi ou échoué. Si une vérification a échoué, l’expert en notation de scénario fournit des recommandations sur la manière de s’assurer que le scénario répond à ces vérifications.

![ Score du scénario ](assets/scenario-score.png)

## Vérifications du score du scénario

L’expert en notation de scénario effectue les vérifications suivantes :

* Le scénario doit être nommé.
* Tous les modules doivent être étiquetés.
* Le scénario doit s’exécuter selon un planning défini.

  Pour obtenir des instructions, voir [Planification d’un scénario](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).
* La taille du plan directeur du scénario doit être inférieure à 5 Mo.

  Pour plus d’informations, voir [ Mécanismes de sécurisation des performances de Fusion ](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios).
* Si un module de déclenchement instantané Workfront est utilisé, il doit être filtré.

  Pour obtenir des instructions, consultez [Filtres d’abonnement aux événements dans le module  [!DNL Workfront] > [!UICONTROL Événements Espion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module).

