---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrer les rapports par périodes.
description: Vous pouvez filtrer un rapport en fonction de la période d’une date qui existe sur un objet. Par exemple, vous pouvez filtrer un rapport d’heures en fonction de la période pendant laquelle les heures ont été saisies.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 97%

---

# Filtrer les rapports par périodes.

<!-- Audited: 11/2024 -->

Vous pouvez filtrer un rapport en fonction de la période d’une date qui existe sur un objet. Par exemple, vous pouvez filtrer un rapport d’heures en fonction de la période pendant laquelle les heures ont été saisies.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
      <td> 
      <p>Nouveau :</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Actuel :</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en modification aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et regroupements</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Le rapport doit être créé avant de filtrer les résultats.

Pour plus d’informations sur la création de rapports, consultez [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrer un rapport en fonction de la période d’une date. {#filter-a-report-by-the-time-frame-of-a-date}

1. Cliquez sur l&#39;icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png), puis sur **Rapports**.

1. Cliquez sur **Nouveau rapport**, puis sélectionnez le type de rapport souhaité.\
   Par exemple, sélectionnez **Rapport sur les heures**.

1. Sélectionnez l’onglet **Filtres**.
1. Cliquez sur **Ajouter une règle de filtre**, puis sélectionnez **Date de saisie des heures**.\
   ![Filtrage du rapport sur les heures par période](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Dans le menu déroulant suivant, sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Égal à</td> 
      <td>Après avoir sélectionné ce modificateur, indiquez la date à laquelle les heures ont été saisies.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non égal à</td> 
      <td>Après avoir sélectionné ce modificateur, indiquez la date à laquelle les heures ont été saisies, afin d’exclure cette date de votre rapport. Le rapport affiche les heures enregistrées à toutes les dates, à l’exception de la date que vous avez spécifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null</td> 
      <td>Sélectionnez ce modificateur pour n’afficher que les heures pour lesquelles la date de saisie est manquante.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non null</td> 
      <td>Sélectionnez ce modificateur pour n’afficher que les heures pour lesquelles la date de saisie a une valeur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entre</td> 
      <td>Après avoir sélectionné ce modificateur, indiquez une période pendant laquelle les heures ont été saisies. Le rapport présente les heures saisies entre les dates spécifiées.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inférieur à</td> 
      <td>Après avoir sélectionné ce modificateur, indiquez une date avant laquelle les heures ont été saisies. Le rapport présente les heures saisies avant la date spécifiée, sans compter la date spécifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inférieur ou égal à</td> 
      <td>Après avoir sélectionné ce modificateur, indiquez une date avant laquelle les heures ont été saisies. Le rapport présente les heures saisies avant la date spécifiée, y compris la date spécifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supérieur à</td> 
      <td>Après avoir sélectionné ce modificateur, indiquez une date après laquelle les heures ont été saisies. Le rapport présente les heures saisies après la date spécifiée mais pas à la date spécifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supérieur ou égal à</td> 
      <td> <p>Après avoir sélectionné ce modificateur, indiquez une date après laquelle les heures ont été saisies. Le rapport présente les heures saisies après la date spécifiée, y compris la date spécifiée.</p> <p>Sélectionnez l’un des modificateurs de période intégrés, tel que décrit dans <a href="#built-in-time-frame-modifiers" class="MCXref xref">Modificateurs de période intégrés</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ces modificateurs sont disponibles pour tout champ de date dans un filtre ou une invite dans un rapport.
1. Cliquez sur **Enregistrer + Fermer**.

## Modificateurs de période intégrés {#built-in-time-frame-modifiers}

Adobe Workfront dispose de modificateurs de période intégrés que vous pouvez utiliser sans définir de date spécifique. 

Ces modificateurs sont disponibles pour tout champ de date dans un filtre ou une invite dans un rapport. 

Pour plus d’informations sur la manière de filtrer un rapport en fonction d’une période associée à une date, voir [Filtrer un rapport en fonction de la période d’une date](#filter-a-report-by-the-time-frame-of-a-date).

Par exemple, si vous créez un rapport sur les heures et que vous souhaitez afficher les heures saisies au cours d’une période spécifique, vous pouvez choisir parmi les options de filtrage par période intégrée suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aujourd’hui</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est aujourd’hui.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cette semaine</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date de la semaine en cours, la semaine commençant un dimanche et se terminant un samedi.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Semaine prochaine</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date de la semaine suivant la semaine en cours, la semaine commençant un dimanche et se terminant un samedi. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Semaine dernière</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date de la semaine précédant la semaine en cours, la semaine commençant un dimanche et se terminant un samedi. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ce mois</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date du mois en cours.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mois prochain</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date du mois suivant le mois en cours.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Mois dernier</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date du mois précédant le mois en cours.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ce trimestre</td> 
   <td> <p>Affiche les heures pour lesquelles la date de saisie est une date du trimestre en cours, les trimestres étant définis comme suit :</p> 
    <ul> 
     <li>Premier trimestre : du 1er janvier au 30 mars</li> 
     <li>Deuxième trimestre : du 1er avril au 30 juin</li> 
     <li>Troisième trimestre : du 1er juillet au 30 septembre</li> 
     <li>Quatrième trimestre : du 1er octobre au 31 décembre</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Trimestre prochain</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date du trimestre suivant le trimestre en cours, les trimestres ayant été définis ci-dessus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Trimestre dernier</td> 
   <td> <p>Affiche les heures pour lesquelles la date de saisie est une date du trimestre précédant le trimestre en cours, les trimestres ayant été définis ci-dessus.</p> <p>Remarque : si votre administrateur ou administratrice Workfront a activé et défini des trimestres personnalisés pour votre système, les filtres intégrés pour les trimestres sont remplacés par vos informations personnalisées sur les trimestres. Pour plus d’informations sur l’activation des trimestres personnalisés, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Activer les trimestres personnalisés pour les projets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cette année</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date de l’année en cours, l’année en cours commençant le 1er janvier et se terminant le 31 décembre.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Année passée</td> 
   <td>Affiche les heures pour lesquelles la date de saisie est une date de l’année écoulée, l’année écoulée commençant 12 mois avant la date actuelle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Année dernière</td> 
   <td> <p>Affiche les heures pour lesquelles la date de saisie est une date de l’année écoulée, l’année écoulée commençant le 1er janvier et se terminant le 31 décembre de l’année précédant l’année en cours.</p> <p>Remarque : il n’y a pas de période intégrée pour l’année fiscale. Vous pouvez créer un rapport et filtrer les informations par date en utilisant un modificateur personnalisé pour la période de l’année fiscale, telle qu’elle est définie dans votre entreprise. Si vous souhaitez choisir une période pour un exercice comptable sur place, vous devez utiliser une invite plutôt qu’un filtre. </p> </td> 
  </tr> 
 </tbody> 
</table>
