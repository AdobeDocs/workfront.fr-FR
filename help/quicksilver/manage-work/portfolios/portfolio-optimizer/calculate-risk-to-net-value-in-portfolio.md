---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calculer le rapport risque/valeur nette d’un portfolio
description: Dans Portfolio Optimizer, l’indicateur [!UICONTROL Risque par rapport à la valeur nette] mesure le Risque potentiel en prenant en compte la valeur nette fournie par tous les projets affichés dans Portfolio Optimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 5%

---

# Calculer le [!UICONTROL risque vers la valeur nette] dans un portefeuille

Dans [!UICONTROL Portfolio Optimizer], l’indicateur [!UICONTROL  Risk to Net Value] mesure le risque potentiel en tenant compte de la [!UICONTROL valeur réseau] fournie par tous les projets affichés dans [!UICONTROL Portfolio Optimizer]. 

Pour optimiser l’efficacité au sein du portefeuille, vous souhaitez vérifier que l’indicateur [!UICONTROL Risk] est faible et que l’indicateur [!UICONTROL Net Value] est élevé. 

Les indicateurs [!UICONTROL Risk] et [!UICONTROL Net Value] sont représentés du point de vue de leur relation les uns avec les autres.

[!DNL Adobe Workfront] calcule les indicateurs [!UICONTROL Risk] et [!UICONTROL Net Value] à l&#39;aide des formules suivantes :

* L&#39;indicateur [!UICONTROL Risk] est calculé par la formule suivante :

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* L&#39;indicateur [!DNL Net Value] est calculé par les formules suivantes :

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  Ou

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>L’indicateur [!UICONTROL Risque jusqu’à la valeur nette] se calcule en fonction des projets que vous affichez dans l’ [!UICONTROL Portfolio Optimizer], et non sur tous les projets associés au portefeuille. 
