---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]
description: Le mappage désigne le processus d’affectation des sorties d’un module, structurées en éléments, aux champs d’entrée d’un autre.
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 3772223938008e3a54ce0a48aaae1f3edb5bf252
workflow-type: tm+mt
source-wordcount: '1567'
ht-degree: 100%

---

# Mapper les informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]

Le mappage désigne le processus d’affectation des sorties d’un module, structurées en éléments, aux champs d’entrée d’un autre.

Le panneau de mappage s’affiche lorsque vous cliquez sur un champ dans lequel vous souhaitez insérer une valeur émise par un module précédent dans un scénario. Dans n’importe quel champ disponible pour le mappage au sein d’un module, vous pouvez créer une formule à l’aide de n’importe quelle combinaison de fonctions et d’éléments mappés du panneau de mappage avec le texte statique saisi. Ces éléments peuvent être imbriqués les uns dans les autres.

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

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Lots et éléments

L’opération d’un module produit zéro, un ou plusieurs lots en tant que sortie. Un lot se compose d’un ou de plusieurs éléments.

Pour explorer la sortie d’un module, procédez comme suit :

1. Cliquez sur **[!UICONTROL Exécuter une fois]** pour lancer le module.
1. Cliquez sur la bulle au-dessus du module.

   Un journal contenant toutes les phases du module s’affiche. Vous trouverez le ou les lots émis par la phase d’opération d’un module sous l’en-tête **[!UICONTROL Sortie]**. Chaque lot contient ses éléments et les valeurs de chaque élément.

>[!INFO]
>
>**Exemple :** l’exemple suivant illustre le module [!UICONTROL E-mail] > [!UICONTROL Surveiller les e-mails]. Vous constaterez qu’une opération a été effectuée et produit un seul lot contenant divers éléments, tels que `Date`, `Email ID (UID)`, `size`, etc.
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>Les sorties des modules placés entre un [!UICONTROL itérateur] et [!UICONTROL agrégateur] ne sont pas accessibles au-delà du module [!UICONTROL agrégateur].

## Mapper un élément

Après avoir créé une séquence de modules en les liant, chaque module peut traiter les valeurs des éléments générés par les modules qui le précèdent.

Pour affecter les éléments aux champs de saisie d’un module, procédez comme suit :

1. Cliquez sur le module qui doit traiter la sortie du ou des modules précédents.
1. Dans le panneau Paramètres du module qui s’affiche, cliquez sur un champ dans lequel vous souhaitez utiliser la valeur d’un élément généré à partir d’un ou plusieurs modules précédents.

   Le panneau de mappage s’ouvre.

1. Cliquez sur un élément du panneau de mappage pour l’insérer dans le champ.
1. (Facultatif) Pour trouver un champ spécifique dans le panneau de mappage, cliquez sur la barre de recherche du panneau de mappage et saisissez le terme souhaité. Cliquez sur le champ lorsqu’il apparaît dans la liste.

   Les résultats de recherche contiennent le terme de recherche et ne sont pas sensibles à la casse.

Pour plus d’informations, voir [Configurer les paramètres d’un module dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## Formules

Vous pouvez mapper plusieurs éléments dans un champ, les combiner avec des littéraux (valeurs fixes) et utiliser des opérateurs et des fonctions pour créer des formules complexes :

![](assets/operators-and-functions.png)

Les fonctions et opérateurs sont disponibles dans le panneau de mappage sous l’un de ses onglets.

![](assets/functions-toolbar-350x189.png)

Le premier onglet ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (affiché à l’ouverture du panneau) affiche les éléments que vous pouvez mapper à partir d’autres modules.

Les autres onglets contiennent les types de fonctions suivants :

* **Fonctions générales** ![](assets/toolbar-icon-general-function.png) - Voir [Fonctions générales dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) pour plus d’informations.

* **Fonctions mathématiques** ![](assets/toolbar-icon-math-functions.png) - Voir [Fonctions mathématiques dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) pour plus d’informations.

* **Fonctions de texte et binaires** ![](assets/toolbar-icon-text&binary-functions.png) - Voir [Fonctions de chaîne de caractères dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) pour plus d’informations.

* **Date et heure** ![](assets/toolbar-icon-date&time-functions.png) - Voir [Fonctions de date et d’heure dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) et les articles ci-dessous pour plus d’informations.

   * [Jetons pour le formatage de la date et de l’heure dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Jetons d’analyse de la date et de l’heure dans Adobe Workfront Fusion](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Fonctions relatives à l’utilisation de tableaux** ![](assets/toolbar-icon-functions-for-arrays.png) - Voir [Fonctions de tableau dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) pour plus d’informations.

>[!TIP]
>
>Lorsque vous créez une formule complexe que vous souhaitez réutiliser dans un autre champ, vous pouvez cliquer sur le champ qui contient la combinaison, utiliser Commande-A ou Ctrl-A pour la sélectionner, puis la copier et la coller dans l’autre champ.

Pour plus d’informations sur le mappage des éléments à l’aide de fonctions, voir [Mapper des éléments à l’aide de fonctions dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## Collections

Certains éléments peuvent contenir plusieurs valeurs de différents types. Il s’agit d’éléments de type collection.

Vous pouvez identifier un élément de type [!UICONTROL collection] par le petit rectangle noir affiché à droite du libellé de l’élément et sa liste de sous-éléments automatiquement développée :

![](assets/collection.png)

>[!NOTE]
>
>Dans la plupart des cas, vous mappez les sous-éléments de la collection plutôt que l’élément représentant l’ensemble de la collection.

Pour plus d’informations sur les collections, voir [Types de données d’élément dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

## Tableaux

Certains éléments peuvent contenir plusieurs éléments du même type. Il s’agit d’éléments de type tableau.

Vous pouvez identifier un élément de type tableau par les crochets à la fin du libellé de l’élément. Cliquez sur le petit rectangle noir à droite du libellé de l’élément pour afficher les éléments de l’élément :

![](assets/array.png)

Pour plus d’informations sur les tableaux, voir [Types de données d’élément dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### Mapper le premier élément d’un tableau

Si vous mappez un élément `Recipient name` de tableau, il s’affiche dans le champ comme suit :

![](assets/map-array-1st-element.png)

Le nombre entre crochets est un index qui détermine l’élément du tableau qui sera utilisé. Il est défini sur 1 par défaut.

### Mapper le n-ième élément d’un tableau

Si vous souhaitez accéder à un autre élément, cliquez sur les crochets et modifiez la valeur de l’index :

![](assets/access-another-element.png)

### Mapper l’élément d’un tableau avec une clé donnée

Certains tableaux contiennent plusieurs collections avec des éléments de clé et de valeur. Il s’agit généralement de différents attributs, métadonnées, etc.

L’exemple suivant illustre la sortie de l’application [!DNL Jira].

![](assets/output-of-jira-app-350x100.png)

Dans cet exemple, nous obtenons un nom du fichier provenant d’un tableau de pièces jointes pour la pièce jointe spécifique ayant un ID de 10108.

La sortie de [!DNL Jira] ressemble à ceci :

![](assets/output-from-jira-350x261.png)

En règle générale, il est nécessaire de rechercher un élément par sa valeur de clé donnée et d’obtenir la valeur correspondante de l’élément de valeur. Cela peut être obtenu avec une formule utilisant une combinaison des fonctions `map()` et `get()`.

Vous trouverez ci-dessous une ventilation détaillée de la formule :

1. Le premier paramètre de la fonction `map()` est l’élément de tableau entier.
1. Le deuxième paramètre est le nom brut de l’élément de valeur. Pour obtenir le nom brut, pointez sur l’élément dans le panneau de [!UICONTROL mapping] :

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >Tous les paramètres respectent la casse. Même si, dans cet exemple particulier, le libellé de l’élément ne diffère de son nom brut que par la mise en majuscules, il est nécessaire d’utiliser le nom brut, qui est entièrement en minuscules, contrairement au libellé Valeur.

1. Le troisième paramètre est le nom brut de l’élément clé :

   ![](assets/3rd-parameter-350x166.png)

1. Le quatrième paramètre est la valeur de clé donnée.

Parce que la fonction `map()` renvoie un tableau (puisqu’il peut y avoir plus d’éléments avec la valeur de clé donnée), il est nécessaire d’appliquer la fonction `get()` pour obtenir son premier élément :

* Le premier paramètre de la fonction `get()` est le résultat de la fonction `map()`.

* Le deuxième paramètre est l’index de l’élément - un.

Pour plus d’informations sur la fonction `map()`, voir [Fonctions de tableau dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

Pour plus d’informations sur la fonction `get()`, voir [Fonctions générales dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## Conversion d’éléments en une série de lots

Les tableaux peuvent être convertis en une série de lots à l’aide du module [!UICONTROL Itérateur]. Pour plus d’informations, consultez le module [[!UICONTROL Itérateur] dans [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## Dépannage

### Éléments manquants dans le panneau de mappage

Pour chaque module, le panneau de mappage affiche tous les éléments de sortie, répertoriés par l’auteur ou l’autrice du module. Dans certains cas, cette liste peut être incomplète pour diverses raisons et certains éléments peuvent être manquants. [!DNL Workfront Fusion] peut déterminer automatiquement les éléments de sortie manquants lorsque vous exécutez le module dans l’éditeur de scénario. La procédure exacte diffère légèrement selon le type du module :

#### Déclencheur instantané

1. Cliquez avec le bouton droit sur le module, puis cliquez sur **[!UICONTROL Exécuter ce module uniquement]** dans le menu qui s’affiche.

   S’il n’existe aucun webhook en file d’attente, le module attend qu’un nouveau webhook soit traité.

1. Générez un webhook.

   Par exemple, le module webhook **[!DNL Slack] > [!UICONTROL Écouter les nouveaux événements]** (qui recherche les nouveaux messages de canal dans un canal) envoie un message au canal.

1. Lorsque l’exécution du module est terminée, cliquez sur la bulle au-dessus du module pour explorer sa sortie complète.

   Le panneau de mappage contient tous les éléments qui ont été découverts dans la sortie du module.

#### Déclencheur d’attente active

1. Cliquez avec le bouton droit sur le module, puis cliquez sur **[!UICONTROL Exécuter ce module uniquement]** dans le menu qui s’affiche.
1. Si aucune sortie n’est disponible, cliquez sur **[!UICONTROL Choisir l’emplacement de départ]** et ajustez les paramètres.
1. S’il n’y a aucun événement à traiter, créez-en un et revenez à l’étape 2.

   Par exemple, le module webhook **[!UICONTROL Gmail] > [!UICONTROL Surveiller les e-mails]** envoie un e-mail au dossier que le module surveille.

1. Lorsque l’exécution du module est terminée, cliquez sur la bulle au-dessus du module pour explorer sa sortie complète.

   Le panneau de mappage contient désormais tous les éléments qui ont été découverts dans la sortie du module.

#### Autres modules

Vous pouvez choisir d’exécuter les éléments suivants :

* L’ensemble du scénario (ou seulement la partie contenant le module)

  Si votre scénario commence par un déclencheur, reportez-vous à la section [Déclencheur instantané](#instant-trigger) ou [Déclencheur d’attente active](#polling-trigger) ci-dessus.

* Seulement le module unique

Si vous choisissez d’exécuter seulement le module unique, procédez comme suit :

1. Cliquez avec le bouton droit sur le module, puis cliquez sur **[!UICONTROL Exécuter ce module uniquement]** dans le menu qui s’affiche.
1. Indiquez des exemples de valeurs pour les éléments d’entrée, puis cliquez sur **[!UICONTROL OK]**.
1. Lorsque l’exécution du module est terminée, cliquez sur la bulle au-dessus du module pour explorer sa sortie complète.

   Le panneau de mappage contient désormais tous les éléments qui ont été découverts dans la sortie du module.
