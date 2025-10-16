---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Exporter des données depuis Workfront via les Kick-Starts
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser l’exportateur de données Kickstart pour exporter des données de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 89%

---

# Exporter des données depuis Workfront via les Kick-Starts

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser l’exportateur de données Kickstart pour exporter des données de Workfront. Vous pouvez les utiliser dans d’autres applications après les avoir exportées.

L’export de données par le biais des Kickstarts permet également de comprendre quels champs sont associés à chaque objet, la manière dont ces champs sont codés, ainsi que la manière dont les valeurs de ces champs sont formatés dans la base de données.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Administrateur ou administratrice système</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Avantages et inconvénients de l’utilisation de Kickstarts pour exporter des données

Il existe deux manières d’exporter des données dans Workfront :

* Exporter des données depuis un rapport ou une liste

  Pour plus d’informations sur l’export de données depuis un rapport ou une liste, voir [Exporter des données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exporter des données par le biais de Kickstarts

Le tableau suivant présente les avantages et les inconvénients de chaque méthode :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Les données exportées incluent des valeurs d’objet et de champ.</p> </th> 
   <th> <p>Possibilité d’exporter simultanément des données autour de plusieurs types d’objets</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exporter des données à partir d’une vue Liste</strong> </p> <p>Pour plus d’informations sur l’export de données depuis une liste, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exporter des données</a>.</p> </td> 
   <td> <p>Oui</p> <p>Les champs natifs Workfront et les champs personnalisés associés aux objets sont exportés.</p> </td> 
   <td> <p>Non</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exporter des données par le biais de Kickstarts</strong> </p> </td> 
   <td> <p>Oui (limité)</p> <p>La plupart des champs natifs Workfront associés aux objets sont exportés, mais certains ne le sont pas. Par exemple, vous ne pouvez pas exporter les champs Planning, Personne propriétaire du projet ou Personne sponsor du projet par le biais d’un export Kickstart de projet.</p> <p>Dans un projet auquel est associé un formulaire personnalisé, les données saisies dans les champs du formulaire ne sont pas exportées.</p> <p>Vous pouvez toutefois exporter un formulaire personnalisé. Le fichier obtenu répertorie les champs configurés dans le formulaire, tels que les zones de texte et les boutons radio.</p> </td> 
   <td> <p>Oui</p> <p>L’utilisation des Kickstarts pour exporter des données Workfront vous permet d’exporter des données liées à plusieurs types d’objets dans un seul export. Par exemple, vous pouvez inclure des tâches, des problèmes et des projets dans un seul export.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limites d’export

Les restrictions suivantes s’appliquent lors de l’export de données par le biais de Kickstarts (les données sont exportées au format de fichier Excel) :

* **50 000 lignes :** nombre de lignes autorisé dans le fichier.
* **65 530 liens hypertexte :** il s’agit d’une limite imposée par Excel aux documents qui contiennent plus de 65 530 liens hypertexte. Une fois exportés, ces documents ne peuvent plus être ouverts. Notez qu’un document Excel peut ne contenir que 200 lignes de données, mais s’il existe plus de 65 530 liens dans le document, celui-ci ne s’ouvre pas.

## Exporter des données par le biais de Kickstarts

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Kickstarts**, puis cliquez sur **Exporter des données.**

1. Sélectionnez l’objet à exporter. Par défaut, les objets suivants sont affichés sous **Éléments à inclure** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objet</strong> </p> </th> 
      <th> <p><strong>Feuilles exportées du fichier Excel</strong> </p> </th> 
      <th> <p> <strong>Format d’export</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Tableau de bord</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Paramètre<br>Option de paramètre<br>Groupe de paramètres<br>Paramètre de catégorie<br>Catégorie<br>Rapport<br>Section Onglet de portail<br>Tableau de bord<br>Préférences</p> </td> 
      <td scope="col" valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Rapport</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Paramètre<br>Option de paramètre<br>Groupe de paramètres<br>Paramètre de catégorie<br>Catégorie<br>Rapport<br>Préférences</td> 
      <td scope="col" valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Approbation</p> </td> 
      <td scope="col" valign="top"> <p>Personne approbatrice d’étape<br>Étape d’approbation<br>Approbation<br>Processus d’approbation<br>Préférences</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Données personnalisées</p> </td> 
      <td scope="col" valign="top"> <p>Paramètre<br>Option de paramètre<br>Groupe de paramètres<br>Paramètre de catégorie<br>Catégorie<br>Préférences</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Type de frais</p> </td> 
      <td valign="top"> <p>Type de dépense<br>Préférences</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Type d’heure</p> </td> 
      <td valign="top"> <p>Type d’heure<br>Préférences</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Equipe</p> </td> 
      <td valign="top"> Personnes membre de l’équipe<br>Équipe<br>Préférences </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
      <td valign="top"> <p>Utilisateur ou utilisatrice<br>Préférences</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Si l’option **Tableau de bord** n’est pas disponible, cela signifie que votre système ne comporte aucun tableau de bord partagé à l’échelle du système. Vous ne pouvez pas exporter de tableaux de bord privés.

1. Cliquez sur **Plus d’options** pour afficher la liste intégrale des objets.

   Tous les objets répertoriés ici peuvent également être utilisés pour importer des données dans Workfront.

   La seule exception est l’objet **Niveaux d’accès**. La feuille de données des niveaux d’accès incluse dans un export est fournie à titre de référence uniquement. Elle vous permet d’attribuer un niveau d’accès à un nouveau compte d’utilisateur ou d’utilisatrice par ID.

   Pour plus d’informations sur l’import de données dans Workfront par le biais de Kickstarts, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Voici une liste de tous les objets qui peuvent être exportés par le biais de Kickstarts :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Objet</p> </th> 
      <th> <p>Feuilles exportées du fichier Excel</p> </th> 
      <th> <p>Format d’export</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Niveau d’accès</td> 
      <td scope="col" valign="top">Niveau d’accès<br>Préférences</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Affectation</td> 
      <td scope="col" valign="top">Affectation<br>Préférences</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Entreprise</td> 
      <td scope="col" valign="top"> Entreprise<br>Préférences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Modèle d'e-mail</td> 
      <td scope="col" valign="top"> Modèle d’e-mail<br>Préférences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Frais</td> 
      <td valign="top"> Dépense<br>Préférences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Page externe</td> 
      <td valign="top"> Page externe<br>Préférences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filtre</td> 
      <td valign="top"> Filtre<br>Préférences </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Groupe</td> 
      <td valign="top"> Groupe<br>Préférences  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Regroupement </td> 
      <td valign="top"> Regroupement<br>Préférences </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Heure</td> 
      <td valign="top"> Heure<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Problème</td> 
      <td valign="top"> Problème<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Fonction</td> 
      <td valign="top"> Fonction<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Chemin jalonné</td> 
      <td valign="top"> Jalon<br>Chemin jalonné<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Note</td> 
      <td valign="top"> Note<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfolio</td> 
      <td valign="top"> Portfolio<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Projet</td> 
      <td valign="top"> File d’attente<br>Projet<br>Règle de transmission<br>Rubrique de file d’attente<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Estimation de ressources</td> 
      <td valign="top"> Estimation de ressource<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Pool de ressources</td> 
      <td valign="top"> Groupe de ressources<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risque</td> 
      <td valign="top"> Risque<br>Préférences  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Type de risque</td> 
      <td valign="top"> Type de risque<br>Préférences  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Carte de score</td> 
      <td valign="top">Questions relatives aux cartes de performance<br>Option de carte de performance<br>Carte de performance<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tâche</td> 
      <td valign="top"> Tâche<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Modèle</td> 
      <td valign="top"> File d’attente<br>Modèle<br>Règle de transmission<br>Rubrique de file d’attente<br>Préférences </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Modèle d'affectation</td> 
      <td valign="top"> Affectation de modèle<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tâche de modèle</td> 
      <td valign="top"> Tâche de modèle<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Feuille de temps</td> 
      <td valign="top"> Profil de feuille de temps<br>Feuille de temps<br>Préférences </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Afficher </td> 
      <td valign="top"> Vue<br>Préférences  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Télécharger**.

   Le fichier Kickstart exporté est téléchargé sur votre ordinateur sous la forme d’un fichier Excel ou d’un fichier compressé contenant plusieurs fichiers Excel et fichiers de propriétés. Chaque fichier Excel est un ensemble de feuilles, chacune représentant un champ associé à l’objet sélectionné. Une feuille **Propriétés** est associée à chaque export.

   Les options **Tableau de bord** et **Rapport** permettent de sélectionner des tableaux de bord et des rapports spécifiques à inclure dans le téléchargement. Pour les tableaux de bord, vous pouvez uniquement exporter des tableaux de bord partagés à l’échelle du système.

   Il n’est pas possible d’exporter les rapports de matrice. Pour plus d’informations sur les rapports de matrice, voir la section [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Kick-Starts ne prend pas en charge les filtres ou les regroupements en mode texte. Pour une exportation réussie, les filtres et les regroupements de rapports doivent passer en mode standard.

   Vous pouvez sélectionner jusqu’à 100 tableaux de bord et 100 rapports dans une seule exportation.

   ![Exportation Kickstart](assets/kickstart-export-spreadsheet-options.png)

   Vous pouvez exporter plusieurs objets simultanément.

1. (Recommandé) Analysez les données exportées pour vous assurer que toutes les informations voulues ont été exportées.

   Pour les exports volumineux, Workfront fonctionne en arrière-plan pour produire le fichier Excel et vous avertit du retard. Le fichier de démarrage vous est envoyé par e-mail à la fin du téléchargement.

