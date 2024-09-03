---
title: Créer un champ de formule dans la zone de travail de reporting
description: Créer un champ de formule dans la zone de travail de reporting
hidefromtoc: true
hide: true
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 100%

---

# Créer un champ de formule dans la zone de travail de reporting

Le générateur de champs dans la zone de travail de reporting vous permet de créer des champs qui effectuent des calculs personnalisés.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta de la zone de travail de reporting. Pour plus d’informations, voir [Version bêta de la zone de travail de reporting : vue d’ensemble](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Créer un champ de formule

1. Créez un bloc de tableau ou naviguez jusqu’à lui, comme décrit dans [Ajouter ou modifier un bloc de tableau dans la zone de travail de reporting](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. Dans l’en-tête du tableau du rapport, cliquez sur l’icône **Modifier** ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Si vous venez de créer le tableau et que vous n’avez pas encore ajouté de champs, cliquez plutôt sur le bouton Modifier au centre du tableau.

1. Cliquez sur **Nouveau +** en haut de la liste **Champs** dans le panneau de droite.
1. Dans la nouvelle page qui s’ouvre, cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) à côté du nom du champ dans le coin supérieur gauche pour modifier le nom du champ de formule.
1. Faites glisser les **fonctions** ou les **champs** du panneau de gauche sur le créateur de champ au centre pour les ajouter à votre champ de formule.


   >[!TIP]
   >
   >Au fur et à mesure que vous construisez votre champ de formule, l’**aperçu du champ** sur la droite affiche des exemples du champ résultant.

   Chaque fonction contient un certain nombre de rectangles pointillés vides qui seront utilisés comme arguments dans le calcul d’un résultat. Ils peuvent être remplis en saisissant du texte statique ou des nombres, en glissant-déposant un champ à partir du panneau de gauche (en utilisant la valeur du champ dans le calcul), ou en glissant-déposant une autre fonction (en créant une fonction imbriquée). Les fonctions possibles sont les suivantes :

   | Fonction | Description | Sortie |
   |---|---|---|
   | IF | Compare deux arguments en fonction d’un modificateur sélectionné, puis effectue une action spécifiée en fonction de la valeur True (Is True :) ou False (Is False :) qui en résulte. Note : actuellement, le deuxième argument ne peut pas être une valeur statique True ou False. À la place, vous pouvez utiliser une fonction imbriquée comme ISBLANK(Nom du projet) qui renvoie toujours False comme solution de contournement. | True/False, date, nombre ou chaîne de caractères |
   | CONCAT | Fusionne deux ou plusieurs chaînes de caractères bout à bout pour créer une nouvelle chaîne. | Chaîne |
   | CONTIENT | Détermine si un champ d’argument de type chaîne (Trouver le texte) est contenu dans un autre champ d’argument de type chaîne (Dans le texte). | Vrai/Faux |
   | DANS | Évalue si la valeur d’un champ d’argument (Trouver) correspond à la valeur d’au moins un autre champ d’argument (Dans). | Vrai/Faux |
   | ISBLANK | Évalue si un champ d’argument est vide. | Vrai/Faux |
   | LEN | Mesure la longueur (en nombre de caractères) d’un champ d’argument. | Nombre |
   | ARRONDIR | Renvoie un nombre arrondi en fonction de la précision choisie. | Nombre |
   | ARRONDI À L’INFÉRIEUR | Renvoie le nombre entier le plus proche, arrondi à l’unité inférieure. | Nombre |
   | NUMBER | Renvoie l’entier le plus grand inférieur à la valeur d’un argument numérique (identique à la fonction d’arrondi à l’inférieur). | Nombre |
   | STRING | Convertit le contenu d’un champ d’arguments en une chaîne. | Chaîne |
   | SUBSTR | Crée une nouvelle chaîne à partir d’une plus grande chaîne, qui contient les caractères compris entre un numéro d’index (Début) et un autre (Fin). | Chaîne |
   | GAUCHE | Crée une nouvelle chaîne à partir d’une plus grande chaîne, qui contient des caractères en commençant par celui à l’extrémité gauche et en comptant jusqu’à un certain nombre de caractères (Longueur). | Chaîne |
   | DROITE | Crée une nouvelle chaîne à partir d’une plus grande chaîne, qui contient des caractères en commençant par celui à l’extrémité droite et en comptant jusqu’à un certain nombre de caractères (Longueur). | Chaîne |
   | SOM. | Additionne les valeurs de deux champs d’argument ou plus. | Nombre |
   | SUB | Soustrait les valeurs de deux champs d’argument ou plus (dans l’ordre de gauche à droite). | Nombre |
   | PROD | Multiplie les valeurs de deux champs d’argument ou plus. | Nombre |
   | DIV | Divise la valeur de deux champs d’argument ou plus (dans l’ordre de gauche à droite). | Nombre |
   | MOIS | Renvoie un nombre égal à la valeur du mois pour une date. | Nombre |
   | ANNÉE | Renvoie un nombre égal à la valeur de l’année pour une date. | Nombre |
   | DATEDIFF | Calcule le nombre total de jours entre deux dates, arrondi à une décimale. | Nombre |
   | WEEKDAYDIFF | Calcule le nombre de jours de la semaine entre deux dates, arrondi à une décimale. | Nombre |

   {style="table-layout:auto"}

1. Cliquez sur la flèche **Revenir en arrière** dans le coin supérieur gauche de l’écran pour retourner à votre tableau.
