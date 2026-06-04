---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calculer le rapport risque/valeur nette d’un portfolio
description: Dans l’optimisateur de portfolio, l’indicateur [!UICONTROL Risque/valeur nette] mesure le risque potentiel en prenant en compte la valeur nette fournie par tous les projets affichés dans l’optimisateur de portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
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
