---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer l’Indice Coûts Horaire Performances (CSI)
description: L’Indice Coûts Horaire Performances (CSI) est un calcul automatique qui combine l’Indice Coûts Performance (ICP) et l’Indice Horaire Perdormances (SPI) en une mesure générale qui équilibre les coûts et le planning.
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 99%

---

# Calculer l’Indice Coûts Horaire Performances (CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Vue d’ensemble de l’Indice Coûts Horaire Performances (CSI)

L’Indice Coûts Horaire Performances (CSI) est un calcul automatique qui combine l’Indice Coûts Performance (ICP) et l’Indice Horaire Perdormances (SPI) en une mesure générale qui équilibre les coûts et le planning. Si vous multipliez ces valeurs, une seule mesure peut expliquer un planning prolongé à un budget réduit ou vice versa. Les personnes gestionnaires de projet peuvent l’utiliser pour déterminer l’intégrité générale du projet ou de la tâche lorsque le coût est sacrifié pour respecter le planning à mi-projet.

>[!TIP]
>
>Adobe Workfront calcule le CSI pour les tâches et les projets. Workfront ne calcule pas le CSI des problèmes.

Vous ne pouvez bénéficier des informations fournies par cette mesure que si les conditions suivantes sont remplies :

* Vos utilisateurs et utilisatrices consignent les heures pour le travail effectué.\
  Le CSI sera calculé en fonction des heures.
* Des taux de coût par heure sont associés à vos utilisateurs et utilisatrices ou fonctions. 

  Le CSI sera calculé en fonction des coûts.

## Calcul de l’Indice Coûts Horaire Performances (CSI) par Workfront

Workfront calcule l’Indice Coûts Horaire Performances (CSI) d’un projet ou d’une tâche à l’aide de la formule suivante :

`CSI = CPI x SPI`

Pour plus d’informations sur l’ICP, voir l’article [Calculer l’Indice Coûts Performances (ICP)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Pour plus d’informations sur le SPI, voir l’article [Calcul de l’Indice Horaire Performances (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

Le CSI a les trois valeurs possibles suivantes :

* 1 = Suit le plan général.
* \>1 = Est inférieur à la combinaison du planning et des coûts.
* &lt;1 = Est supérieur à la combinaison du planning et des coûts.

![ICH](assets/csi-highlighted.png)

## Localiser l’Indice Coûts Horaire Performances (CSI)

>[!CAUTION]
>
>Vous devez avoir un accès en affichage aux données financières de votre niveau d’accès et des autorisations d’affichage sur le projet ou la tâche pour voir la valeur du CSI d’un projet ou d’une tâche.

Vous trouverez le CSI dans les zones suivantes de Workfront :

* Zone Finance dans la section Détails du projet.
* Zone Finance dans la section Détails de la tâche.
* Vue de projet ou de tâche.
* Rapport de projet ou de tâche.
