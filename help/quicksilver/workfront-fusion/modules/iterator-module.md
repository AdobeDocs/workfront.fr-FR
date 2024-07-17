---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Module d’itération dans Adobe Workfront Fusion
description: Un module Itérateur est un type spécial de module qui convertit un tableau en une série de lots. Chaque élément du tableau est généré sous la forme d’un lot distinct.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 8%

---

# Module [!UICONTROL Itérateur] dans [!DNL Adobe Workfront Fusion]

Un module [!UICONTROL Itérateur] est un type spécial de module qui convertit un tableau en une série de lots. Chaque élément du tableau est généré sous la forme d’un lot distinct.

Pour plus d’informations, voir [Types de modules](../../workfront-fusion/modules/module-types.md) et [Mappage d’un tableau dans Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

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
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter Adobe Workfront Fusion ainsi qu’Adobe Workfront pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Configuration du module [!UICONTROL Itérateur]

Vous configurez un module [!UICONTROL Itérateur] de la même manière que vous configurez tout autre module. Le champ [!UICONTROL Array] contient le tableau à convertir ou à diviser en lots distincts.

![](assets/set-up-iterator-350x190.jpg)

Pour plus d’informations, voir [Configuration des paramètres d’un module dans Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Exemples :**
>
>* Le scénario ci-dessous montre comment récupérer des emails avec des pièces jointes et enregistrer les pièces jointes en tant que fichiers uniques dans un dossier [!DNL Dropbox] sélectionné.
>
>   Les emails peuvent contenir un tableau de pièces jointes. Le module [!UICONTROL Itérateur] inséré après le premier module vous permettra de gérer chaque pièce jointe séparément. Le module [!UICONTROL Itérateur] divise le tableau de pièces jointes en lots uniques. Chaque lot, accompagné d’une pièce jointe, est ensuite enregistré un par un dans un dossier [!DNL Dropbox] sélectionné. La configuration du module [!UICONTROL Itérateur] est présentée ci-dessus : le champ [!UICONTROL Tableau] doit contenir le tableau `Attachments`.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Pour votre commodité, de nombreuses applications [!DNL Workfront Fusion] proposent des modules [!UICONTROL Iterator] spécialisés avec une configuration simplifiée. Par exemple, l’application [!UICONTROL Email] contient le module spécial [!UICONTROL Itérateur] [!UICONTROL Email] > [!UICONTROL Itérer les pièces jointes] qui produira les mêmes résultats que le module général [!UICONTROL Itérateur].
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Dépannage : le panneau de mappage n’affiche pas les éléments mappables sous le module [!UICONTROL Itérateur]

Lorsqu’un module [!UICONTROL Itérateur] ne dispose pas d’informations sur la structure des éléments du tableau, le panneau de mappage dans les modules qui suivent le module [!UICONTROL Itérateur] n’affiche que 2 éléments sous le module [!UICONTROL Itérateur] : `Total number of bundles` et `Bundle order position` :

![](assets/mapping-panel-doesnt-display-350x147.png)

Cela est dû au fait que chaque module est chargé de fournir des informations sur les éléments qu’il génère afin que ces éléments puissent être correctement affichés dans le panneau de mappage dans les modules suivants. Cependant, plusieurs modules peuvent ne pas être en mesure de fournir ces informations dans certains cas, par exemple, les modules [!UICONTROL JSON] > [!UICONTROL Parse JSON] ou [!UICONTROL Webhooks] > [!UICONTROL Custom Webhook] avec structure de données manquante.

La solution consiste à exécuter manuellement le scénario pour faire en sorte que le module découvre les éléments qu’il génère afin qu’il puisse fournir les informations aux modules suivants.

Par exemple, si vous disposez d’un module [!UICONTROL JSON] > [!UICONTROL Parse JSON] sans structure de données comme ci-dessous :

![](assets/json-parse-json-350x285.png)

Ensuite, si vous connectez un module [!UICONTROL Itérateur] à celui-ci, vous ne pourrez pas mapper la sortie du module au champ Tableau dans le panneau de configuration du module [!UICONTROL Itérateur] :

![](assets/connect-iterator-module-350x146.png)

Pour résoudre ce problème, démarrez manuellement le scénario dans l’éditeur de scénarios. Vous pouvez dissocier les modules après le module [!UICONTROL JSON] > [!UICONTROL Parse JSON] pour empêcher le flux de continuer. Vous pouvez également cliquer avec le bouton droit sur le module [!UICONTROL JSON] > [!UICONTROL Parse JSON] et choisir **[!UICONTROL Exécuter ce module uniquement]** dans le menu contextuel pour exécuter uniquement le module [!UICONTROL JSON] > [!UICONTROL Parse JSON].

Lorsque le [!UICONTROL JSON] > [!UICONTROL Parse JSON] s’exécute, il découvre les éléments qu’il génère et fournit ces informations à tous les modules suivants, y compris le module d’itérateur. Le panneau de mappage dans la configuration de l’itérateur affiche ensuite les éléments :

![](assets/mapping-panel-displays-items-350x131.png)

De plus, le panneau de mappage dans les modules connectés après le module [!UICONTROL Itérateur] affiche les éléments contenus dans les éléments du tableau :

![](assets/items-contained-in-array-350x156.png)

Si vous ne pouvez pas voir certains éléments dans le panneau de mappage d’un module, exécutez le scénario une fois afin que tous les modules puissent en savoir plus sur les éléments qu’ils génèrent et fournissez ces informations aux modules suivants.
