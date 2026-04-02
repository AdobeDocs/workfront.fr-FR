---
title: Limiter l’accès aux données financières dans les champs personnalisés
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Lorsque vous créez un champ personnalisé, vous pouvez définir des paramètres facultatifs pour restreindre l’accès aux données financières.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 5cdaccd9381b02f183b837208eaac4389b0b7a24
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 9%

---


# Limiter l’accès aux données financières dans les champs personnalisés

{{highlighted-preview-article-level}}

Lorsque vous créez un champ personnalisé, vous pouvez définir des paramètres facultatifs pour restreindre l’accès aux données financières. Ainsi, les utilisateurs et utilisatrices disposant de certaines autorisations définies dans leurs niveaux d’accès peuvent voir les données et ne peuvent pas voir de données financières auxquelles ils ne devraient pas avoir accès.

Pour plus d’informations sur la création d’un champ personnalisé, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Pour plus d&#39;informations sur les niveaux d&#39;accès, voir [Présentation des niveaux d&#39;accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md). Pour plus d’informations sur le partage et les autorisations, voir [Présentation des autorisations de partage sur les objets](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr>  
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Accès administratif aux formulaires personnalisés</td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limiter l’accès aux données financières d’un champ personnalisé

1. Créez un formulaire personnalisé ou ouvrez un formulaire existant.

   Pour plus d’informations, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Ajoutez un champ personnalisé au formulaire ou sélectionnez un champ existant.

   Ces types de champs peuvent être restreints en fonction de l’accès aux données financières :

   * Texte sur une seule ligne
   * Paragraphe
   * Liste déroulante à sélection unique
   * Liste déroulante à sélection multiple
   * Groupe Case à cocher
   * Cases d’option
   * Recherche externe
   * Recherche externe multi-sélection
   * Calculé

1. Dans le champ **Format**, sélectionnez **Devise**.

   >[!NOTE]
   >
   >Pour les champs calculés, n’importe quel format est autorisé. Tous les autres types de champs doivent utiliser le format **Devise**, sinon le champ **Type d’autorisation Finance** ne sera pas disponible.

1. (Facultatif) Pour les champs calculés uniquement, activez l’option **Autorisation automatique** pour permettre aux autorisations financières de provenir automatiquement des champs de la formule.

1. Sélectionnez une option pour le **Type d’autorisation Finance**.

   Les utilisateurs doivent disposer de ce type d&#39;autorisation finance avant de pouvoir afficher ou modifier ce champ personnalisé dans le formulaire.

   * **Aucune autorisation requise :** tous les utilisateurs peuvent voir ce champ
   * **Général :** les utilisateurs doivent disposer des autorisations de modification ou d’affichage de General Finance
   * **Facturation :** les utilisateurs doivent disposer des autorisations nécessaires pour modifier ou afficher les taux de facturation
   * **Coût :** les utilisateurs doivent disposer des autorisations pour modifier ou afficher les taux de coût

   Pour les champs calculés :

   * Le champ **Type d’autorisation Finance** n’est pas disponible pour la définition manuelle des autorisations si le champ **Autorisation automatique** est activé.
   * Les champs utilisés dans la formule déterminent si le champ d’autorisation est actif. Si le champ d’autorisation est vide (et que les autorisations automatiques ne sont pas activées), les champs de la formule ne prennent pas en charge les autorisations financières.
   * L&#39;accès est requis pour tous les champs de la formule. Par exemple, si deux champs sont utilisés dans un champ calculé et que l’un d’eux dispose d’une autorisation de facturation et que le second dispose d’une autorisation de coûts, l’utilisateur doit disposer des autorisations pour afficher les taux de facturation et de coûts afin d’afficher la valeur calculée.

1. Pour enregistrer vos modifications, cliquez sur **Appliquer** et continuez à créer votre formulaire.

   Ou

   Cliquez sur **Enregistrer et fermer**.

## Exemple

Deux projets sont partagés avec un utilisateur :

* L’utilisateur est autorisé à modifier toutes les options financières du premier projet
* L’utilisateur est autorisé à afficher les taux de facturation et les finances générales du second projet

Lorsque l’utilisateur modifie le premier projet, tous les champs financiers du formulaire personnalisé sont modifiables. Lorsque l’utilisateur modifie le deuxième projet, les champs définis sur **Facturation** ou **Général** sont en lecture seule et les champs définis sur **Coût** ne sont pas visibles.

Lorsque l’utilisateur consulte les projets dans une liste ou un rapport :

* Les champs Finances sont visibles ou modifiables en fonction des autorisations et des paramètres du rapport
* Les champs Finances sont vides si l’utilisateur ne dispose pas des autorisations pour les afficher

L’exportation des détails du projet affiche les mêmes valeurs de champ financier (ou champs vides) que dans la liste.

Lors de la modification en masse des deux projets, les champs facturation et finances générales s’affichent en lecture seule et les champs de coût s’affichent sans objet.

