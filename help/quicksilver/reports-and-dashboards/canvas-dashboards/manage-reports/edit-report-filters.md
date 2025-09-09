---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Modification des filtres de rapport dans un tableau de bord Zone de travail
description: Vous pouvez modifier les filtres de rapport après les avoir appliqués à un tableau de bord de zone de travail.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 5205c342-7f63-438e-97c8-e74f7dfecfd0
source-git-commit: 56d0b9281387cc7b35055461e7868c7e4a194f81
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 44%

---

# Modification des filtres de rapport dans un tableau de bord Zone de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, voir [Contacter le service clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform

Vous pouvez modifier les filtres de rapport une fois que vous les avez appliqués à un tableau de bord de la zone de travail afin de mettre à jour les données qui s’affichent au fur et à mesure de la progression du projet.

## Conditions d’accès

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
        <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td><p>Gestion des autorisations relatives au tableau de bord</p>
  </td> 
  </tr>
</tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

Vous devez ajouter un filtre à un rapport avant de pouvoir le modifier.

## Modification d’un filtre de rapport

>[!NOTE]
>
>De nombreux outils de configuration sont disponibles pour créer et modifier un filtre de rapport. Pour plus d’informations sur ces outils, consultez la section suivante de cet article : [Remarques concernant la modification d’un filtre de rapport](#considerations-when-editing-a-report-filter).


{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Sur la page **Tableaux de bord de la zone de travail**, cliquez sur l’icône **Plus** ![Plus](assets/more-icon.png) dans le coin supérieur droit du rapport qui contient le filtre à modifier, puis sélectionnez **Modifier**.

   ![Modifier un rapport](assets/edit-report-box.png)

1. Sur le côté gauche de la boîte de dialogue **Configurer**, sélectionnez le panneau **Filtres**.

1. Cliquez sur **Modifier le filtre**.

1. Sélectionnez le champ ou le modificateur que vous souhaitez modifier, puis ajustez les sélections actuelles selon vos besoins.

   ![ Ajouter une condition ](assets/add-condition.png)

1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Cliquer sur **Enregistrer**.

## Remarques concernant la modification d’un filtre de rapport

### Variables de filtre de caractères génériques basées sur la date

Les options de caractères génériques basés sur la date peuvent être utilisées en combinaison avec n’importe quel attribut de filtre de date. Pour plus d’informations sur l’ajout d’un caractère générique basé sur la date à un rapport, consultez l’article [Utiliser des caractères génériques basés sur la date pour généraliser des rapports](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Si vous créez un calcul de date et heure qui n’inclut pas de partie horaire ou qui utilise les caractères génériques $$TODAY ou $$NOW, le système utilise la date selon le fuseau horaire universel coordonné (UTC), et non selon votre fuseau horaire local. Cela peut entraîner un résultat de date inattendu.

Vous pouvez choisir parmi les caractères génériques suivants basés sur la date :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>Nous vous recommandons de créer des filtres sensibles à la date à l’aide de ce caractère générique afin d’éviter de les recréer demain, la semaine prochaine ou le mois prochain.</p> <p>Par exemple, si vous souhaitez afficher toutes les tâches qui doivent être effectuées avant aujourd’hui, vous pouvez utiliser la règle suivante dans un filtre de tâche : <em>Date de début prévue inférieure à $$TODAY</em>.</p> <p>$$TODAY est toujours égal à minuit pour le jour en cours.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Cette opération est similaire au caractère générique $$TODAY, mais inclut la date et l’heure actuelles. $$NOW est égal à la date et à l’heure actuelles.</p> <p>Par exemple, si vous souhaitez afficher toutes les entrées d’heure fournies jusqu’à l’heure actuelle, vous pouvez le faire en utilisant la règle suivante dans un filtre d’heure : <em>Date de début prévue inférieure à $$NOW</em>.</p> <p>Note : ce caractère générique n’est pas pris en charge dans le planificateur de ressources.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour indiquer différentes périodes et différents points dans le temps (futur ou passé), vous pouvez combiner les caractères génériques ci-dessus avec les éléments suivants :

| Attributs |   |
|---|---|
| **q** | Trimestre du calendrier |
| **h** | heure |
| **d** | jour |
| **w** | semaine |
| **m** | mois |
| **y** | an |

{style="table-layout:auto"}

| **Qualificateurs** | |
|---|---|
| **b** | début de la période (sans attribut spécifié, début de la semaine par défaut : dimanche) |
| **e** | fin de la période (sans attribut spécifié, fin de la semaine par défaut : samedi) |

{style="table-layout:auto"}

| **Opérateurs** | |
|---|---|
| **+** | Ajouter la valeur à la valeur d’un caractère générique |
| **-** | Soustraire la valeur de la valeur d’un caractère générique |

{style="table-layout:auto"}

Par exemple, le caractère générique `$$TODAYb+2w` fait référence à « 2 semaines à partir du début de cette semaine ». Le caractère générique *`$$NOW+2h` fait référence à « dans 2 heures ».

### Variables de filtre de caractères génériques de l’utilisateur connecté

* Lors du filtrage sur l’attribut de `name` utilisateur, vous verrez l’option **Moi (utilisateur connecté)**.

  ![Attribut de nom d’utilisateur](assets/user-name-attribute.png)

* Lors du filtrage sur un attribut de `name` de groupe, vous verrez les options **Mon groupe principal (groupe d’utilisateurs connectés)** et **Mes autres groupes (groupes d’utilisateurs connectés)** à utiliser dans une condition de filtre.

  ![Attribut du nom du groupe](assets/group-name-attribute.png)

* Lors du filtrage sur un attribut de `name` d’équipe, vous verrez les options **Mon équipe par défaut (équipe utilisateur connectée)** et **Mes autres équipes (équipes utilisateurs connectées)** parmi lesquelles effectuer votre choix dans la condition de filtrage.

  ![Attribut de nom d’équipe](assets/team-name-attribute.png)


### Référencer des objets enfants

Les relations disponibles pour les colonnes supplémentaires, les options de filtre et les attributs de regroupement sont généralement limitées aux objets situés plus haut dans la hiérarchie d&#39;objets Workfront ou comportent une seule sélection sur l&#39;objet d&#39;entité de base du rapport. Il existe certaines exceptions à cette règle, notamment :

* Projet > Tâches
* Approbation de document > Étapes d&#39;approbation de document
* Étapes d&#39;approbation du document > Participants à l&#39;étape d&#39;approbation du document

Lors de l’utilisation de l’une des relations parent-enfant répertoriées ci-dessus, une ligne s’affiche dans le tableau pour chaque enregistrement enfant connecté à l’objet parent.

### Opérateurs de champ par type de champ

+++ Développez pour afficher la liste des opérateurs de champ par type de champ. 

<table>
    <tr>
        <td><b>Type de champ</b></td>
        <td><b>Exemple</b></td>
       <td><b>Opérateurs</b></td>
        <td><b>Caractères génériques</b></td>
    </tr>
    <tr>
        <td>Nom de l’objet/référence</td>
        <td>Tout attribut de nom natif ou recherche personnalisée</td>
              <td><ul>
        <li>Égal à (non sensible à la casse)</li>
        <li>Non égal à (non sensible à la casse)</li>
        <li>Contient</li>
          <li>Ne contient pas</li>
            <li>Est nul</li>
              <li>N’est pas nul</li>
        </ul></td>
        <td>Utilisateur : nom
        <ul>
        <li>Moi (personne connectée)</li>
        </ul>
        Groupe : Nom
        <ul>
          <li>Mon groupe principal (groupe des utilisateurs et utilisatrices connectés)</li>
            <li>Mes autres groupes (groupes des utilisateurs et utilisatrices connectés)</li>
          </ul>
          Équipe : Nom
                  <ul>
          <li>Mon équipe par défaut (équipe des utilisateurs et utilisatrices connectés)</li>
            <li>Mes autres équipes (équipes d’utilisateurs et d’utilisatrices connectés)</li>
          </ul>
        </td>
    </tr>
    <tr>
        <td>Chaîne / Entrée De Texte </td>
                <td>Projet : Description</td>
                      <td><ul>
             <li>Égal à (non sensible à la casse)</li>
        <li>Non égal à (non sensible à la casse)</li>
        <li>Contient</li>
          <li>Ne contient pas</li>
            <li>Est nul</li>
              <li>N’est pas nul</li>
        </ul></td>
        <td></td>
    </tr>
    <tr>
        <td>Nombre entier/double</td>
             <td>Projet : heures prévues
        <br>Tâche : Pourcentage d'achèvement</td>
              <td><ul>
        <li>Égal à (non sensible à la casse)</li>
        <li>Non égal à (non sensible à la casse)</li>
        <li>Supérieur à</li>
          <li>Supérieur ou égal à</li>
          <li>Inférieur à</li>
          <li>Inférieur ou égal à</li>
            <li>Est nul</li>
              <li>N’est pas nul</li>
        </ul></td>
        <td></td>
    </tr>
       <tr>
        <td> Date/Date/Heure </td>
                    <td>Projet : Date de début prévue
        <br>Heure : Date d'entrée</td>
              <td><ul>
        <li>Égal à (non sensible à la casse)</li>
        <li>Non égal à (non sensible à la casse)</li>
        </ul></td>
        <td>En activant l’option <b>Définir la date relative</b>, vous pouvez appliquer des caractères génériques de date relative pour rendre le rapport plus dynamique et l’ajuster automatiquement en fonction de périodes courantes. 
         <ul><li>$$TODAY</li>
         <li>$$NOW</li>
         </ul>
        </td>
    </tr>
       <tr>
        <td>Booléen </td>
                  <td>Projet : contient des documents
        <br>Tâche : est critique
        Utilisateur <br> : Est Actif</td>
        <td><ul>
        <li>Égal à (non sensible à la casse)</li>
        <li>Non égal à (non sensible à la casse)</li>
        </ul></td>
        <td> </td>
    </tr>
   </table>

+++
