---
title: Restaurer les enregistrements supprimés
description: Vous pouvez récupérer les enregistrements supprimés de la zone Récemment supprimés dans Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 21%

---

# Restaurer les enregistrements supprimés

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez récupérer les enregistrements supprimés de la zone Récemment supprimés dans Adobe Workfront Planning.

Pour plus d&#39;informations sur la suppression d&#39;enregistrements, voir [Supprimer des enregistrements](/help/quicksilver/planning/records/delete-records.md).

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
   <td><p> Standard</p>
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
   <td>   <p>Autorisations de niveau Contributeur ou supérieur à un espace de travail <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de disposition</p></td> 
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Planning dans le menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à la récupération des enregistrements supprimés

* Les enregistrements sont stockés dans la classe Récemment supprimés pendant 30 jours. Au bout de 30 jours, les enregistrements sont définitivement supprimés de Workfront Planning.
* Si les enregistrements supprimés sont liés à d&#39;autres enregistrements, les enregistrements liés ne sont pas supprimés, mais les informations de l&#39;enregistrement supprimé sont également supprimées. La restauration des enregistrements supprimés restaurera les informations des enregistrements connectés.
* Vous pouvez restaurer des enregistrements en bloc.
* Lorsque les enregistrements sont supprimés, les informations suivantes sont stockées dans la classe Récemment supprimés :
   * **Nom** : il s’agit des informations figurant dans le champ de Principal de l’enregistrement. Pour plus d’informations sur les champs de Principal d’enregistrement, consultez la présentation des champs de Principal [](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Date de suppression** : l’heure et la date de suppression de l’enregistrement.
   * **Temps écoulé depuis la suppression récente** : temps écoulé depuis la suppression de l’enregistrement. Les enregistrements supprimés plus de 30 jours avant la date actuelle ne s&#39;affichent pas dans la classe Récemment supprimés.
   * **Supprimé par** : nom de l’utilisateur qui a supprimé l’enregistrement.

## Restaurer les enregistrements supprimés

1. Accédez à la page de type d’enregistrement dans laquelle vous avez supprimé des enregistrements.
1. Cliquez sur l’icône **Annuler** ![Icône Annuler](assets/undo-icon.png) dans le coin supérieur droit de n’importe quel type d’enregistrement affiché sur la page, puis cliquez sur **Récemment supprimé**.

   La zone **Récemment supprimé** s’affiche.

   ![Zone récemment supprimée](assets/recently-deleted-box.png)

1. Sélectionnez les enregistrements à supprimer, puis cliquez sur **Restaurer** > **Restaurer**. Vous pouvez sélectionner plusieurs enregistrements.

   Si la restauration a réussi, vous recevez une notification de succès en bas de l’écran.
1. Accédez à la vue Tableau et passez en revue les enregistrements restaurés.
