---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mapper un tableau dans  [!DNL Adobe]  Workfront Fusion
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 41%

---

# Mapper un tableau dans [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Mapper un tableau ou un élément de tableau](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-an-array.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Un tableau est un type spécial d’élément qui peut contenir les éléments suivants :

* Une ou plusieurs valeurs de texte (tableau simple)
* Une ou plusieurs collections du même type (tableau complexe)

>[!INFO]
>
>**Exemple :** le module [!UICONTROL Contrôle des e-mails] renvoie un tableau de pièces jointes pour chaque e-mail. Chaque pièce jointe représente une collection pouvant contenir un nom, un contenu, une taille, etc.

Pour plus d’informations, consultez [Types de données d’élément dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Mapper un tableau entier

1. Dans les modules auxquels vous mappez le tableau, cliquez sur le champ dans lequel vous souhaitez mapper le tableau. Il s’agit du champ auquel le tableau est mappé.

1. Dans la zone qui s’affiche, mappez l’élément.

   Le panneau vous permet de mapper les champs de la même manière qu’avec tout autre type d’élément. Si vous ne souhaitez pas remplir chaque élément séparément, mais que vous souhaitez mapper un autre tableau dans le champ cible, utilisez le bouton [!UICONTROL Mapper]. Dans ce cas, assurez-vous que les deux tableaux (le tableau source et le tableau cible) ont la même structure.

   Vous pouvez ajouter n’importe quel nombre d’éléments à un tableau.

Vous pouvez diviser un tableau en lots individuels à l’aide d’un itérateur. Pour plus d’informations, consultez Module d’[[!UICONTROL itération] dans  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/modules/iterator-module.md).

## Mapper des éléments dans un nouveau tableau

Certains champs de Workfront Fusion vous permettent de mapper des éléments dans un tableau. Par exemple, vous pouvez créer un tableau d’éléments de liste de contrôle dans le module Tableaux Workfront > Ajouter un élément de liste de contrôle . Lorsque le module est exécuté, tous les éléments de la liste de contrôle sont ajoutés à la carte.

Tout champ de module qui affiche « Ajouter un élément » crée un tableau.

![Ajouter un élément](assets/add-item.png)

Pour ajouter des éléments au tableau :

1. Cliquez sur **Ajouter un élément**
1. Dans le panneau qui s’ouvre, saisissez les détails de l’élément.
1. Cliquez sur **Ajouter**.
1. (Facultatif) Répétez les étapes 1 à 3 pour chaque élément à ajouter au tableau .

## Mapper des éléments de tableau


### Mapper des éléments de tableau par nombre

Les éléments de tableau s’affichent sous la forme d’un nombre entre crochets après le nom du tableau. Vous pouvez mapper un élément individuel d’un tableau dans un champ à l’aide de ce numéro d’index.

![](assets/map-array-1st-element.png)

>[!NOTE]
>
>L’indexation des tableaux dans Workfront Fusion commence à partir de 1.

Pour mapper un élément de tableau :

1. Cliquez sur le champ dans lequel vous souhaitez mapper l’élément.

   Le panneau de mappage s’ouvre.

1. Recherchez le tableau contenant l’élément que vous souhaitez mapper.
1. Cliquez sur la flèche de liste déroulante en regard du tableau.
1. Cliquez sur l’élément à mapper.

   L’élément est mappé avec l’index de 1. Cela mappe le premier élément du tableau .

1. Pour mapper un autre élément du tableau, cliquez sur le [1] et saisissez le numéro d’index de l’élément du tableau que vous souhaitez mapper.

   ![](assets/access-another-element.png)

### Mapper l’élément d’un tableau avec une clé donnée

Certains tableaux contiennent des collections avec des éléments clé-valeur tels que des métadonnées, des attributs, etc. Pour utiliser l’une de ces valeurs, vous pouvez rechercher un élément par sa valeur de clé donnée et obtenir la valeur correspondante à partir de l’élément de valeur. Il est recommandé d’utiliser une formule combinant les fonctions `map()` et `get()`.



>[!BEGINSHADEBOX]

L’exemple suivant illustre la sortie de l’application [!DNL Jira].

![](assets/output-of-jira-app-350x100.png)

Cet exemple obtient un nom de fichier à partir d’un tableau de pièces jointes, pour la pièce jointe spécifique avec l’ID 10108.

Cet exemple génère la sortie suivante :

![](assets/output-from-jira-350x261.png)

La formule peut être expliquée comme suit :

* `map`

   1. Le premier paramètre de la fonction `map()` est l’élément de tableau entier.
   1. Le deuxième paramètre est le nom brut de l’élément de valeur. Pour obtenir le nom brut, pointez sur l’élément dans le panneau de [!UICONTROL mapping] :

      ![](assets/obtain-raw-name-350x124.png)

      >[!NOTE]
      >
      >Tous les paramètres respectent la casse. Même si dans cet exemple particulier, le libellé de l’élément diffère de son nom brut uniquement en majuscules, il est nécessaire d’utiliser le nom brut.

   1. Le troisième paramètre est le nom brut de l’élément de clé :

      ![](assets/3rd-parameter-350x166.png)

   1. Le quatrième paramètre est la valeur de clé donnée.

  Parce que la fonction `map()` renvoie un tableau (puisqu’il peut y avoir plus d’éléments avec la valeur de clé donnée), il est nécessaire d’appliquer la fonction `get()` pour obtenir son premier élément :

* `get`

   1. Le premier paramètre de la fonction `get()` est le résultat de la fonction `map()`.

   1. Le deuxième paramètre est l’index de l’élément . Dans cet exemple, l’index est `1`.

Cet exemple génère la sortie suivante :

![](assets/output-from-jira-350x261.png)

>[!ENDSHADEBOX]

Pour plus d&#39;informations sur la fonction `map()`, voir [Fonctions de tableau](/help/quicksilver/workfront-fusion/functions/array-functions.md).

Pour plus d&#39;informations sur la fonction `get()`, voir [Fonctions générales](/help/quicksilver/workfront-fusion/functions/general-functions.md).

## Convertir des éléments de tableau en une série de lots

Les tableaux peuvent être convertis en une série de lots à l’aide du module [!UICONTROL Itérateur]. Pour plus d’informations, voir [[!UICONTROL Module Itérateur]](/help/quicksilver/workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles.png)

