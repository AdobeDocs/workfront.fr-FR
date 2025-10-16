---
content-type: reference
product-area: reporting
keywords: audit, journal, personnalisé, champ
navigation-topic: calculate-custom-data-reports
title: 'Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ'
description: Si les utilisateurs et utilisatrices mettent régulièrement à jour les champs personnalisés et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi que la date à laquelle ces modifications ont eu lieu, vous pouvez capturer ces informations dans un champ personnalisé calculé.
author: Jenny
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 54%

---

# Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ

Si les utilisateurs et utilisatrices mettent régulièrement à jour les champs personnalisés et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi que la date à laquelle ces modifications ont eu lieu, vous pouvez capturer ces informations dans un champ personnalisé calculé.

L&#39;exemple suivant montre comment créer le champ calculé Instructions Edit History pour capturer toutes les modifications apportées à un champ de texte d&#39;une seule ligne appelé Instructions.

>[!TIP]
>
>Vous pouvez suivre cet exemple pour tous les types de champs personnalisés, et pas seulement pour les champs de texte d’une seule ligne.

Cela permet d’effectuer les opérations suivantes :

* Limite le champ Instructions Modifier l’historique aux 2 000 caractères les plus récents afin de respecter la limite de la base de données Workfront.
* Vérifie si la valeur actuelle du champ Instructions correspond au recto de la valeur Instructions Modifier l’historique ; il suppose qu’elle est vide et dans le cas contraire, il effectue les opérations suivantes :

   * S’ils correspondent, les instructions Modifier l’historique restent inchangées ;
   * S’ils ne correspondent pas, il remplace l’historique de modification des instructions par la dernière valeur du champ Instructions, suivie de la date actuelle entre parenthèses, d’une barre verticale et de l’historique de modification des instructions précédent, ce qui conserve la ou les valeurs précédentes et la ou les dates auxquelles elles ont été saisies.

## Conditions d’accès

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Package Adobe Workfront</p> </td> 
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
   <td> <p>Accès administratif à Custom Forms</p> </td> 
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

   1. Cliquez sur **Texte monoligne**.
   1. Spécifiez un **Libellé** pour le champ personnalisé. Par exemple, vous pouvez le nommer « Instructions ».
   1. Cliquez sur **Appliquer**.

1. Cliquez sur **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Spécifiez un **Libellé** pour le champ personnalisé calculé. Par exemple, vous pouvez le nommer « Instructions Modifier l’historique ».

   Il s’agit du champ qui capture toutes les modifications apportées au premier champ que vous avez créé (« Instructions »).

1. Cliquez sur **Enregistrer et fermer**.
1. Cliquez sur le nom du formulaire dans lequel vous avez ajouté deux champs pour le rouvrir.
1. Cliquez sur le champ personnalisé calculé **Instructions Modifier l’historique**, puis copiez et collez les éléments suivants dans la zone **Calcul** :

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recommandé) Collez le même calcul dans le champ **Instructions** sur le champ calculé du formulaire.
1. Assurez-vous que **Texte** est sélectionné dans le champ **Format** pour mettre en forme le champ personnalisé calculé en tant que texte.

   Il s’agit de la valeur par défaut.

1. Cliquez sur **Enregistrer et fermer**.

   Désormais, lorsque vous joignez le formulaire personnalisé à un objet, puis que quelqu’un modifie les informations dans le champ **Instructions**, le champ **Instructions Modifier l’historique** affiche la dernière valeur, suivie de la date actuelle entre parenthèses, et d’une barre verticale. Si d’autres modifications sont apportées, elles sont ajoutées à ces informations de la même manière.

   Dans le calcul ci-dessus, vous pouvez remplacer *Instructions* par le nom exact de votre champ de texte à une seule ligne dont vous voulez suivre l’historique, et **Historique des modifications des instructions** par le nom exact de votre champ calculé.
