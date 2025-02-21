---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modification d’un regroupement à l’aide du mode texte
description: Vous pouvez modifier un regroupement dans une liste ou un rapport à l’aide du mode texte afin d’accéder aux champs non disponibles dans l’interface standard et créer des regroupements plus complexes.
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 94%

---

# Modification d’un regroupement à l’aide du mode texte

<!-- Audited: 1/2025 -->

Vous pouvez modifier un regroupement dans une liste ou un rapport à l’aide du mode texte afin d’accéder aux champs non disponibles dans l’interface standard et créer des regroupements plus complexes.

>[!TIP]
>
>Nous vous recommandons de créer autant du regroupement que possible en mode standard, puis de le convertir en mode texte pour le modifier.

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
   <td> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier les regroupements dans un rapport</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport pour modifier des regroupements dans un rapport</p> <p>Gérer les autorisations d’un regroupement pour le modifier</p></td> 
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

## Modification d’un regroupement à l’aide du mode texte

La modification d’un regroupement en mode texte est identique pour les rapports et les listes. L’accès au regroupement à partir d’un rapport ou d’une liste diffère.

>[!NOTE]
>
>Les regroupements sont un élément de rapport obligatoire pour créer des graphiques dans les rapports. Les regroupements en mode texte ne sont pas pris en charge dans les graphiques.Pour plus d’informations sur l’ajout de graphiques aux rapports, voir [Ajouter un graphique à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Pour plus d’informations sur la création de regroupements, voir [Créer des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Utilisez l’une des méthodes suivantes :

   1. Pour accéder au regroupement à partir d’un rapport, accédez au rapport, puis cliquez sur l’onglet **Actions de rapport** > **Modifier** > **Regroupements**.
   1. Pour accéder au regroupement à partir d&#39;une liste, positionnez-vous dans la liste puis, dans le menu déroulant **Regroupement**, placez le pointeur de la souris sur le regroupement à modifier et cliquez sur l&#39;icône **Modifier** ![Icône Modifier](assets/edit-icon.png).

      Le créateur de regroupement s’ouvre.

1. Cliquez sur **Ajouter un regroupement** pour ajouter des regroupements, cliquez sur **Passer en mode Texte** dans le coin supérieur droit du créateur, puis cliquez sur **Modifier le mode Texte**.

   >[!TIP]
   >
   >Vous pouvez ajouter jusqu’à 3 regroupements dans l’interface standard. Vous pouvez ajouter un 4ème regroupement uniquement en mode texte et vous ne pouvez pas avoir plus de 4 niveaux de regroupement dans Workfront.

1. Commencez à saisir le nom d’un champ en fonction duquel vous souhaitez effectuer un regroupement.

   Sélectionnez le nom du champ lorsque vous le voyez dans la liste.

1. Cliquez sur **Passer en mode Texte** dans le coin supérieur droit du créateur.

   Le regroupement est alors affiché en mode texte.

   Lorsque vous éditez un regroupement en mode texte, Workfront ajoute la

   ```
   textmode=true
   ```

   ligne de code au regroupement. Cela indique que le regroupement est modifié en mode texte.

   **Exemple :** pour regrouper une liste de tâches par nom de projet, puis par nom du cessionnaire principal, votre regroupement doit ressembler à ce qui suit, en mode texte.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >Les lignes en gras sont obligatoires.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   Chaque champ du regroupement comporte plusieurs lignes de code qui font référence à ce champ.

   Le tableau ci-dessous décrit les lignes clés d’un regroupement en mode texte.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   >Les lignes clés d’un regroupement en mode texte sont similaires aux lignes requises pour créer des vues en mode texte.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>Exemple de ligne</strong> </th> 
      <th><strong>Description</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>group.&lt;nombre&gt;.</strong> </td> 
      <td> <p>Chaque ligne de code est précédée de ce texte. Les lignes de code qui font référence au même champ sélectionné dans le regroupement sont numérotées du même nombre, comme suit :</p> 
       <ul> 
        <li>Le premier regroupement du rapport a un nombre de groupe de 0. Toutes les lignes faisant référence au premier regroupement commencent par <code>group.0</code>.</li> 
        <li>Le second regroupement du rapport a un numéro de groupe de 1. Toutes les lignes faisant référence au second regroupement commencent par <em><code>group.1</code></em>.</li> 
        <li>Le troisième regroupement du rapport a un nombre de groupe de 2. Toutes les lignes faisant référence au troisième regroupement commencent par <em><code>group.2</code></em>.</li> 
        <li>En mode texte uniquement, vous pouvez ajouter un nombre de groupe de 3, pour un quatrième regroupement. Toutes les lignes faisant référence au quatrième regroupement commencent par <em><code>group.3</code></em>.</li> 
       </ul> <p>Remarque : 4 regroupements ne sont pas pris en charge dans le créateur. Ils ne sont pris en charge que lorsque vous utilisez le mode texte. Workfront ne prend pas en charge plus de 4 niveaux de regroupements.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>Il s’agit du nom de l’objet ou du champ tel qu’il apparaît dans la base de données. Pour plus d’informations sur l’affichage des objets et des champs dans la base de données, voir <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">Explorateur d’API</a>.</p> <p>Les scénarios suivants sont possibles :</p> 
       <ol> 
        <li value="1"> <p> Si le nom du champ que vous affichez est une expression au lieu d’un nom unique, vous devez utiliser la syntaxe « camel case » pour le <code>valuefield</code>. Par exemple, pour la Date de début prévue d’une tâche, le code est :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple :</b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Si vous souhaitez afficher un champ personnalisé, la valeur <code>valuefield</code> est le nom réel du champ, comme vous le voyez dans l’interface. Par exemple, pour un champ personnalisé nommé « Plus d’informations », le code est :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple :</b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Si vous souhaitez regrouper des objets associés à d’autres objets à l’aide de la ligne de code <code>valuefield</code>, les noms et attributs des objets sont séparés par des deux-points.</p> <p>Par exemple, un regroupement par nom de portfolio pour une liste de tâches a la valeur suivante pour la ligne de champ de valeur :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple :</b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Cela indique qu’à partir de l’objet du rapport (tâche), vous pouvez accéder à l’objet associé suivant (projet). À partir de là, vous pouvez accéder à l’objet associé suivant à partir du projet (portfolio), puis au nom du portfolio (nom).</p> </li> 
       </ol> <p>Pour plus d’informations sur la façon dont les objets se connectent les uns aux autres, voir la section <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdépendance et hiérarchie des objets</a> dans <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Présentation des objets dans Adobe Workfront</a>.</p> <p>Note : si vous choisissez un champ en mode texte non valide dans l’interface standard et passez à l’interface standard, le regroupement est supprimé.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Cette ligne représente le format utilisé pour afficher <code>valuefield</code>. Le <code>valueformat</code> identifie si un objet ou un champ s’affiche sous forme de texte, de nombre, de pourcentage ou de date.</p> <p>Nous vous recommandons d’utiliser <code>HTML</code> pour votre <code>valueformat</code>, en particulier lors de l’utilisation d’<code>valueexpression</code>, afin d’assurer l’affichage le plus précis de vos informations.</p> <p>Pour plus d’informations sur les valeurs supplémentaires de cette ligne, voir <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Utiliser la mise en forme conditionnelle en mode texte</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>Vous pouvez ajouter cette ligne pour remplacer <code>valuefield</code>, si vous souhaitez associer votre liste par un calcul entre plusieurs champs.</p> <p>Vous devez joindre le <code>valuefield</code> des objets entre accolades chaque fois que vous l’utilisez dans une <code>valueexpression</code>.</p> <p>Les scénarios suivants sont possibles :</p> 
       <ol> 
        <li value="1"> <p>Si vous souhaitez afficher le nom d’un regroupement en majuscules, procédez comme suit :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>Le <code>valuefield</code> de l’objet est orthographié tel qu’il apparaît dans l’explorateur d’API.</p> </li> 
        <li value="2">Si vous souhaitez ajouter plusieurs <code>valuefields</code> en les reliant dans une ligne <code>valueexpression </code>, vous devez les séparer par un point.<p>Par exemple, si vous souhaitez afficher le nom du portfolio en majuscules dans une liste de tâches, vous utiliserez le code suivant dans la ligne <code>valueexpression</code> :</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Si vous souhaitez utiliser un champ personnalisé dans une ligne <code>valueexpression</code>, vous devez faire précéder le nom du champ par <code>DE:</code> pour indiquer qu’il s’agit d’un champ personnalisé. Le nom du champ est orthographié tel qu’il apparaît dans l’interface.</p><p>Important : <span>lorsque vous utilisez un champ personnalisé placé dans une section de formulaire personnalisé dotée d’autorisations restreintes pour certaines personnes, le calcul de l’<code>valueexpression </code> est vide lorsque ces personnes affichent ce calcul dans un rapport. Pour plus d’informations sur l’ajustement des autorisations sur les sections de formulaire personnalisé, voir </span> <span href="help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Création d’un formulaire personnalisé</a></span>.</p><p>Par exemple, si vous disposez d’un champ personnalisé intitulé « Nom du développeur ou de la développeuse » et que vous souhaitez le regrouper en fonction de ce champ et l’afficher en majuscules, vous pouvez utiliser <code>valueexpression</code> pour l’indiquer :</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Lors du référencement d’un champ personnalisé de type saisie semi-automatique, utilisez l’expression suivante pour référencer le nom de l’objet sélectionné dans un champ intitulé « Nom du développeur ou de la développeuse » :</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Cette ligne définit le libellé du regroupement. Dans ce cas, il utilise la valeur abrégée en fonction de la clé.</p> <p>Si vous souhaitez modifier le nom du regroupement, vous pouvez modifier cette valeur, comme suit :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> permet de saisir n’importe quel texte pour le nom du regroupement, tandis que <code>namekey</code> a besoin d’une clé qui est utilisée pour traduire le nom d’un regroupement.</p> <p>Pour modifier le nom du regroupement, vous pouvez également ajouter la ligne <code>displayname </code>, si elle n’est pas déjà présente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Vous pouvez ajouter la ligne suivante pour modifier le nom d’une colonne, ce qui remplace la valeur <code>namekey/name</code> :</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Nous vous recommandons de supprimer toutes les lignes qui contiennent <code>name </code> lorsque vous renommez un regroupement.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Ajoutez l’une des lignes de code suivantes à un regroupement quelconque pour indiquer si les résultats du regroupement doivent s’afficher dans une liste développée ou réduite. Par défaut, les regroupements s’affichent de manière étendue :


   ```
   group.0.iscollapsed=true
   ```

   si vous souhaitez que le regroupement s’affiche avec les résultats réduits ;

   ```
   group.0.iscollapsed=false
   ```

   si vous souhaitez que le regroupement s’affiche avec les résultats développés.

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   >* Lorsque vous ajustez manuellement les regroupements lors de l’affichage d’une liste, Workfront mémorise vos préférences manuelles jusqu’à ce que vous vous déconnectiez. Lorsque vous vous reconnectez, la liste s’affiche en fonction de ce paramètre.
   >* Les résultats d’un regroupement s’affichent toujours développés après que l’on y a accédé à partir d’un élément de graphique.

1. Cliquez sur **Terminé** si vous souhaitez enregistrer vos modifications et continuer à modifier le regroupement ou le rapport.
1. Cliquez sur **Enregistrer le regroupement** dans une liste ou **Enregistrer et Fermer** pour enregistrer votre rapport.
