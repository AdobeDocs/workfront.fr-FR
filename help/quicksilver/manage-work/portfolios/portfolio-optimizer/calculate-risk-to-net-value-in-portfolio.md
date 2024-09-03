---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calculer le rapport risque/valeur nette d’un portfolio
description: Dans l’optimisateur de portfolio, l’indicateur [!UICONTROL Risque/valeur nette] mesure le risque potentiel en prenant en compte la valeur nette fournie par tous les projets affichés dans l’optimisateur de portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 100%

---

# Calculer le [!UICONTROL Risque/valeur nette] dans un portfolio

Dans l’[!UICONTROL optimisateur de portfolio], l’indicateur [!UICONTROL Risque/valeur nette] mesure le risque potentiel en tenant compte de la [!UICONTROL Valeur nette] fournie par tous les projets affichés dans l’[!UICONTROL optimisateur de portfolio].

Pour optimiser l’efficacité au sein du portfolio, vous souhaitez que l’indicateur [!UICONTROL Risque] soit faible et que l’indicateur [!UICONTROL Valeur nette] soit élevé.

Les indicateurs [!UICONTROL Risque] et [!UICONTROL Valeur nette] sont représentés sous l’angle de leur relation l’un envers l’autre.

[!DNL Adobe Workfront] calcule les indicateurs [!UICONTROL Risque] et [!UICONTROL Valeur nette] en utilisant les formules suivantes :

* L’indicateur [!UICONTROL Risque] est calculé par la formule suivante :

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* L’indicateur [!DNL Net Value] est calculé par les formules suivantes :

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  Ou

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>L’indicateur [!UICONTROL Risque/valeur nette] calcule en fonction des projets que vous affichez dans l’[!UICONTROL optimisateur de portfolio], et non de tous les projets associés au portfolio.
