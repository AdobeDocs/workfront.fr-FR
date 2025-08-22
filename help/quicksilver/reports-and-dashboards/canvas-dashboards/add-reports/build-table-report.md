---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Créer un rapport de tableau dans un tableau de bord de zones de travail
description: Vous pouvez ajouter un rapport tabulaire à un tableau de bord Zone de travail afin de visualiser vos données dans un format de tableau.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 72344e5c1607ba6b4dd2a1e71a462bba93369b27
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 11%

---

# Créer un rapport de tableau dans un tableau de bord de zones de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Pour plus d’informations, voir [Informations bêta sur les tableaux de bord de la zone de travail](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Vous pouvez ajouter un rapport tabulaire à un tableau de bord Zone de travail afin de visualiser vos données dans un format de tableau.

![Exemple de rapport de tableau](assets/table-example-main.png)

+++ Développez pour afficher les exigences d’accès. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront</p></td> 
   <td> 
<p>Tous </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
<p>Actuelle : formule </p> 
<p>Nouveau : Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td><p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p>
  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

Vous devez créer un tableau de bord avant de pouvoir créer un rapport tabulaire.

## Créer un rapport de tableau dans un tableau de bord de zones de travail

De nombreuses options de configuration sont disponibles pour créer un rapport tabulaire. Dans cette section, nous vous guiderons à travers le processus général de création d’un rapport.

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Cliquez sur **Nouveau tableau de bord** dans le coin supérieur droit.

1. Dans la zone **Créer un tableau de bord**, saisissez les **Nom** et **Description** du tableau de bord.

1. Cliquez sur **Créer**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Tableau**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. (Facultatif) Suivez les étapes ci-dessous pour configurer la section **Détails** :

   1. Saisissez un rapport **Nom**.

   1. Saisissez un état **Description**.

1. Pour configurer la section **Créer une table**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes du tableau** ![Icône Créer un tableau](assets/drilldown-column.png).

   1. Cliquez sur **Ajouter une colonne** puis sélectionnez le champ à afficher en tant que colonne dans le tableau. La colonne s’affiche dans la section de prévisualisation à droite.

   1. Répétez l’étape ci-dessus pour chaque colonne à ajouter.

1. Pour configurer la section **Filtre**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![Icône Filtrer](assets/filter-icon.png).

   1. Sélectionnez **Modifier le filtre**.

   1. Cliquez sur **Ajouter une condition** puis spécifiez le champ à utiliser comme filtre et le modificateur qui définit le type de condition auquel le champ doit répondre. La colonne s’affiche dans la section de prévisualisation à droite.

1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Suivez les étapes ci-dessous pour configurer la section **Paramètres du groupe d’analyse** :

   1. Dans le panneau de gauche, cliquez sur l’icône **Paramètres du groupe** ![Icône Paramètres du groupe](assets/drilldown-group-icon.png).

   1. Cliquez sur le bouton **Ajouter un regroupement** puis sélectionnez le champ à créer en tant que regroupement. La colonne de regroupement s’affiche dans la section de prévisualisation à droite.

1. Cliquez sur **Enregistrer** pour créer le rapport et l’ajouter au tableau de bord.

## Création d’un exemple de rapport tabulaire

Dans cette section, nous allons passer en revue les étapes de création d&#39;un rapport tabulaire qui affiche les approbations de documents en attente.

Pour plus d&#39;informations sur les exemples de rapports de table, voir [Créer un tableau de bord de rapport pour révision et approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Cliquez sur **Nouveau tableau de bord** dans le coin supérieur droit.

1. Dans la zone **Créer un tableau de bord**, saisissez les **Nom** et **Description** du tableau de bord.

1. Cliquez sur **Créer**.

1. Dans la zone **Ajouter un rapport**, sélectionnez **Créer un rapport**.

1. Sur le côté gauche, sélectionnez **Tableau**.

1. Dans le coin supérieur droit, cliquez sur **Créer un rapport**.

1. Pour configurer la section **Détails**, procédez comme suit :

   1. Saisissez _Approbations en attente_ dans le champ **Nom**.
   1. Saisissez une description dans le champ **Description**. Ce texte s’affiche sous forme d’info-bulle en regard du nom du graphique.

1. Pour configurer la section **Créer une table**, procédez comme suit :

   1. Dans le panneau de gauche, cliquez sur l’icône **Colonnes du tableau** ![Icône Colonnes du tableau](assets/drilldown-column.png).
   1. Cliquez sur **Ajouter une colonne**.
   1. Faites défiler vers le bas et sélectionnez **Approbations de documents** > **Statut**.
   1. Ajoutez les colonnes suivantes :

   <table>
    <tr>
    <td><strong>Nom du projet</strong></td>
    <td>Version du document &gt; Document &gt; Projet &gt; Nom</td>
    </tr>
    <tr>
    <td><strong>Nom du document</strong></td>
    <td>Version du document &gt; Document &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
    </tr>
    <tr>
    <td><strong>Version du document</strong></td>
    <td>Version Du Document &gt; Document &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Échéance</strong></td>
    <td>Approbation du document &gt; Étape d’approbation &gt; Échéance</td>
    </tr>
    <tr>
    <td><strong>Demandé par</strong></td>
    <td>Approbation du document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Demandeur &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
    </tr>
    <tr>
    <td><strong>Date demandée</strong></td>
    <td>Approbation du document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Créé le</td>
    </tr>
    <tr>
    <td><strong>Approbateur</strong></td>
    <td>Approbation du document &gt; Étape d’approbation &gt; Participants à l’étape d’approbation* &gt; Utilisateur participant &gt; saisissez <em>Nom</em> dans la zone de recherche.</td>
    </tr>
    </table>


   *Les participants à l&#39;étape d&#39;approbation sont tronqués à _Pa étape d&#39;approbation_.


1. Pour configurer la section **Filtre**, procédez comme suit :
   1. Dans le panneau de gauche, cliquez sur l’icône **Filtrer** ![icône de l’onglet Filtrer](assets/filter-tab.png).
   1. Cliquez sur **Modifier le filtre**, puis **Ajouter une condition**.
   1. Cliquez dans le filtre de condition vide, puis cliquez sur **Choisir un champ**.
   1. Sélectionnez **Statut**.
   1. Remplacez l’opérateur par **Égal**, puis saisissez _en attente d’approbation_ dans la zone de texte.
      ![exemple de filtre de table d&#39;approbation en attente](assets/pending-approval-table-filter.png)
   1. (Facultatif) Ajoutez des filtres supplémentaires comme décrit dans la section **Filtres facultatifs** ci-dessous.
1. Cliquez sur **Enregistrer** dans le coin supérieur droit de l’écran.
