---
title: Importation de champs à partir d’Adobe Workfront
description: Dans Adobe Workfront Planning, vous pouvez créer des champs personnalisés pour chaque type d’enregistrement. Vous pouvez ensuite associer le champ à des enregistrements Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 0da877936ba8f52341a5b151f76710c979ce9294
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 29%

---


<!--add to TOC-->

# Importer des champs depuis Adobe Workfront

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez importer des copies de champs Workfront existants. L’importation de champs à partir de Workfront crée une copie de chaque champ pour un type d’enregistrement Workfront Planning.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès à la planification Workfront.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des projets Workfront suivants est prévu :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>La planification Workfront n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package de planification Adobe Workfront*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de la planification Workfront.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>La planification Workfront n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations de gestion pour un espace de travail</a> </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques concernant l’importation de champs à partir de Workfront

* Vous pouvez importer des champs Workfront natifs ou personnalisés dans un type d’enregistrement dans Workfront Planning.
* L’importation de champs Workfront crée des copies des mêmes champs et conserve leur nom dans Workfront Planning. Une fois copiés dans Workfront Planning, les champs sont indépendants des champs Workfront d’origine et ne partagent pas d’informations.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* Vous pouvez ajouter des champs natifs ou personnalisés à partir des objets Workfront suivants :
   * Portfolio
   * Programme
   * Projet
   * Tâche
   * Problème
   * Document
   * Entreprise
   * Groupe
   * l’utilisateur ou de l’utilisatrice
   * Fonction
   * Affectation
   * Heure
   * Enregistrement de facturation
     <!--Available only to Preview, but might not come to Prod:* Rate card-->
   * Frais
   * Itération
     <!--* Non-labor resource-->
     <!--* Non-labour resource category-->
* Une fois importés dans Workfront Planning, les champs Workfront peuvent ne pas conserver leur type de champ.

  Le tableau ci-dessous présente les types de champ Workfront et le type de champ Workfront Planning correspondant.

  | Type de champ Workfront | Type de champ Planification Workfront |
  |------------------------------------------|-------------------------------|
  | Texte sur une seule ligne au format texte | Texte à une ligne |
  | Texte mono-ligne au format numérique | Nombre |
  | Texte sur une seule ligne au format monétaire | Devise |
  | Paragraphe | Paragraphe |
  | Texte avec formatage | Paragraphe |
  | Liste déroulante à sélection unique | Sélection unique |
  | Menu déroulant multi-sélection | Sélection multiple |
  | Les filtres de type utilisateur ne sont pas pris en charge | Personnes |
  | Calculé* | Formule |
  | Date | Date |
  | Groupe Case à cocher | Sélection multiple |
  | Bouton radio | Sélection multiple |

  *Les champs calculés seront disponibles à une date ultérieure.
Tous les autres types de champ Workfront ne sont pas pris en charge dans la planification Workfront.


## Importer les champs depuis Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Cliquez sur l’espace de travail pour lequel vous souhaitez créer des champs.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur la carte d’un type d’enregistrement.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue Tableau.

   >[!TIP]
   >
   >    Certains champs peuvent être masqués. Cliquez sur **Champs** et activez la bascule pour les champs que vous souhaitez afficher en tant que colonnes dans la vue de tableau.

1. Cliquez sur l’icône **+** dans le coin supérieur droit de la vue de tableau.

   Ou

   Pointez sur l’en-tête d’une colonne, cliquez sur la flèche pointant vers le bas située après le nom du champ, puis cliquez sur **Insérer à gauche** ou **Insérer à droite** pour ajouter le nouveau champ.
1. Cliquez sur **Ajouter existant** dans le coin inférieur droit de l’onglet **Nouveau champ** . <!--check UI - did they change this??-->

   ![](assets/add-existing-fields-from-workfront-modal.png)

1. Commencez à saisir le nom d’un champ Workfront existant dans la zone de recherche, puis cliquez sur **+** lorsqu’il s’affiche dans la liste.
1. (Facultatif) Saisissez un autre champ, puis cliquez sur **+** lorsqu’il s’affiche dans la liste.
1. (Facultatif) Cliquez sur l&#39;icône **Filtres** ![](assets/filters-in-import-fields-icon.png), puis mettez à jour l&#39;un ou les deux champs suivants :

   * Type d’objet : sélectionnez un type d’objet Workfront dont vous souhaitez importer les champs.
   * Formulaire personnalisé : sélectionnez un ou plusieurs formulaires personnalisés dans Workfront. Vous pouvez sélectionner un formulaire personnalisé sans d’abord sélectionner un type d’objet.
1. Cliquez sur **+**, puis **Ajouter des champs**.
Les champs sont ajoutés à la vue de la table et aux pages de détails des enregistrements.

