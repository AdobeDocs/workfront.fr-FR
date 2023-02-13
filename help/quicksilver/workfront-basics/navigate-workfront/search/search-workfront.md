---
navigation-topic: search
title: Recherche [!DNL Adobe Workfront]
description: Vous pouvez facilement localiser des éléments dans [!DNL Adobe Workfront] en les recherchant quand vous ne pouvez pas vous rappeler de leur emplacement exact.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 1%

---

# Recherche [!DNL Adobe Workfront]

Vous pouvez facilement localiser des éléments dans [!DNL Adobe Workfront] en les recherchant quand vous ne pouvez pas vous rappeler de leur emplacement exact.

Vous pouvez voir la variable [!UICONTROL Rechercher] dans le coin supérieur droit d’une page dans [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

Vous devez disposer des autorisations nécessaires pour afficher un objet avant de pouvoir le trouver dans une recherche. Pour cette raison, les résultats de recherche varient d’un utilisateur à l’autre.

## Exigences d’accès

+++ Développez cette section pour afficher l’accès nécessaire pour effectuer les étapes de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>Accès à [!UICONTROL View] au type d’objet </p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Vous devez disposer des autorisations nécessaires pour afficher un objet avant de pouvoir le trouver dans une recherche.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

+++

## Présentation de la recherche

* [[!UICONTROL Objets disponibles pour la recherche]](#objects-available-for-search)
* [[!UICONTROL Champs disponibles pour la recherche]](#fields-available-for-search)

### Objets disponibles pour la recherche

Vous pouvez rechercher les objets suivants dans Workfront :

* Projets
* Tâches
* Événements
* Rapports
* Utilisateurs
* Modèles
* Documents
* Portefeuilles
* Programmes
* Tableaux de bord
* Entreprises
* Notes

### Champs disponibles pour la recherche

Les champs disponibles pour la recherche sont basés sur le type de recherche : De base ou [!UICONTROL Recherche avancée].

* **Recherche de base**: Lors de la recherche d’objets dans une recherche de base, [!DNL Workfront] recherche du texte pouvant contenir vos mots-clés dans les champs suivants :

   * Noms d’objet
   * Descriptions
   * Champs de données personnalisés
   * Mises à jour
   * Noms de document (dans des recherches de documents spécifiques et dans une recherche de base)

   Pour plus d’informations sur la recherche de base dans [!DNL Workfront], voir [Recherche de base](#basic-search) dans cet article.

* **[!UICONTROL Recherche avancée]**: Dans un [!UICONTROL Recherche avancée], vous pouvez configurer des filtres pour rechercher des champs non disponibles dans la recherche de base. Par conséquent, [!UICONTROL Recherche avancée] vous permet de rechercher n’importe quel champ de l’objet.

   Pour plus d’informations sur [!UICONTROL Recherche avancée], voir [Recherche avancée](#advanced-search) dans cet article.

>[!NOTE]
>
>Pour effectuer une [!UICONTROL Recherche avancée], vous devez sélectionner la variable [!UICONTROL Recherche avancée] lors du début de la recherche. Vous ne pouvez pas affiner une recherche de base dans une [!UICONTROL Recherche avancée].

## Comprendre les limites de [!DNL Workfront] recherches

Tenez compte des restrictions suivantes lors de l’utilisation de [!UICONTROL Rechercher] in [!DNL Workfront]:

* Les recherches ne sont pas sensibles à la casse
* [!DNL Workfront] ne corrige pas ou ne comprend pas les fautes de frappe
* Recherche dans [!DNL Workfront] ne prend pas en charge les caractères génériques
* Recherche dans [!DNL Workfront] prend en charge les recherches de mots partielles, mais ne prend pas en charge les recherches de sous-chaînes.\
   Par exemple, le mot-clé de recherche &quot;stand&quot; renvoie des résultats comprenant le mot &quot;standard&quot;, mais ne renvoie pas de résultats comprenant le mot &quot;understand&quot;.

## Recherche de plusieurs mots

Lorsque vous incluez plusieurs mots dans une recherche et que vous ne souhaitez trouver que les objets qui correspondent à tous les mots de la zone de recherche, vous pouvez les entrer dans n’importe quel ordre.

Par exemple, la recherche de &quot;Démo marketing&quot; (sans guillemets) recherche des objets portant les noms suivants :

* Démonstration marketing
* Démonstration marketing
* Démonstration de l’analyse du marché de janvier

Il trouve également les objets pouvant avoir &quot;Marketing&quot; dans le nom et &quot;Demo&quot; dans la description.

Cependant, vous pouvez effectuer les opérations suivantes dans la variable [!UICONTROL Rechercher] pour ajuster les résultats de recherche qui s’affichent :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Inclure des guillemets</td> 
   <td> <p>La saisie de mots dans l’ordre correct au sein de guillemets doubles permet de ne trouver que les objets correspondant exactement à.<br>Par exemple, la recherche de "Démo marketing" (avec guillemets) recherche des objets portant les noms suivants :</p> 
    <ul> 
     <li> Démonstration marketing</li> 
     <li> Démonstration marketing de janvier</li> 
     <li>Plan de démonstration marketing</li> 
    </ul> <p>Toutefois, cette recherche ne trouvera pas d’objet nommé "Demo Marketing".</p> </td> 
  </tr> 
  <tr> 
   <td>Inclure OU</td> 
   <td> <p>La connexion de mots par "OR" (sans guillemets) permet de trouver uniquement les objets correspondant à au moins un des mots de la zone [!UICONTROL Search]. Ces mots peuvent être entrés dans n’importe quel ordre.<br>Par exemple, si vous recherchez "Marketing OR Demo" (sans guillemets), les objets portant les noms suivants sont recherchés :</p> 
    <ul> 
     <li> Démonstration de l’analyse du marché</li> 
     <li>Démonstration de l’analyse du marché de janvier</li> 
     <li>Démonstration</li> 
     <li>Analyse du marché</li> 
    </ul> <p>Remarque : "OU" doit être en majuscules. Sinon, il est interprété comme un autre mot de l’expression que vous recherchez.</p> </td> 
  </tr> 
  <tr> 
   <td>Inclure ET</td> 
   <td> <p>La connexion de mots par "AND" (sans guillemets) permet de trouver uniquement les objets qui correspondent à tous les mots de la zone [!UICONTROL Rechercher]. Ces mots peuvent être entrés dans n’importe quel ordre.<br>Par exemple, la recherche de "Marketing AND Demo" (sans guillemets) recherche des objets portant les noms suivants :</p> 
    <ul> 
     <li>Démonstration marketing</li> 
     <li>Démonstration marketing</li> 
     <li>Démonstration de l’analyse du marché de janvier</li> 
    </ul> <p>Remarque : "AND" doit être en majuscules. Sinon, il est interprété comme un autre mot de l’expression que vous recherchez. De même, l’inclusion de "&amp;" (sans guillemets) recherche uniquement les objets contenant l’esperluette.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Utiliser la recherche dans [!DNL Workfront]

[!DNL Workfront] propose deux types de recherche : De base et avancé. Utilisez la recherche de base si vous souhaitez trouver des mots-clés dans des champs d’objet communs tels que le nom ou la description. Utilisation [!UICONTROL Recherche avancée] si vous souhaitez utiliser des filtres pour rechercher d’autres champs d’objet.

* [Recherche simple](#basic-search)
* [Recherche avancée](#advanced-search)

### Recherche simple

Une recherche de base vous permet de rechercher des mots-clés sur tous les objets du système ou sur un seul objet à la fois (comme les projets). [!DNL Workfront] puis recherche ces mots-clés dans quelques champs spécifiques. Vous pouvez ensuite affiner vos résultats de recherche en fonction d’autres champs spécifiques à l’objet sélectionnés par [!DNL Workfront].

Pour obtenir la liste des champs spécifiques recherchés dans la recherche de base, voir [Champs disponibles pour la recherche](#fields-available-for-search) dans cet article.

>[!NOTE]
>
>Pour effectuer une [!UICONTROL Recherche avancée], vous devez sélectionner la variable [!UICONTROL Recherche avancée] lors du début de la recherche. Vous ne pouvez pas affiner une recherche de base dans une [!UICONTROL Recherche avancée].

* [Exécution d’une recherche de base](#perform-a-basic-search)
* [Affiner une recherche de base](#refine-a-basic-search)

#### Exécution d’une recherche de base

Vous pouvez effectuer une recherche de base de l’une des façons suivantes :

* Sur tous les objets du système (recherche générale).
* Sur un seul objet à la fois (recherche spécifique à un objet).

Pour effectuer une recherche de base :

1. Cliquez sur la loupe ![](assets/search-icon.png) dans le coin supérieur droit de la page. Vous pouvez également saisir **[!UICONTROL ALT + /]** ou **[!UICONTROL Option + /]** pour ouvrir le [!UICONTROL Rechercher] .

1. (Facultatif) Pour rechercher un objet spécifique, cliquez sur le bouton **[!UICONTROL Tous]** et sélectionnez l’objet à rechercher.

   ![](assets/search-objecttype.png)

1. Dans le **[!UICONTROL Rechercher]** , commencez à saisir les informations que vous recherchez.\
   Pour plus d’informations sur les champs recherchés dans [!DNL Workfront], voir [Présentation de la recherche](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   Lorsque vous commencez à saisir du texte dans la barre de recherche, [!DNL Workfront] effectue des recommandations en fonction de votre historique de consultation et met en surbrillance le mot-clé que vous recherchez en bleu.

1. Si l’élément que vous recherchez s’affiche dans la variable [!UICONTROL typeforward] , cliquez dessus.

   Ou

   Press **[!UICONTROL Entrée]** pour effectuer une recherche complète. Cette recherche interroge l’ensemble de la base de données au lieu des éléments que vous avez récemment consultés.

   Le [!UICONTROL Résultats de la recherche] Les diapositives de la page s’ouvrent à gauche et couvrent la plupart de la page précédente.

   Si vous avez effectué une recherche générale, [!DNL Workfront] renvoie des résultats pour tout objet qui correspond au terme recherché dans l’un des champs recherchés, comme décrit dans la section [Présentation de la recherche](#understand-search). Les objets correspondant à votre recherche s’affichent dans une liste.

   >[!NOTE]
   >
   >Parfois, des variantes d’un mot s’affichent dans la liste des éléments trouvés.\
   >Par exemple, la recherche de &quot;marketing&quot; affiche les objets qui contiennent &quot;marketing&quot; ou &quot;marché&quot; dans le nom.

1. (Facultatif) Si votre recherche a généré trop de résultats, affinez votre recherche comme décrit dans la section [Affiner une recherche de base](#refine-a-basic-search).
1. (Facultatif) Pour revenir à la page sur laquelle vous vous trouviez avant la recherche, cliquez sur **[!UICONTROL Fermer]** dans le coin supérieur droit.

>[!NOTE]
>
>Le [!UICONTROL Résultats de la recherche] ne reste ouverte que lorsqu’elle est active. Si vous cliquez en dehors de la page ou si vous ouvrez une autre page, la fonction [!UICONTROL Résultats de la recherche] page.

#### Affiner une recherche de base

Après avoir effectué une recherche de base, comme décrit dans [[!UICONTROL Exécution d’une recherche de base]](#perform-a-basic-search): vous pouvez affiner la recherche.

Utilisez la barre d’outils située à gauche des résultats de recherche pour réduire les informations que vous recherchez.

Pour affiner une recherche :

1. (Conditionnel) Si vous avez effectué une recherche générale, sélectionnez l’objet que vous recherchiez dans la liste des objets située dans le coin supérieur gauche de vos résultats.
1. Localisez les champs disponibles pour les objets affichés dans la recherche dans la barre d’outils située à gauche de vos résultats.\
   Les valeurs de chaque champ s’affichent, triées par nombre, jusqu’à 10 valeurs pour chaque champ.
1. Cliquez dans l’un des champs disponibles pour raccourcir la liste des résultats.\
   Les sélections que vous effectuez sont surlignées en bleu et les valeurs de champ que vous ne sélectionnez pas sont masquées.\
   Après avoir sélectionné chaque nouvelle valeur, les résultats sont dynamiquement mis à jour.\
   ![](assets/qs-refine-search-350x175.png)

1. (Facultatif) Cliquez sur les valeurs sélectionnées pour les désélectionner et afficher à nouveau toutes les valeurs de chaque champ.

### [!UICONTROL Recherche avancée]

[!UICONTROL Recherche avancée] vous permet de rechercher à l’aide de champs et de filtres non disponibles pour la recherche de base. Par exemple, vous pouvez rechercher des projets avec une priorité spécifique ou un nom de propriétaire de document.

>[!NOTE]
>
>Pour effectuer une [!UICONTROL Recherche avancée], vous devez sélectionner la variable [!UICONTROL Recherche avancée] lors du début de la recherche. Vous ne pouvez pas affiner une recherche de base dans une [!UICONTROL Recherche avancée].

* [Utilisez la fonctionnalité de [!UICONTROL Recherche avancée]](#use-advanced-search)

#### Utilisez la fonctionnalité de [!UICONTROL Recherche avancée]

Vous pouvez utiliser [!UICONTROL Recherche avancée] pour filtrer votre recherche selon des critères spécifiques.\
Ce type de recherche s’avère utile lorsque vous ne pouvez pas mémoriser un mot-clé associé à un objet, mais que vous connaissez des informations spécifiques sur cet objet (par exemple : Priorité du projet, nom du propriétaire du document, etc.).

Pour effectuer une recherche avancée :

1. Dans le coin supérieur droit d’une page de [!DNL Workfront], cliquez sur le bouton **[!UICONTROL Rechercher]** icon ![](assets/search-icon.png). Le [!DNL Search] s’affiche.

1. Au bas de la [!UICONTROL Rechercher] , cliquez sur **[!UICONTROL Recherche avancée]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   Le [!UICONTROL Recherche avancée] Les diapositives de page s’ouvrent à droite et couvrent la plupart de la page précédente.

1. Sélectionnez le type d’objet que vous recherchez.\
   **[!UICONTROL Projets]** est sélectionné par défaut.

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. (Facultatif) Saisissez un mot-clé dans le champ situé en haut de la liste.
1. (Facultatif) Cliquez sur **[!UICONTROL Filtrage des résultats]** pour filtrer les résultats de recherche en fonction de types de champ spécifiques, sélectionnez un champ dans la liste. Au besoin, sélectionnez également une valeur pour le champ.\
   Ou\
   Ajoutez un nouveau filtre.

1. Cliquez sur **[!UICONTROL Rechercher]**.\
   Une liste des éléments correspondant à votre recherche s’affiche à droite du champ [!UICONTROL Recherche avancée] de la barre d’outils.

1. (Facultatif) Pour revenir à la page sur laquelle vous vous trouviez avant la recherche, cliquez sur **[!UICONTROL Fermer]** dans le coin supérieur droit.

>[!NOTE]
>
>Le [!UICONTROL Résultats de la recherche] ne reste ouverte que lorsqu’elle est active. Si vous cliquez en dehors de la page ou si vous ouvrez une autre page, la fonction [!UICONTROL Résultats de la recherche] page.
