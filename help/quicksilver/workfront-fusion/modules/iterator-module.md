---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Module itérateur dans Adobe Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 89%

---

# Module [!UICONTROL Itérateur] dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Module Itérateur](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/iterator-module.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Un module [!UICONTROL Itérateur] module est un type spécial de module qui convertit un tableau en une série de lots. Chaque élément du tableau est généré sous la forme d’un lot.

Pour plus d’informations, voir [Types de modules](../../workfront-fusion/modules/module-types.md) et [Mapper un tableau dans Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter Adobe Workfront Fusion ainsi qu’Adobe Workfront pour utiliser les fonctionnalités décrites dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Configuration du module [!UICONTROL Itérateur]

Vous configurez un module [!UICONTROL Itérateur] de la même manière que vous configurez tout autre module. Le champ [!UICONTROL Tableau] contient le tableau à convertir ou à diviser en lots distincts.

![](assets/set-up-iterator-350x190.jpg)

Pour plus d’informations, voir [Configurer les paramètres d’un module dans Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Exemples :**
>
>* Le scénario ci-dessous montre comment récupérer des e-mails avec des pièces jointes et enregistrer les pièces jointes en tant que fichiers uniques dans un dossier [!DNL Dropbox] sélectionné.
>
>   Les e-mails peuvent contenir un tableau de pièces jointes. Le module [!UICONTROL Itérateur] inséré après le premier module vous permettra de gérer chaque pièce jointe séparément. La module [!UICONTROL Itérateur] divise le tableau de pièces jointes en lots uniques. Chaque lot, accompagné d’une pièce jointe, est ensuite enregistré un par un dans un dossier [!DNL Dropbox] sélectionné. La configuration du module [!UICONTROL Itérateur] est illustrée ci-dessus : le champ [!UICONTROL Tableau] doit contenir le tableau `Attachments`.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Pour votre commodité, de nombreuses applications [!DNL Workfront Fusion] offrent des modules [!UICONTROL Itérateurs] spécialisés avec une configuration simplifiée. Par exemple, l’application [!UICONTROL E-mail] contient le module [!UICONTROL Itérateur] [!UICONTROL E-mail] > [!UICONTROL Itérer les pièces jointes] qui produira les mêmes résultats que le module [!UICONTROL Itérateur] général.
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Dépannage : le panneau de mappage n’affiche pas les éléments mappables sous le module [!UICONTROL Itérateur].

Lorsqu’un module [!UICONTROL Itérateur] ne contient pas d’informations sur la structure des éléments du tableau, le panneau de mappage dans les modules qui suivent le module [!UICONTROL Itérateur] n’affiche que deux éléments sous le module [!UICONTROL Itérateur] : `Total number of bundles` et `Bundle order position` :

![](assets/mapping-panel-doesnt-display-350x147.png)

Cela est dû au fait que chaque module est chargé de fournir des informations sur les éléments qu’il génère afin que ces éléments puissent être correctement affichés dans le panneau de mappage dans les modules suivants. Cependant, plusieurs modules peuvent ne pas être en mesure de fournir ces informations dans certains cas, par exemple, les modules [!UICONTROL JSON] > [!UICONTROL Parse JSON] ou [!UICONTROL Webhooks] > [!UICONTROL Webhook personnalisé] avec structure de données manquante.

La solution consiste à exécuter manuellement le scénario pour faire en sorte que le module découvre les éléments qu’il génère afin qu’il puisse fournir les informations aux modules suivants.

Par exemple, si vous avez un module [!UICONTROL JSON] > [!UICONTROL Parse JSON] sans structure de données, comme ci-dessous :

![](assets/json-parse-json-350x285.png)

Et si vous connectez un module [!UICONTROL Itérateur], vous ne pourrez pas mapper la sortie du module au champ Tableau dans le panneau de configuration du module [!UICONTROL itérateur] :

![](assets/connect-iterator-module-350x146.png)

Pour résoudre ce problème, démarrez manuellement le scénario dans l’éditeur de scénario. Vous pouvez annuler la liaison des modules après le module [!UICONTROL JSON] > [!UICONTROL Parse JSON] pour empêcher le flux de continuer. Vous pouvez également cliquer avec le bouton droit sur le module [!UICONTROL JSON] > [!UICONTROL Parse JSON] et choisir **[!UICONTROL Exécuter ce module uniquement]** dans le menu contextuel pour exécuter uniquement le module [!UICONTROL JSON] > [!UICONTROL Parse JSON].

Lorsque le module [!UICONTROL JSON] > [!UICONTROL Parse JSON] s’exécute, il identifie les éléments qu’il génère et fournit ces informations à tous les modules suivants, y compris le module Itérateur. Le panneau de mappage dans la configuration du module Itérateur affiche alors les éléments :

![](assets/mapping-panel-displays-items-350x131.png)

De plus, le panneau de mappage dans les modules connectés après le module [!UICONTROL Itérateur] affiche les éléments contenus dans les éléments du tableau :

![](assets/items-contained-in-array-350x156.png)

Si vous ne pouvez pas voir certains éléments dans le panneau de mappage d’un module, exécutez le scénario une fois afin que tous les modules puissent prendre connaissance des éléments qu’ils génèrent et fournir ces informations aux modules suivants.
