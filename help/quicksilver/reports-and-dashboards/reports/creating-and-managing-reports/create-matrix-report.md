---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Créer un rapport de matrice
description: Les rapports de matrice présentent des informations récapitulatives sous la forme d’un tableau agrégé, ce qui facilite l’affichage par rapport à si elles étaient affichées dans une liste comme dans un rapport traditionnel.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 97%

---

# Créer un rapport de matrice

Les rapports de matrice présentent des informations récapitulatives sous la forme d’un tableau agrégé, ce qui facilite l’affichage par rapport à si elles étaient affichées dans une liste comme dans un rapport traditionnel.

## Quand utiliser un rapport de matrice

Vous pouvez créer un rapport de matrice pour tout rapport qui contient 2 regroupements ou plus. Un rapport traditionnel peut contenir jusqu’à 3 regroupements et un rapport de matrice peut contenir jusqu’à 4 regroupements.

Par exemple, vous souhaitez créer un rapport sur les heures qui affiche les heures consignées au cours d’une période de 3 mois et vous souhaitez que le rapport soit organisé en fonction de la personne ayant saisi les heures, ainsi que par mois et par semaine.

![Présentation de la matrice des rapports](assets/report-matrix-overview-350x123.png)

## Affichage des données dans un rapport de matrice

Les informations du rapport de matrice sont toujours affichées sous forme de valeur numérique. Dans la plupart des cas, les colonnes contenant une valeur numérique sont mieux adaptées à l’affichage dans un rapport de matrice (heures consignées et coût réel, par exemple).

Cependant, d’autres colonnes (comme Statut) peuvent toujours être affichées dans le rapport de matrice, comme illustré dans le graphique suivant :\
![Statut de la matrice](assets/report-matrix-status-350x73.png)

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
   <td><p>Modifier l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et regroupements</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer un rapport de matrice

1. Créez un rapport traditionnel contenant des données numériques dans la sortie du rapport.\
   Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Accédez au rapport que vous avez créé à l’étape 1, puis cliquez sur **Actions de rapport**, puis sélectionnez **Modifier**.

1. (Le cas échéant) Si vous avez déjà créé une vue et que vous souhaitez l’appliquer à ce rapport, cliquez sur **Appliquer une vue existante**, puis sélectionnez la vue dans la liste déroulante.
1. (Le cas échéant) Si vous souhaitez créer une vue pour le rapport, procédez comme suit :

   1. Cliquez sur l’onglet **Colonnes (vue)**, puis sélectionnez une colonne que vous souhaitez résumer dans le rapport de matrice.
   1. Dans la zone **Paramètres des colonnes**, cliquez sur la liste déroulante **Résumer cette colonne par**, puis sélectionnez l’une des options disponibles pour résumer les informations.

      >[!IMPORTANT]
      >
      >Si cette option n’est pas sélectionnée, les informations de la colonne ne s’affichent pas correctement dans le rapport de matrice.

      ![Matrice résumée](assets/qs-report-matrix-summarized-350x392.png)

   1. Répétez cette opération pour chaque colonne de l’onglet Colonnes (vue), puis cliquez sur **Terminé**.

1. Cliquez sur l’onglet **Regroupements**.
1. (Le cas échéant) Si vous avez déjà créé un regroupement et que vous souhaitez l’appliquer à ce rapport, cliquez sur **Appliquer un regroupement existant**, puis sélectionnez le regroupement dans la liste déroulante.
1. (Le cas échéant) Si vous souhaitez créer un nouveau regroupement de matrice pour le rapport, procédez comme suit :

   1. Sélectionner **Basculer vers le regroupement de matrice** dans le coin supérieur droit de l’interface du créateur.
   1. Dans la section **Regroupements de lignes**, identifiez le regroupement des lignes, qui établit les regroupements horizontaux du tableau.
   1. (Facultatif) Pour ajouter un regroupement de lignes supplémentaire, cliquez sur **Ajouter un regroupement de lignes secondaire**.
   1. Dans la section **Regroupements de colonnes**, identifiez le regroupement des colonnes, qui permet de définir les regroupements verticaux du tableau.
   1. (Facultatif) Pour ajouter un regroupement de colonnes supplémentaire, cliquez sur **Ajouter un regroupement de colonnes secondaire**.
   1. (Le cas échéant) Si vous ajoutez un regroupement par date, indiquez également si les résultats sont regroupés par jour, semaine, mois, trimestre ou année.\
      ![Regroupement par options de date](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. (Le cas échéant) Si vous avez choisi de regrouper par date et d’afficher les résultats par trimestre, indiquez par exemple si vous souhaitez afficher les trimestres sans données en sélectionnant la case à cocher **Afficher les trimestres sans résultat**.\
      ![Afficher les trimestres sans résultats](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >Le champ **Afficher les trimestres sans résultat** n’est disponible que pour les regroupements de matrice, et non pour les regroupements standard.\
      >Seuls les trimestres sans données situés entre deux trimestres contenant des données valides affichent zéro pour les valeurs des données de l’onglet Matrice. Les trimestres qui ne comportent aucune donnée se trouvant au début et à la fin de la période sélectionnée par votre filtre n’apparaissent pas du tout dans le regroupement par matrice. Les trimestres sans résultat ne s’afficheront pas dans un regroupement dans l’onglet Détails du rapport.

1. (Facultatif et le cas échéant) Cliquez sur **Paramètres de matrice**, puis sélectionnez l’une des options suivantes :\
   **Afficher le nombre d’enregistrements :** sélectionnez cette option pour afficher une ligne contenant le nombre total d’entrées pour le champ donné.\
   **Afficher la colonne Valeur :** sélectionnez cette option pour afficher les informations suivantes dans la matrice :

   * Nombre d’enregistrements
   * Colonne Valeur

     >[!NOTE]
     >
     >Cette colonne contient des informations qui décrivent ce que représentent les données de chaque ligne.\
     >Les exceptions suivantes s’appliquent aux objets parent (par exemple, les tâches parent) lorsque vous agrégez des valeurs pour les champs suivants en regroupements :
     >
     >   
     >   
     >   * Tous les champs de nombre et de devise, à l’exception des heures effectives (par exemple, le coût prévu/réel de main-d’œuvre, le coût réel/prévu des dépenses, le coût prévu/réel, le nombre d’heures prévues), n’agrègent que les valeurs des tâches enfant et des tâches autonomes. Ils n’agrègent pas les valeurs des tâches parent ou des parents des parents.
     >   * Les heures effectives agrègent les valeurs principales des tâches parent et des tâches autonomes. Elles n’agrègent pas les nombres pour les parents des tâches parent ou des tâches enfant.
     >   * Les champs de données personnalisées de valeurs numériques et de devise regroupent toutes les tâches : parents, enfants, parents de parents et tâches autonomes. Si vous avez créé le rapport de matrice pour afficher le nombre d’heures prévues ou les heures effectives dans la colonne **Valeur**, sachez que les informations sur les heures ou les coûts de tout objet parent (telles que les tâches parent) ne sont pas affichées dans le rapport de matrice. Pour afficher les heures sur les objets parent, vous devez afficher l’onglet **Détails**.
     >   
     >   
     >

   **Règles conditionnelles :** configurez toute règle de mise en forme pour les valeurs qui sont agrégées.\
   Après avoir ajouté une règle, vous pouvez définir des styles de champ et de texte définissant le mode d’affichage des champs correspondant à cette règle. Après avoir défini la règle, cliquez sur **Ajouter une règle**, puis sur **Terminé** pour l’enregistrer.

1. Cliquez sur l’onglet **Filtres** pour définir les informations qui s’afficheront dans le rapport.
1. (Le cas échéant) Si vous avez déjà créé un filtre et que vous souhaitez l’appliquer à ce rapport, cliquez sur **Appliquer un filtre existant**, puis sélectionnez-le dans la liste déroulante.
1. (Le cas échéant) Si vous souhaitez créer un filtre pour ce rapport, voir la section [Modificateurs de filtre et de condition](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   pour plus d’informations sur les différents qualificateurs que vous pouvez utiliser lors de la création de filtres.

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer et afficher le rapport de matrice.
