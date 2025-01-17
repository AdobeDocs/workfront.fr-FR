---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modifier un filtre en mode texte
description: Vous pouvez modifier un filtre dans une liste ou un rapport à l’aide du mode texte pour accéder aux champs qui ne sont pas disponibles dans l’interface standard et créer des filtres plus complexes.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 86%

---

# Modifier un filtre en mode texte

<!-- Audited: 1/2025 -->

Vous pouvez modifier un filtre dans une liste ou un rapport à l’aide du mode texte pour accéder aux champs qui ne sont pas disponibles dans l’interface standard et créer des filtres plus complexes.

Pour plus d’exemples du mode texte lors de la création d’un filtre, voir également la section [Exemples de filtres personnalisés](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) dans l’article [Exemples de vue, de filtre et de regroupement personnalisés : index des articles](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
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
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux filtres, aux vues et aux regroupements</p> <p>Modifier l’accès aux rapports, aux tableaux de bord et aux calendriers pour modifier des éléments de création de rapports d’un rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier des filtres dans un rapport</p> <p>Gérer les autorisations d’un filtre pour le modifier</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer à utiliser le mode texte dans un rapport ou une liste, assurez-vous toujours de bien connaître la syntaxe du mode texte Workfront.

Pour plus d’informations, voir :

* [Vue d’ensemble du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Vue d’ensemble de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exemples de vues, de filtres et de regroupements personnalisés : index des articles](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modifier un filtre en mode texte

La modification d’un filtre en mode texte est identique pour les rapports et les listes. L’accès au filtre à partir d’un rapport ou d’une liste diffère.

>[!TIP]
>
>Nous vous recommandons de créer la plus grande partie possible du filtre en mode standard, puis de convertir le filtre en mode texte pour le modifier.

Pour plus d’informations sur la création de filtres, voir [Vue d’ensemble des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Utilisez l’une des méthodes suivantes :

   Pour accéder au filtre depuis une liste, accédez à la liste et cliquez sur l’icône **Filtre**, puis pointez sur le filtre du panneau latéral **Filtres** que vous souhaitez modifier, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png). Le panneau latéral **Filtres** affiche le filtre sélectionné ou le créateur de filtres hérité s’ouvre.

   OU

   Pour accéder au filtre à partir d’un rapport, accédez au rapport, puis cliquez sur l’onglet **Actions du rapport** > **Modifier** > **Filtres** .

1. Utilisez l’une des méthodes suivantes :

   Si vous utilisez le panneau latéral **Filtres** sur une liste, cliquez sur **Mode texte**.

   OU

   Si vous utilisez l’ancien créateur de filtres ou dans un rapport, cliquez sur **Ajouter une règle de filtre** pour commencer à ajouter les conditions de votre filtre. Cliquez ensuite sur **Passer en mode texte** puis **Modifier le mode texte** sur le côté droit du créateur.

1. Ajoutez des instructions de filtre à l’aide du mode texte. Chaque instruction de filtre peut contenir les lignes suivantes et des informations supplémentaires :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Ligne/information de filtre</b></td> 
      <td><b>Exemple</b></td> 
     </tr> 
     <tr> 
      <td> <p>Nom du champ et valeur correspondante tels qu’ils apparaissent dans la base de données Workfront.</p> <p>Cette ligne est obligatoire.</p> <p> Pour plus d’informations sur l’affichage des objets et des champs dans la base de données, voir <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorateur d’API</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Pour filtrer les tâches dont le statut est En cours, utilisez la ligne suivante :</p> <p><code>status=INP</code> </p> <p><b>CONSEIL</b>

   Lorsque vous filtrez les statuts, vous devez utiliser le code à trois lettres du statut et non son nom.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Modificateur de nom de champ et ce à quoi il correspond. Cela indique les conditions que le champ que vous filtrez doit remplir.</p> <p>Cette ligne est obligatoire.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Pour indiquer que le statut des tâches que vous filtrez doit être égal à En cours, utilisez la ligne suivante en plus de celle ci-dessus :</p> <p><code>status_Mod=in</code> </p> <p>Si le modificateur est une plage, il y a deux lignes pour indiquer le modificateur.</p> 
       <div> <span class="autonumber"><span><b>EXEMPLE</b></span></span> 
        <p>Il s’agit d’un filtre en mode texte qui recherche les tâches en cours, dont la date d’achèvement prévue se situe dans le mois en cours et qui sont affectées à un utilisateur ou une utilisatrice disposant d’un GUID spécifique :</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Pour obtenir la liste complète des modificateurs de filtre en mode texte, consultez l’article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificateurs de filtre et de condition</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Opérateur d’instruction. Par défaut, chaque instruction de filtre est connectée par l’opérateur « AND ». Cela ne s’affiche pas dans l’interface en mode texte. Vous pouvez également ajouter un opérateur « OR » entre deux instructions pour indiquer que vous souhaitez filtrer les objets pouvant remplir l’une ou l’autre des deux conditions.</p> <p>Les opérateurs de filtre ne sont requis que pour les filtres comportant plusieurs instructions.</p> <p>Conseil :   
        <ul> 
         <li> <p>« OR » est sensible à la casse et doit toujours être en majuscules.</p> </li> 
         <li> <p>Lorsque vous changez votre opérateur de AND en OR, le nombre d’éléments de la liste peut augmenter.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>EXEMPLE</b></span></span> 
        <p>Pour filtrer les tâches dont le statut est En cours ou dont la date d’achèvement prévue est aujourd’hui, utilisez les méthodes suivantes : </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Caractère générique qui permet de généraliser les informations dans un filtre et de référencer l’heure actuelle ou la personne connectée.</p> <p>Les caractères génériques sont facultatifs.</p> <p>Conseil :   <p>Il est recommandé d’utiliser des caractères génériques dans la mesure du possible pour rendre vos filtres plus dynamiques et ne pas dupliquer les mêmes filtres pour chaque utilisateur ou utilisatrice ou pour des périodes similaires.</p> <p>Pour plus d’informations sur les caractères génériques de filtre, consultez <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Vue d’ensemble des variables de filtrage des caractères génériques</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>EXEMPLE</b></span></span> 
        <p>Pour filtrer les tâches affectées à la personne actuellement connectée, utilisez les méthodes suivantes :</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Pour ajouter une instruction de filtre connectée par l’opérateur « OR », procédez comme suit :

   1. Ajoutez une nouvelle ligne de code et saisissez OR:1: suivi de l’objet ou de l’attribut par lequel vous souhaitez filtrer et de la valeur avec laquelle vous souhaitez le comparer. Pour référencer des tâches dont le statut est différent de Nouveau, utilisez la ligne suivante :

      `OR:1:status=NEW`

   1. Ajoutez une seconde ligne et saisissez OU:1: suivi de l’objet, du modificateur et du code du modificateur. Pour définir le modificateur de la ligne de code faisant référence à tous les statuts de tâche, à l’exception de Nouveau, utilisez la ligne de modificateur suivante :

      `OR:1:status_Mod=notin`

      Chaque ligne de la nouvelle instruction doit être précédée de « OR:`<number>`: ».

      Pour plus d’informations sur la création d’instructions « OR » dans un filtre, consultez [Créer des instructions « OR » dans les filtres en mode texte](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >Vous pouvez avoir plusieurs instructions « OR » dans le même filtre. Chaque fois que vous disposez d’une nouvelle instruction « OR », le nombre après « OR: » augmente.
      >
      >Pour filtrer les tâches dont le statut est En cours ou qui sont affectées à la personne connectée ou dont la date d’achèvement prévue est aujourd’hui, utilisez les méthodes suivantes :
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. Cliquez sur **Appliquer** ou **Terminé** pour enregistrer vos modifications du mode texte et continuer à modifier le rapport ou le filtre.
1. Cliquez sur **Enregistrer et fermer** pour enregistrer votre rapport ou **Enregistrer le filtre** pour enregistrer le filtre dans la liste.


