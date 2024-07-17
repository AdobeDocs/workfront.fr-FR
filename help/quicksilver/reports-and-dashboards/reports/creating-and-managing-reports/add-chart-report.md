---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Ajouter un graphique à un rapport
description: Vous pouvez améliorer vos rapports en ajoutant un graphique. Vous pouvez ajouter des graphiques aux rapports existants ou aux rapports que vous créez.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 2%

---

# Ajouter un graphique à un rapport

<!--Audited: 01/2024-->

Vous pouvez améliorer vos rapports en ajoutant un graphique. Vous pouvez ajouter des graphiques aux rapports existants ou aux rapports que vous créez.

Avant d’ajouter un graphique à un rapport, vous devez créer une Vue et un Groupement pour le rapport.

Vous ne pouvez pas ajouter de graphiques à la plupart des rapports, sauf si vous commencez par regrouper les informations dans le rapport. Le seul graphique qui peut être ajouté sans groupement est un graphique à jauge.

Pour plus d’informations sur les vues, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Pour plus d’informations sur les groupements, consultez la [présentation des groupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Si votre rapport affiche trop d’éléments, aucun graphique n’est créé. Dans ce cas, vous devez également ajouter un filtre au rapport pour réduire le nombre de résultats dans votre rapport.

Pour plus d’informations sur les filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Actuelle : formule </p>
   Ou
   <p>Nouvelle : standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations sur les exigences d’accès, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Ajouter un graphique à un rapport

1. Accédez à un rapport existant ou créez-en un nouveau. Pour plus d&#39;informations sur la création d&#39;un nouveau rapport, voir [Création d&#39;un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. (Conditionnel) Si vous êtes allé à un rapport existant, cliquez sur **Actions de rapport** > **Modifier**.

1. Assurez-vous que l&#39;onglet **Colonnes (vues)** a été mis à jour afin d&#39;afficher les informations que vous souhaitez illustrer dans le rapport.

   Pour plus d’informations sur la création ou la modification de la vue pour le rapport, voir [Création ou modification de vues dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

1. Cliquez sur l&#39;onglet **Groupings** et ajoutez un groupement.

   >[!TIP]
   >
   >* Vous ne pouvez ajouter un graphique à un rapport que lorsque les résultats du rapport sont regroupés.
   >* Les regroupements en mode texte ne sont pas pris en charge dans les graphiques. Pour plus d’informations sur les regroupements en mode texte, voir [Modifier le mode texte dans un groupement](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Si vous ajoutez un groupement unique qui représente une mesure, tous les graphiques, à l’exception d’un graphique circulaire, affichent chaque résultat du groupement avec la même couleur.

   Pour plus d’informations sur la création de groupements, voir [Création de groupements dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md).

1. Sélectionnez l&#39;onglet **Graphique** .
1. Cliquez sur un type de graphique pour le sélectionner.\
   ![](assets/qs-report-builder-chart-350x265.png)

1. Choisissez parmi les types de graphiques suivants :

   * [Graphique en colonnes](#column-chart)
   * [Graphique à barres](#bar-chart)
   * [Graphique en secteurs](#pie-chart)
   * [Graphique en courbes](#line-chart)
   * [Graphique de jauge](#gauge-chart)
   * [Graphique à bulles](#bubble-chart)

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le graphique et le rapport.

### Graphique en colonnes {#column-chart}

Pour ajouter un graphique **Column** à votre rapport :

1. Commencez à ajouter un graphique à votre rapport, comme décrit dans [Ajouter un graphique à un rapport](#add-a-chart-to-a-report).
1. Dans le champ **Axe gauche (Y)** , sélectionnez les valeurs que vous souhaitez inclure sur l’axe des ordonnées du graphique, ainsi que la manière dont vous souhaitez que les informations soient résumées.
1. Dans le champ **Axe inférieur (X)** , sélectionnez le Groupement que vous souhaitez inclure dans le graphique.
1. (Facultatif) Sélectionnez **Couleurs personnalisées** pour attribuer les couleurs de votre choix à chacune des colonnes.\
   Pour plus d’informations sur la personnalisation des couleurs des graphiques, voir [Personnalisation des couleurs des graphiques](#customize-chart-colors).

1. (Facultatif) Sélectionnez **Afficher en 3D** pour afficher le graphique dans une vue en 3 dimensions.
1. (Facultatif) **Colonnes de groupe** : sélectionnez cette option pour définir comment vous souhaitez que les colonnes soient regroupées.\
   Sélectionnez l’une des options suivantes :

   * Cliquez sur l&#39;une des options suivantes pour sélectionner l&#39;affichage des colonnes regroupées :

      * **Côté à côté**
      * **Stacked**
      * **Empilé à 100 %**

   * Sélectionnez le Groupement que vous souhaitez inclure dans le graphique dans le menu déroulant **Grouper les données par** .
   * (Facultatif) Sélectionnez **Couleurs personnalisées** pour personnaliser les couleurs des colonnes.\
     Pour plus d’informations sur la personnalisation des couleurs des graphiques, voir [Personnalisation des couleurs des graphiques](#customize-chart-colors).

1. (Facultatif) Sélectionnez **Graphique en combinaison** pour inclure une valeur supplémentaire dans le graphique, ainsi que la manière dont vous souhaitez que les informations soient résumées.\
   Tenez compte des options suivantes :

   * **Graphique sur l’axe Secondaire** : sélectionnez cette option pour tracer les données sur le côté droit du graphique.
   * **Type de graphique** : choisissez si vous souhaitez que cette valeur supplémentaire s’affiche sous forme d’une ligne ou d’une troisième colonne.\
     ![](assets/qs-column-chart-350x163.png)

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le graphique et le rapport.

### Graphique en barres {#bar-chart}

Pour ajouter un graphique **Bar** à votre rapport :

1. Commencez à ajouter un graphique à votre rapport, comme décrit dans [Ajouter un graphique à un rapport](#add-a-chart-to-a-report).
1. Dans le champ **Axe inférieur (X)** , sélectionnez les valeurs à inclure sur l’axe des x du graphique, ainsi que la manière dont vous souhaitez que les informations soient résumées.
1. Dans le champ **Axe gauche (Y)** , sélectionnez le Groupement que vous souhaitez inclure dans le graphique.
1. (Facultatif) Sélectionnez **Couleurs personnalisées** pour personnaliser les couleurs des barres.\
   Pour plus d’informations sur la personnalisation des couleurs des graphiques, voir [Personnalisation des couleurs des graphiques](#customize-chart-colors).

1. (Facultatif) Sélectionnez **Afficher en 3D** pour afficher le graphique dans une vue en 3 dimensions.
1. (Facultatif) Sélectionnez **Barres de groupe** pour définir comment vous souhaitez que les barres soient regroupées.\
   Sélectionnez l’une des options suivantes :

   * Cliquez sur l’une des options suivantes pour sélectionner l’affichage des barres regroupées :

      * **Côté à côté**
      * **Stacked**
      * **Empilé à 100 %**

   * Sélectionnez le mode de regroupement des informations dans le graphique dans le menu déroulant **Regrouper les données par** .
   * (Facultatif) Sélectionnez **Couleurs personnalisées** pour personnaliser les couleurs de vos colonnes.\
     Pour plus d’informations sur la personnalisation des couleurs des graphiques, voir [Personnalisation des couleurs des graphiques](#customize-chart-colors).

1. (Facultatif) Sélectionnez **Graphique en combinaison** pour inclure une valeur supplémentaire dans le graphique, ainsi que la manière dont vous souhaitez que les informations soient résumées.\
   ![](assets/qs-bar-chart-350x167.png)

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le graphique et le rapport.

>[!IMPORTANT]
>
>Limitez les histogrammes à 23 ou moins, car les histogrammes contenant plus de 23 barres n&#39;afficheront pas correctement tous les libellés de barres.

### Graphique circulaire {#pie-chart}

Pour ajouter un graphique **circulaire** à votre rapport :

1. Commencez à ajouter un graphique à votre rapport, comme décrit dans [Ajouter un graphique à un rapport](#add-a-chart-to-a-report).
1. Dans le champ **Valeurs** , sélectionnez les valeurs à afficher dans le rapport, ainsi que la manière dont vous souhaitez les résumer.\
   Dans le champ **Ponts** , sélectionnez le Groupement que vous souhaitez inclure dans le graphique. Le Regroupement est représenté par les contours du graphique.

1. (Facultatif) Sélectionnez **Couleurs personnalisées** pour personnaliser les couleurs des contours du graphique.\
   Pour plus d’informations sur la personnalisation des couleurs des graphiques, voir [Personnalisation des couleurs des graphiques](#customize-chart-colors).

1. (Facultatif) Sélectionnez **Afficher en 3D** pour afficher le graphique dans une vue en 3 dimensions.
1. Dans le champ **Afficher les résultats sous** , sélectionnez le mode d’affichage des résultats dans le graphique. Tenez compte des options suivantes :

   * **Pourcentage** : les résultats du graphique s’affichent en pourcentage.
   * **Nombres** : les résultats du graphique s’affichent sous la forme d’un nombre.\
     ![](assets/qs-pie-chart-350x171.png)

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le graphique et le rapport.

### Graphique en courbes {#line-chart}

Pour ajouter un graphique **Line** à votre rapport :

1. Commencez à ajouter un graphique à votre rapport, comme décrit dans [Ajouter un graphique à un rapport](#add-a-chart-to-a-report).
1. Dans le champ **Axe gauche (Y)** , sélectionnez les valeurs que vous souhaitez inclure sur l’axe des ordonnées du graphique, ainsi que la manière dont vous souhaitez que les informations soient résumées.
1. Dans le champ **Axe inférieur (X)** , sélectionnez le Groupement que vous souhaitez inclure dans le graphique.
1. (Facultatif) Sélectionnez une couleur pour personnaliser la couleur de la ligne.
1. (Facultatif) Sélectionnez **Lignes de groupe** pour sélectionner un groupement supplémentaire pour le graphique.\
   (Facultatif) Sélectionnez **Couleurs personnalisées** pour personnaliser les couleurs de votre nouveau regroupement.\
   Pour plus d’informations sur la personnalisation des couleurs des graphiques, voir [Personnalisation des couleurs des graphiques](#customize-chart-colors).

1. (Facultatif) Sélectionnez **Combinination Chart** pour combiner vos lignes par une valeur supplémentaire.\
   Tenez compte des options suivantes :

   * Sélectionnez la valeur que vous souhaitez inclure dans le graphique, ainsi que la manière dont vous souhaitez que les informations soient résumées.
   * Sélectionnez le champ **Tracé sur l’axe Secondaire** pour tracer les données sur le côté droit du graphique.\
     ![](assets/qs-line-chart-350x172.png)

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le graphique et le rapport.

### Graphique d’évaluation {#gauge-chart}

Un graphique **Évaluation** affiche le nombre d&#39;enregistrements qui répondent à un certain critère dans un format de jauge. L&#39;indicateur de la jauge pointe vers le nombre d&#39;enregistrements répondant aux critères sélectionnés dans la vue et le regroupement du rapport. Un regroupement de rapports n’est pas nécessaire pour configurer un graphique à jauge.

Pour ajouter un graphique **jauge** à votre rapport :

1. Commencez à ajouter un graphique à votre rapport, comme décrit dans [Ajouter un graphique à un rapport](#add-a-chart-to-a-report).
1. Dans le champ **Valeurs** , sélectionnez les valeurs à afficher dans le rapport, ainsi que la manière dont vous souhaitez les résumer. Si vous sélectionnez **Record Count**, les valeurs affichées sont l’objet du rapport.

1. Dans le champ **Indicateurs** , sélectionnez le Regroupement à inclure dans le graphique. Le Regroupement est représenté par la ligne d&#39;indicateur sur le graphique.\
   Si un Groupement contient deux éléments, deux indicateurs sont affichés sur le graphique.\
   Par exemple, si vous disposez d’un regroupement de l’état du projet et qu’il existe deux états du projet (actuel et en attente), votre graphique Évaluation contient deux indicateurs de jauge. Ils indiquent le nombre de projets qui se trouvent dans cet état.\
   (Facultatif) Sélectionnez **Total** dans le champ **Indicateurs** pour afficher le total des objets sélectionnés dans le champ **Valeurs** .

1. Dans le champ **Plage de valeurs**, spécifiez la plage de valeurs et la couleur à représenter ces valeurs à afficher sur le graphique Jauge.
1. (Facultatif) Cliquez sur **Ajouter une plage de valeurs** pour ajouter des plages de valeurs supplémentaires au graphique.\
   ![](assets/qs-gauge-chart-350x181.png)

1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le graphique et le rapport.

### Graphique à bulles {#bubble-chart}

Vous pouvez afficher jusqu’à trois champs d’un objet dans un graphique **Bulle**. Cela signifie que vous pouvez afficher jusqu’à quatre points de données dans un graphique à bulles. Chaque entité ayant trois champs associés s’affiche sous la forme d’un cercle qui exprime deux des champs de son emplacement dans les axes X et Y. Le troisième champ est représenté par la taille du cercle.

Pour ajouter un graphique **Bubble** à votre rapport :

1. Commencez à ajouter un graphique à votre rapport, comme décrit dans [Ajouter un graphique à un rapport](#add-a-chart-to-a-report).
1. Dans le champ **Axe gauche (Y)** , sélectionnez les valeurs à inclure sur l’axe Y du graphique. Les valeurs proviennent de la vue du rapport. Indiquez le mode de résumé des informations.
1. Dans le champ **Axe inférieur (X)**, sélectionnez les valeurs à inclure sur l’axe X du graphique. Les valeurs proviennent de la vue du rapport. Indiquez le mode de résumé des informations.

   >[!NOTE]
   >
   >Assurez-vous qu’au moins une colonne est résumée pour que ce champ soit actif.\
   >Pour plus d’informations sur la synthèse des informations dans une colonne de rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Dans le champ **Taille de la bulle**, sélectionnez les valeurs que vous souhaitez représenter par la taille des bulles dans le graphique. Les valeurs proviennent de la vue du rapport. Indiquez le mode de résumé des informations.

   >[!NOTE]
   >
   >Assurez-vous qu’au moins une colonne est résumée pour que ce champ soit actif.\
   >Pour plus d’informations sur la synthèse des informations dans une colonne de rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Dans le champ **Bulles** , sélectionnez le Groupement que vous souhaitez inclure dans le graphique. Le Regroupement est représenté par le positionnement des bulles sur le graphique.
1. Dans le champ **Couleur de la bulle**, sélectionnez le champ que vous souhaitez représenter par les couleurs des bulles.

   ![](assets/qs-bubble-chart-350x103.png)


   La **couleur de la bulle** peut être un groupement que vous définissez dans le rapport, mais elle n&#39;est disponible que lorsque vous sélectionnez la colonne **Nom** pour l&#39;objet du rapport dans le champ **Bulles**.

   Par exemple, si vous avez sélectionné **Nom de la tâche** dans un rapport de tâche, vous pouvez ajouter **État de la tâche** comme champ **Couleur de la bulle**.

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   Cependant, si vous avez sélectionné **État de la tâche** pour le champ **Bulles**, vous ne pouvez pas sélectionner un champ **Couleur de la bulle**. De plus, vous ne pouvez pas sélectionner **Nom du projet** pour le champ **Couleur de la bulle**, même si vous sélectionnez **Nom de la tâche** pour le champ **Bubble**.

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)


1. Cliquez sur **Enregistrer + Fermer** pour enregistrer les modifications apportées au créateur d’interface.

## Exporter un graphique

Vous pouvez exporter un graphique dans un fichier .pdf.

Pour exporter un graphique :

1. Cliquez sur **Exporter** pour exporter le graphique au format .pdf.\
   Un fichier .pdf est téléchargé sur votre ordinateur.

1. Ouvrez le fichier .pdf .\
   Le fichier exporté comprend les informations suivantes :

   * Image du graphique.
   * Titre qui correspond au nom du rapport.
   * Nom de fichier unique qui correspond au nom du rapport.
   * Un pied de page avec la date et l’heure d’export du rapport et le numéro de page.

## Personnalisation des couleurs des graphiques {#customize-chart-colors}

Vous pouvez laisser Workfront sélectionner les couleurs des éléments de votre graphique ou les personnaliser lorsque vous ajoutez un graphique à vos rapports. Si votre graphique contient un seul groupement qui représente une mesure (un rapport de tâche qui indique le nombre de tâches regroupées par date d’achèvement réelle, par exemple), chaque résultat du groupement est affiché dans la même couleur.

Vous ne pouvez choisir qu&#39;une seule couleur pour les champs affichés dans la Vue du rapport. Vous pouvez choisir plusieurs couleurs, une pour chaque option, pour les champs affichés dans le Groupement du rapport.

>[!IMPORTANT]
>
>Pour les champs de date, vous ne pouvez sélectionner qu’une seule couleur pour les éléments de graphique.

Pour personnaliser les couleurs des graphiques :

1. Lors de la création d’un rapport, accédez à l’onglet **Graphique** du créateur de rapports.
1. Sélectionnez un type de graphique à ajouter à votre rapport.\
   Pour plus d&#39;informations sur l&#39;ajout d&#39;un graphique à votre rapport, voir [Ajout d&#39;un graphique à un rapport](#add-a-chart-to-a-report).

1. Cliquez sur **Couleurs personnalisées** lorsque ce champ est disponible.\
   La boîte de dialogue Couleurs personnalisées s’affiche.\
   ![](assets/custom-colors-in-charts-350x286.png)

   >[!NOTE]
   >
   >Vous pouvez associer des couleurs personnalisées à n’importe quel champ que vous pouvez regrouper et à certains champs pouvant être affichés dans une vue, y compris les champs personnalisés. Les champs personnalisés ou les options personnalisées des champs que vous choisissez dans la boîte de dialogue Couleur personnalisée sont sensibles à la casse.

1. Choisissez l’une des options suivantes :

   * **Utiliser une couleur** : tous les éléments du graphique s’affichent dans la couleur sélectionnée.

      1. Commencez à saisir le nom d’une option du champ sélectionné, puis sélectionnez une couleur. Cette option s’affiche dans la couleur sélectionnée sur le graphique.
      1. (Facultatif) Spécifiez une valeur hexadécimale de couleur pour votre couleur, au lieu d’en sélectionner une parmi les échantillons de couleurs disponibles.\
         Ou\
         Cliquez sur le sélecteur de couleurs qui s’affiche après avoir cliqué sur le code hexadécimal, puis sélectionnez une autre couleur.

   * **Ajouter une couleur** : continuez à ajouter des couleurs personnalisées pour toutes les autres options possibles du champ sélectionné.
   * **Tout supprimer** : sélectionnez cette option pour supprimer toutes les couleurs et options du champ sélectionné ci-dessus.
   * **Options avancées** : effectuez un choix parmi les options suivantes :

      * **Aucune valeur** : sélectionnez ce champ et une couleur personnalisée pour afficher la colonne du graphique qui regroupe les éléments &quot;aucune valeur&quot;. Il s’agit d’éléments qui ne peuvent pas être regroupés par l’une des options du champ sélectionné dans votre groupement.
      * **Toutes les autres valeurs** : sélectionnez ce champ et une couleur personnalisée pour afficher tous les autres éléments de graphique dont les options ne sont pas sélectionnées ci-dessus.

        >[!NOTE]
        >
        >Les couleurs que vous avez utilisées le plus récemment s’affichent en haut de la boîte de dialogue Couleurs personnalisées . Lorsque vous passez la souris sur une couleur qui a été récemment utilisée, le nom du champ qui lui est associé s’affiche.

1. Cliquez sur le &quot;x&quot; dans le coin supérieur droit de l’option Couleurs personnalisées pour fermer la boîte de dialogue Couleurs personnalisées . Les couleurs sélectionnées sont automatiquement enregistrées.
1. Cliquez sur **Enregistrer + Fermer** pour enregistrer le diagramme et exécuter le rapport.

## Supprimer un graphique d’un rapport

Pour supprimer un graphique d’un rapport :

1. Ouvrez l’onglet **Graphique** du créateur de rapports.
1. Placez le pointeur de la souris sur l’icône du type de graphique que vous avez choisi et un bouton &quot;x&quot; s’affiche dans le coin supérieur droit de l’icône.
1. Cliquez sur le &quot;x&quot; pour supprimer le graphique.
1. Cliquez sur **Enregistrer + Fermer**.

## Limites lors de l’utilisation de graphiques

Tenez compte des limites suivantes lorsque vous utilisez des graphiques :

* La section **Aperçu du graphique** située à droite du créateur de rapports ne contient pas de données réelles provenant de votre rapport. Vous devez enregistrer le graphique et le visualiser à partir de l’onglet **Chart** afin de voir le graphique avec vos données.

* Certains éléments de graphique ne sont pas modifiables :

   * Vous ne pouvez pas modifier le type de police ni la taille sur les valeurs de chaque élément.
   * Vous ne pouvez pas modifier les noms de vos axes dans le graphique.

* Vous ne pouvez pas modifier la légende du graphique.
* Lorsque vous utilisez des champs calculés pour vos groupements, vous ne pouvez pas cliquer sur les éléments du graphique.
* Le plus grand nombre de points de données que vous pouvez afficher dans un graphique est de quatre, dans un graphique à bulles. Tous les autres types de graphique affichent deux points de données ou un maximum de trois.
