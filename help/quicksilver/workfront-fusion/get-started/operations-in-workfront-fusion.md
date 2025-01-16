---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Opérations dans Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 80%

---

# Opérations dans [!DNL Adobe Workfront Fusion]



>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [ Opérations ](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/operations-in-workfront-fusion.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans [!DNL Adobe Workfront Fusion], une opération est une tâche effectuée par un module. À des fins de suivi, toute action effectuée avec succès par un module est une opération.

## Éléments à prendre en compte lors du comptage du nombre d’opérations

* En général, toute exécution réussie d’une étape-action est considérée comme une opération.

* Le premier module d’un scénario ne s’exécute qu’une seule fois et est toujours compté comme une opération, même s’il ne renvoie pas de lot.

* Le nombre d’exécutions des autres modules dépend du nombre de lots qu’ils doivent traiter.  Une exécution d’un module pour un lot constitue une seule opération. Le module agrégateur fait exception à la règle, puisqu’il est compté comme une opération pour chaque ensemble de lots traités.

* Les opérations sont comptées lors de l’étape [!UICONTROL Finalisation] de l’exécution d’un scénario.

* Les éléments suivants ne sont **pas** comptés comme des opérations :

   * Toutes les étapes de filtrage.

   * Toute action qui provoque une erreur ou qui est interrompue.

   * Tout itinéraire qui n’est pas exécuté parce que les règles de l’itinéraire n’ont pas été satisfaites, tels que les itinéraires de secours ou les itinéraires désactivés.

   * Toute action qui ne s’exécute pas, soit parce qu’un filtre n’a pas autorisé le passage des données, soit parce que le scénario s’est arrêté en raison d’une erreur.

## Limites d’opérations

Votre organisation peut avoir une limite mensuelle d’opérations. Celle-ci est basée sur la formule [!DNL Workfront] que votre organisation a acheté. La formule [!DNL Workfront] [!UICONTROL Ultimate] permet des opérations illimitées.

Si votre organisation est soumise à une limite mensuelle, vous recevez une notification lorsque vous approchez de cette limite. Si vous dépassez la limite, [!DNL Workfront] contacte votre organisation pour s’assurer que votre formule répond à vos besoins.

## Consulter le nombre d’opérations effectuées au cours des 30 derniers jours

Vous pouvez consulter des graphiques qui indiquent le nombre d’opérations effectuées. Ces graphiques sont disponibles aux endroits suivants :

* **Tableau de bord de l’organisation** : opérations utilisées par l’ensemble de l’organisation.
* **Tableau de bord de l’équipe** : opérations utilisées par les scénarios appartenant à cette équipe ([!DNL Adobe Experience Cloud] uniquement).
* **Page des détails du scénario** : opérations utilisées par ce scénario ([!DNL Adobe Experience Cloud] uniquement).
