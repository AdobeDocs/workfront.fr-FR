---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Groupement : indiquer si les résultats d’un groupement doivent être réduits ou développés à l’aide du mode texte."'
description: '''Groupement : indiquer si les résultats d’un groupement doivent être réduits ou développés à l’aide du mode texte."'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Regroupement : indiquer si les résultats d’un groupement doivent être réduits ou développés à l’aide du mode texte ;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Vous pouvez indiquer si les résultats d’un groupement doivent s’afficher, réduit ou développé, dans une liste ou un rapport à l’aide du Créateur de rapports standard. Par défaut, l’affichage d’un groupement est agrandi. Pour plus d’informations sur la création d’un groupement, voir [Création de groupes dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Lorsque vous ajustez manuellement les groupements lors de l&#39;affichage d&#39;une liste, Adobe Workfront mémorise vos préférences manuelles jusqu&#39;à ce que vous vous déconnectiez. Lorsque vous vous reconnectez, la liste s’affiche en fonction de ce paramètre.
>* Les résultats d’un groupement s’affichent toujours agrandi après leur accès à partir d’un élément de graphique.
>


Vous pouvez également indiquer si un groupement doit s’afficher développé ou réduit en mode texte.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un groupement </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification d’un rapport</p> <p>Editer l'accès aux Filtres, Vues, Groupements pour modifier un groupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Indique si les résultats d’un groupement doivent être réduits ou développés à l’aide du mode texte.

1. Accédez à une liste d’objets.
1. Dans la **Regroupement** menu déroulant, sélectionnez **Nouveau groupement**.

1. Ajoutez un groupement et cliquez sur **Passer en mode Texte**.

   Ou

   Si le groupement est déjà en mode texte, ajoutez le code suivant au niveau de groupement que vous souhaitez afficher réduit :

   ```
   group.0.iscollapsed=true
   ```

1. (Facultatif) Si vous souhaitez que le regroupement s’affiche de manière étendue, ajoutez le code suivant au niveau de regroupement approprié :

   ```
   group.0.iscollapsed=false
   ```

1. Cliquez sur **Terminé**, puis **Enregistrer le groupement**.
