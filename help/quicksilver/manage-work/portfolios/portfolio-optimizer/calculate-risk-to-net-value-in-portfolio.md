---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcul du risque par rapport à la valeur nette d’un portefeuille
description: Dans Portfolio Optimizer, la variable [!UICONTROL Risque de valeur nette] mesure le risque potentiel en prenant en compte la valeur nette fournie par tous les projets affichés dans Portfolio Optimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Calculez la variable [!UICONTROL Risque de valeur nette] dans un portfolio

Dans le [!UICONTROL Portfolio Optimizer], la variable [!UICONTROL Risque de valeur nette] l&#39;indicateur mesure le risque potentiel en tenant compte de la variable [!UICONTROL Valeur nette] fourni par tous les projets affichés dans le [!UICONTROL Portfolio Optimizer]. 

Pour optimiser l’efficacité au sein du portfolio, vous souhaitez que la variable [!UICONTROL Risque] est faible et la variable [!UICONTROL Valeur nette] est élevé. 

Le [!UICONTROL Risque] et [!UICONTROL Valeur nette] Les indicateurs sont représentés sous l’angle de leur relation les uns avec les autres.

[!DNL Adobe Workfront] calcule la variable [!UICONTROL Risque] et [!UICONTROL Valeur nette] indicateurs utilisant les formules suivantes :

* Le [!UICONTROL Risque] est calculé par la formule suivante :

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* Le [!DNL Net Value] est calculé par les formules suivantes :

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   Ou

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>Le [!UICONTROL Risque de valeur nette] calcule en fonction des projets que vous affichez dans la variable [!UICONTROL Portfolio Optimizer], et non sur tous les projets associés au portfolio. 
