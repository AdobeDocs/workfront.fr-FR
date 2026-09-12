---
title: Partager un espace d'idées avec d'autres personnes
description: Adobe Workfront Planning offre désormais une fonctionnalité supplémentaire pour identifier avant de lancer vos campagnes. Tirez parti de la puissance de l’IA pour créer des idées et collaborer avec d’autres personnes avant qu’elles ne deviennent des enregistrements de planification.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 9%

---


# Partager un espace d&#39;idées avec d&#39;autres personnes

<!--add to TOC and miniTOC-->

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Il est disponible uniquement dans le cadre du programme **Ideation space Beta**. </span>

<span class="preview">Pour plus d’informations, voir [Prise en main de l’espace d’idéation pour Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

<!--ome of this information is also duplicated in the section for Ideation space permissions in the Access needed to use Ideation space article-->

Les autorisations d’enregistrement de Workfront Planning sont transférées vers l’espace d’idéation d’un enregistrement.

En outre, vous pouvez accorder à d’autres utilisateurs les autorisations nécessaires pour utiliser l’espace d’idéation et y ajouter des idées.

Tenez compte des points suivants :

* Les créateurs d’idées disposent toujours des autorisations d’éditeur sur leurs propres idées.

* Vous devez disposer des autorisations d’éditeur sur un espace d’idéation pour créer des résumés et les exporter vers d’autres applications.

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Tout Workfront ou workflow avec un package Planning</p></li>
Ou
<li><p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Produits supplémentaires</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence de workflow Adobe</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> 
   <ul>
   <li><p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   </li>
   <li><p>Le paramètre Désactiver l’espace d’idéation de votre niveau d’accès doit être désélectionné</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td> <p>Autorisations de niveau Contributeur ou supérieur à l’espace de travail et au type d’enregistrement dans lesquels vous souhaitez ajouter des enregistrements </p>
      <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>
      <p>Afficher les autorisations d’accès aux objets Workfront pour les ajouter aux résumés <!--not sure if this is available--></p>
      <p>Autorisations d’éditeur dans l’espace Idéation pour créer des résumés</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Rôles utilisateur Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Tout rôle d’utilisateur GenStudio pour accéder aux campagnes, aux produits et aux rôles</li>
   <li>GenStudio System Manager pour accéder aux activations <!--and Events--></li></ul>
   Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> Rôles utilisateur et autorisations </a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Partage d’un espace d’idées

1. Accédez à l’espace Idéation d’un enregistrement Planning.

   Pour plus d’informations, consultez l’un des articles suivants :

   * [Créer des enregistrements Planning à partir de résumés d&#39;espace d&#39;idées](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
   * [Créer des briefs dans l’espace Idéation](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

1. Cliquez sur **Partager** dans le coin supérieur droit, puis cliquez sur l’icône **Paramètres** ![Icône Paramètres](assets/setting-icon.png) dans le coin supérieur droit de la zone **Partager le document**.
1. Dans la liste Qui a accès , choisissez l’une des options suivantes :

   * **Seules les personnes invitées peuvent y accéder**

     Vous devez ajouter des utilisateurs individuels à l&#39;espace Idéation et leur attribuer un niveau d&#39;autorisation.
   * **Tout le monde peut apporter des commentaires dans &lt; l’environnement Workfront de votre entreprise >**

     Toute personne de votre organisation disposant d’un niveau d’accès Workflow et Licence Planning peut rechercher et commenter l’idée.
   * **Toute personne disposant du lien peut ajouter des commentaires**

     Toute personne avec laquelle vous partagez un lien vers l’idée peut la commenter, y compris les personnes extérieures à votre organisation.

1. Cliquez sur **Copier le lien** pour générer un lien vers l’idéation et le partager avec d’autres personnes. Le lien est ajouté à votre presse-papiers.
1. Cliquez sur la flèche vers l’arrière de la zone Paramètres pour revenir au partage.
1. (Conditionnel) Si vous avez choisi de partager l&#39;espace d&#39;idéation avec des personnes spécifiques, commencez à saisir leur nom ou leur adresse e-mail, puis sélectionnez l&#39;un des niveaux d&#39;autorisation suivants :

   | Autorisation de l’emplacement | Fonctionnalités |
   |---|---|
   | **Éditeur** | Peut modifier, télécharger et partager l’espace d’idéation |
   | **Commentateur** | Peut afficher et commenter l’espace d’idéation |
   | **Visionneuse** | Peut afficher l’espace d’idéation |

1. (Facultatif) Incluez un message dans votre affectation, puis cliquez sur **Inviter**.

   Les utilisateurs invités reçoivent une notification par e-mail concernant leur attribution d’autorisations.

1. Cliquez sur l’icône **X** pour fermer la zone **Partager le document**.











