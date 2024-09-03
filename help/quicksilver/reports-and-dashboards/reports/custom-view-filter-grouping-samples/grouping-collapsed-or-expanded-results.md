---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Regroupement : indiquer si les résultats d’un regroupement doivent être réduits ou développés en mode texte. »'
description: '« Regroupement : indiquer si les résultats d’un regroupement doivent être réduits ou développés en mode texte. »'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 100%

---

# Regroupement : indiquer si les résultats d’un regroupement doivent être réduits ou développés en mode texte

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
   <td> <p>Demander à modifier un regroupement </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et regroupements pour modifier un regroupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Indiquer si les résultats d’un regroupement doivent être réduits ou développés en mode texte

1. Accédez à une liste d’objets.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Ajoutez un regroupement et cliquez sur **Passer en mode Texte**.

   Ou

   Si le regroupement est déjà en mode texte, ajoutez le code suivant au niveau du regroupement que vous souhaitez afficher réduit :

   ```
   group.0.iscollapsed=true
   ```

1. (facultatif) Si vous souhaitez que le regroupement s’affiche de manière développée, ajoutez le code suivant au niveau du regroupement approprié :

   ```
   group.0.iscollapsed=false
   ```

1. Cliquez sur **Terminé**, puis sur **Enregistrer le regroupement**.
