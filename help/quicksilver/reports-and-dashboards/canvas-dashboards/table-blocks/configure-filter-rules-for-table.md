---
title: Filtrer un tableau dans la zone de travail de reporting
description: Filtrer un tableau dans la zone de travail de reporting
hidefromtoc: true
hide: true
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 9%

---

# Filtrer un tableau dans la zone de travail de reporting

Après avoir ajouté un bloc de tableau à un rapport, vous pouvez configurer des filtres pour limiter les informations affichées dans le tableau.

Une règle de filtre comporte 3 composants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">champ</td> 
   <td> <p>Le champ contenant les informations selon lesquelles vous souhaitez filtrer votre tableau .</p> </td> 
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

**Exemple :** Si vous souhaitez limiter les résultats de votre rapport afin d’afficher uniquement les projets appartenant à Jane Doe, vous pouvez créer une règle de filtrage avec le champ &quot;Propriétaire du projet&quot;, l’opérateur &quot;Égal à&quot; et la valeur &quot;Jane Doe&quot;.

Vous pouvez également afficher uniquement les projets auxquels un propriétaire de projet est affecté, avec le champ &quot;Propriétaire du projet&quot; et l’opérateur &quot;N’est pas vierge&quot;.

## Conditions préalables

Avant de commencer, vous devez vous inscrire à la version bêta du canevas de création de rapports. Pour plus d’informations, reportez-vous à la section [Présentation du canevas de rapports bêta : présentation](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configuration des règles de filtrage pour un tableau

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Création de rapports**.

1. Cliquez sur **Nouveau rapport**.

   Ou

   Accédez à un rapport existant, cliquez sur l&#39;icône **Plus de menu** ![](assets/more-icon.png) dans l&#39;en-tête du rapport, puis sélectionnez **Modifier**.

1. Pour regrouper des lignes sur un nouveau tableau, faites glisser ou double-cliquez sur un bloc de tableau sur la zone de travail.

   Ou

   Pour regrouper des lignes sur une table existante, cliquez sur l&#39;icône **Modifier** ![](assets/edit-icon.png) dans l&#39;en-tête du tableau.

1. Dans le panneau de droite, localisez le champ selon lequel vous souhaitez filtrer votre tableau, puis faites-le glisser vers la section Filtre .

   Un jeu de règles de filtrage s’affiche avec le nom du champ que vous avez sélectionné.

1. Sélectionnez l’opérateur de votre choix dans le menu déroulant :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Égal À</strong> </td> 
      <td> <p>Cela ne renvoie qu’une correspondance exacte de la valeur recherchée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Not Equal To</strong> </td> 
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
      <td role="rowheader"><strong>Est Inférieur À</strong> </td> 
      <td> <p>Cela permet de rechercher tous les résultats dont la valeur est inférieure à ce qui est entré, sans inclure la valeur saisie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est Inférieur Ou Égal À</strong> </td> 
      <td> <p>Cela permet de rechercher tous les résultats dont la valeur est inférieure ou égale à la valeur saisie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est Supérieur À</strong> </td> 
      <td> <p>Cela permet de rechercher tous les résultats dont la valeur est supérieure à la valeur saisie, sans inclure la valeur saisie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Est Supérieur Ou Égal À</strong> </td> 
      <td> <p>Cela permet de rechercher tous les résultats avec des valeurs supérieures ou égales à la valeur saisie.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Entre</strong> </td> 
      <td> <p>Fournit 2 valeurs de champ requises et effectue des recherches pour tous les résultats compris dans la plage des deux champs, y compris les valeurs saisies.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contient</strong> </td> 
      <td> <p>Cela permet de rechercher le texte spécifié dans toute une chaîne de texte.</p> <p>Par exemple, l’utilisation de "Contains Inf" (Contient Inf) capture tout ce qui contient "Inf" (Inf) ou "inf" (Inf), par exemple).</p> <p>Remarque : Adobe Workfront recherche l’intégralité du mot ou de l’expression saisi pour chaque règle de filtre. Par exemple, si vous recherchez des champs dont le nom contient l’expression "nouveau projet", Workfront n’affiche pas les projets dont le nom contient uniquement "nouveau" ou "projet", ni les expressions qui contiennent des mots supplémentaires entre ceux-ci, tels que "nouveau projet principal". Le filtre recherche uniquement les projets dont le nom contient exactement l’expression "nouveau projet".</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ne contient pas</strong> </td> 
      <td> <p>Cela filtre les éléments qui ne comportent pas de texte spécifié.</p> <p>Par exemple, "ne contient pas inf" renvoie les champs dont le nom ne contient pas "Inf" ou "inf".</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Saisissez la dernière valeur pour terminer la règle de filtrage, en fonction de l’opérateur que vous avez sélectionné.

   >[!NOTE]
   >
   >Les valeurs saisies ici sont **non** sensibles à la casse.

1. (Facultatif) Pour ajouter une autre règle de filtre à votre jeu de règles, procédez comme suit :

   1. Faites glisser un autre champ vers la zone **Déposez pour ajouter une autre règle** dans la section Filtres sous votre autre règle.
   1. Répétez les étapes 4 à 6.
   1. Dans la liste déroulante des opérateurs située à gauche de la nouvelle règle, sélectionnez **AND** ou **OR**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>ET</p> </td> 
         <td> <p>Lorsque vous associez des règles de filtrage ou des ensembles de règles à l’opérateur AND, vous indiquez que vous souhaitez que toutes les règles au même niveau soient respectées.</p> <p>Par défaut, les instructions d’un filtre sont jointes par l’opérateur AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>OU</p> </td> 
         <td> <p>Lorsque vous associez des règles de filtrage ou un jeu de règles à l’opérateur OU, vous indiquez que vous souhaitez <strong>au moins</strong> qu’une règle, ou un jeu de règles, soit à ce niveau soit respectée.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >Les opérateurs ET et OU au même niveau (connexion de plusieurs règles au sein d’un jeu de règles ou d’ensembles complets de règles) correspondent toujours. Par exemple, si vous changez l’opérateur entre deux règles au sein d’un jeu de règles, tous les autres opérateurs de ce jeu de règles changent automatiquement pour correspondre.

1. (Conditionnel) Pour ajouter un jeu de règles de filtrage supplémentaire, procédez comme suit :

   1. Faites glisser le champ que vous souhaitez ajouter à la zone **Ajouter un jeu de règles** sous vos autres jeux de règles de filtre.
   1. Répétez les étapes 4 à 7.
   1. Dans la liste déroulante des opérateurs située à gauche du nouveau jeu de règles, sélectionnez **AND** ou **OR**. Ces opérateurs fonctionnent de la même manière que ceux répertoriés à l’étape 7, mais s’appliquent à l’ensemble des ensembles de règles, par opposition aux règles individuelles d’un ensemble.****
