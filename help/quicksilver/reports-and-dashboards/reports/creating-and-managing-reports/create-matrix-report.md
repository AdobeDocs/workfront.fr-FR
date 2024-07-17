---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Créer un rapport de matrice
description: Les rapports matriciel présentent des informations récapitulatives sous la forme d’un tableau agrégé, ce qui facilite l’affichage que si elles étaient affichées dans une liste comme dans un rapport traditionnel.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 9%

---

# Créer un rapport de matrice

Les rapports matriciel présentent des informations récapitulatives sous la forme d’un tableau agrégé, ce qui facilite l’affichage que si elles étaient affichées dans une liste comme dans un rapport traditionnel.

## Quand utiliser un rapport de matrice

Vous pouvez créer un rapport de matrice pour tout rapport qui contient 2 groupes ou plus. Un rapport traditionnel peut contenir jusqu’à 3 groupes et un rapport matrice peut contenir jusqu’à 4 groupes.

Par exemple, vous souhaitez créer un rapport Heure qui affiche les heures consignées au cours d’une période de 3 mois et vous souhaitez que le rapport soit organisé en fonction de la personne ayant saisi les heures, ainsi que par mois et par semaine.

![](assets/report-matrix-overview-350x123.png)

## Affichage des données dans un rapport de matrice

Les informations du rapport de matrice sont toujours affichées sous forme de valeur numérique. Dans la plupart des cas, les colonnes contenant une valeur numérique sont mieux adaptées à l’affichage dans un rapport de matrice (heures consignées et coût réel, par exemple).

Cependant, d’autres colonnes (comme Etat) peuvent toujours être affichées dans le rapport de matrice, comme illustré dans le graphique suivant :\
![](assets/report-matrix-status-350x73.png)

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Configurer un rapport de matrice

1. Créez un rapport traditionnel contenant des données numériques dans la sortie du rapport.\
   Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Accédez au rapport que vous avez créé à l’étape 1, cliquez sur **Actions de rapport**, puis sélectionnez **Modifier**.

1. (Conditionnel) Si vous avez déjà créé une vue et que vous souhaitez l’appliquer à ce rapport, cliquez sur **Appliquer une vue existante**, puis sélectionnez la vue dans la liste déroulante.
1. (Conditionnel) Si vous souhaitez créer une vue pour le rapport, procédez comme suit :

   1. Cliquez sur l&#39;onglet **Colonnes (vues)** , puis sélectionnez une colonne que vous souhaitez résumer dans le rapport de matrice.
   1. Dans la zone **Paramètres de colonne**, cliquez sur la liste déroulante **Résumer cette colonne par** , puis sélectionnez l’une des options disponibles pour résumer les informations.

      >[!IMPORTANT]
      >
      >Si cette option n&#39;est pas sélectionnée, les informations de la colonne ne s&#39;affichent pas correctement dans le rapport de matrice.

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. Répétez cette procédure pour chaque colonne dans l’onglet Colonnes (vue), puis cliquez sur **Terminé**.

1. Cliquez sur l’onglet **Groupings** .
1. (Conditionnel) Si vous avez déjà créé un groupement et que vous souhaitez l&#39;appliquer à ce rapport, cliquez sur **Appliquer un groupement existant**, puis sélectionnez le groupement dans la liste déroulante.
1. (Conditionnel) Si vous souhaitez créer un nouveau groupement de matrice pour le rapport, procédez comme suit :

   1. Sélectionnez **Basculer vers le regroupement matriciel** dans le coin supérieur droit de l’interface du créateur.
   1. Dans la section **Regroupements de lignes** , identifiez le groupement de lignes qui établit les groupements horizontaux du tableau.
   1. (Facultatif) Pour ajouter un groupement de lignes supplémentaire, cliquez sur **Ajouter un groupement de lignes secondaires**.
   1. Dans la section **Regroupements de colonnes** , identifiez le groupement de colonnes, qui établit les groupements verticaux du tableau.
   1. (Facultatif) Pour ajouter un groupement de colonnes supplémentaire, cliquez sur **Ajouter un groupement de colonnes secondaire**.
   1. (Conditionnel) Si vous ajoutez un groupement par date, indiquez également si les résultats sont regroupés par jour, semaine, mois, trimestre ou année.\
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. (Conditionnel) Si vous avez choisi de regrouper par date et d’afficher les résultats par trimestre, par exemple, indiquez si vous souhaitez afficher les trimestres sans données en cochant la case **Afficher les trimestres sans résultats** .\
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >Le champ **Afficher les trimestres sans résultats** est disponible uniquement pour les regroupements de matrice et non pour les regroupements standard.\
      >Seuls les trimestres sans données situés entre deux trimestres et contenant des données valides affichent zéro pour les valeurs des données de l&#39;onglet Matrice. Les trimestres qui ne comportent aucune donnée se trouvant au début et à la fin de la période sélectionnée par votre filtre n&#39;apparaissent pas du tout dans le groupement de la matrice. Les trimestres sans résultat ne s&#39;afficheront pas dans un groupement dans l&#39;onglet Détails du rapport.

1. (Facultatif et conditionnel) Cliquez sur **Paramètres de matrice**, puis sélectionnez l’une des options suivantes :\
   **Afficher le nombre d’enregistrements :** Sélectionnez cette option pour afficher une ligne avec le nombre total d’entrées pour le champ donné.\
   **Afficher la colonne de valeur :** Sélectionnez cette option pour afficher les informations suivantes dans la matrice :

   * Nombre d’enregistrements
   * La colonne Valeur

     >[!NOTE]
     >
     >Cette colonne contient des informations qui décrivent ce que représentent les données de chaque ligne.\
     >Les exceptions suivantes s’appliquent aux objets parents (par exemple, les tâches parents) lorsque vous agrègez des valeurs pour les champs suivants en regroupements :
     >
     >   
     >   
     >   * Tous les champs de nombre et de devise, à l’exception des heures réelles (par exemple, le coût du travail planifié/réel, le coût des dépenses planifiées/réelles, le coût planifié/réel, les heures planifiées), ne regroupent que les valeurs des tâches enfants et des tâches autonomes. Ils n’agrégent pas les valeurs des tâches parents ou des parents des parents.
     >   * Les heures réelles combinent les valeurs des tâches principales du parent et des tâches autonomes ; elles n’agrégent pas les nombres des parents des tâches parents ou des tâches enfants.
     >   * Les champs de données personnalisés pour les valeurs numériques et monétaires regroupent toutes les tâches : parents, enfants, parents de parents et tâches autonomes. Si vous avez créé le rapport de matrice pour afficher les heures planifiées ou les heures réelles dans la colonne **Valeur**, sachez que les informations sur les heures ou les coûts pour les objets parents (tels que les tâches parents) ne sont pas affichées dans le rapport de matrice. Pour afficher les heures sur les objets parents, vous devez afficher l’onglet **Détails** .
     >   
     >   
     >

   **Règles conditionnelles :** Configurez des règles de mise en forme pour les valeurs qui sont agrégées.\
   Après avoir ajouté une règle, vous pouvez définir des styles de champ et de texte pour l’affichage des champs correspondant à cette règle. Cliquez sur **Ajouter une règle** après avoir défini la règle, puis sur **Terminé** pour enregistrer la règle.

1. Cliquez sur l&#39;onglet **Filtres** pour définir les informations qui s&#39;afficheront dans le rapport.
1. (Conditionnel) Si vous avez déjà créé un filtre et que vous souhaitez l’appliquer à ce rapport, cliquez sur **Appliquer un filtre existant**, puis sélectionnez le filtre dans la liste déroulante.
1. (Conditionnel) Si vous souhaitez créer un filtre pour ce rapport, reportez-vous à la section [Modificateurs de condition et de filtre](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   pour plus d’informations sur les différents qualificateurs que vous pouvez utiliser lors de la création de filtres.

1. Cliquez sur **Enregistrer+Fermer** pour enregistrer et afficher le rapport de matrice.
