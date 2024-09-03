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
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 100%

---

# Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ

Si les utilisateurs et utilisatrices mettent régulièrement à jour les champs personnalisés et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi que la date à laquelle ces modifications ont eu lieu, vous pouvez capturer ces informations dans un champ personnalisé calculé.

L’exemple suivant vous montre comment construire le champ calculé *Historique des modifications des instructions* pour capturer toutes les modifications apportées à un champ de texte d’une seule ligne appelé *Instructions*.

>[!TIP]
>
>Vous pouvez suivre cet exemple pour tous les types de champs personnalisés, et pas seulement pour les champs de texte d’une seule ligne.

Cela permet d’effectuer les opérations suivantes :

* Limiter le champ *Historique des modifications des instructions* aux 2 000 caractères les plus récents pour rester dans la limite de la base de données Workfront.
* Vérifier si la valeur actuelle du champ *Instructions* correspond au début de la valeur *Historique des modifications des instructions* ; on suppose qu’elle est vide et, si ce n’est pas le cas, l’opération suivante est effectuée : 

   * S’ils correspondent bien, l’*historique des modifications des instructions* reste inchangé ;
   * S’ils ne correspondent pas, l’*historique des modifications des instructions* est remplacé par la dernière valeur du champ *Instructions*, suivie de la date du jour entre parenthèses, d’une barre verticale et de l’ancien *historique des modifications des instructions*, qui conserve la ou les valeurs précédentes et la ou les dates auxquelles elles ont été saisies.

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
   <td> <p>Accès administratif aux formulaires personnalisés</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
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

   1. Cliquez sur **Champ de texte sur une seule ligne**.
   1. Spécifiez un **libellé** pour le champ personnalisé, tel que *Instructions*.
   1. Cliquez sur **Appliquer**.

1. Sélectionnez **Ajouter un champ**, puis **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Indiquez un **Libellé** pour le champ personnalisé calculé, tel que *Historique des modifications des instructions*.

   Il s’agit du champ qui enregistrera toutes les modifications apportées au premier champ que vous avez créé (*Instructions*).

1. Cliquez sur **Enregistrer + Fermer**.
1. Cliquez sur le nom du formulaire dans lequel vous avez ajouté deux champs pour le rouvrir.
1. Cliquez sur le champ personnalisé calculé *Historique des modifications des instructions,* puis copiez et collez ce qui suit dans la zone de calcul :
1. Dans le champ **Calcul**, indiquez le calcul suivant pour votre champ personnalisé :

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recommandé) Collez le même calcul dans le champ **Instructions** sur le champ calculé du formulaire.
1. Assurez-vous que **Texte** est bien sélectionné dans le champ **Format** pour formater le champ personnalisé calculé en tant que texte.

   Il s’agit de la valeur par défaut.

1. Cliquez sur **Enregistrer + Fermer**.

   Désormais, lorsque vous attachez le formulaire personnalisé à un objet et que quelqu’un modifie les informations contenues dans le champ *Instructions*, le champ « Historique des modifications des instructions » affiche la dernière valeur, suivie de la date du jour entre parenthèses et d’une barre verticale. Si d’autres modifications sont apportées, elles sont ajoutées à ces informations de la même manière.

   Dans le calcul ci-dessus, vous pouvez remplacer *Instructions* par le nom exact de votre champ de texte à une seule ligne dont vous voulez suivre l’historique, et *Historique des modifications des instructions* par le nom exact de votre champ calculé.
