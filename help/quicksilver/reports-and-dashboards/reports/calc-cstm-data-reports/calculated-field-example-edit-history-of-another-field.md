---
content-type: reference
product-area: reporting
keywords: audit,track,custom,field
navigation-topic: calculate-custom-data-reports
title: "Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ."
description: Si les utilisateurs mettent à jour des champs personnalisés de manière régulière et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi qu’une date à laquelle les modifications se produisent, vous pouvez capturer ces informations dans un champ personnalisé calculé.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Exemple de champ personnalisé calculé : afficher l’historique de modification d’un champ ;

Si les utilisateurs mettent à jour des champs personnalisés de manière régulière et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi qu’une date à laquelle les modifications se produisent, vous pouvez capturer ces informations dans un champ personnalisé calculé.

L’exemple suivant montre comment créer la variable *Instructions Modifier l’historique* champ calculé pour capturer toutes les modifications apportées à un champ de texte sur une seule ligne appelé *Instructions*.

>[!TIP]
>
>Vous pouvez suivre cet exemple pour tous les types de champs personnalisés, et pas seulement pour les champs de texte d’une seule ligne.

Pour ce faire, procédez comme suit : 

* Limite la variable *Instructions Modifier l’historique* à la limite de 2 000 caractères la plus récente pour rester dans la base de données Workfront.
* Vérifie si la valeur actuelle de la variable *Instructions* correspond à l’avant du champ *Instructions Modifier l’historique* value; il suppose qu’il est vide et, dans le cas contraire, il effectue les opérations suivantes : 

   * S’ils correspondent, le paramètre *Instructions Modifier l’historique* en l’état :
   * S’ils ne correspondent pas, il remplace la fonction *Instructions Modifier l’historique* avec la dernière valeur dans la variable *Instructions* , suivie de la date actuelle entre parenthèses, d’une barre verticale et du *Instructions Modifier l’historique*, qui conserve la ou les valeurs précédentes et la ou les dates auxquelles elles ont été saisies.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Formule Adobe Workfront*</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>Accès administratif à Forms personnalisé</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Gestion des autorisations sur les formulaires personnalisés </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partage d’un formulaire personnalisé</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Conditions préalables

Pour ajouter un champ calculé qui affiche l’historique de modification d’un champ à un formulaire personnalisé, vous devez d’abord :

* Création d’un formulaire personnalisé
* Ajoutez au formulaire personnalisé le champ dont vous souhaitez capturer l’historique.

## Afficher l’historique de modification d’un champ

1. Accédez à un formulaire personnalisé dans lequel vous souhaitez ajouter le champ calculé.

1. Pour créer le champ personnalisé de texte sur une seule ligne, procédez comme suit :

   1. Cliquez sur **Champ de texte d’une seule ligne**.
   1. Spécifiez un **Libellé** pour le champ personnalisé, comme *Instructions*.
   1. Cliquez sur **Appliquer**.

1. Sélectionner **Ajouter un champ**, puis sélectionnez **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Spécifiez un **Libellé** pour le champ personnalisé calculé, tel que *Instructions Modifier l’historique*.

   Il s’agit du champ qui capture toutes les modifications apportées au premier champ que vous avez créé (*Instructions*).

1. Cliquez sur **Enregistrer + Fermer**.
1. Cliquez sur le nom du formulaire dans lequel vous avez ajouté deux champs pour le rouvrir.
1. Cliquez sur le champ personnalisé calculé *Instructions Modifier l’historique,* copiez et collez ensuite les éléments suivants dans la zone Calcul :
1. Dans le **Calcul** , indiquez le calcul suivant pour votre champ personnalisé :

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recommandé) Collez le même calcul dans la variable **Instructions** sur le champ calculé du formulaire.
1. Assurez-vous que  **Texte** est sélectionné dans la variable **Format** pour formater le champ personnalisé calculé en tant que texte.

   Il s’agit de la valeur par défaut.

1. Cliquez sur **Enregistrer + Fermer**.

   Désormais, lorsque vous joignez le formulaire personnalisé à un objet et qu’une personne modifie les informations de la variable *Instructions* , le champ *Instructions Modifier l’historique&quot; affiche la dernière valeur, suivie de la date actuelle entre parenthèses et d’une barre verticale. Si d’autres modifications sont apportées, elles sont ajoutées à ces informations de la même manière.

   Dans le calcul ci-dessus, vous pouvez remplacer *Instructions* avec le nom exact de votre champ de texte d’une seule ligne dont vous souhaitez effectuer le suivi, et *Instructions Modifier l’historique* avec le nom exact de votre champ calculé.
