---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Exporter des données d’Adobe Workfront par le biais de Démarrages de session
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser l’exportateur de données de démarrage rapide pour exporter des données de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 8e076e9c89ad208aa94ddefead4b8c6105992542
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Exporter des données d’Adobe Workfront par le biais de Démarrages de session

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser l’exportateur de données de démarrage rapide pour exporter des données de Workfront. Vous pouvez l’utiliser dans d’autres applications après l’avoir exportée.

L’export de données par le biais des Kick-Starts permet également de comprendre les champs associés à chaque objet, la manière dont ces champs sont codés, ainsi que la manière dont les valeurs de ces champs sont formatées dans la base de données.

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
   <p>Nouveau : Standard</p>
   Ou
   <p>Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Avantages et inconvénients de l’utilisation de lancements d’essai pour exporter des données

Il existe deux manières d’exporter des données dans Workfront :

* Exporter des données depuis un rapport ou une liste

  Pour plus d’informations sur l’export de données depuis un rapport ou une liste, voir [Exporter des données](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exporter des données par le biais de démarrages

Le tableau suivant présente les avantages et les inconvénients de chaque méthode :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Les données exportées incluent des valeurs d’objet et de champ</p> </th> 
   <th> <p>Possibilité d’exporter simultanément des données autour de plusieurs types d’objets</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exportation de données à partir d’un mode Liste</strong> </p> <p>Pour plus d’informations sur l’export de données depuis une liste, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exporter des données</a></p> </td> 
   <td> <p>Oui</p> <p>Les champs natifs Workfront et les champs personnalisés associés aux objets sont exportés.</p> </td> 
   <td> <p>Non</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exporter des données par le biais de start-ups</strong> </p> </td> 
   <td> <p>Oui (limité)</p> <p>La plupart des champs natifs Workfront associés aux objets sont exportés, mais certains ne le sont pas. Par exemple, vous ne pouvez pas exporter les champs Planification, Propriétaire du projet ou Parrain du projet par le biais d’une exportation de lancement de projet.</p> <p>Dans un projet auquel est associé un formulaire personnalisé, les données saisies dans les champs du formulaire ne sont pas exportées.</p> <p>Vous pouvez toutefois exporter un formulaire personnalisé. Le fichier obtenu répertorie les champs configurés dans le formulaire, tels que les zones de texte et les boutons radio.</p> </td> 
   <td> <p>Oui</p> <p>L’utilisation du bouton de sélection pour exporter des données Workfront vous permet d’exporter des données liées à plusieurs types d’objets dans une seule exportation. Par exemple, vous pouvez inclure des tâches, des problèmes et des projets dans un seul export.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limites d’exportation

Les restrictions suivantes s’appliquent lors de l’exportation de données par démarrage rapide (les données sont exportées au format de fichier Excel) :

* **50 000 lignes :** Le nombre de lignes autorisé dans le fichier.
* **65 530 liens hypertexte :** Il s’agit d’une limite imposée par Excel aux documents qui contiennent plus de 65 530 liens hypertexte. Une fois exportés, ces documents ne peuvent plus être ouverts. Notez qu’un document Excel ne peut contenir que 200 lignes de données, mais s’il existe plus de 65 530 liens dans le document, celui-ci ne s’ouvre pas.

## Exporter des données par le biais de lancements

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Démarrages,** puis cliquez sur **Exporter des données.**

1. Sélectionnez l’objet à exporter. Par défaut, les objets suivants sont affichés sous **Eléments à inclure**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objet</strong> </p> </th> 
      <th> <p><strong>Feuilles exportées du fichier Excel</strong> </p> </th> 
      <th> <p> <strong>Format d’exportation</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Tableau de bord</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Paramètre<br>Option de paramètre<br>Groupe de paramètres<br>Paramètre de catégorie<br>Catégorie<br>Rapport<br>Section d’onglet Portail<br>Tableau de bord<br>Préférences</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Rapport</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Paramètre<br>Option de paramètre<br>Groupe de paramètres<br>Paramètre de catégorie<br>Catégorie<br>Rapport<br>Préférences</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Approbation</p> </td> 
      <td scope="col" valign="top"> <p>Approbateur d’étape<br>Étape de validation<br>Validation<br>Processus d’approbation<br>Préférences</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Données personnalisées</p> </td> 
      <td scope="col" valign="top"> <p>Paramètre<br>Option de paramètre<br>Groupe de paramètres<br>Paramètre de catégorie<br>Catégorie<br>Préférences</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
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
      <td valign="top"> Membre de l’équipe<br>Équipe<br>Préférences </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>l’utilisateur ou de l’utilisatrice</p> </td> 
      <td valign="top"> <p>Utilisateur<br>Préférences</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Plus d’options** pour afficher la liste complète des objets.

   Tous les objets répertoriés ici peuvent également être utilisés pour importer des données dans Workfront.

   La seule exception est la **Niveaux d’accès** . La feuille de données des niveaux d’accès incluse dans une exportation est fournie à titre de référence uniquement. Il vous permet d’attribuer un niveau d’accès à un nouveau compte utilisateur par identifiant.

   Pour plus d’informations sur l’importation de données dans Workfront par le biais de démarrages de session, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Voici une liste de tous les objets qui peuvent être exportés par le biais de démarrages :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Objet</p> </th> 
      <th> <p>Feuilles exportées du fichier Excel</p> </th> 
      <th> <p>Format d’exportation</p> </th> 
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
      <td scope="col" valign="top">Attribution<br>Préférences</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Entreprise</td> 
      <td scope="col" valign="top"> Société<br>Préférences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Modèle d'e-mail</td> 
      <td scope="col" valign="top"> Modèle de courrier électronique<br>Préférences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Frais</td> 
      <td valign="top"> Dépense<br>Préférences </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Page externe</td> 
      <td valign="top"> Page externe<br>Préférences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filtre</td> 
      <td valign="top"> Filtrer<br>Préférences </td> 
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
      <td valign="top"> Rôle de tâche<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Chemin jalonné</td> 
      <td valign="top"> Milestone<br>Chemin Milestone<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Note</td> 
      <td valign="top"> Remarque<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfolio</td> 
      <td valign="top"> Portfolio<br>Préférences  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Projet</td> 
      <td valign="top"> File d’attente<br>Projet<br>Règle de routage<br>Rubrique de la file d’attente<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Estimation de ressources</td> 
      <td valign="top"> Estimation de ressource<br>Préférences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Pool de ressources</td> 
      <td valign="top"> Pool de ressources<br>Préférences </td> 
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
      <td valign="top">Questions relatives à la Fiche d’évaluation<br>Option de Fiche d’évaluation<br>Fiche d’évaluation<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tâche</td> 
      <td valign="top"> Tâche<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Modèle</td> 
      <td valign="top"> File d’attente<br>Modèle<br>Règle de routage<br>Rubrique de la file d’attente<br>Préférences </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Modèle d'affectation</td> 
      <td valign="top"> Attribution de modèles<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tâche de modèle</td> 
      <td valign="top"> Tâche du modèle<br>Préférences </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Feuille de temps</td> 
      <td valign="top"> Profil de feuille de calcul<br>Feuille de calcul<br>Préférences </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Afficher </td> 
      <td valign="top"> Affichage<br>Préférences  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Téléchargez.**

   Le fichier de démarrage rapide exporté est téléchargé sur votre ordinateur sous la forme d’un fichier Excel ou d’un fichier . fichier zip contenant plusieurs fichiers Excel et de propriétés. Chaque fichier Excel est un ensemble de feuilles, où chaque feuille représente un champ associé à l’objet sélectionné. Il existe une **Propriétés** feuille associée à chaque export.

   La variable **Tableau de bord** et **Rapport** Les options vous permettent de sélectionner des tableaux de bord et des rapports spécifiques à inclure dans le téléchargement. Vous ne pouvez exporter que les tableaux de bord, qui sont partagés à l’échelle du système.

   Vous ne pouvez pas exporter de rapports de matrice. Pour plus d’informations sur les rapports de matrice, voir [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Le démarrage rapide ne prend pas en charge les filtres en mode texte. Pour réussir l’exportation, les filtres de création de rapports doivent être basculés en mode standard.

   Vous pouvez sélectionner jusqu’à 100 tableaux de bord et 100 rapports dans un seul export.

   ![](assets/kickstart-export-350x381.png)

   Vous pouvez exporter plusieurs objets simultanément.

1. (Recommandé) Analysez les données exportées pour vous assurer que toutes les informations que vous attendez à voir ont été exportées.

   Pour les exportations volumineuses, Workfront fonctionne en arrière-plan pour produire le fichier Excel et vous avertit du retard. Le fichier de démarrage vous est envoyé par courrier électronique à la fin du téléchargement.

   ![](assets/large-kick-start-file-warning-350x65.png)
