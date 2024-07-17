---
content-type: reference
product-area: reporting
keywords: audit,track,custom,field
navigation-topic: calculate-custom-data-reports
title: "Exemple de champ personnalisé calculé : afficher l’historique de modification d’un champ"
description: Si les utilisateurs mettent à jour des champs personnalisés de manière régulière et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi qu’une date à laquelle les modifications se produisent, vous pouvez capturer ces informations dans un champ personnalisé calculé.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 13%

---

# Exemple de champ personnalisé calculé : afficher l’historique des modifications d’un champ

Si les utilisateurs mettent à jour des champs personnalisés de manière régulière et que vous souhaitez capturer un journal de toutes les modifications apportées à un champ ainsi qu’une date à laquelle les modifications se produisent, vous pouvez capturer ces informations dans un champ personnalisé calculé.

L’exemple suivant montre comment créer le champ calculé *Instructions Edit History* pour capturer toutes les modifications apportées à un champ de texte d’une seule ligne appelé *Instructions*.

>[!TIP]
>
>Vous pouvez suivre cet exemple pour tous les types de champs personnalisés, et pas seulement pour les champs de texte d’une seule ligne.

Pour ce faire, procédez comme suit : 

* Limite le champ *Instructions pour la modification de l’historique* aux 2 000 caractères les plus récents pour rester dans la limite de la base de données Workfront.
* Vérifie si la valeur actuelle du champ *Instructions* correspond au devant de la valeur *Instructions Edit History* ; suppose qu’elle est vide et, dans le cas contraire, il effectue les opérations suivantes : 

   * S’ils correspondent, il laisse l’historique *Instructions Edit* tel quel ;
   * S’ils ne correspondent pas, il remplace la valeur *Instructions Edit History* par la dernière valeur du champ *Instructions*, suivie de la date actuelle entre parenthèses, une barre verticale, et de la précédente *Instructions Edit History*, qui conserve la ou les valeurs précédentes et la ou les dates auxquelles elles ont été entrées.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Forfait Adobe Workfront*</p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td> <p>Licence Workfront*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Accès administratif à Forms personnalisé</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorisations d’objets</strong> </p> </td> 
   <td> <p>Gestion des autorisations sur les formulaires personnalisés </p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Partage d’un formulaire personnalisé</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Conditions préalables

Pour ajouter un champ calculé qui affiche l’historique de modification d’un champ à un formulaire personnalisé, vous devez d’abord :

* Créer un formulaire personnalisé
* Ajoutez au formulaire personnalisé le champ dont vous souhaitez capturer l’historique.

## Affichage de l’historique de modification d’un champ

1. Accédez à un formulaire personnalisé dans lequel vous souhaitez ajouter le champ calculé.

1. Pour créer le champ personnalisé de texte sur une seule ligne, procédez comme suit :

   1. Cliquez sur **Champ de texte d’une seule ligne**.
   1. Spécifiez un **libellé** pour le champ personnalisé, tel que *Instructions*.
   1. Cliquez sur **Applye**.

1. Sélectionnez **Ajouter un champ**, puis **Calculé** pour ajouter un champ personnalisé calculé au formulaire.
1. Spécifiez un **Libellé** pour le champ personnalisé calculé, tel que *Instructions Edit History*.

   Il s’agit du champ qui capture toutes les modifications apportées au premier champ que vous avez créé (*Instructions*).

1. Cliquez sur **Enregistrer + Fermer**.
1. Cliquez sur le nom du formulaire dans lequel vous avez ajouté deux champs pour le rouvrir.
1. Cliquez sur le champ personnalisé calculé *Instructions Edit History,* , puis copiez et collez les éléments suivants dans la zone Calcul :
1. Dans le champ **Calcul** , spécifiez le calcul suivant pour votre champ personnalisé :

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recommandé) Collez le même calcul dans le champ **Instructions** sur le champ calculé du formulaire.
1. Assurez-vous que  **Texte** est sélectionné dans le champ **Format** pour formater le champ personnalisé calculé en tant que texte.

   Il s’agit du paramètre par défaut.

1. Cliquez sur **Enregistrer+Fermer**.

   Désormais, lorsque vous joignez le formulaire personnalisé à un objet, puis qu’une personne modifie les informations dans le champ *Instructions*, le champ *Instructions Edit History&quot; (Instructions Modifier l’historique) affiche la dernière valeur, suivie de la date actuelle entre parenthèses et une barre verticale. Si d’autres modifications sont apportées, elles sont ajoutées à ces informations de la même manière.

   Dans le calcul ci-dessus, vous pouvez remplacer *Instructions* par le nom exact de votre champ de texte d’une seule ligne dont vous souhaitez effectuer le suivi, et *Instructions Edit History* par le nom exact de votre champ calculé.
