---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Flux d’exécution du scénario dans Adobe Workfront Fusion
description: Cet article explique comment un scénario s’exécute et comment les données s’y déplacent. Il explique également où vous pouvez trouver des informations sur vos données traitées et comment les lire.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 75cf9af858e90a640c45b211d36f35b684128c2f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 16%

---

# Flux d’exécution de scénario dans [!DNL Adobe Workfront Fusion]

Cet article explique comment un scénario s’exécute et comment les données s’y déplacent. Il explique également où vous pouvez trouver des informations sur vos données traitées et comment les lire.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Flux d’exécution du scénario

Une fois qu’un scénario est configuré correctement et activé, il s’exécute selon son planning défini.

Au fur et à mesure que le scénario démarre, le premier module répond à un événement qu’il a été défini pour surveiller. S’il renvoie des lots (données), ils sont transmis au module suivant et le scénario se poursuit, en transmettant les lots à travers chaque module successif, un par un.

Si les lots sont traités correctement dans tous les modules, le scénario est marqué comme une réussite dans la zone de détails du scénario, comme expliqué dans la section [Détails du scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Pour plus d’informations sur la configuration d’un scénario, voir [L’éditeur de scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
* Pour plus d’informations sur l’activation d’un scénario, voir [Activation ou désactivation d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Pour plus d’informations sur la planification d’un scénario, voir [Planification d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Pour plus d’informations sur les modules, voir [Types de modules](../../workfront-fusion/modules/module-types.md).

### Exemple : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]

>[!INFO]
>
>**Exemple :** Dans un scénario qui recherche les requêtes entrantes dans [!DNL Workfront] et les convertit ensuite en [!DNL Workfront] projets, les données se déplacent comme suit.
>
>La première étape du scénario, effectuée par le premier module, consiste à surveiller les requêtes. Chaque requête qui entre est considérée comme un lot. Si le module s’exécute sans trouver de lots, le scénario se termine après le premier module.
>
>Si le premier module renvoie un lot, le lot passe par le reste du scénario. Dans cet exemple, le reste du scénario se compose du deuxième et du dernier module, qui convertit la requête en projet.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Exemple : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail et l’intégration]

>[!INFO]
>
>**Exemple :** Dans un scénario qui télécharge des documents à partir de [!DNL Adobe Workfront] et les envoie vers un dossier dans [!DNL Dropbox], les données se déplacent comme suit.
>
>La première étape du scénario, effectuée par le premier module, consiste à surveiller les lots (documents). Dans cet exemple, le module recherche les lots dans [!DNL Workfront]. S’il ne renvoie pas de lot, le scénario se termine après le premier module.
>
>Si un lot est renvoyé, le lot passe par le reste du scénario. Dans cet exemple, le reste du scénario consiste en le deuxième et le dernier module, qui charge le lot dans le dossier [!DNL Dropbox].
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Si le premier module renvoie plusieurs lots, le premier lot est chargé vers [!DNL Dropbox] avant le second chargement. Ensuite, le deuxième lot se charge, puis le troisième, etc.

## Informations sur les lots traités

Pour chaque module, le lot passe par un processus en 4 étapes avant de passer au module suivant ou d’atteindre sa destination finale. Le processus en 4 étapes est Initialisation, Opération, Validation/Restauration et Finalisation. Cela s’appelle le traitement des transactions et permet d’expliquer comment les données ont été traitées dans un module.

Une fois l’exécution d’un scénario terminée, chaque module affiche une icône indiquant le nombre d’opérations effectuées. Vous pouvez cliquer sur cette icône pour afficher les informations détaillées sur les lots traités, au format décrit ci-dessus. Vous pouvez voir quels paramètres de module ont été utilisés et quels lots ont été renvoyés par quel module.

![](assets/info-processed-bundles-350x396.png)

Un module a reçu des informations d’entrée telles que :

* Image convertie
* Dossier sélectionné dans lequel l’image doit être téléchargée
* Nom original de l’image [!DNL Facebook]

Après le traitement, le module a renvoyé ces informations de sortie :

* ID d’image attribué par [!DNL Dropbox]
* Chemin complet où dans [!DNL Dropbox] [!DNL Workfront Fusion] a téléchargé le fichier

Les informations ci-dessus sont capturées séparément pour chaque lot, comme indiqué dans les listes déroulantes [!UICONTROL Opération 1] et [!UICONTROL Opération 2] dans l’image.

Pour plus d’informations sur le traitement des transactions, voir [Exécution de scénario, cycles et phases dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Une erreur s’est produite lors de l’exécution d’un scénario

Une erreur peut se produire lors de l’exécution du scénario. Par exemple, si vous supprimez le dossier [!DNL Dropbox] que vous avez défini comme dossier cible dans le paramètre de module , le scénario se termine par un message d’erreur. Pour plus d&#39;informations sur la façon de gérer les erreurs, voir [Traitement des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
