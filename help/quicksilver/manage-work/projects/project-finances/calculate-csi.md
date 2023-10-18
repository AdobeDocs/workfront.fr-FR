---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcul de l’index de performance de la planification des coûts (CSI)
description: L’indice de performance de la planification des coûts (CSI) est un calcul automatique qui combine l’indice de performance des coûts (IPC) et l’indice de performance de la planification (SPI) en une mesure générale qui équilibre les coûts et la planification.
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: 1cf679376517293f0e0f28b461bd9ecab9283035
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Calcul de l’index de performance de la planification des coûts (CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Présentation de l’indice de performance de la planification des coûts (CSI)

L’indice de performance de la planification des coûts (CSI) est un calcul automatique qui combine l’indice de performance des coûts (IPC) et l’indice de performance de la planification (SPI) en une mesure générale qui équilibre les coûts et la planification. Si vous multipliez ces valeurs, une seule mesure peut comptabiliser un planning prolongé à un budget inférieur ou vice versa. Les chefs de projet peuvent l’utiliser pour déterminer l’intégrité générale du projet ou de la tâche lorsque le coût est sacrifié pour planifier le milieu du projet.

>[!TIP]
>
>Adobe Workfront calcule CSI pour les tâches et les projets. Workfront ne calcule pas de valeur CSI pour les problèmes.

Vous ne pouvez bénéficier des informations fournies par cette mesure que si les éléments suivants existent dans votre entreprise :

* Vos utilisateurs ouvrent une session pour le travail qu’ils terminent.\
  Ceci calcule Les Experts En Fonction Des Heures.
* Les taux de coût par heure sont associés à vos utilisateurs ou rôles de tâche. 

  Cela calcule les CSI en fonction des coûts.

## Comment Workfront calcule l’index de performance de la planification des coûts (CSI)

Workfront calcule l’indice de performance des coûts (CSI) d’un projet ou d’une tâche à l’aide de la formule suivante :

`CSI = CPI x SPI`

Pour plus d’informations sur l’IPC, voir l’article [Calculer l’indice de performance des coûts (IPC)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Pour plus d’informations sur SPI, voir l’article [Calcul de l’index de performance de planification (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI a les trois valeurs possibles suivantes :

* 1 = Suivre le plan général
* \>1 = Combinaison du planning de budget
* &lt;1 = Combinaison de planning de dépassement de budget

![](assets/csi-highlighted.png)

## Localisation de l’index de performance de la planification des coûts (CSI)

>[!CAUTION]
>
>Vous devez avoir accès à l’option Afficher les données financières de votre niveau d’accès et aux autorisations d’afficher le projet ou la tâche pour pouvoir voir la valeur CSI d’un projet ou d’une tâche.

Vous pouvez trouver CSI dans les zones suivantes de Workfront :

* Zone Finance dans la section Détails du projet .
* Zone Finance dans la section Détails de la tâche.
* Un affichage de projet ou de tâche
* Un rapport de projet ou de tâche
