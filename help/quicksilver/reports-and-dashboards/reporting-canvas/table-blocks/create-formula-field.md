---
title: Créer un champ de formule dans le canevas de création de rapports
description: Créer un champ de formule dans le canevas de création de rapports
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: ca70952bf0acd71f748b042852d434b560727a83
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 7%

---


# Créer un champ de formule dans le canevas de création de rapports

Le créateur de champs du Canevas de création de rapports vous permet de créer des champs qui effectuent des calculs personnalisés.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, voir [Version bêta du canevas de création de rapports : aperçu](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Créer un champ de formule

1. Créez ou accédez à un bloc de tableau, comme décrit dans la section [Ajouter ou modifier un bloc de tableau dans le canevas de création de rapports](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. Dans l’en-tête du tableau du rapport, cliquez sur le **Modifier** icon ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Si vous venez de créer le tableau et n’avez encore ajouté aucun champ, cliquez sur le bouton Editer situé au centre du tableau.

1. Cliquez sur **Nouveau +** en haut de la page **Champs** dans le panneau de droite.
1. Dans la nouvelle page qui s’ouvre, cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png) en regard du nom du champ dans le coin supérieur gauche pour modifier le nom du champ de formule.
1. Faire glisser **Fonctions** ou **Champs** du panneau de gauche au créateur de champs au centre pour les ajouter à votre champ de formule.


   >[!TIP]
   >
   >Lorsque vous créez votre champ de formule, la variable **Aperçu du champ** à droite affiche des exemples du champ obtenu.

   Chaque fonction contient un certain nombre de rectangles en pointillés vides qui seront utilisés comme arguments dans le calcul d’un résultat. Elles peuvent être renseignées en saisissant du texte ou des nombres statiques, en faisant glisser et en déposant un champ à partir du panneau de gauche (à l’aide de la valeur du champ dans le calcul), ou en faisant glisser une autre fonction (créant une fonction imbriquée). Les fonctions possibles sont les suivantes :

   | Fonction | Description | Sortie |
   |---|---|---|
   | IF | Comparez deux arguments basés sur un modificateur sélectionné, puis effectuez une action spécifiée en fonction de la valeur True (Is True:) ou False (Is False:) obtenue. Remarque : actuellement, le deuxième argument ne peut pas être une valeur statique True ou False. Vous pouvez plutôt utiliser une fonction imbriquée telle que ISBLANK(Project Name) qui renvoie toujours la valeur False comme solution. | True/False, Date, Number ou String |
   | CONCAT | Fusionnez plusieurs chaînes de bout en bout pour créer une nouvelle chaîne. | Chaîne |
   | CONTIENT | Évaluez si un champ d’argument de chaîne (Rechercher du texte) est contenu dans un autre champ d’argument de chaîne (Dans du texte). | Vrai/Faux |
   | DANS | Évaluer si la valeur d’un champ d’argument (Find) correspond à la valeur d’au moins un autre champ d’argument (Within) | Vrai/Faux |
   | ISBLANK | Évaluez si un champ d’argument est vide. | Vrai/Faux |
   | LEN | Permet de mesurer la longueur (en nombre de caractères) d’un champ d’argument. | Nombre |
   | ARRONDIR | Renvoie un nombre arrondi en fonction de la précision sélectionnée. | Nombre |
   | ARRONDI À L’INFÉRIEUR | Renvoie le nombre entier le plus proche, arrondi au bas. | Nombre |
   | NUMBER | Renvoie le plus grand entier inférieur à la valeur d’un argument numérique (identique à une fonction Floor). | Nombre |
   | STRING | Convertit le contenu d’un champ d’argument en chaîne | Chaîne |
   | SUBSTR | Créez une nouvelle chaîne à partir d’une chaîne plus grande, qui contient les caractères entre un numéro d’index (Début) et un autre (Fin). | Chaîne |
   | GAUCHE | Créez une nouvelle chaîne à partir d’une chaîne plus grande, qui contient des caractères commençant par le plus à gauche et comptant à droite un certain nombre de caractères (Longueur). | Chaîne |
   | DROITE | Créez une nouvelle chaîne à partir d’une chaîne plus grande, qui contient des caractères commençant par le plus à droite et comptant un certain nombre de caractères (Longueur). | Chaîne |
   | SOM. | Ajoutez ensemble les valeurs de deux champs d’argument ou plus. | Nombre |
   | SUB | Soustrayez les valeurs de plusieurs champs d’argument (de gauche à droite). | Nombre |
   | PROD | Multipliez les valeurs de deux champs d’argument ou plus. | Nombre |
   | DIV | Divisez la valeur de plusieurs champs d’argument (dans l’ordre de gauche à droite). | Nombre |
   | MOIS | Renvoie un nombre égal à la valeur du mois pour une date. | Nombre |
   | ANNÉE | Renvoie un nombre égal à la valeur de l’année pour une date. | Nombre |
   | DATEDIFF | Calcule le nombre total de jours entre deux dates, arrondi à une décimale. | Nombre |
   | WEEKDAYDIFF | Calcule le nombre de jours de la semaine entre deux dates, arrondi à une décimale. | Nombre |

   {style="table-layout:auto"}

1. Cliquez sur le bouton **Revenir** flèche dans le coin supérieur gauche de l’écran pour revenir à votre tableau.
