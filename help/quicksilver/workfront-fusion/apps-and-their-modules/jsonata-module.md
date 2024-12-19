---
title: Modules JSONata
description: Le connecteur JSONata d’Adobe Workfront Fusion fournit un module pour traiter les données au format JSON afin qu’Adobe Workfront Fusion puisse continuer à utiliser le contenu des données.
author: Becky
feature: Workfront Fusion
source-git-commit: b7a6ecd9089c3a5517c56b849b860d57a900dade
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 41%

---

# Modules [!UICONTROL JSONata]

Le connecteur [!DNL Adobe Workfront Fusion] [!UICONTROL JSONata] vous permet d’interroger des objets JSON. Ce module ne nécessite pas de connexion.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous disposez du plan de [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter du [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Module JSONata et ses champs

### Evaluate

Ce module d’action interroge un objet JSON et renvoie un tableau.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expression]</td> 
   <td>Saisissez l’expression à utiliser pour évaluer l’objet JSON. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data] </td> 
   <td> Saisissez l’objet JSON à évaluer.  </td> 
  </tr> 
  </tbody>
  </table>

>[!BEGINSHADEBOX]

**Exemple** :

L’objectif est de renvoyer un tableau de noms à partir de l’objet JSON suivant :

```JSON
{
  "people": [
    { "name": "Alice", "age": 30 },
    { "name": "Bob", "age": 25 },
    { "name": "Charlie", "age": 35 }
  ]
}
```

1. Dans le champ d’expression, saisissez `people.name`.
1. Dans le champ de données, saisissez l’objet JSON.

Le module renvoie un tableau de noms extraits de l’objet JSON.

>[!ENDSHADEBOX]
