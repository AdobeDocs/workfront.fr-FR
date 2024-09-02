---
title: Filtrer un tableau dans la zone de travail des rapports
description: Filtrer un tableau dans la zone de travail des rapports
hidefromtoc: true
hide: true
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: f994a3f79df0594ea190a3dd77853c4b4ea89afb
workflow-type: ht
source-wordcount: '864'
ht-degree: 100%

---

# Filtrer un tableau dans la zone de travail des rapports

Après avoir ajouté un bloc de tableau à un rapport, vous pouvez configurer des filtres pour limiter les informations affichées dans le tableau.

Une règle de filtre comporte 3 composants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">champ</td> 
   <td> <p>Le champ contenant les informations selon lesquelles vous souhaitez filtrer votre tableau.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Opérateur</td> 
   <td> <p>La manière dont le filtre détermine quelles valeurs de champ sont incluses ou exclues de votre tableau. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Valeur</td> 
   <td> <p>Les valeurs du champ sélectionné qui sont évaluées en fonction de l’opérateur.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple :** si vous souhaitez limiter les résultats dans votre rapport afin d’afficher uniquement les projets appartenant à Jacques Dupond, vous pouvez créer une règle de filtrage avec le champ « Propriétaire du projet », l’opérateur « Égal à » et la valeur « Jacques Dupond ».

Vous pouvez également afficher uniquement les projets auxquels une personne propriétaire de projet est affectée, avec le champ « Propriétaire du projet » et l’opérateur « N’est pas vide ».

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta de la zone de travail de reporting. Pour plus d’informations, voir [Version bêta de la zone de travail des rapports : vue d’ensemble](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configurer des règles de filtrage pour un tableau

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.

1. Cliquez sur **Nouveau rapport**.

   Ou

   Accédez à un rapport existant, cliquez sur l’icône **Menu Plus** ![](assets/more-icon.png) dans l’en-tête du rapport, puis sélectionnez **Modifier**.

1. Pour regrouper des lignes sur un nouveau tableau, faites glisser ou double-cliquez sur un bloc du tableau sur la zone de travail.

   Ou

   Pour regrouper des lignes sur un tableau existant, cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) dans l’en-tête du tableau.

1. Dans le panneau de droite, localisez le champ selon lequel vous souhaitez filtrer votre tableau, puis faites-le glisser vers la section Filtre 

   Un jeu de règles de filtrage s’affiche avec le nom du champ que vous avez sélectionné.

1. Sélectionnez l’opérateur de votre choix dans le menu déroulant :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Est égal à</strong> </td> 
      <td> <p>Cela ne renvoie qu’une correspondance exacte de la valeur recherchée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est différent de</strong> </td> 
      <td> <p>Cela renvoie uniquement les résultats qui ne correspondent pas exactement à la valeur recherchée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est vide</strong> </td> 
      <td> <p>Le champ existe pour l’objet mais il n’a pas encore reçu de valeur.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>N’est pas vide</strong> </td> 
      <td> <p>Le champ pour lequel vous filtrez existe et a reçu une valeur.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est inférieur à</strong> </td> 
      <td> <p>Cela permet de rechercher tous les résultats dont la valeur est inférieure à ce qui est saisi, sans inclure la valeur saisie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est inférieur ou égal à</strong> </td> 
      <td> <p>Cela permet de rechercher tous les résultats dont la valeur est inférieure ou égale à la valeur saisie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est supérieur à</strong> </td> 
      <td> <p>Cela permet de rechercher tous les résultats dont la valeur est supérieure à la valeur saisie, sans inclure la valeur saisie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est supérieur ou égal à</strong> </td> 
      <td> <p>Cela permet de rechercher tous les résultats avec des valeurs supérieures ou égales à la valeur saisie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Entre</strong> </td> 
      <td> <p>Fournit 2 valeurs de champ requises et effectue des recherches pour tous les résultats compris dans la plage des deux champs, y compris les valeurs saisies.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contient</strong> </td> 
      <td> <p>Cela permet de rechercher le texte spécifié dans toute une chaîne de texte.</p> <p>Par exemple, l’utilisation de « Contains Inf » capture tout ce qui contient « Inf » ou « inf », tel que le mot « Infinité ».</p> <p>Remarque : Adobe Workfront recherche l’intégralité du mot ou de l’expression saisi pour chaque règle de filtre. Par exemple, si vous recherchez des champs dont le nom contient l’expression « nouveau projet », Workfront n’affiche pas les projets dont le nom contient uniquement « nouveau » ou « projet », ni les expressions qui contiennent des mots supplémentaires entre ceux-ci, tels que « nouveau projet principal ». Le filtre recherche uniquement les projets dont le nom contient exactement l’expression « nouveau projet ».</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ne contient pas</strong> </td> 
      <td> <p>Cette option filtre les éléments qui ne comportent pas le texte spécifié.</p> <p>Par exemple, « ne contient pas inf » renvoie les champs dont le nom ne contient pas « Inf » ou « inf ».</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Saisissez la dernière valeur pour terminer la règle de filtrage, en fonction de l’opérateur que vous avez sélectionné.

   >[!NOTE]
   >
   >Les valeurs saisies ici ne sont **pas** sensibles à la casse.

1. (Facultatif) Pour ajouter une autre règle de filtre à votre jeu de règles, procédez comme suit :

   1. Faites glisser un autre champ vers la zone **Déposer pour ajouter une autre règle** dans la section « Filtres » sous votre autre règle.
   1. Répétez les étapes 4 à 6.
   1. Dans la liste déroulante des opérateurs située à gauche de la nouvelle règle, sélectionnez **AND** ou **OR**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>ET</p> </td> 
         <td> <p>Lorsque vous associez des règles de filtrage ou des jeux de règles à l’opérateur AND, vous indiquez que vous souhaitez que toutes les règles au même niveau soient respectées.</p> <p>Par défaut, les instructions d’un filtre sont jointes par l’opérateur AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>OU</p> </td> 
         <td> <p>Lorsque vous associez des règles de filtrage ou un jeu de règles à l’opérateur OR, vous indiquez que vous souhaitez qu’<strong>au moins</strong> une règle (ou un jeu de règles) à ce niveau soit respectée.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >Les opérateurs AND et OR au même niveau (reliant plusieurs règles au sein d’un jeu de règles ou des jeux de règles entiers) correspondent toujours. Par exemple, si vous changez l’opérateur entre deux règles au sein d’un jeu de règles, tous les autres opérateurs de ce jeu de règles changent automatiquement pour correspondre.

1. (Le cas échéant) Pour ajouter un jeu de règles de filtrage supplémentaire, procédez comme suit :

   1. Faites glisser le champ à ajouter à la zone **Ajouter un jeu de règles** sous vos autres jeux de règles de filtrage.
   1. Répétez les étapes 4 à 7.
   1. Dans la liste déroulante des opérateurs située à gauche du nouveau jeu de règles, sélectionnez **AND** ou **OR**. Ces opérateurs fonctionnent de la même manière que ceux énumérés à l’étape 7, mais ils s’appliquent à des jeux de règles entiers plutôt qu’à des règles individuelles au sein d’un jeu.****
