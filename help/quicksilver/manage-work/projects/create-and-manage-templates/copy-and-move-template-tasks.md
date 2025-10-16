---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copier et déplacer les tâches du modèle
description: Vous pouvez copier ou déplacer une tâche de modèle dans le même modèle ou dans un autre modèle.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '2090'
ht-degree: 94%

---

# Copier et déplacer les tâches du modèle

Vous pouvez copier une tâche de modèle vers un autre modèle ou la déplacer vers un autre modèle ou à un autre endroit du même modèle.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérez les autorisations d’un modèle.</p> <p>Vous ne pouvez pas partager une tâche de modèle.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template.</p> <p>You cannot share a template task.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Considérations relatives à la copie ou au déplacement des tâches de modèle

Tenez compte des points suivants lorsque vous copiez des tâches de modèle :

* Les informations suivantes ne sont pas transférées à la tâche copiée :

   * Jalons

* Vous pouvez choisir de copier certains éléments associés à la tâche de modèle dans la tâche copiée au cours du processus de copie. Cependant, par défaut, les objets suivants ne sont pas transférés vers la tâche copiée :

   * Commentaires des utilisateurs et des utilisatrices

* Les formulaires personnalisés sont copiés avec la tâche de modèle lorsque vous copiez une tâche de modèle. Les informations contenues dans les champs personnalisés ne sont transférées dans la nouvelle tâche de modèle que si vous choisissez de copier les données personnalisées.

* Les éléments suivants sont transférés par défaut dans la tâche de modèle copiée :

   * Sous-tâches

Tenez compte des éléments suivants lorsque vous déplacez des tâches de modèle :

* Les informations suivantes sont transférées par défaut dans la tâche déplacée :

   * Formulaires personnalisés et informations sur les champs personnalisés
   * Sous-tâches
   * Commentaires des utilisateurs et des utilisatrices

* Les informations suivantes ne sont pas transférées dans la tâche déplacée :

   * Jalons.

## Copier les tâches de modèle

Vous pouvez copier une seule tâche de modèle ou plusieurs tâches de modèle en masse.

1. Accédez au modèle qui contient la ou les tâches de modèle que vous souhaitez copier.
1. Cliquez sur **Tâches de modèle** dans le panneau de gauche.
1. Utilisez l’une des méthodes suivantes :
   * Cliquez sur le nom d’une tâche de modèle pour l’ouvrir.
   * Sélectionnez une ou plusieurs tâches de modèle dans la liste.
1. (Conditionnel) Cliquez sur le menu **Plus** ![Icône Plus](assets/more-icon.png) en haut de la liste des tâches de modèle ou à droite du nom de la tâche de modèle si vous avez ouvert la tâche, puis cliquez sur **Copier vers** ou **Copier**, selon l’emplacement depuis lequel vous accédez à l’option Copier.
La zone Copier la tâche de modèle s’affiche.
   ![Zone Copier la tâche de modèle](assets/copy-template-task-box-unshimmed.png)
1. (Facultatif) Renommez la tâche de modèle dans le champ **Nom de tâche de modèle**.

   >[!TIP]
   >
   >Ce champ est grisé et n’est pas modifiable lors de la copie de plusieurs tâches de modèle dans une liste. Si vous pointez sur le champ Nom de la tâche de modèle, une liste de toutes les tâches de modèle sélectionnées s’affiche.

1. Commencez à saisir le nom du **Modèle de destination** où vous souhaitez copier la tâche de modèle dans le champ **Sélectionner le modèle de destination**, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   Le nom du modèle actuel s’affiche par défaut. Si vous souhaitez copier la tâche de modèle dans le même modèle, ne modifiez pas ce champ.

   >[!TIP]
   >
   >Vous pouvez également commencer à taper le numéro de référence ou saisir l’ID du modèle. Cela peut vous aider à distinguer des modèles portant des noms identiques.

1. (Facultatif) Cliquez sur **Demander l’accès** pour demander l’accès au modèle de destination, si vous n’avez pas accès au modèle sélectionné.
1. (Facultatif) Continuez pour copier la tâche de modèle vers le modèle de destination sélectionné sans demander d’accès si vous avez le droit d’ajouter des tâches de modèle à l’une des tâches de modèle sur le modèle de destination.

1. Cliquez sur **Options** dans le panneau de gauche, puis désélectionnez les attributs de la tâche de modèle que vous ne souhaitez pas copier avec la tâche modèle. Toutes les options sont sélectionnées par défaut.

   >[!TIP]
   >
   >La désélection de **Tout sélectionner** désélectionne toutes les options.

   Désélectionnez les options suivantes pour ne pas les transférer à la tâche de modèle copiée. Le tableau suivant décrit ce qui se produit lorsque les options sont désélectionnées :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Sélectionner tout</td> 
      <td>Désélectionnez cette option pour supprimer toutes les informations de la tâche de modèle lorsque vous la copiez dans son nouvel emplacement. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Contrainte</td> 
      <td> <p>La contrainte de tâche de modèle est définie sur Aussi Tôt Que Possible ou Aussi Tard Que Possible en fonction du paramètre Mode de planification du modèle.</p> <p> Lorsque cette option est sélectionnée, la contrainte actuelle de la tâche de modèle est transférée à la tâche de modèle copiée. </p> 
      <p><b>NOTE</b>

   Lors de la copie d’une tâche de modèle avec des contraintes de date dans un autre modèle et si les dates de contrainte de la tâche de modèle sont en dehors des dates du nouveau modèle, soit la contrainte de la tâche de modèle devient Aussi Tôt Que Possible ou Aussi Tard Que Possible, soit les dates de début ou de fin prévues des modèles sont ajustées.

   Vous trouverez ci-dessous des exemples de contraintes spécifiques aux dates :
   <ul>
      <li> Il Faut Commencer Le</li>
      <li> Il Faut Finir Le</li>
      <li> Commencer Au Plus Tôt</li>
      <li> Commencer Au Plus Tard</li>
      </ul>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td> <p>Toutes les affectations sont supprimées de la tâche de modèle. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processus d’approbation</td> 
      <td>Tous les processus d’approbation sont supprimés de la tâche de modèle.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Toutes les tâches antérieures</td> 
      <td> <p>Cela signifie que les dépendances ne seront pas reportées sur les tâches de modèle copiées. </p> <p>Lorsque cette option est sélectionnée, les tâches antérieures au sein du groupe de tâches de modèle copié sont conservées, les autres sont supprimées.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Données personnalisées</td> 
      <td> <p>Les valeurs des champs personnalisés sont effacées et les formulaires personnalisés sont transférés dans la tâche de modèle copiée. </p> <p>Lorsque cette option est sélectionnée, les formulaires et les valeurs des champs personnalisés sont transférés dans la tâche de modèle copiée. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informations financières</td> 
      <td>Les informations financières de la tâche de modèle copiée sont supprimées et Workfront met à jour le Type de coût de la tâche de modèle en Aucun coût et le Type de revenu de la tâche de modèle en Non facturable.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>Les documents joints à la tâche de modèle ne sont pas transférés à la tâche de modèle copiée. Il s’agit notamment des versions, des épreuves et des documents associés.</p> <p><b>NOTE</b></p>

   <p>Les approbations de documents suivent un processus distinct. Les approbations de documents ne peuvent jamais être copiées lorsqu’une tâche de modèle est copiée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Les rappels de la tâche de modèle ne sont pas transférés à la tâche de modèle copiée. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td>Les dépenses enregistrées sur la tâche de modèle ne sont pas transférées à la tâche de modèle copiée. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Facultatif) Cliquez sur **Sélectionner un parent** dans le panneau de gauche, puis sélectionnez la tâche de modèle dans le modèle de destination qui doit devenir le parent de la tâche de modèle copiée.

   >[!TIP]
   >
   >Lors de la sélection pour copier plusieurs tâches de modèle dans une liste, tous les tâches de modèle sélectionnées deviennent les enfants du parent sélectionné et sont ajoutées après les tâches enfants existantes.

   Sélectionnez un parent en effectuant l’une des opérations suivantes :

   * Dans la liste des tâches de modèle, sélectionnez l’un des parents dans le plan du modèle.
   * Cliquez sur l’icône de recherche ![icône de recherche](assets/search-icon.png) et recherchez une tâche de modèle parent par son nom.

   La tâche de modèle doit apparaître dans la liste.

1. Sélectionnez la case d’option du parent une fois que vous l’avez trouvée.

   Si vous ne sélectionnez pas de tâche de modèle parent, les tâches de modèle sont copiées en tant que tâches de modèle principales plutôt que sous-tâches et elles sont placées à la fin de la liste des tâches de modèle sur le modèle de destination.

1. Cliquez sur **Copier la tâche de modèle**.

   Les tâches de modèle copiées se trouvent maintenant sur le modèle spécifié et sont soit des sous-tâches de la tâche de modèle parent sélectionnée, soit les dernières tâches de modèle sur le modèle.


## Déplacer les tâches de modèle

Vous pouvez déplacer une tâche de modèle vers une autre tâche du même modèle ou vers un autre modèle. Vous pouvez déplacer une ou plusieurs tâches de modèles, en bloc.

1. Accédez au modèle qui contient la ou les tâches de modèle que vous souhaitez déplacer.
1. Cliquez sur **Tâches de modèle** dans le panneau de gauche.
1. Utilisez l’une des méthodes suivantes :
   * Cliquez sur le nom d’une tâche de modèle pour l’ouvrir.
   * Sélectionnez une ou plusieurs tâches de modèle dans la liste.
1. (Conditionnel) Cliquez sur le menu **Plus** ![Icône Plus](assets/more-icon.png) en haut de la liste des tâches de modèle ou à droite du nom de la tâche de modèle si vous avez ouvert la tâche, puis cliquez sur **Déplacer vers** ou **Déplacer**, selon l’endroit où vous accédez à l’option Déplacer.
La zone Déplacer la tâche de modèle s’ouvre.
   ![Déplacer la zone de tâche de modèle](assets/move-template-task-box-unshimmed.png)

1. (Facultatif) Renommez la tâche de modèle dans le champ **Nom de la tâche de modèle**.

   >[!TIP]
   >
   >Ce champ est grisé et n’est pas modifiable lors de la sélection pour déplacer plusieurs tâches de modèle dans une liste. Si vous pointez sur le champ Nom de la tâche de modèle, une liste de toutes les tâches de modèle sélectionnées s’affiche.

1. Commencez à taper le nom du **Modèle de destination** où vous souhaitez déplacer la tâche de modèle dans le champ **Sélectionner le modèle de destination**, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   >[!TIP]
   >
   >Vous pouvez également commencer à taper le numéro de référence ou saisir l’ID du modèle. Cela peut vous aider à distinguer des modèles portant des noms identiques.

1. (Le cas échéant) Cliquez sur **demander un accès** pour demander l’accès au modèle, si vous n’avez pas accès au modèle de destination.
1. (Le cas échéant) Continuez à déplacer la tâche de modèle vers le modèle de destination sélectionné sans demander d’accès si vous avez accès à l’ajout de tâches de modèle pour l’une des tâches de modèle sur le modèle de destination.

1. Cliquez sur **Options** dans le panneau de gauche, puis décochez les attributs de la tâche de modèle que vous ne souhaitez pas copier avec la tâche de modèle. Toutes les options sont sélectionnées par défaut.

   >[!TIP]
   >
   >* La section Options n’est disponible qu’après avoir sélectionné un modèle de destination.
   >* Le fait de décocher de **Sélectionner tout** désélectionne toutes les options.

   Décochez l’une des options suivantes pour ne pas transférer les informations à la tâche de modèle déplacée. Le tableau suivant décrit ce qui se produit lorsque les options sont désélectionnées :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Sélectionner tout</td> 
      <td>Décochez cette option pour supprimer toutes les informations de la tâche de modèle lorsque vous la déplacez vers son nouvel emplacement. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Contrainte</td> 
      <td> <p>La contrainte de tâche de modèle est définie sur Aussi Tôt Que Possible ou Aussi Tard Que Possible en fonction du paramètre Mode de planification du modèle.</p> <p> Lorsque cette option est sélectionnée, la contrainte actuelle de la tâche de modèle est transférée à la tâche de modèle déplacée. </p>

   <p><b>NOTE</b>

   Lors du déplacement d’une tâche de modèle avec des contraintes de date spécifiques vers un autre modèle et si les dates de contrainte de la tâche de modèle sont en dehors des dates du nouveau modèle, soit la contrainte de la tâche de modèle devient Aussi tôt que possible ou Aussi tard que possible, soit les dates de début ou de fin planifiées des modèles sont ajustées.

   Vous trouverez ci-dessous des exemples de contraintes spécifiques aux dates :
   <ul>
      <li> Démarré le</li>
      <li> Il Faut Finir Le</li>
      <li> Commencer Au Plus Tôt</li>
      <li> Commencer Au Plus Tard</li>
      </ul>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Affectations</td> 
      <td> <p>Toutes les affectations sont supprimées de la tâche de modèle. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Processus d’approbation</td> 
      <td>Tous les processus d’approbation sont supprimés de la tâche de modèle.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Toutes les tâches antérieures</td> 
      <td> <p>Cela signifie que les dépendances ne seront pas transférées avec les tâches de modèle déplacées. </p> <p>Lorsque cette option est sélectionnée, les tâches antérieures au sein du groupe de tâches de modèle déplacées sont conservées, les autres sont supprimées.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Données personnalisées</td> 
      <td> <p>Les valeurs des champs personnalisés sont effacées et les formulaires personnalisés sont transférés avec la tâche de modèle déplacée. </p> <p>Lorsque cette option est sélectionnée, les formulaires et les valeurs des champs personnalisés sont transférés avec la tâche de modèle déplacée. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informations financières</td> 
      <td>Les informations financières de la tâche de modèle déplacée sont supprimées et Workfront met à jour le type de coût de la tâche de modèle sur Aucun coût et le type de revenu de la tâche de modèle sur Non facturable.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td> <p>Les documents attachés à la tâche de modèle ne sont pas transférés avec la tâche de modèle déplacée. Il s’agit notamment des versions, des épreuves et des documents associés.</p>

   <p><b>NOTE</b></p>

   <ul><li>
      <p>Les approbations de documents suivent un processus distinct. Les approbations de documents ne peuvent jamais être déplacées avec une tâche de modèle.</p> </li>
      <li>Si vous choisissez de ne pas déplacer les documents avec la tâche de modèle, les documents sont supprimés et placés dans la corbeille pendant 30 jours. Un administrateur ou une administratrice peut les restaurer sur la tâche de modèle déplacée.

   Si la tâche de modèle est supprimée après avoir été déplacée, les documents restaurés seront placés dans la zone Documents de la page utilisateur de l’administrateur ou administratrice qui les a restaurés. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Les rappels de la tâche de modèle ne sont pas transférés à la tâche de modèle déplacée. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td>Les dépenses enregistrées sur la tâche de modèle ne sont pas transférées avec la tâche de modèle déplacée. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Facultatif) Cliquez sur **Sélectionner le parent** dans le panneau de gauche, puis sélectionnez la tâche de modèle dans le modèle de destination qui doit devenir le parent de la tâche de modèle déplacée.

   >[!TIP]
   >
   >Lors de la sélection pour déplacer plusieurs tâches de modèle dans une liste, toutes les tâches de modèle sélectionnées deviennent les enfants du parent sélectionné et sont ajoutées après les tâches enfants existantes.

   Sélectionnez un parent en effectuant l’une des opérations suivantes :

   * Dans la liste des tâches de modèle, sélectionnez l’un des parents dans le plan du modèle.
   * Cliquez sur l’icône de recherche ![icône de recherche](assets/search-icon.png) et recherchez une tâche de modèle parent par son nom.

   La tâche de modèle doit apparaître dans la liste.

1. Sélectionnez la case d’option du parent une fois que vous l’avez trouvée.

   Si vous ne sélectionnez pas de tâche de modèle parent, les tâches de modèle sont déplacées en tant que tâches de modèle principales plutôt que sous-tâches, et elles sont placées à la fin de la liste des tâches de modèle sur le modèle de destination.

1. Cliquez sur **Déplacer la tâche de modèle**.

   Les tâches de modèle déplacées se trouvent maintenant sur le modèle spécifié et sont soit des sous-tâches de la tâche du modèle parent sélectionné, soit les dernières tâches du modèle.
