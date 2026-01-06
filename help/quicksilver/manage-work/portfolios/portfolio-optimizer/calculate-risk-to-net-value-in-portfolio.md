---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calculer le rapport risque/valeur nette d’un portfolio
description: Dans l’optimisateur de portfolio, l’indicateur [!UICONTROL Risque/valeur nette] mesure le risque potentiel en prenant en compte la valeur nette fournie par tous les projets affichés dans l’optimisateur de portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 52%

---

# Calculer le [!UICONTROL Risque/valeur nette] dans un portfolio

Dans [!UICONTROL Portfolio Optimizer], l&#39;indicateur [!UICONTROL Risque à la valeur nette] mesure le risque potentiel en prenant en compte la [!UICONTROL Valeur nette] fournie par tous les projets affichés dans [!UICONTROL Portfolio Optimizer].

Pour optimiser l&#39;efficacité au sein du portefeuille, vous devez veiller à ce que l&#39;indicateur [!UICONTROL Risque] soit faible et que l&#39;indicateur [!UICONTROL Valeur nette] soit élevé.

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
>L&#39;indicateur [!UICONTROL Risque par rapport à la valeur nette] est calculé en fonction des projets que vous affichez dans [!UICONTROL Portfolio Optimizer], et non en fonction de tous les projets associés au portefeuille.
