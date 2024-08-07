---
title: Configurer une colonne de tableau dans la zone de travail de reporting
description: Configurer une colonne de tableau dans la zone de travail de reporting
hidefromtoc: true
hide: true
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 4%

---

# Configurer une colonne de tableau dans la zone de travail de reporting

Les colonnes d’un tableau peuvent être configurées pour l’affichage. Vous pouvez modifier les aspects suivants d&#39;une colonne :

* Nom
* Tri
* Modifier l’autorisation
* Texte de pointage
* Agrégation
* Mise en forme conditionnelle

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, reportez-vous à la section [Présentation du canevas de rapports bêta : présentation](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Modifier les colonnes d’un tableau

1. Accédez à un rapport existant, cliquez sur l&#39;icône **Plus de menu** ![](assets/more-icon.png) dans l&#39;en-tête du rapport, puis sélectionnez **Modifier**.
1. Dans l’en-tête du tableau du rapport, cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) .

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Si vous venez de créer le tableau et n’avez encore ajouté aucun champ, cliquez sur le bouton Editer situé au centre du tableau.

1. (Facultatif) Ajoutez, repositionnez ou supprimez des colonnes du tableau. Pour plus d’informations sur la modification des champs d’un tableau, voir [Ajout ou modification d’un bloc de tableau dans le canevas de création de rapports](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Ajouter une nouvelle colonne | Pour ajouter une colonne à un tableau, cliquez sur un champ du panneau **Champs** situé à droite de la page et faites-le glisser sur le tableau où vous souhaitez le placer, ou double-cliquez sur un champ pour l’ajouter en tant que colonne la plus à droite. |
   |---|---|
   | Déplacer une colonne | Pour réorganiser l’ordre des colonnes dans un tableau, cliquez sur le nom d’une colonne et faites-la glisser vers un nouvel emplacement. |
   | Suppression d’une colonne | Pour supprimer une colonne d’un tableau, cliquez sur la colonne à supprimer, puis sur le x situé à droite du nom de la colonne. |

   {style="table-layout:auto"}

1. Pour configurer une colonne, cliquez sur le nom de la colonne à modifier dans la ligne d’en-tête du tableau, puis sur l’un des onglets suivants du panneau de droite :

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Onglet Données</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Agrégé sur la base de</td>
      <td><p> Pour agréger (résumer dans l'en-tête) les informations d'une colonne, sélectionnez le type d'agrégation souhaité dans le menu déroulant <strong>Agrégat basé sur</strong> . Les options disponibles dépendent du type de données contenues dans la colonne.</p><p>Si vous utilisez des groupes dans le tableau, la valeur agrégée s’affiche dans la ligne de groupe au-dessus du nom de la colonne plutôt qu’à côté du nom de la colonne.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Format du champ</td>
      <td><p>(Disponible uniquement lorsque la colonne contient des données de date, de pourcentage, de devise ou d’heure, et non de texte.) Sélectionnez le format souhaité pour les données dans la liste déroulante <b>Format du champ</b>. Par exemple, vous pouvez afficher des signes de pourcentage après les chiffres d’une colonne ou modifier l’affichage des dates.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Le champ peut être modifié.</td>
      <td><span>Activez le <strong>champ modifiable</strong> si vous souhaitez permettre aux utilisateurs qui affichent le tableau de modifier le nom de la colonne.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Trier</strong></td>
      <td><p>Par défaut, le tableau est classé selon les données de sa colonne la plus à gauche, dans l’ordre croissant. Pour trier selon la colonne sélectionnée à la place, cliquez sur la flèche vers le bas en regard de <strong>Trier</strong>, puis cochez la case <b>Trier par cette colonne</b>. Vous pouvez ensuite sélectionner une direction <strong>Tri</strong> (valeurs ascendantes ou descendantes) et une <strong>Ordre de tri</strong> (priorité de tri relative de cette colonne par rapport aux autres colonnes de tri du tableau).</p><p>Vous pouvez répéter ce processus pour trier le tableau par 5 colonnes différentes au maximum. Assurez-vous que chaque colonne présente l’<strong>ordre de tri</strong> correct par rapport à toutes les nouvelles colonnes que vous sélectionnez pour le tri.</p><p>Remarque : Si vous supprimez une colonne sélectionnée pour trier un tableau et qu’une autre colonne est également sélectionnée pour le tri, cette colonne est utilisée pour trier le tableau dans l’ordre décroissant. Si aucune autre colonne n’est sélectionnée pour le tri, le tableau retourne à la valeur par défaut : le tri par sa première colonne.</p><p>Lorsque vous définissez une colonne pour trier le tableau, une petite zone s’affiche en regard du nom de la colonne avec un nombre indiquant la priorité relative de la colonne lors du tri du tableau (le tableau est trié en premier par 1, puis par 2, etc.) et une flèche pour indiquer si le sens du tri est croissant ou décroissant. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">Onglet Style</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Étiquette de colonne personnalisée</strong> </td> 
      <td>Saisissez un nouveau nom d’affichage pour la colonne (limite de 100 caractères).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher le texte de pointage</td> 
      <td> <p>Déterminez si vous souhaitez que le texte d’explication s’affiche lorsque quelqu’un survole le nom d’une colonne.</p> <p>Cette option est désactivée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texte de pointage</td> 
      <td>(Disponible uniquement lorsque l’option <strong>Afficher le texte de survol</strong> est activée.) Personnalisez le texte d’explication qui s’affiche lorsque quelqu’un survole le nom d’une colonne.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mise en forme conditionnelle</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Ajoutez <img src="assets/add-rule.png">, modifiez <img src="assets/edit-icon.png"> ou supprimez <img src="assets/delete.png"> une règle qui formate les cellules dans la colonne lorsque leurs valeurs répondent aux critères que vous spécifiez.</p> <p>Par exemple, vous pouvez créer une règle qui change la police du champ "État du projet" en violet gras lorsque la valeur de ce champ est égale à "Création".</p> <p>Vous pouvez également utiliser <b>Afficher une icône</b> pour ajouter une icône verte à chaque élément de la colonne ayant l’état "Actuel".</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Remarque : Si vous utilisez <strong>Afficher une icône</strong>, les autres options de formatage ne sont pas disponibles.</p> <p>Vous pouvez sélectionner <strong>Appliquer à la ligne entière</strong> si vous souhaitez que la mise en forme affecte la ligne entière d’une cellule qui respecte la condition de votre règle. Vous pouvez, par exemple, mettre en surbrillance les projets qui doivent être réalisés après une certaine date en appliquant une couleur d’arrière-plan jaune non seulement aux cellules de date de la colonne "Échéance le", mais également à toute la ligne où ces dates se produisent.</p> <p>Conseil : Lorsque vous ajoutez des options de formatage à une règle, le format de cellule obtenu s’affiche sous <strong>Aperçu</strong> au bas du panneau.</p> </li> 
        <li value="2">Lorsque vous avez terminé d’ajouter une règle, cliquez sur <strong>Enregistrer</strong>.</li> 
        <li value="3"> <p>(Facultatif) Cliquez sur <b>+ Ajouter une règle</b> pour ajouter des règles supplémentaires à la même colonne.</p> <p>Plusieurs règles de mise en forme conditionnelle dans un tableau sont appliquées dans l’ordre suivant :</p> 
         <ul> 
          <li> <p>Les règles qui s’appliquent à des lignes entières sont évaluées en premier, de gauche à droite pour chaque colonne, puis de haut en bas dans une colonne.</p> <p>Remarque : le formatage des lignes remplace le formatage conditionnel des cellules de cette ligne, même si, dans le cas contraire, elles respectent la condition de la règle d’une autre colonne.</p> </li> 
          <li> <p>Les autres règles sont évaluées ensuite, de haut en bas, car elles sont répertoriées dans le panneau de droite pour une colonne. Vous pouvez faire glisser <img src="assets/drag-object-icon.png"> règles enregistrées dans ce panneau pour modifier leur ordre.</p> <p>Remarque : les cellules sont formatées selon la première condition qu’elles remplissent et ne le seront pas davantage, même si elles répondent à d’autres conditions.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur la flèche **Revenir en arrière** dans le coin supérieur gauche de l’écran pour revenir à votre rapport.
