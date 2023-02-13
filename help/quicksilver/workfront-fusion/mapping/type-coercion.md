---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Contrainte de type dans Adobe Workfront Fusion
description: Ce document décrit comment [!DNL Adobe Workfront Fusion] se comporte dans des situations où il reçoit des valeurs dans des formats de données attendus et inattendus.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 1%

---

# Type de contrainte dans [!DNL Adobe Workfront Fusion]

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

### Contrainte de type

Ce document décrit comment [!DNL Adobe Workfront Fusion] se comporte dans des situations où il reçoit des valeurs dans des formats de données attendus et inattendus.

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Attendu</th> 
   <th>Reçu</th> 
   <th> <p>Description</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>tableau </td> 
   <td>tableau </td> 
   <td> <p>La valeur est transmise telle quelle.</p> </td> 
  </tr> 
  <tr> 
   <td>tableau </td> 
   <td>other </td> 
   <td> <p>Si la valeur reçue n’est pas du type de tableau, [!DNL Workfront Fusion] crée un tableau et le premier élément (et le seul) est la valeur reçue.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>boolean </td> 
   <td> <p>La valeur est transmise telle quelle.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>nombre </td> 
   <td> <p>La valeur est convertie en Oui logique, même si la valeur est 0.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>text </td> 
   <td> <p>Si la valeur est égale à false ou si elle est vide, elle est convertie en Non logique. Dans le cas contraire, il est converti en Oui logique.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>other </td> 
   <td> <p>La valeur est convertie en Oui logique lorsque la valeur reçue existe (elle n’est pas nulle).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>La valeur n’est transmise inchangée que si la page de code est la suivante : Si la page de code diffère, [!DNL Workfront Fusion] essaiera de convertir la valeur reçue en page de code demandée. Si cette conversion n’est pas prise en charge, [!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>boolean </td> 
   <td> <p>La valeur est convertie en texte (vrai/faux), puis en données binaires en suivant les étapes mentionnées ci-dessus pour la conversion en texte.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>date </td> 
   <td> <p>La valeur est convertie en texte ISO 8601, puis en données binaires suivant les étapes mentionnées pour la conversion en texte.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>nombre </td> 
   <td> <p>La valeur est convertie en texte, puis en données binaires en suivant les étapes mentionnées ci-dessus pour la conversion en texte.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>text </td> 
   <td> <p>La valeur est convertie en données binaires et codée comme prévu. Si l'encodage attendu n'est pas spécifié, l'encodage utf8 sera utilisé.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>collection </td> 
   <td>collection </td> 
   <td> <p>La valeur est transmise telle quelle.</p> </td> 
  </tr> 
  <tr> 
   <td>collection </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>date </td> 
   <td> <p>La valeur est transmise telle quelle.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] essaiera de convertir le texte en date. Si la conversion échoue, elle renvoie une erreur de validation. La date doit contenir jour, mois et année. La date peut contenir l’heure et le fuseau horaire. Le fuseau horaire par défaut est basé sur vos paramètres. Exemples:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>nombre </td> 
   <td>nombre </td> 
   <td> <p>La valeur est transmise telle quelle.</p> </td> 
  </tr> 
  <tr> 
   <td>nombre </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] essaiera de convertir le texte en nombre. Si la conversion échoue, elle renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>nombre </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>text </td> 
   <td> <p>La valeur est transmise telle quelle.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>tableau </td> 
   <td> <p>Si le tableau donné prend en charge la conversion en texte, la valeur est convertie. Si ce n’est pas le cas, [!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>boolean </td> 
   <td> <p>La valeur est convertie en texte (vrai/faux).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffer </td> 
   <td> <p>Si le codage de texte est spécifié pour les données binaires, la valeur est convertie en texte. Si ce n’est pas le cas, [!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>date </td> 
   <td> <p>La valeur est convertie en texte ISO 8601.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>nombre </td> 
   <td> <p>La valeur est convertie en texte.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>heure </td> 
   <td>heure </td> 
   <td> <p>La valeur est transmise telle quelle.</p> </td> 
  </tr> 
  <tr> 
   <td>heure </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] essaiera de convertir le temps en heures:minutes:format des secondes. Si la conversion échoue, elle renvoie une erreur de validation.</p> </td> 
  </tr> 
  <tr> 
   <td>heure </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] renvoie une erreur de validation.</p> </td> 
  </tr> 
 </tbody> 
</table>
