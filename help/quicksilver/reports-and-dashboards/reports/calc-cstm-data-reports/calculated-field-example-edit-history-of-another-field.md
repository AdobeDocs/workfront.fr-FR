---
content-type: reference
product-area: reporting
keywords: audit, journal, personnalisé, champ
navigation-topic: calculate-custom-data-reports
title: '« Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ »'
description: Si les utilisateurs et utilisatrices mettent régulièrement à jour les champs personnalisés et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi que la date à laquelle ces modifications ont eu lieu, vous pouvez capturer ces informations dans un champ personnalisé calculé.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 58%

---

# Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ

Si les utilisateurs et utilisatrices mettent régulièrement à jour les champs personnalisés et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi que la date à laquelle ces modifications ont eu lieu, vous pouvez capturer ces informations dans un champ personnalisé calculé.

L’exemple suivant montre comment créer le champ calculé Historique d’édition des instructions pour capturer toutes les modifications apportées à un champ de texte d’une seule ligne appelé Instructions.

>[!TIP]
>
>Vous pouvez suivre cet exemple pour tous les types de champs personnalisés, et pas seulement pour les champs de texte d’une seule ligne.

Pour ce faire, procédez comme suit :

* Limite le champ Instructions Modifier l’historique aux 2 000 caractères les plus récents pour rester dans la limite de la base de données Workfront.
* Vérifie si la valeur actuelle du champ Instructions correspond à l’avant de la valeur Instructions Edit History . Elle suppose qu’elle est vide et, dans le cas contraire, elle effectue les opérations suivantes :

   * S’ils correspondent, l’historique de modification des instructions est conservé tel quel.
   * S’ils ne correspondent pas, il remplace la valeur Instructions Edit History par la dernière dans le champ Instructions , suivie de la date actuelle entre parenthèses, d’une barre verticale et de l’historique d’édition des instructions précédent(s), qui conserve la ou les valeurs précédentes et la ou les dates auxquelles elles ont été entrées.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Accès administratif à Forms personnalisé</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorisations sur un objet</strong> </p> </td> 
   <td> <p>Autorisations de gestion sur les formulaires personnalisés </p> <p>Pour plus d’informations, consultez <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partager un formulaire personnalisé</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Conditions préalables

Pour ajouter un champ calculé qui affiche l’historique des modifications d’un champ dans un formulaire personnalisé, vous devez tout d’abord :

* Créer le formulaire personnalisé
* Ajouter le champ dont vous voulez capturer l’historique au formulaire personnalisé

## Afficher l’historique des modifications d’un champ

1. Accéder au formulaire personnalisé dans lequel vous souhaitez ajouter le champ calculé.

1. Pour créer un champ personnalisé de texte sur une seule ligne, par exemple, procédez comme suit :

   1. Cliquez sur **Texte sur une seule ligne**.
   1. Spécifiez un **libellé** pour le champ personnalisé. Par exemple, vous pouvez le nommer &quot;Instructions&quot;.
   1. Cliquez sur **Appliquer**.

1. Cliquez sur **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Spécifiez un **libellé** pour le champ personnalisé calculé. Par exemple, vous pouvez le nommer &quot;Instructions Modifier l’historique&quot;.

   Il s’agit du champ qui capture toutes les modifications apportées au premier champ que vous avez créé (&quot;Instructions&quot;).

1. Cliquez sur **Enregistrer et fermer**.
1. Cliquez sur le nom du formulaire dans lequel vous avez ajouté deux champs pour le rouvrir.
1. Cliquez sur le champ personnalisé calculé **Instructions Edit History**, puis copiez et collez les éléments suivants dans la zone **Calcul** :

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recommandé) Collez le même calcul dans le champ **Instructions** sur le champ calculé du formulaire.
1. Assurez-vous que **Texte** est sélectionné dans le champ **Format** pour formater le champ personnalisé calculé en tant que texte.

   Il s’agit de la valeur par défaut.

1. Cliquez sur **Enregistrer et fermer**.

   Désormais, lorsque vous joignez le formulaire personnalisé à un objet, puis qu’une personne modifie les informations du champ **Instructions**, le champ **Instructions Edit History** affiche la dernière valeur, suivie de la date actuelle entre parenthèses et une barre verticale. Si d’autres modifications sont apportées, elles sont ajoutées à ces informations de la même manière.

   Dans le calcul ci-dessus, vous pouvez remplacer *Instructions* par le nom exact de votre champ de texte à une seule ligne dont vous voulez suivre l’historique, et **Historique des modifications des instructions** par le nom exact de votre champ calculé.
