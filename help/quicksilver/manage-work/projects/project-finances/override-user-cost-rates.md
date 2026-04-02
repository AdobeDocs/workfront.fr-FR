---
content-type: overview
product-area: projects
navigation-topic: financials
title: Remplacer les taux de coûts utilisateur au niveau du projet
description: Cet article décrit comment remplacer les taux de coûts utilisateur système pour un projet.
author: Lisa
feature: Work Management
source-git-commit: cb21414992587c62c37580f156100f2b5b755e9b
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 27%

---

# Remplacer les taux de coûts utilisateur au niveau du projet

{{highlighted-preview-article-level}}

Vous pouvez spécifier le taux de coût pour un utilisateur ou une utilisatrice sur un projet spécifique. Ce taux de coût au niveau du projet remplace le taux de coût au niveau du système pour cet utilisateur. Workfront utilise le taux de coût au niveau du projet de la fonction pour calculer le coût, au lieu d&#39;utiliser le taux de coût au niveau du système.

Cet article décrit comment remplacer les taux de coûts utilisateur système pour un projet.

Pour plus d&#39;informations sur le calcul des coûts du projet, voir [Généralités sur les revenus et la hiérarchie des coûts](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) et [Suivre les coûts](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets et aux données financières</p>
       <p><p>Vous devez également disposer de l’un des éléments suivants :</p> 
        <ul> 
          <li> <p>Niveau d’accès de l’administrateur système. </li> 
          <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Gérer les autorisations du projet qui inclut Modifier les données financières </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Le champ **Remplacement du taux de coût autorisé** doit être activé pour l’utilisateur dans son profil utilisateur. Lorsque le champ de remplacement des coûts n&#39;est pas activé pour un utilisateur, les remplacements des coûts ne sont autorisés pour cet utilisateur sur aucun projet et le système utilise le taux du profil utilisateur pour calculer les coûts.

Pour plus d’informations, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Remplacer les taux de coûts utilisateur au niveau du projet

1. Accédez au projet pour lequel vous souhaitez remplacer les taux de coûts.
1. Cliquez sur **Taux** dans le panneau de gauche. Vous devrez peut-être d’abord cliquer sur **Afficher plus**.
1. Cliquez sur l’onglet **Coût** s’il n’est pas déjà sélectionné.
1. Cliquez sur **Ajouter un taux de coûts** > **Nouveau taux de coûts utilisateur**.

   La boîte Nouveau taux de coût utilisateur s&#39;ouvre.

1. Dans le champ **Utilisateur**, sélectionnez l&#39;utilisateur dont vous souhaitez modifier le taux de coût.
1. Sélectionnez la **Devise** pour le remplacement du taux de coût.
1. Dans le champ **Taux de coût**, saisissez le premier remplacement du taux de coût.
1. (Facultatif) Cliquez sur **Ajouter un taux de validité de date** pour ajouter d&#39;autres remplacements de taux de coût.

   >[!NOTE]
   >
   >Si vous saisissez un seul remplacement de taux, il s&#39;applique pendant toute la durée de vie du projet.
   >Si vous souhaitez avoir des taux différents au fil du temps, vous pouvez ajouter plusieurs remplacements avec effet de date.

1. (Conditionnel) Si vous ajoutez plusieurs remplacements de taux de coût, spécifiez les informations suivantes pour chaque ligne :

   * **Taux de coût** : valeur du taux de coût au cours de la période spécifiée.
   * **Date de début** : date à laquelle le remplacement du taux de coût commence.
   * **Date de fin** : date de fin de remplacement du taux de coût.

   ![Nouvelle zone Taux de coût utilisateur affichant les dates d&#39;entrée en vigueur](assets/new-user-cost-rate-box.png)

   Workfront applique le taux de remplacement de la fonction aux heures qui se produisent pendant ces périodes lors du calcul du coût du projet.

   Il ne doit pas y avoir d’écart entre les périodes de deux taux de remplacement. La **Date de début** d’un taux de remplacement doit être le jour suivant la **Date de fin** de la date de remplacement précédente.

   Il n&#39;est pas nécessaire de spécifier une date de début pour le premier taux de remplacement ni une date de fin pour le dernier taux de remplacement.

   Nous vous recommandons d’utiliser le taux par défaut pour le premier taux de remplacement.

   Workfront suppose que le premier taux de remplacement est appliqué pour toutes les heures dont la date est antérieure à la date de fin du premier remplacement et que le dernier est appliqué pour toutes les heures dont la date est plus récente que la date de début du dernier remplacement.

   Si une heure est enregistrée avant la date de début prévue du projet, le tout premier taux de coût est utilisé.

   Si une heure est consignée après la date d&#39;achèvement prévue du projet, le dernier taux de coût est utilisé.

1. Cliquez sur **Enregistrer**.


