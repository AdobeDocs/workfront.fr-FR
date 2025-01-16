---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Flux d’exécution des scénarios dans Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 89%

---

# Flux d’exécution du scénario dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Flux d’exécution du scénario](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/scenario-execution-flow.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Cet article explique comment un scénario s’exécute et comment les données y circulent. Il explique également où vous pouvez trouver des informations sur vos données traitées et comment les lire.

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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Flux d’exécution du scénario

Une fois qu’un scénario est correctement défini et activé, il s’exécute selon le planning défini.

Au début du scénario, le premier module réagit à un événement qu’il a été chargé de surveiller. S’il renvoie des lots (données), ceux-ci passent au module suivant et le scénario se poursuit en faisant passer les lots dans chaque module successif, un par un.

Si les lots sont traités correctement dans tous les modules, le scénario est marqué comme un succès dans la zone de détail du scénario, comme expliqué dans [Détails du scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Pour plus d’informations sur la configuration d’un scénario, voir [L’éditeur de scénarios dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
* Pour plus d’informations sur l’activation d’un scénario, voir [Activer ou désactiver un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Pour plus d’informations sur la planification d’un scénario, voir [Planifier un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Pour plus d’informations sur les modules, voir [Types de modules](../../workfront-fusion/modules/module-types.md).

### Exemple : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation du travail]

>[!INFO]
>
>**Exemple :** dans un scénario qui surveille les demandes entrantes dans [!DNL Workfront] et les convertit ensuite en projets [!DNL Workfront], les données circuleraient comme suit.
>
>La première étape du scénario, réalisée par le premier module, consiste à surveiller les demandes. Chaque demande reçue est considérée comme un lot. Si le module s’exécute sans trouver de lot, le scénario se termine après le premier module.
>
>Si le premier module renvoie un lot, le lot passe par le reste du scénario. Dans cet exemple, le reste du scénario est constitué du deuxième et dernier module, qui convertit la demande en projet.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Exemple : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail]

>[!INFO]
>
>**Exemple :** dans un scénario qui télécharge des documents à partir d’[!DNL Adobe Workfront] et les envoie dans un dossier dans [!DNL Dropbox], les données circuleraient comme suit.
>
>La première étape du scénario, réalisée par le premier module, consiste à surveiller les lots (documents). Dans cet exemple, le module recherche des lots dans [!DNL Workfront]. S’il ne renvoie pas de lot, le scénario se termine après le premier module.
>
>Si un lot est renvoyé, le lot passe par le reste du scénario. Dans cet exemple, le reste du scénario est constitué du deuxième et dernier module, qui charge le lot dans le dossier [!DNL Dropbox].
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Si le premier module renvoie plusieurs lots, le premier lot est chargé sur [!DNL Dropbox] avant le second. Ensuite, le deuxième lot est chargé, puis le troisième, et ainsi de suite.

## Informations sur les lots traités

Pour chaque module, le lot passe par un processus en quatre étapes avant de passer au module suivant ou d’atteindre sa destination finale. Les quatre étapes du processus sont : l’initalisation, l’exploitation, la validation/la restauration et la finalisation. C’est ce qu’on appelle le traitement des transactions, qui permet d’expliquer comment les données ont été traitées dans un module.

Une fois le scénario terminé, chaque module affiche une icône indiquant le nombre d’opérations effectuées. Vous pouvez cliquer sur cette icône pour afficher les informations détaillées sur les lots traités, dans le format décrit ci-dessus. Vous pouvez voir quels paramètres des modules ont été utilisés et quels lots ont été renvoyés par quel module.

![](assets/info-processed-bundles-350x396.png)

Un module a reçu des informations d’entrée telles que les suivantes :

* Image convertie
* Dossier sélectionné dans lequel charger l’image
* Nom original de l’image [!DNL Facebook]

Après traitement, le module a renvoyé les informations de sortie suivantes :

* ID de l’image attribué par [!DNL Dropbox]
* Chemin complet dans [!DNL Dropbox] où [!DNL Workfront Fusion] a chargé le fichier.

Les informations ci-dessus sont saisies pour chaque lot séparément, comme indiqué par les cases déroulantes [!UICONTROL Opération 1] et [!UICONTROL Opération 2] dans l’image.

Pour plus d’informations sur le traitement des transactions, voir [Exécution de scénarios, de cycles et de phases dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Une erreur s’est produite lors de l’exécution d’un scénario.

Une erreur peut se produire pendant l’exécution du scénario. Par exemple, si vous supprimez le dossier [!DNL Dropbox] que vous avez défini comme dossier cible dans les paramètres du module, le scénario se termine par un message d’erreur. Pour plus d’informations sur le traitement des erreurs, voir [Traitement des erreurs dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
