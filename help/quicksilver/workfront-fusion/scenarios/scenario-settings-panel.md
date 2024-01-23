---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Panneau des paramètres du scénario dans Adobe Workfront Fusion
description: Cet article décrit les paramètres disponibles dans la variable [!UICONTROL paramètres de scénario] dans votre [!DNL Adobe Workfront Fusion] scénarios.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 4d9832d0870c3fccf847c3932ad4f985a62b9672
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# Le panneau des paramètres de scénario dans [!DNL Adobe Workfront Fusion]

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
   <td>
   <p>Exigences de licence actuelles : non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail, [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de l’[!UICONTROL Select] ou de l’[!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ouvrir les paramètres du scénario

1. Ouvrez l’éditeur de scénario, en suivant la procédure décrite à la section [L’éditeur de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Cliquez sur l’icône d’engrenage près du coin inférieur gauche de la page.

   ![](assets/scenario-settings-350x221.png)

   Dans le [!UICONTROL Paramètres du scénario] qui s’affiche, vous pouvez configurer différents paramètres avancés pour le scénario.

## [!UICONTROL Autoriser le stockage d’exécutions incomplètes]

Cette option détermine comment [!DNL Adobe Workfront Fusion] s’exécute si une erreur se produit lors de l’exécution d’un scénario. Lorsque cette option est activée, le scénario est suspendu et déplacé vers [Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Vous avez ainsi la possibilité de résoudre le problème et de continuer à exécuter à partir de l’endroit où le scénario a été arrêté. Si cette option est désactivée, l’exécution du scénario s’arrête et une phase de restauration est lancée.

## [!UICONTROL Traitement séquentiel]

Cette option détermine comment [!DNL Workfront Fusion] se poursuit si une erreur se produit et que l’exécution d’un scénario est déplacée vers l’événement [Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Si la variable [!UICONTROL Traitement séquentiel] est activée, Workfront Fusion cesse de traiter la séquence des tâches jusqu’à ce que toutes les exécutions incomplètes soient résolues. Si la variable [!UICONTROL Traitement séquentiel] est désactivée, le scénario continue de fonctionner conformément à son planning, accompagné de tentatives répétées d’exécution incomplète.

>[!NOTE]
>
>Le traitement séquentiel peut entraîner un retard dans l’exécution d’un scénario. Si des exécutions incomplètes se trouvent toujours dans la file d’attente lorsqu’un scénario instantané se déclenche ou qu’un scénario planifié est défini pour s’exécuter, ce scénario s’exécutera une fois toutes les exécutions avant qu’il ne soit dans la file d’attente terminées.
>
>Si le cas d’utilisation de vos scénarios ne nécessite pas de traitement séquentiel, nous vous recommandons de désactiver l’option de traitement séquentiel.

Pour plus d’informations sur la planification, voir [Planification d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Les données sont confidentielles

Une fois qu’un scénario a été exécuté, vous pouvez afficher par défaut des informations sur les données qui ont été traitées par les modules du scénario. Si vous ne souhaitez pas que ces informations soient stockées, activez la variable [!UICONTROL Les données sont confidentielles] .

Pour plus d’informations sur l’affichage des informations, voir [Flux d’exécution du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Si vous activez cette option, il peut être difficile de résoudre les erreurs qui peuvent se produire lors de l’exécution d’un scénario.

## Perte de données

Cette option concerne l’activation de la perte de données si [!DNL Workfront Fusion] échoue à enregistrer un lot dans la file d’attente de [Afficher et résoudre les exécutions incomplètes dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (par exemple, à cause d&#39;un manque d&#39;espace libre). Lorsque cette option est activée, les données sont perdues afin d’éviter des interruptions dans l’exécution globale du scénario. Cela s’avère utile dans les cas où la priorité la plus élevée est l’exécution continue et où les données erronées entrantes ne sont pas si importantes.

En outre, lors de l’exécution d’un scénario, un module peut parfois rencontrer un fichier plus volumineux que la taille maximale autorisée. Dans ce cas, [!DNL Workfront Fusion] procède conformément à la définition de la variable [!UICONTROL Perte de données] et un message d’avertissement s’affiche.

Pour plus d’informations sur la taille de fichier maximale, voir [À propos du mappage des fichiers dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Pour plus d’informations sur les avertissements, voir [Traitement des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Validation automatique]

La variable [!UICONTROL Validation automatique] s’applique aux transactions et définit la manière de traiter un scénario. Si l’option Validation automatique est activée, la phase de validation de chaque module démarre immédiatement après avoir terminé la phase d’opération. Lorsque l’option Validation automatique est désactivée, aucune validation n’a lieu tant que les opérations ne sont pas exécutées pour tous les modules (il s’agit du mode par défaut).

Pour plus d’informations sur les transactions, voir [Exécution, cycles et phases d’un scénario [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Nombre maximum de cycles

La définition de davantage de cycles peut s’avérer utile lorsque vous souhaitez empêcher l’interruption de connexion à un service tiers et vous assurer que tous les enregistrements sont traités dans un seul scénario d’exécution.

* Si le scénario commence par un déclencheur d’interrogation, le paramètre définit le nombre maximal de cycles autorisés lors de l’exécution du scénario.

  Pour plus d’informations sur les déclencheurs d’interrogation, voir [Déclencheurs d’interrogation](../../workfront-fusion/modules/module-types.md#polling) in [Types de modules](../../workfront-fusion/modules/module-types.md).

* Si le scénario commence par un déclencheur instantané, le paramètre est ignoré et tous les événements en attente sont traités lors d’une seule exécution de scénario, un événement par cycle.

  Pour plus d’informations sur les déclencheurs instantanés, voir [Déclencheurs instantanés](../../workfront-fusion/modules/module-types.md#instant) in [Types de modules](../../workfront-fusion/modules/module-types.md).

* Si le scénario ne commence pas par un déclencheur (instantané/interrogation), le nombre maximal de cycles spécifié est toujours effectué.

>[!INFO]
>
>**Exemples :**  [!DNL Workfront] > [!UICONTROL Surveiller les enregistrements] recherche les nouveaux problèmes qui surviennent et [!DNL Workfront] >[!UICONTROL Conversion, objet] convertit la nouvelle requête en projet et lui affecte le modèle approprié.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL cycles supplémentaires] est appliqué uniquement lorsque vous planifiez l’exécution de votre scénario. Lorsque vous utilisez la variable [!UICONTROL Exécuter une seule fois] , les paramètres du cycle sont pris en compte.
>
>### Le nombre maximal de cycles est défini sur 1 (valeur par défaut)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>La variable [!UICONTROL Nombre maximal de fichiers renvoyés] dans le [!UICONTROL Dropbox] >[!UICONTROL Fichiers de contrôle] module est défini sur `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Si 100 requêtes sont envoyées à [!DNL Workfront], et la variable [!UICONTROL Limite] est défini sur 10, 90 fichiers ne sont pas traités après l’exécution d’un scénario. Les 10 fichiers suivants sont traités lors de la prochaine exécution du scénario planifiée.
>
>### Le nombre maximal de cycles est défini sur 10.
>
>La variable [!UICONTROL Nombre maximal de fichiers renvoyés] dans le [!UICONTROL Dropbox] >[!UICONTROL Fichiers de contrôle] module est défini sur `10`.
>
>Si 100 fichiers sont ajoutés au dossier du Dropbox et au dossier [!UICONTROL Nombre maximal de fichiers renvoyés] est définie sur 10, puis 10 fichiers sont traités au cours du premier cycle, les 10 fichiers suivants au cours du deuxième cycle, les 10 fichiers suivants au cours du troisième cycle, etc., jusqu’à ce que tous les fichiers soient traités.
>
>Tous les fichiers sont traités dans un scénario d’exécution.
>
>Vous pouvez voir les cycles déjà exécutés dans les détails du scénario :
>
>![](assets/scenario-detail-350x207.png)
>
>Pour plus d’informations sur cette page, voir [Détails du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Nombre d&#39;erreurs consécutives

Définit le nombre maximum de tentatives d’exécution consécutives avant la désactivation de l’exécution d’un scénario (à l’exception de [!UICONTROL DataError], [!UICONTROL DuplicateDataError] et [!UICONTROL ConnectionError]).

Pour plus d’informations sur les erreurs, voir [Traitement des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Si un scénario commence par un déclencheur instantané, le paramètre est ignoré et le scénario est désactivé immédiatement une fois la première erreur survenue.
