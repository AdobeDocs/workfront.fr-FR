---
title: Importer des champs depuis Adobe Workfront
description: Dans Adobe Workfront Planning, vous pouvez créer des champs personnalisés pour chaque type d’enregistrement. Vous pouvez ensuite associer le champ à des enregistrements Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 24%

---

<!--add to TOC-->

# Importer des champs depuis Adobe Workfront

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Vous pouvez importer des copies de champs Workfront existants. L’importation de champs depuis Workfront crée une copie de chaque champ pour un type d’enregistrement Workfront Planning.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

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
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre entreprise doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à toutes les fonctionnalités de Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations pour un espace de travail <span class="preview">et le type d’enregistrement</span> </a> </p>  
   <p>Les équipes d’administration système ont des droits sur tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut Planning.</p>
<p><span class="preview">Dans l’environnement de Prévisualisation, les utilisateurs et utilisatrices standard et les administrateurs et administratrices système ont Planning activé par défaut.</span></p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considérations relatives à l’importation de champs depuis Workfront

* Vous pouvez importer des champs Workfront natifs ou personnalisés dans un type d&#39;enregistrement dans Workfront Planning.
* L’importation de champs Workfront crée des copies des mêmes champs et conserve le nom du champ dans Workfront Planning. Une fois copiés dans Workfront Planning, les champs sont indépendants des champs Workfront d’origine et ne partagent pas d’informations.
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
     <!--Available only to Preview, but might not come to Prod:* Rate card - visible in Production but asking PM if it should be hidden-->
   * Frais
   * Itération
     <!--* Non-labor resource - - visible in Production but asking PM if it should be hidden-->
     <!--* Non-labour resource category - - visible in Production but asking PM if it should be hidden-->
* Il se peut que les champs Workfront ne conservent pas leur type de champ après leur importation dans Workfront Planning.

  Le tableau ci-dessous présente les types de champs Workfront et le type de champ Workfront Planning correspondant.

  | Type de champ Workfront | Type de champ Workfront Planning |
  |------------------------------------------|-------------------------------|
  | Texte d’une seule ligne au format texte | Texte à une ligne |
  | Texte d’une seule ligne au format numérique | Nombre |
  | Texte d’une seule ligne au format monétaire | Devise |
  | Paragraphe | Paragraphe |
  | Texte avec formatage | Paragraphe |
  | Liste déroulante à sélection unique | Sélection unique |
  | Menu déroulant multi-sélection | Sélection multiple |
  | Les filtres de saisie semi-automatique ne sont pas pris en charge | Personnes |
  | Calculé* | Formule |
  | Date | Date |
  | Groupe Case à cocher | Sélection multiple |
  | Bouton radio | Sélection multiple |

  *Les champs calculés seront disponibles ultérieurement.
Tous les autres types de champ Workfront ne sont pas pris en charge dans Workfront Planning.


## Importer les champs depuis Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez créer les types d’enregistrements pour les champs.

   L’espace de travail et les types d’enregistrement s’affichent.

1. Cliquez sur la carte d’un type d’enregistrement.

   Tous les enregistrements existants associés au type d’enregistrement s’affichent dans les lignes de la vue Tableau.

   >[!TIP]
   >
   >    Certains champs peuvent être masqués. Cliquez sur **Champs** et activez le bouton (bascule) pour les champs que vous souhaitez afficher en tant que colonnes dans la vue Tableau.

1. Cliquez sur l’icône **+** dans le coin supérieur droit de la vue Tableau

   Ou

   Pointez sur l’en-tête d’une colonne, cliquez sur la flèche pointant vers le bas après le nom du champ, puis cliquez sur **Insérer à gauche** ou **Insérer à droite** pour ajouter le nouveau champ.
1. Cliquez sur **Ajouter un existant** dans le coin inférieur droit de l’onglet **Nouveau champ**. <!--check UI - did they change this??-->

   ![Boîte de dialogue modale Ajouter des champs existants à partir de Workfront](assets/add-existing-fields-from-workfront-modal.png)

1. Commencez à saisir le nom d’un champ Workfront existant dans la zone de recherche, puis cliquez sur **+** lorsqu’il s’affiche dans la liste.
1. (Facultatif) Saisissez un autre champ, puis cliquez sur **+** lorsqu’il s’affiche dans la liste.
1. (Facultatif) Cliquez sur l’icône **Filtres** ![Icône Filtres dans les champs d’importation](assets/filters-in-import-fields-icon.png), puis mettez à jour l’un des champs suivants, ou les deux :

   * Type d’objet : sélectionnez un type d’objet Workfront dont vous souhaitez importer les champs.
   * Formulaire personnalisé : sélectionnez un ou plusieurs formulaires personnalisés dans Workfront. Vous pouvez sélectionner un formulaire personnalisé sans sélectionner au préalable un type d’objet.
1. Cliquez sur **+**, puis sur **Ajouter des champs**.
Les champs sont ajoutés en mode Tableau et dans les pages de détails des enregistrements.

   >[!IMPORTANT]
   >
   >    Il existe une limite de 500 champs pour tout type d’enregistrement. Les champs existants ainsi que les champs importés contribuent à cette limite.

   Les champs ajoutés sont des copies des champs Workfront et ne se connectent plus aux champs d’origine dans Workfront.
