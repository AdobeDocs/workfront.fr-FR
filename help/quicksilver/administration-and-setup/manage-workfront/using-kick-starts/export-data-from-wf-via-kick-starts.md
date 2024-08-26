---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Exportation des données de Workfront via le démarrage
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser l’exporteur de données Kickstart pour exporter des données à partir de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '1011'
ht-degree: 98%

---

# Exportation des données de Workfront via le démarrage

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser l’exporteur de données Kickstart pour exporter des données à partir de Workfront. Vous pouvez les utiliser dans d’autres applications après les avoir exportées.

L’export de données par le biais des Kickstarts permet également de comprendre quels champs sont associés à chaque objet, la manière dont ces champs sont codés, ainsi que la manière dont les valeurs de ces champs sont formatées dans la base de données.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouvelle : standard</p>
   Ou
   <p>Actuelle : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Avantages et inconvénients de l’utilisation de Kickstarts pour exporter des données

Il existe deux manières d’exporter des données dans Workfront :

* Exporter des données depuis un rapport ou une liste

  Pour plus d’informations sur l’export de données depuis un rapport ou une liste, consultez [Exporter des données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exporter des données via des Kickstarts

Le tableau suivant présente les avantages et les inconvénients de chaque méthode :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Les données exportées incluent des valeurs d’objets et de champs.</p> </th> 
   <th> <p>Possibilité d’exporter simultanément des données impliquant plusieurs types d’objets</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exporter des données à partir d’une vue Liste</strong> </p> <p>Pour plus d’informations sur l’export de données depuis une liste, consultez <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exporter des données</a>.</p> </td> 
   <td> <p>Oui</p> <p>Les champs natifs Workfront et les champs personnalisés associés aux objets sont exportés.</p> </td> 
   <td> <p>Non</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exporter des données via des Kickstarts</strong> </p> </td> 
   <td> <p>Oui (limité)</p> <p>La plupart des champs natifs Workfront associés aux objets sont exportés, mais certains ne le sont pas. Par exemple, vous ne pouvez pas exporter les champs Planning, Personne propriétaire du projet ou Personne sponsor du projet via un export Kickstart de projet.</p> <p>Dans un projet auquel est associé un formulaire personnalisé, les données saisies dans les champs du formulaire ne sont pas exportées.</p> <p>Vous pouvez toutefois exporter un formulaire personnalisé. Le fichier obtenu répertorie les champs configurés dans le formulaire, tels que les zones de texte et les cases d’option.</p> </td> 
   <td> <p>Oui</p> <p>L’utilisation des Kickstarts pour exporter des données Workfront vous permet d’exporter des données impliquant plusieurs types d’objets dans un seul export. Par exemple, vous pouvez inclure des tâches, des problèmes et des projets dans un seul export.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limites d’export

Les restrictions suivantes s’appliquent lors de l’export de données via des Kickstarts (les données sont exportées au format de fichier Excel) :

* **50 000 lignes :** nombre de lignes autorisé dans le fichier.
* **65 530 liens hypertexte : il s’agit d’une limite imposée par Excel aux documents qui contiennent plus de 65 530 liens hypertexte.** Une fois exportés, ces documents ne peuvent plus être ouverts. Notez que si un document Excel ne contient que 200 lignes de données, mais plus de 65 530 liens, il ne s’ouvrira pas.

## Exporter des données via des Kickstarts

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Kickstarts**, puis cliquez sur **Exporter des données.**

1. Sélectionnez l’objet que vous souhaitez exporter. Par défaut, les objets suivants sont affichés dans **Éléments à inclure** :

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
      <td valign="top"> Personne membre de l’équipe<br>Équipe<br>Préférences </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
      <td valign="top"> <p>Utilisateur ou utilisatrice<br>Préférences</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Plus d’options** pour afficher la liste complète des objets.

   Tous les objets répertoriés ici peuvent également être utilisés pour importer des données dans Workfront.

   La seule exception est l’objet Niveaux d’accès. **** La feuille de données des niveaux d’accès incluse dans un export est fournie à titre de référence uniquement. Elle vous permet d’affecter un niveau d’accès à un nouveau compte d’utilisateur ou d’utilisatrice par ID.

   Pour plus d’informations sur l’import de données dans Workfront via des Kickstarts, consultez Importer des données dans Adobe Workfront à l’aide d’un modèle Kickstart. [](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md) Voici une liste de tous les objets qui peuvent être exportés via des Kickstarts :

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
      <td scope="col" valign="top">Modèle d’e-mail</td> 
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
      <td valign="top"> PortfolioPréférences <br> </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Projet</td> 
      <td valign="top"> File d’attente<br>Projet<br>Règle de routage<br>Rubrique de file d’attente<br>Préférences </td> 
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
      <td valign="top"> File d’attente<br>Modèle<br>Règle de routage<br>Rubrique de file d’attente<br>Préférences </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Modèle d’affectation</td> 
      <td valign="top"> Modèle d’affectation<br>Préférences </td> 
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

   Le fichier Kickstart exporté est téléchargé sur votre ordinateur sous la forme d’un fichier Excel ou d’un fichier compressé ZIP contenant plusieurs fichiers Excel et fichiers de propriétés. Chaque fichier Excel est un ensemble de feuilles, chacune représentant un champ associé à l’objet que vous avez sélectionné. Une feuille **Propriétés** est associée à chaque export.

   Les options **Tableau de bord** et **Rapport** permettent de sélectionner des tableaux de bord et des rapports spécifiques à inclure dans le téléchargement. Vous ne pouvez exporter que les tableaux de bord qui sont partagés à l’échelle du système.

   Il n’est pas possible d’exporter les rapports de matrice. Pour plus d’informations sur les rapports de matrice, consultez la section [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Kick-Starts ne prend pas en charge les filtres en mode texte. Pour effectuer un export, les filtres de création de rapports doivent être définis en mode standard.

   Vous pouvez sélectionner jusqu’à 100 tableaux de bord et 100 rapports pour un seul export.

   ![](assets/kickstart-export-350x381.png)

   Vous pouvez exporter plusieurs objets simultanément.

1. (Recommandé) Analysez les données exportées pour vous assurer que toutes les informations souhaitées ont été exportées.

   Pour les exports volumineux, Workfront fonctionne en arrière-plan pour produire le fichier Excel et vous avertit du délai d’attente supplémentaire. Le fichier Kickstart vous est envoyé par e-mail à la fin du téléchargement.

   ![](assets/large-kick-start-file-warning-350x65.png)
