---
content-type: reference
product-area: reporting
keywords: audit, journal, personnalisé, champ
navigation-topic: calculate-custom-data-reports
title: 'Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ'
description: Si les utilisateurs et utilisatrices mettent régulièrement à jour les champs personnalisés et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi que la date à laquelle ces modifications ont eu lieu, vous pouvez capturer ces informations dans un champ personnalisé calculé.
author: Courtney
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 55%

---

# Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ

Si les utilisateurs et utilisatrices mettent régulièrement à jour les champs personnalisés et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi que la date à laquelle ces modifications ont eu lieu, vous pouvez capturer ces informations dans un champ personnalisé calculé.

The following example shows you how to build the Instructions Edit History calculated field to capture all the change made to a single-line text field called Instructions.

>[!TIP]
>
>Vous pouvez suivre cet exemple pour tous les types de champs personnalisés, et pas seulement pour les champs de texte d’une seule ligne.

This does this following:

* Limits the Instructions Edit History field to the most recent 2000 characters to stay within the Workfront database limit.
* Checks if the current value of the Instructions field matches the front of the Instructions Edit History value; it assumes it is blank and if it is not, it does the following:

   * If they match, it leaves the Instructions Edit History as is;
   * If they do not match, it replaces the Instructions Edit History with the latest value in the Instructions field, followed by the current date in parentheses, a vertical bar, and the previous Instructions Edit History, which preserves the previous value(s) and the date(s) when they were entered.

## Conditions d’accès

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Package Adobe Workfront</p> </td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configurations des niveaux d’accès</p></td> 
   <td> <p>Administrative access to Custom Forms</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet</p> </td> 
   <td> <p>Autorisations de gestion sur les formulaires personnalisés</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Pour ajouter un champ calculé qui affiche l’historique des modifications d’un champ dans un formulaire personnalisé, vous devez tout d’abord :

* Créer le formulaire personnalisé
* Ajouter le champ dont vous voulez capturer l’historique au formulaire personnalisé

## Afficher l’historique des modifications d’un champ

1. Accéder au formulaire personnalisé dans lequel vous souhaitez ajouter le champ calculé.

1. Pour créer un champ personnalisé de texte sur une seule ligne, par exemple, procédez comme suit :

   1. Click **Single line text**.
   1. Specify a **Label** for the custom field. For example, you can name it &quot; Instructions&quot;.
   1. Cliquez sur **Appliquer**.

1. Cliquez sur **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Specify a **Label** for the calculated custom field. For example, you can name it &quot;Instructions Edit History&quot;.

   This is the field that will capture any changes made to the first field you created (&quot;Instructions&quot;).

1. Cliquez sur **Enregistrer et fermer**.
1. Cliquez sur le nom du formulaire dans lequel vous avez ajouté deux champs pour le rouvrir.
1. Click the calculated custom field **Instructions Edit History**, then copy and paste the following in the **Calculation** box:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recommandé) Collez le même calcul dans le champ **Instructions** sur le champ calculé du formulaire.
1. Make sure that  **Text** is selected in the **Format** field to format the calculated custom field as text.

   Il s’agit de la valeur par défaut.

1. Cliquez sur **Enregistrer et fermer**.

   Now, when you attach the custom form to an object and then someone changes the information in the **Instructions** field, the **Instructions Edit History** field displays the latest value, followed by the current date in parentheses, and a vertical bar. Si d’autres modifications sont apportées, elles sont ajoutées à ces informations de la même manière.

   Dans le calcul ci-dessus, vous pouvez remplacer *Instructions* par le nom exact de votre champ de texte à une seule ligne dont vous voulez suivre l’historique, et **Historique des modifications des instructions** par le nom exact de votre champ calculé.
