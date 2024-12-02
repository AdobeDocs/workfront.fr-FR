---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exécutez l’expert en notation de scénario
description: Gérer des scénarios verrouillés dans  [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: ed100c6ba32a6fbff6fa68ac7a4bfb38db861b17
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 26%

---

# Exécution de l’expert en notation de scénario dans Adobe Workfront Fusion

L’expert en notation de scénario peut vous aider à vous assurer que votre scénario est configuré de manière conforme aux bonnes pratiques. Il vérifie votre scénario et fournit des recommandations pour sa structure et son organisation.

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

Exécutez l’expert en notation de scénario

1. Cliquez sur l’onglet **[!UICONTROL Scénario]** dans le panneau de gauche.
1. Sélectionnez le scénario dans lequel vous souhaitez exécuter l’expert en notation de scénario.
1. Cliquez n’importe où sur le scénario pour accéder à l’éditeur de scénario.
1. Cliquez sur l’icône ![Expert en notation de scénario](assets/scoring-expert-icon.png) près du bas de l’écran de l’icône .

   Le panneau Scenario Score Expert s’ouvre.
1. Cliquez sur **Evaluate**.

L’expert en notation de scénario renvoie un score sur 10 et indique les vérifications qui ont réussi ou échoué. Si une vérification a échoué, l’expert en notation de scénario fournit des recommandations pour savoir comment s’assurer que le scénario respecte ces vérifications.

![Scenario Scenario](assets/scenario-score.png)

## Vérifications de notation du scénario

L’expert en notation de scénario effectue les vérifications suivantes :

* Le scénario doit être nommé.
* Tous les modules doivent être étiquetés.
* Le scénario doit s’exécuter selon une planification définie.

  Pour obtenir des instructions, voir [Planification d’un scénario](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).
* La taille du plan directeur du scénario doit être inférieure à 5 Mo.

  Pour plus d’informations, voir [Barrières de sécurité des performances de fusion](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios).
* Si un module de déclenchement instantané Workfront est utilisé, il doit être filtré.

  Pour obtenir des instructions, reportez-vous à la section [Filtres d’abonnement aux événements dans le module  [!DNL Workfront] > [!UICONTROL Surveiller les événements]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module).





