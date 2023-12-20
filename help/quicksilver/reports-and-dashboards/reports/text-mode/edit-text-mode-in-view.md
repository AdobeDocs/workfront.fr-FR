---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modification d’une vue en mode texte
description: "REMARQUE : ajoutez une section dans cet article : /Content/Reports and Dashboard/Reports/Reporting Elements/create-customize-views.html *** Également, rédigez cette zone dans l’article Présentation du mode texte )"
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1639'
ht-degree: 0%

---

# Modification d’une vue en mode texte

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

Vous pouvez modifier une vue dans une liste ou un rapport à l’aide du mode texte pour accéder à des champs qui ne sont pas disponibles dans l’interface standard et créer des vues plus complexes.

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
   <td> <p>Gérer les autorisations d’un rapport pour modifier les vues d’un rapport</p> <p>Gérer les autorisations pour une vue pour la modifier</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
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

## Mode Modifier le texte dans une vue

La modification d’une vue en mode texte est identique pour les rapports et les listes. L’accès à la vue depuis un rapport ou depuis une liste diffère.

>[!TIP]
>
>Nous vous recommandons de créer autant de vue que possible en mode standard, puis de la convertir en mode texte pour l’éditer.

Pour plus d’informations sur la création de vues, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Utilisez l’une des méthodes suivantes :

   1. Pour accéder à la vue depuis un rapport, accédez au rapport, puis cliquez sur **Actions de rapport** > **Modifier** > **Colonnes (affichage)** .
   1. Pour accéder à la vue depuis une liste, accédez à la liste et à la **Affichage** dans le menu déroulant, placez le pointeur de la souris sur la vue à modifier, puis cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png).

      Le créateur de vues s’ouvre.

1. Sélectionnez une colonne dans la vue.

   Ou

   Sélectionnez la variable **Colonnes (affichage)** du créateur de rapports, puis sélectionnez une colonne.

   >[!TIP]
   >
   >Pour modifier une vue en mode texte, vous devez modifier une colonne à la fois.

1. Cliquez sur **Passer en mode Texte** dans le coin supérieur droit du créateur.

   >[!NOTE]
   >
   >Lorsque vous modifiez une colonne en mode texte, Workfront ajoute la variable `textmode=true` ligne de code vers la colonne . Cela indique que la colonne est modifiée en mode texte.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   Le tableau suivant décrit les lignes clés dans une vue en mode texte :

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Exemple de ligne</th> 
      <th>Description</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>Il s’agit du nom de l’objet ou du champ tel qu’il apparaît dans la base de données. Pour plus d’informations sur l’affichage des objets et des champs dans la base de données, voir <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorateur d’API</a>.</p> <p>Les scénarios suivants existent :</p> 
       <ol> 
        <li value="1"> <p> Si le nom du champ que vous affichez est une expression au lieu d’un nom unique, vous devez utiliser la syntaxe de casse mixte pour la variable <code>valuefield</code>. Par exemple, pour la Date de début planifiée d’une tâche, le code est : </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Si vous souhaitez afficher un champ personnalisé, la variable <code>valuefield</code> value est le nom réel du champ, comme vous le voyez dans l’interface. Par exemple, pour un champ personnalisé nommé "Plus d’informations", le code est :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Si vous souhaitez afficher les objets associés à d’autres objets dans une vue à l’aide de la propriété <code>valuefield</code> ligne de code les noms et attributs des objets sont séparés par des deux-points. </p> <p>Par exemple, une colonne dans une vue de tâche qui afficherait le nom du Propriétaire du Portfolio a la valeur suivante pour la ligne de champ de valeur :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>Cela indique qu’à partir de l’objet du rapport (tâche), vous pouvez accéder à l’objet associé suivant (projet), à partir de là, vous pouvez accéder à l’objet associé suivant à partir du projet (portefeuille), puis au propriétaire (propriétaire) du portefeuille, puis à son nom (nom). </p> </li> 
       </ol> <p>Pour plus d’informations sur la façon dont les objets se connectent les uns aux autres, voir la section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdépendance et hiérarchie des objets</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Présentation des objets dans Adobe Workfront</a>.</p> <p>Remarque : si vous choisissez un champ en mode texte non valide dans l’interface standard, vous ne pourrez pas revenir à l’interface standard dans la colonne.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Cette ligne représente le format utilisé pour afficher la variable <code>valuefield</code>. La variable <code>valueformat</code> identifie si un objet ou un champ s’affiche sous forme de texte, de nombre, de pourcentage ou de date.</p> <p>Nous vous recommandons d’utiliser <code>HTML</code> pour votre <code>valueformat</code>, en particulier lors de l’utilisation de <code>valueexpression</code>, afin d’assurer l’affichage le plus précis de vos informations. </p> <p>Pour plus d’informations sur les valeurs supplémentaires de cette ligne, voir <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Utilisation de la mise en forme conditionnelle en mode Texte</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Vous pouvez ajouter cette ligne pour remplacer <code>valuefield</code>, si vous souhaitez afficher un champ calculé dans la colonne .</p> <p>Vous devez joindre la variable <code>valuefield</code> des objets entre accolades chaque fois que vous les utilisez dans une balise <code>valueexpression</code>.</p> <p>Les scénarios suivants existent : </p> 
       <ol> 
        <li value="1"> <p>Si vous souhaitez afficher un champ dans une colonne en majuscules, utilisez :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>La variable <code>valuefield</code> de l’objet est orthographié tel qu’il apparaît dans l’explorateur d’API. </p> </li> 
        <li value="2">Si vous souhaitez ajouter plusieurs <code>valuefields</code> en les liant, vous devez les séparer par un point.</li> 
        <li value="3"> <p>Par exemple, si vous souhaitez afficher le nom du Principal cessionnaire d’une tâche à l’aide de <code>valueexpression</code>, vous utiliseriez :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>Si vous souhaitez utiliser un champ personnalisé dans une <code>valueexpression</code> vous devez précéder le nom du champ de <code>DE:</code> pour indiquer qu’il s’agit d’un champ personnalisé. Le nom du champ est orthographié tel qu’il apparaît dans l’interface. </p> <p>Important : Lorsque vous utilisez un champ personnalisé placé dans une section de formulaire personnalisée dotée d’autorisations restreintes pour certains utilisateurs, le calcul de l’expression de valeur est vide lorsque ces utilisateurs voient ce calcul dans un rapport. Pour plus d’informations sur l’ajustement des autorisations des sections de formulaire personnalisées, voir <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a></span>.</p> <p>Par exemple, si vous disposez d’un champ personnalisé intitulé "Nom du développeur" et que vous souhaitez afficher ce champ en majuscules dans une colonne, vous pouvez utiliser les éléments suivants : <code>valueexpression</code> pour indiquer :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>Lors du référencement d’un champ personnalisé de type Type , utilisez l’expression suivante pour référencer le nom de l’objet sélectionné dans un champ intitulé "Nom du développeur" :</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>Cette ligne définit le texte d’une info-bulle lorsque vous placez le pointeur de la souris sur le nom de la colonne. Dans ce cas, il utilise une clé pour traduire la valeur name dans le texte de description. Si vous souhaitez modifier la description, modifiez la ligne suivante : </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Cette ligne définit le libellé de la colonne. Dans ce cas, il utilise la valeur abrégée en fonction de la clé.</p> <p>Si vous souhaitez modifier le nom de la colonne, vous pouvez définir cette valeur sur : </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> permet de saisir le nom de la colonne, tandis que<code>namekey</code> nécessite de saisir une clé qui est utilisée pour traduire le nom d’une colonne.</p> <p>Pour modifier le nom de la colonne, vous pouvez également ajouter la variable <code>displayname </code>, si elle n’est pas présente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Vous pouvez ajouter la ligne suivante pour modifier le nom d’une colonne, ce qui permet de suspendre l’événement <code>namekey/name</code> value:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>Cette ligne définit le mode de tri des résultats lorsque l’utilisateur clique sur l’en-tête de colonne. S’il n’est pas présent, la colonne ne peut pas être triée après l’exécution du rapport.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>Cette ligne représente le nombre de pixels utilisés pour la colonne. Si la ligne est omise ou définie sur 0 (zéro), la colonne n’apparaît pas dans la vue.</p> <p>Lorsque vous modifiez ce champ manuellement en mode texte, vous devez également ajouter la variable <code>usewidths=true</code> à votre colonne .</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>Vous devez utiliser cette ligne en plus de la fonction <code>width=</code> lors de la personnalisation de la largeur d’une colonne. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>Cette ligne définit si la valeur affichée dans une colonne est modifiable en ligne ou non. Si cette ligne est égale à <strong>true</strong>, la valeur de la colonne est modifiable en ligne. Si cette ligne est égale à <code>false</code>, la valeur de la colonne n’est pas modifiable en ligne.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>Insérez cette ligne uniquement lorsque vous souhaitez que la valeur affichée dans une colonne soit associée à l’objet qui lui est associé. Le lien ouvre la page de détails de l’objet. Cette valeur doit correspondre à la variable <code>valuefield=</code> ligne. Lorsque vous insérez ceci, vous devez également ajouter le <code>link.valueformat=</code> ligne. </p> <p> Par exemple, vous pouvez insérer <code>link.valuefield=priority</code> dans une vue issue d’un problème, et la priorité du problème s’affiche sous la forme d’un lien. Cliquez sur ce lien pour ouvrir la page Problème .</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>Insérez cette ligne uniquement lorsque vous avez inséré la <code>link.valuefield</code> pour ajouter un lien vers la valeur d’une colonne. Le lien ouvre la page de détails de l’objet. Cette valeur doit correspondre à la variable <code>valueformat=</code> et indique le format utilisé pour afficher la variable <code>valuefield</code>. </p> <p>Important : Lorsque vous affichez le mode texte dans une colonne intégrée qui comprend également un lien, vous remarquerez que plusieurs lignes font référence au lien. Certaines de ces lignes peuvent ne plus être prises en charge ou ne plus être inutiles lorsque vous créez votre propre colonne personnalisée en mode texte et que vous y ajoutez les instructions de lien. Les lignes obligatoires lors de l’ajout d’une valeur liée sont<code> link.valuefield</code> et <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggator.function=</strong> </td> 
      <td> <p>Cela fait référence à la manière dont les valeurs de chaque colonne sont résumées. Plusieurs lignes commencent par <code>aggregator.</code> et ils font tous référence à l'agrégateur qui résume les résultats de la colonne. </p> <p>En règle générale, la variable <code>aggregator.</code> les lignes correspondent à celles de l’objet column . </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>Exemple : </b></span></span> 
        <p>La colonne Heures planifiées d’un rapport de tâche résumée par Somme peut se présenter comme suit : </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valuefield=workRequired</pre>
         <pre>valueformat=composé</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        La variable <code>aggregator. </code>les lignes peuvent contenir un <code>valuefield </code>ou <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Appliquer** si vous souhaitez enregistrer vos modifications et continuer à modifier la vue.
1. Cliquez sur **Enregistrer + Fermer** pour enregistrer votre rapport.

   Ou

   Cliquez sur **Enregistrer la vue** pour enregistrer la vue dans une liste.
