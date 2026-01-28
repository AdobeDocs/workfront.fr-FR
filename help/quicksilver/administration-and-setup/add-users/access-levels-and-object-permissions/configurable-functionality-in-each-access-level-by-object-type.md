---
title: Accès configurable à la fonctionnalité pour chaque type d’objet (hérité)
description: Cet article explique ce que vous pouvez autoriser en tant qu’administrateur ou administratrice Adobe Workfront pour chaque type d’objet, à chaque niveau d’accès. Il explique également quelle est la configuration par défaut pour chaque type de niveau d’accès.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '3510'
ht-degree: 96%

---

# Accès configurable à la fonctionnalité pour chaque type d’objet (hérité)

>[!NOTE]
>
>Les informations de cet article font référence aux niveaux d’accès hérités. Pour plus d’informations sur les niveaux d’accès actuels, voir [Présentation des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Lors de la configuration d’un niveau d’accès pour votre organisation, vous pouvez déterminer quelles actions spécifiques sont disponibles pour le niveau d’accès.

Cet article explique les options qu’un administrateur Adobe Workfront peut sélectionner pour chaque type d’objet, dans chaque niveau d’accès. Il explique également quelle est la configuration par défaut pour chaque type de niveau d’accès.

Par exemple, si un administrateur Workfront sélectionne « Afficher » pour les projets avec un niveau d’accès donné, les utilisateurs disposant de ce niveau d’accès ne pourront afficher que les projets, et non les modifier.

Pour plus d’informations sur toutes les fonctionnalités disponibles pour un type d’objet à chaque niveau d’accès, voir [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Projets

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les projets :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur (type de licence de plan)</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner cela, vous pouvez configurer la possibilité de partager des projets. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès complet à la modification des projets.</p> <p>Pour affiner ce réglage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Copier</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Afficher</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner cela, vous pouvez configurer la possibilité de partager des projets. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès limité à la modification des projets. Pour voir la limitation de l’accès à la modification dans un niveau d’accès Employé ou employée par rapport à un niveau d’accès Planificateur ou planificatrice (qui permet un accès complet à la modification des projets), voir la section <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Projets</a> dans l’article <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Fonctionnalités disponibles pour chaque type d’objet</a>.</p> <p>Pour affiner cela, vous pouvez configurer la possibilité de partager des projets. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Modifier, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> (sélection par défaut) <p>L’accès Afficher est limité, car il n’est pas possible de l’affiner pour activer ou désactiver le partage de projets.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux projets n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tâches

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les tâches :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner cela, vous pouvez configurer la possibilité de partager des tâches. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès intégral à la modification des tâches.</p> <p>Pour affiner cela, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner cela, vous pouvez configurer la possibilité de partager des tâches. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès intégral à la modification des tâches.</p> <p>Pour affiner cela, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> (sélection par défaut)<p>L’accès Afficher est limité, car il n’est pas possible de l’affiner pour activer ou désactiver le partage de projets.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux tâches n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problèmes

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les problèmes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <p><b>Afficher</b></p><p>Pour affiner ceci, vous pouvez configurer la possibilité de partager les problèmes. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès intégral à la modification des problèmes.</p> <p>Pour affiner ceci, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner ceci, vous pouvez configurer la possibilité de partager les problèmes. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès intégral à la modification des problèmes.</p> <p>Pour affiner ceci, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner ceci, vous pouvez configurer la possibilité de partager les problèmes. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès intégral à la modification des problèmes.</p> <p>Pour affiner ceci, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner ceci, vous pouvez configurer la possibilité de partager les problèmes. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès intégral à la modification des problèmes.</p> <p>Pour affiner ceci, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux problèmes n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portefeuilles

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les portfolios :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner cela, vous pouvez configurer la possibilité de partager des portfolios. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès intégral à la modification des portfolios.</p> <p>Pour affiner ceci, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifer</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> (sélection par défaut)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> <p>L’accès aux portfolios n’est pas disponible.</p> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux portfolios n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programmes

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les programmes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner cette option, vous pouvez configurer la possibilité de partager des programmes. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde un accès de modification complet des programmes.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> (sélection par défaut)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> <p>L’accès aux programmes n’est pas disponible.</p> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux programmes n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Rapports, tableaux de bord et calendriers

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les rapports, les tableaux de bord et les calendriers :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <p><b>Afficher</b></p><p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des actions suivantes. Les deux sont activées par défaut :</p> 
      <ul> 
       <li> <p>Afficher les rapports intégrés</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde un accès de modification complet des rapports, tableaux de bord et calendriers.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Toutes ces options sont activées par défaut, à l’exception d’<b>Afficher les rapports intégrés</b>, <b>Partager les rapports publiquement</b>, et <b>Partager sur le système</b>.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Afficher les rapports intégrés</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager les rapports publiquement (en externe)</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> (sélection par défaut)<p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des actions suivantes. Les deux sont activées par défaut :</p> 
      <ul> 
       <li> <p>Afficher les rapports intégrés</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <p><b>Afficher</b> (sélection par défaut)<p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des actions suivantes. Seule l’option Partager est activée par défaut.</p> 
      <ul> 
       <li> <p>Afficher les rapports intégrés</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <p><b>Afficher</b> (sélection par défaut) : accorde l’accès en lecture seule aux rapports, tableaux de bord et calendriers qui ont été partagés avec eux.</p> <p>Pour affiner cette option, vous pouvez configurer la possibilité d’afficher les rapports intégrés. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Afficher</b>, puis désactivez ou activez <b>Affichage intégré</b> (désactivé par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux rapports, aux tableaux de bord et aux calendriers n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filtres, vues et regroupements

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les filtres, les vues et les regroupements :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <p><b>Afficher</b></p><p>Pour affiner cette option, vous pouvez configurer la possibilité de partager des filtres, des vues et des regroupements. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde un accès complet à la modification des filtres, des vues et des regroupements.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <p><b>Afficher</b></p><p>Pour affiner cette option, vous pouvez configurer la possibilité de partager des filtres, des vues et des regroupements. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde un accès complet à la modification des filtres, des vues et des regroupements.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner cette option, vous pouvez configurer la possibilité de partager des filtres, des vues et des regroupements.
Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde un accès complet à la modification des filtres, des vues et des regroupements.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Vue</b> :</p> <p>Pour affiner cette option, vous pouvez configurer la possibilité de partager des filtres, des vues et des regroupements. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde un accès complet à la modification des filtres, des vues et des regroupements.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux filtres, aux vues et aux regroupements n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Documents

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les documents :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner ceci, vous pouvez configurer la possibilité de partager des documents. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde l’accès complet à la modification des documents.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Toutes ces options sont activées par défaut, à l’exception de <b>Partager des documents publiquement</b> et <b>Partager sur le système</b>.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager des documents publiquement (à l’extérieur)</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <p><b>Afficher</b></p><p>Pour affiner ceci, vous pouvez configurer la possibilité de partager des documents. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde l’accès complet à la modification des documents.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Toutes ces options sont activées par défaut, à l’exception de <b>Partager des documents publiquement</b> et <b>Partager sur le système</b>.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager des documents publiquement (à l’extérieur)</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner ceci, vous pouvez configurer la possibilité de partager des documents. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde l’accès complet à la modification des documents.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des actions suivantes. Toutes ces options sont activées par défaut, à l’exception des deux dernières, <b>Partager des documents publiquement</b> et <b>Partager sur le système</b>.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager des documents publiquement (à l’extérieur)</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <p><b>Afficher</b></p><p>Pour affiner ceci, vous pouvez configurer la possibilité de partager des documents. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde l’accès complet à la modification des documents.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux documents n’est pas configurable à ce niveau d’accès. Mais les utilisateurs et les utilisatrices externes peuvent utiliser Workfront pour afficher, réviser et télécharger des documents.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Utilisateurs et utilisatrices

Pour chaque niveau d’accès, vous pouvez configurer les options suivantes pour les utilisateurs et les utilisatrices :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <p><b>Afficher</b></p><p>Pour affiner cette option, vous pouvez configurer la possibilité d’afficher les informations de contact des utilisateurs et des utilisatrices. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Afficher</b>, puis désactivez ou activez l’option <b>Afficher les coordonnées</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde aux utilisateurs et aux utilisatrices un accès complet à la modification.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des actions suivantes. Seules les deux premières options, <b>Créer</b> et <b>Supprimer</b>, sont activées par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li>Administration des utilisateurs (tous les utilisateurs)</li> 
       <li> <p>Administration des utilisateurs (utilisateurs du groupe)</p> </li> 
      </ul> <p>Pour plus d’informations sur les deux options d’administration des utilisateurs et utilisatrices, voir la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurer l’accès des utilisateurs et utilisatrices pour modifier les perdonnes à l’aide d’un niveau d’accès personnalisé</a> dans l’article <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li><p> <b>Vue</b> (seule option disponible)</p><p>Pour affiner cette option, vous pouvez configurer la possibilité d’afficher les informations de contact des utilisateurs et des utilisatrices. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Vue</b>, puis désactivez ou activez l’option <b>Afficher les coordonnées</b> (activée par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li><p> <b>Vue</b> (seule option disponible)</p> <p>Pour affiner cette option, vous pouvez configurer la possibilité d’afficher les informations de contact des utilisateurs et des utilisatrices. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Vue</b>, puis activez ou désactivez l’option <b>Afficher les coordonnées</b> (désactivée par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Vue</b> (seule option disponible)</p><p>Pour affiner cette option, vous pouvez configurer la possibilité d’afficher les informations de contact des utilisateurs et des utilisatrices. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Vue</b>, puis activez ou désactivez l’option <b>Afficher les coordonnées</b> (désactivée par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux utilisateurs et utilisatrices n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Équipes

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les équipes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li><b>Afficher</b> <p>Pour affiner ce réglage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Vue</b>, puis désactivez ou activez l’une des options suivantes*. Les deux sont désactivées par défaut.</p> 
      <ul> 
       <li>Afficher toutes les équipes</li> 
       <li> <p>Afficher les équipes associées à mes groupes</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès complet à la modification des équipes.</p> <p>Pour affiner ce réglage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Vue</b>, puis désactivez ou activez l’une des options suivantes*. Toutes sont activées par défaut, sauf <b>Modifier les équipes dans lesquelles je suis</b>.</p> 
      <ul> 
       <li>Créer</li> 
       <li>Supprimer</li> 
       <li> <p>Modifier les équipes auxquelles j’appartiens</p> </li> 
       <li> <p>Modifier les équipes dans les groupes que je gère (administrateurs de groupe uniquement)</p> </li> 
       <li> <p>Afficher toutes les équipes</p> </li> 
       <li> <p>Afficher les équipes associées à mes groupes</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Afficher</b>
      <p>Pour affiner ce réglage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Vue</b>, puis désactivez ou activez l’une des options suivantes*. Les deux sont activées par défaut.</p> 
      <ul> 
       <li>Afficher toutes les équipes</li> 
       <li> <p>Afficher les équipes associées à mes groupes</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès complet à la modification des équipes.</p> <p>Pour affiner ce réglage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Vue</b>, puis désactivez ou activez l’une des options suivantes*. Seule la première option, <b>Modifier les équipes dans lesquelles je suis</b>, est désactivée par défaut.</p> 
      <ul> 
       <li> <p>Modifier les équipes auxquelles j’appartiens</p> </li> 
       <li> <p>Afficher toutes les équipes</p> </li> 
       <li> <p>Afficher les équipes associées à mes groupes</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <p><b>Afficher</b> (seule option disponible)</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes*. Les deux sont activées par défaut.</p> 
      <ul> 
       <li> <p>Afficher toutes les équipes</p> </li> 
       <li>Afficher les équipes associées à mes groupes</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Afficher</b> (seule option disponible)</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes*. Les deux sont activées par défaut.</p> 
      <ul> 
       <li> <p>Afficher toutes les équipes</p> </li> 
       <li>Afficher les équipes associées à mes groupes</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux équipes n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Modèles

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les modèles :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour affiner cette option, vous pouvez configurer la possibilité de partager des modèles. Cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde l’accès complet à la modification des modèles.</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifier</b>, puis désactivez ou activez l’une des options suivantes. Tous ces éléments sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager sur le système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <p><b>Pas d’accès</b> (seule option disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <p><b>Pas d’accès</b> (seule option disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Pas d’accès</b> (seule option disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux modèles n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Données financières

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les données financières :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <p><b>Afficher</b> :</p> <p>Pour affiner cette option, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Afficher</b>, puis désactivez ou activez l’une des options suivantes*. Les deux sont activées par défaut.</p> 
      <ul> 
       <li>Afficher les taux de facturation et de coûts du rôle</li> 
       <li> <p>Afficher les taux de facturation et de coûts de l'utilisateur</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : accorde l’accès complet à la modification des données financières.</p> <p>Pour affiner ceci, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Afficher</b>, puis désactivez ou activez l’une des options suivantes*. Seules les deux dernières options, <b>Afficher les taux de facturation et de coûts du rôle</b> et <b>Afficher les taux de facturation et de coûts de l’utilisateur ou de l’utilisatrice</b>, sont activées par défaut.</p> 
      <ul> 
       <li>Modifier les taux de facturation et de coûts du rôle</li> 
       <li> <p>Modifier les taux de facturation et de coûts de l'utilisateur</p> </li> 
       <li>Afficher les taux de facturation et de coûts du rôle</li> 
       <li> <p>Afficher les taux de facturation et de coûts de l'utilisateur</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <p><b>Pas d’accès</b> (sélection par défaut)</p> </li> 
     <li> <b>Afficher</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <p><b>Pas d’accès</b> (sélection par défaut)</p> </li> 
     <li><b>Afficher</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Pas d’accès</b> (seule option disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès aux données financières n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour plus d’informations sur ces options, voir [Vue d’ensemble de la facturation et des revenus](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Gestion des ressources

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour la gestion des ressources :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Niveau d’accès</th> 
   <th>Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificateur </td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : permet un accès intégral à la gestion des ressources.</p> <p>Pour affiner ceci, cliquez sur l’icône en forme d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton <b>Modifer</b>, puis désactivez ou activez l’une des options suivantes. Seule la première option, <b>Modifier les priorités et les heures budgétées dans le Planificateur</b>, est activée par défaut.</p> 
      <ul> 
       <li> <p> Modifier les priorités et les heures budgétées dans le Planificateur</p> </li> 
       <li> <p>Gérer les pools de ressources</p> <p><b>NOTE</b> : afin de gérer les groupes de ressources, une personne doit disposer d’un accès supplémentaire aux données financières et des autorisations sur les finances du projet. Si vous accordez l’accès à la gestion des ressources à une personne du planificateur qui n’a pas accès aux données financières, cette personne peut toujours voir les affectations horaires dans le planificateur de ressources, mais elle ne peut pas passer à la vue des coûts ou afficher le business case. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l’accès aux données financières</a> et <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Partager les autorisations financières sur un objet</a>.</p> </li> 
       <li> <p>Mettre à jour les heures planifiées dans l'équilibreur de charge de travail</p> <p><b>NOTE</b> : pour mettre à jour le nombre d’heures prévues dans l’équilibreur de charge de travail, une personne doit être autorisée à contribuer à l’objet, avec l’option Créer des affectations activée dans les paramètres avancés. Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Vue d’ensemble des autorisations de partage sur les objets</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li><b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> </li> 
     <li> <b>Afficher</b> (sélection par défaut)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Pas d’accès</b> (seule option disponible) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur ou utilisatrice externe</td> 
   <td> <p>L’accès n’est pas disponible. Les utilisateurs et utilisatrices externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour consulter les calendriers qui sont partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Zone Planificateur de scénarios

Le paramètre par défaut pour tous les niveaux d’accès est « Pas d’accès ». Un administrateur ou une administratrice Workfront peut modifier ce paramètre pour accorder l’accès à l’affichage ou à la modification pour tous les niveaux d’accès des personnes en charge de la planification, du travail et des révisions.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Les utilisateurs et utilisatrices peuvent afficher un plan créé par une autre personne uniquement si un lien vers le plan est partagé avec eux.

## Zone Objectifs Workfront

L’ensemble des six niveaux d’accès par défaut (et les quatre types de licence) peuvent modifier et afficher Objectifs Workfront.

Modifier est l’option par défaut.
