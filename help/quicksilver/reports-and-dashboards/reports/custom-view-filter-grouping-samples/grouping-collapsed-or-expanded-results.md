---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Regroupement : indique si les résultats d’un groupement doivent être réduits ou développés en mode Texte"
description: '« Regroupement : indiquer si les résultats d’un regroupement doivent être réduits ou développés en mode texte. »'
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 85%

---

# Regroupement : indiquer si les résultats d’un regroupement doivent être réduits ou développés en mode texte

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Vous pouvez indiquer si les résultats d’un regroupement doivent s’afficher réduits ou développés dans une liste ou un rapport à l’aide du Report Builder standard. Par défaut, les résultats d’un regroupement s’affichent de façon développée. Pour plus d’informations sur la création d’un regroupement, voir [Créer des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Lorsque vous ajustez manuellement les regroupements lors de l’affichage d’une liste, Adobe Workfront mémorise vos préférences manuelles jusqu’à ce que vous vous déconnectiez. Lorsque vous vous reconnectez, la liste s’affiche en fonction de ce paramètre.
>* Les résultats d’un regroupement s’affichent toujours développés après que l’on y a accédé à partir d’un élément de graphique.
>

Vous pouvez également indiquer si un regroupement doit s’afficher développé ou réduit en mode texte.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Indiquer si les résultats d’un regroupement doivent être réduits ou développés en mode texte

1. Accédez à une liste d’objets.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Ajoutez un groupement, puis cliquez sur **Passer en mode Texte**.

   Ou

   Si le regroupement est déjà en mode texte, ajoutez le code suivant au niveau du regroupement que vous souhaitez afficher réduit :

   `group.0.iscollapsed=true`

1. (facultatif) Si vous souhaitez que le regroupement s’affiche de manière développée, ajoutez le code suivant au niveau du regroupement approprié :

   `group.0.iscollapsed=false`

1. Cliquez sur **Terminé**, puis sur **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du groupement, puis cliquez sur **Enregistrer le groupement**.
