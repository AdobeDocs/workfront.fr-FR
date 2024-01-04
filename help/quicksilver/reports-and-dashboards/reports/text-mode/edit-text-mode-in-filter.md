---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modification d’un filtre à l’aide du mode texte
description: "REMARQUE : ajoutez une section dans cet article : /Content/Reports and Dashboard/Reports/Reporting Elements/create-customize-fitlers.html; *** Également, brouillez cette zone dans l’article Présentation du mode Texte )"
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# Modification d’un filtre à l’aide du mode texte

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

Vous pouvez éditer un filtre dans une liste ou un rapport à l&#39;aide du mode texte pour accéder aux champs qui ne sont pas disponibles dans l&#39;interface standard et créer des filtres plus complexes.

Pour plus d’exemples de mode texte lors de la création d’un filtre, reportez-vous également à la section &quot;Exemples de filtres personnalisés&quot; dans l’article . [Exemples de filtrage, de filtrage et de regroupement personnalisés : index de l&#39;article](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification des éléments de rapport dans un rapport</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier des filtres dans un rapport</p> <p>Gérer les autorisations d’un filtre pour le modifier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer à utiliser le mode texte dans un rapport ou une liste, assurez-vous toujours de bien connaître la syntaxe du mode texte Workfront.

Pour plus d’informations, voir :

* [Présentation du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Présentation de la syntaxe du mode texte](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exemples de filtrage, de filtrage et de regroupement personnalisés : index de l&#39;article](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Mode d’édition de texte dans un filtre

La modification d’un filtre en mode texte est identique pour les rapports et les listes. L’accès au filtre à partir d’un rapport ou d’une liste diffère.

>[!TIP]
>
>Nous vous recommandons de créer autant de filtre que possible en mode standard, puis de convertir le filtre en mode texte pour l&#39;éditer.

Pour plus d’informations sur la création de filtres, voir [Présentation des filtres](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Utilisez l’une des méthodes suivantes :

   1. Pour accéder au filtre d&#39;un rapport, accédez au rapport, puis cliquez sur **Actions de rapport** > **Modifier** > **Filtres** .
   1. Pour accéder au filtre à partir d&#39;une liste, accédez à la liste et à partir du **Filtrer** dans le menu déroulant, placez le pointeur de la souris sur le filtre à modifier, puis cliquez sur l’icône **Modifier** icon ![](assets/edit-icon.png).

      Le créateur de filtres s’ouvre.

1. Cliquez sur **Ajouter une règle de filtre** pour commencer à ajouter les conditions de votre filtre, puis cliquez sur **Passer en mode Texte** dans le coin supérieur droit du créateur.
1. Ajoutez des instructions de filtre à l’aide du mode texte. Chaque instruction de filtre peut contenir les lignes suivantes et des informations supplémentaires :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Ligne/information de filtre</b></td> 
      <td><b>Exemple</b></td> 
     </tr> 
     <tr> 
      <td> <p>Nom du champ et la valeur à laquelle il est égal, tels qu’ils apparaissent dans la base de données Workfront.</p> <p>Cette ligne est obligatoire.</p> <p> Pour plus d’informations sur l’affichage des objets et des champs dans la base de données, voir <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorateur d’API</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Pour filtrer les tâches dont l'état est En cours, utilisez la ligne suivante :</p> <p><code>status=INP</code> </p> <p><b>CONSEIL</b>

   Lorsque vous filtrez les états, vous devez utiliser le code à trois lettres de l’état et non le nom.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Modificateur de nom de champ et auquel le modificateur est égal. Cela indique les conditions que doit remplir le champ que vous filtrez.</p> <p>Cette ligne est obligatoire.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Pour indiquer que l'état des tâches pour lesquelles vous filtrez doit être égal à En cours, utilisez la ligne suivante en plus de celle ci-dessus :</p> <p><code>status_Mod=in</code> </p> <p>Si le modificateur est une plage, il y a deux lignes pour indiquer le modificateur.</p> 
       <div> <span class="autonumber"><span><b>EXEMPLE </b></span></span> 
        <p>Il s’agit d’un filtre de mode texte qui recherche les tâches en cours, dont la date de fin est planifiée au cours du mois en cours et qui sont affectées à un utilisateur disposant d’un GUID spécifique :</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Pour obtenir la liste complète des modificateurs de filtre en mode texte, voir l’article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificateurs de filtre et de condition</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Opérateur de relevé. Par défaut, chaque instruction de filtre est connectée par l’opérateur "AND". Cela ne s’affiche pas dans l’interface du mode texte. Vous pouvez également ajouter un opérateur "OU" entre deux instructions pour indiquer que vous souhaitez filtrer les objets pouvant remplir l’une ou l’autre des deux conditions.</p> <p>Les opérateurs de filtre ne sont requis que pour les filtres comportant plusieurs instructions.</p> <p>Conseil :   
        <ul> 
         <li> <p>"OU" est sensible à la casse et doit toujours être majuscule.</p> </li> 
         <li> <p>Lorsque vous changez votre opérateur de ET en OU, le nombre d’éléments de liste peut augmenter.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>EXEMPLE </b></span></span> 
        <p>Pour filtrer les tâches dont l’état est En cours ou dont la date d’achèvement prévue est aujourd’hui, utilisez les méthodes suivantes : </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Un caractère générique qui permet de généraliser les informations dans un filtre et de référencer l’heure actuelle de l’utilisateur connecté.</p> <p>Les caractères génériques sont facultatifs.</p> <p>Conseil :   <p>Il est recommandé d’utiliser des caractères génériques chaque fois que possible pour rendre vos filtres plus dynamiques et ne pas dupliquer les mêmes filtres pour chaque utilisateur ou pour des périodes similaires.</p> <p>Pour plus d’informations sur les caractères génériques de filtre, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variables de filtre génériques</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>EXEMPLE</b></span></span> 
        <p>Pour filtrer les tâches affectées à l’utilisateur actuellement connecté, utilisez les méthodes suivantes :</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Pour ajouter une instruction de filtre connectée par l’opérateur &quot;OR&quot;, procédez comme suit :

   1. Ajoutez une nouvelle ligne de code et saisissez OU:1: suivi de l’objet ou de l’attribut par lequel vous souhaitez filtrer et de la valeur avec laquelle vous souhaitez le comparer. Pour référencer des tâches dont l’état est différent de Nouveau, utilisez la ligne suivante :

      ```
      OR:1:status=NEW
      ```

   1. Ajoutez une seconde ligne et saisissez OU:1: suivi de l’objet, du modificateur et du code de modificateur. Pour définir le modificateur de la ligne de code faisant référence à tous les états de tâche, à l’exception de Nouveau, utilisez la ligne de modificateur suivante :

      ```
      OR:1:status_Mod=notin
      ```

      Chaque ligne de la nouvelle instruction doit être précédée de &quot;OR:`<number>`:&quot;.

      Pour plus d’informations sur la création d’instructions &quot;OR&quot; dans un filtre, voir [Créer des instructions &quot;OR&quot; dans les filtres de mode texte](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>Vous pouvez avoir plusieurs instructions &quot;OR&quot; dans le même filtre. Chaque fois que vous disposez d’une nouvelle instruction &quot;OU&quot;, le nombre après &quot;OU&quot; augmente.
>
Pour filtrer les tâches dont l’état est En cours ou qui sont affectées à l’utilisateur connecté ou dont la date d’achèvement prévue est atteinte aujourd’hui, utilisez les méthodes suivantes :
>
`status=INP`
>
`status_Mod=in`
>
`OR:1:assignedToID=$$USER.ID`
>
`OR:1:assignedToID_Mod=in`
>
`OR:2:plannedCompletionDate=$$TODAY`
>
`OR:2:plannedCompletionDate_Mod=eq`

1. Cliquez sur **Terminé** si vous souhaitez enregistrer vos modifications et continuer à modifier le rapport ou le filtre.
1. Cliquez sur **Enregistrer + Fermer** pour enregistrer votre rapport ou **Enregistrer le filtre** pour enregistrer le filtre dans la liste.


