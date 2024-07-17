---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Opérations dans Adobe Workfront Fusion
description: Une opération dans Adobe Workfront Fusion est une tâche effectuée par un module. À des fins de suivi, toute action réussie effectuée par un module est une opération.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Opérations dans [!DNL Adobe Workfront Fusion]

Une opération dans [!DNL Adobe Workfront Fusion] est une tâche effectuée par un module. À des fins de suivi, toute action réussie effectuée par un module est une opération.

## Considérations relatives au comptage du nombre d’opérations

* En règle générale, toute exécution action-étape réussie est considérée comme une opération.

* Le premier module d’un scénario ne s’exécute qu’une seule fois et est toujours compté comme une seule opération, même s’il ne renvoie pas de lot.

* Le nombre de fois où le reste des modules s’exécute dépend du nombre de lots qu’ils doivent traiter.  Une exécution d’un module pour un lot est une opération. Une exception est le module d’agrégation, qui est compté comme une opération par ensemble de lots en cours de traitement.

* Les opérations sont comptabilisées à l’étape [!UICONTROL Finalisation] de l’exécution d’un scénario.

* Les opérations suivantes sont **not** comptabilisées comme des opérations :

   * N’importe quelle étape de filtre.

   * Toute action qui comporte des erreurs ou qui s’arrête.

   * Tout itinéraire qui ne s’exécute pas parce que les règles de l’itinéraire n’ont pas été respectées, comme les itinéraires de secours ou les itinéraires désactivés.

   * Action qui ne s’exécute pas, soit parce qu’un filtre n’a pas autorisé les données à passer, soit parce que le scénario s’est arrêté en raison d’une erreur.

## Limites d’opération

Votre entreprise peut avoir une limite d’opérations mensuelle. Cela est basé sur le plan [!DNL Workfront] que votre entreprise a acheté. Le plan [!UICONTROL Ultimate] [!DNL Workfront] offre un nombre illimité d&#39;opérations.

Si votre entreprise dispose d’une limite mensuelle, vous en serez informé lorsque vous approcherez de cette limite. Si vous dépassez cette limite, [!DNL Workfront] contactera votre organisation pour vous assurer que votre plan répond à vos besoins.

## Afficher le nombre d’opérations effectuées au cours des 30 derniers jours

Vous pouvez voir un graphique indiquant le nombre d’opérations effectuées. Ces graphiques sont disponibles aux emplacements suivants :

* **Tableau de bord de l’organisation** : opérations utilisées par l’ensemble de l’organisation
* **Tableau de bord de l’équipe** : opérations utilisées par des scénarios appartenant à cette équipe ([!DNL Adobe Experience Cloud] uniquement)
* **Page de détails du scénario** : opérations utilisées par ce scénario ([!DNL Adobe Experience Cloud] uniquement)
