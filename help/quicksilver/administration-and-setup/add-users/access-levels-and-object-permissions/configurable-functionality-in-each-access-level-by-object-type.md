---
title: Accès configurable à la fonctionnalité pour chaque type d’objet
description: Cet article explique ce que vous pouvez autoriser en tant qu’administrateur Adobe Workfront pour chaque type d’objet, à chaque niveau d’accès. Il explique également la configuration par défaut pour chaque type de niveau d’accès.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '3435'
ht-degree: 10%

---

# Accès configurable à la fonctionnalité pour chaque type d’objet

Cet article explique ce que vous pouvez autoriser en tant qu’administrateur Adobe Workfront pour chaque type d’objet, à chaque niveau d’accès. Il explique également la configuration par défaut pour chaque type de niveau d’accès.

Pour plus d’informations sur toutes les fonctionnalités disponibles pour un type d’objet dans chaque niveau d’accès, voir [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Projets

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les projets :

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
   <td>Planificateur (type de licence Plan)</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des projets. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des projets.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Copier</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Afficher</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des projets. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès limité à l’édition des projets. Pour voir comment l’accès Modifier est limité dans un niveau d’accès Travailleur par rapport à un niveau d’accès Planificateur (qui permet un accès de modification complet aux projets), consultez la section . <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Projets</a> dans l’article <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Fonctionnalités disponibles pour chaque type d’objet</a>.</p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des projets. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Modifier , puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li> <b>Affichage</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> (sélection par défaut) <p>L’accès aux vues est limité, car vous ne pouvez pas l’affiner pour activer ou désactiver le partage de projet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux projets n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tâches

Dans chaque niveau d&#39;accès, vous pouvez configurer les options suivantes pour les tâches :

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
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire cette fonctionnalité, vous pouvez configurer la possibilité de partager des tâches. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à l'édition des tâches.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire cette fonctionnalité, vous pouvez configurer la possibilité de partager des tâches. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à l'édition des tâches.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
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
     <li> <b>Accès interdit</b> </li> 
     <li> <b>Affichage</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> (sélection par défaut)<p>L’accès aux vues est limité, car vous ne pouvez pas l’affiner pour activer ou désactiver le partage de projet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux tâches n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Événements

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les problèmes :

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
     <li> <b>Accès interdit</b> </li> 
     <li> <p><b>Afficher</b></p><p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des problèmes. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet aux modifications pour les problèmes.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des problèmes. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet aux modifications pour les problèmes.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
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
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des problèmes. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet aux modifications pour les problèmes.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
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
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des problèmes. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet aux modifications pour les problèmes.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux problèmes n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portefeuilles

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les portefeuilles :

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
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des portefeuilles. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des portefeuilles.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li> <b>Affichage</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li> <b>Affichage</b> (sélection par défaut)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> <p>L’accès aux portefeuilles n’est pas disponible.</p> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux portefeuilles n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programmes

Dans chaque niveau d&#39;accès, vous pouvez configurer les options suivantes pour les programmes :

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
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des programmes. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des programmes.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li> <b>Affichage</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li> <b>Affichage</b> (sélection par défaut)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> <p>L’accès aux programmes n’est pas disponible.</p> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux programmes n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Rapports, tableaux de bord et calendriers

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les rapports, les tableaux de bord et les calendriers :

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
     <li> <b>Accès interdit</b> </li> 
     <li> <p><b>Afficher</b></p><p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> ), puis désactivez ou activez l’une des actions suivantes. Les deux sont activés par défaut :</p> 
      <ul> 
       <li> <p>Afficher les rapports intégrés</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des rapports, des tableaux de bord et des calendriers.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut, sauf pour <b>Affichage des rapports intégrés</b>, <b>Partage des rapports publiquement</b>, et <b>Partager à l’échelle du système</b>.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Afficher les rapports intégrés</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partage des rapports publiquement (en externe)</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> (sélection par défaut)<p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des actions suivantes. Les deux sont activés par défaut :</p> 
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
     <li> <b>Accès interdit</b> </li> 
     <li> <p><b>Affichage</b> (sélection par défaut)<p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des actions suivantes. Seule l’option Partager est activée par défaut.</p> 
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
     <li> <b>Accès interdit</b> </li> 
     <li> <p><b>Affichage</b> (sélection par défaut) : Permet un accès en lecture seule aux rapports, tableaux de bord et calendriers qui ont été partagés avec eux.</p> <p>Pour affiner ce paramétrage, vous pouvez configurer la possibilité d’afficher des rapports natifs. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> bouton, puis désactivez ou activez <b>Affichage intégré</b>(désactivé par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux rapports, aux tableaux de bord et aux calendriers n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filtres, vues et regroupements

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les filtres, les vues et les regroupements :

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
     <li> <p><b>Afficher</b></p><p>Pour parfaire cette fonctionnalité, vous pouvez configurer la possibilité de partager des filtres, des vues et des regroupements. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des filtres, des vues et des regroupements.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <p><b>Afficher</b></p><p>Pour parfaire cette fonctionnalité, vous pouvez configurer la possibilité de partager des filtres, des vues et des regroupements. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des filtres, des vues et des regroupements.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire cette fonctionnalité, vous pouvez configurer la possibilité de partager des filtres, des vues et des regroupements. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des filtres, des vues et des regroupements.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Afficher</b>:</p> <p>Pour parfaire cette fonctionnalité, vous pouvez configurer la possibilité de partager des filtres, des vues et des regroupements. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des filtres, des vues et des regroupements.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux filtres, aux vues et aux regroupements n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Documents

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les documents :

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
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des documents. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des documents.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut, sauf pour <b>Partager des documents publiquement</b> et <b>Partager à l’échelle du système</b>.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager des documents publiquement (en externe)</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li> <p><b>Afficher</b></p><p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des documents. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des documents.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut, sauf pour <b>Partager des documents publiquement</b> et <b>Partager à l’échelle du système</b>.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager des documents publiquement (en externe)</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des documents. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des documents.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des actions suivantes. Tous sont activés par défaut, sauf pour les deux derniers, <b>Partager des documents publiquement</b> et <b>Partager à l’échelle du système</b>.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager des documents publiquement (en externe)</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li> <p><b>Afficher</b></p><p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité de partager des documents. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification des documents.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux documents n’est pas configurable dans ce niveau d’accès. Cependant, les utilisateurs externes peuvent utiliser Workfront pour afficher, réviser et télécharger des documents.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Utilisateurs

Dans chaque niveau d&#39;accès, vous pouvez configurer les options suivantes pour les utilisateurs :

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
     <li> <p><b>Afficher</b></p><p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité d'afficher les coordonnées des utilisateurs. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’option <b>Afficher les coordonnées</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à l’édition aux utilisateurs.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des actions suivantes. Seules les deux premières options, <b>Créer</b> et <b>Supprimer</b>, sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li>Administration des utilisateurs (tous les utilisateurs)</li> 
       <li> <p>Administration des utilisateurs (utilisateurs du groupe)</p> </li> 
      </ul> <p>Pour plus d’informations sur les deux options d’administration des utilisateurs, voir la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurer l’accès des utilisateurs à la modification des utilisateurs à l’aide d’un niveau d’accès personnalisé</a> dans l’article <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li><p> <b>Affichage</b> (seule option disponible)</p><p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité d'afficher les coordonnées des utilisateurs. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’option <b>Afficher les coordonnées</b> (activée par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li><p> <b>Affichage</b> (seule option disponible)</p> <p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité d'afficher les coordonnées des utilisateurs. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis activez ou désactivez l’option <b>Afficher les coordonnées</b> (désactivée par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Affichage</b> (seule option disponible)</p><p>Pour parfaire ce paramétrage, vous pouvez configurer la possibilité d'afficher les coordonnées des utilisateurs. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis activez ou désactivez l’option <b>Afficher les coordonnées</b> (désactivée par défaut).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux utilisateurs n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Équipes

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour les équipes :

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
     <li><b>Afficher</b> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’une des options suivantes*. Les deux sont désactivés par défaut.</p> 
      <ul> 
       <li>Afficher toutes les équipes</li> 
       <li> <p>Afficher les équipes associées à mes groupes</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet aux modifications aux équipes.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’une des options suivantes*. Toutes sont activées par défaut, sauf pour <b>Éditer les équipes sur lesquelles je suis</b>.</p> 
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
      <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’une des options suivantes*. Les deux sont activés par défaut.</p> 
      <ul> 
       <li>Afficher toutes les équipes</li> 
       <li> <p>Afficher les équipes associées à mes groupes</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet aux modifications aux équipes.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’une des options suivantes*. Seule la première option, <b>Éditer les équipes sur lesquelles je suis</b>, est désactivé par défaut.</p> 
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
     <li> <p><b>Affichage</b> (seule option disponible)</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’une des options suivantes*. Les deux sont activés par défaut.</p> 
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
     <li> <p><b>Affichage</b> (seule option disponible)</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’une des options suivantes*. Les deux sont activés par défaut.</p> 
      <ul> 
       <li> <p>Afficher toutes les équipes</p> </li> 
       <li>Afficher les équipes associées à mes groupes</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux équipes n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Modèles

Dans chaque niveau d&#39;accès, vous pouvez configurer les options suivantes pour les modèles :

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
     <li> <b>Accès interdit</b> </li> 
     <li><p> <b>Afficher</b></p> <p>Pour parfaire cette fonctionnalité, vous pouvez configurer la possibilité de partager des modèles. Cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le bouton Afficher, puis désactivez ou activez l’option <b>Partager</b> (activée par défaut).</p> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet aux modifications des modèles.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Tous sont activés par défaut.</p> 
      <ul> 
       <li> <p>Créer</p> </li> 
       <li> <p>Supprimer</p> </li> 
       <li> <p>Partager</p> </li> 
       <li> <p>Partager à l’échelle du système</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li> <p><b>Accès interdit</b> (seule option disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <p><b>Accès interdit</b> (seule option disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Accès interdit</b> (seule option disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès aux modèles n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Données financières

Dans chaque niveau d&#39;accès, vous pouvez configurer les options suivantes pour les données financières :

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
     <li> <b>Accès interdit</b> </li> 
     <li> <p><b>Afficher</b>:</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’une des options suivantes*. Les deux sont activés par défaut.</p> 
      <ul> 
       <li>Afficher les taux de facturation et de coûts du rôle</li> 
       <li> <p>Afficher les taux de facturation et de coûts de l'utilisateur</p> </li> 
      </ul> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à l'édition des données financières.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Affichage</b> , puis désactivez ou activez l’une des options suivantes*. Seules les deux dernières options, <b>Afficher la facturation et les taux de coût des rôles</b> et <b>Afficher les taux de facturation et de coûts des utilisateurs</b>, sont activés par défaut.</p> 
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
     <li> <p><b>Accès interdit</b> (sélection par défaut)</p> </li> 
     <li> <b>Afficher</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <p><b>Accès interdit</b> (sélection par défaut)</p> </li> 
     <li><b>Afficher</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <p><b>Accès interdit</b> (seule option disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L'accès aux données financières n'est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Pour plus d’informations sur ces options, voir [Présentation de la facturation et des recettes](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Gestion des ressources

Dans chaque niveau d’accès, vous pouvez configurer les options suivantes pour la gestion des ressources :

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
     <li> <b>Accès interdit</b> </li> 
     <li> <b>Afficher</b> </li> 
     <li> <p><b>Modifier</b> (sélection par défaut) : Permet un accès complet à la modification de la gestion des ressources.</p> <p>Pour affiner ce paramétrage, cliquez sur l’icône d’engrenage <img src="assets/gear-icon-in-access-levels.png"> sur le <b>Modifier</b> , puis désactivez ou activez l’une des options suivantes. Seule la première option, <b>Modifier les priorités et les heures du budget dans le planificateur</b>, est activé par défaut.</p> 
      <ul> 
       <li> <p> Modifier les priorités et les heures budgétées dans le Planificateur</p> </li> 
       <li> <p>Gérer les pools de ressources</p> <p><b>REMARQUE</b>: Pour gérer les pools de ressources, un utilisateur a besoin d’un accès supplémentaire aux données financières et des autorisations pour les finances du projet. Si vous accordez l’accès à la gestion des ressources à un utilisateur du planificateur qui n’a pas accès aux données financières, l’utilisateur peut toujours voir les affectations horaires dans le planificateur de ressources, mais ne peut pas passer en vue Coût ou consulter l’analyse de cas. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l'accès aux données financières</a> et <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Partage des autorisations financières sur un objet</a>.</p> </li> 
       <li> <p>Mettre à jour les heures planifiées dans l'équilibreur de charge de travail</p> <p><b>REMARQUE</b>: Pour mettre à jour les heures planifiées dans l’équilibreur de charge de travail, un utilisateur doit disposer d’une autorisation pour contribuer à l’objet, en activant l’option Rendre les affectations sous Paramètres avancés. Pour plus d’informations, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Présentation des autorisations de partage sur les objets</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Employé </td> 
   <td> 
    <ul> 
     <li><b>Accès interdit</b> </li> 
     <li> <b>Affichage</b> (sélection par défaut) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Réviseur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> </li> 
     <li> <b>Affichage</b> (sélection par défaut)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Demandeur</td> 
   <td> 
    <ul> 
     <li> <b>Accès interdit</b> (seule option disponible) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur externe</td> 
   <td> <p>L’accès n’est pas disponible. Les utilisateurs externes ne peuvent utiliser Workfront que pour consulter et télécharger des documents et pour afficher les calendriers partagés avec eux.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Zone du planificateur de scénario

Le paramètre par défaut pour tous les niveaux d’accès est Aucun accès. Un administrateur de Workfront peut modifier ce paramètre pour afficher ou modifier l’accès pour n’importe quel niveau d’accès de planificateur, de traitement et de réviseur.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Les utilisateurs peuvent afficher un plan créé par un autre utilisateur uniquement si un lien vers le plan est partagé avec eux.

## Zone Objectifs de Workfront

Les six niveaux d’accès par défaut (et les quatre types de licence) peuvent tous modifier et afficher les objectifs de Workfront.

Modifier est l’option par défaut.
