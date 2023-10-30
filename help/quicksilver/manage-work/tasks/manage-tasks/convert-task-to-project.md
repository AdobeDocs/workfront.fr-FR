---
product-area: projects
navigation-topic: manage-tasks
title: Convertir une tâche en projet
description: Lorsqu’une tâche d’un projet nécessite un effort plus important que celui initialement prévu, vous pouvez la convertir en projet.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: b781687b175167784367a2fdec158d97fb3fd6a4
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 2%

---

# Convertir une tâche en projet

Lorsqu’une tâche d’un projet nécessite un effort plus important que celui initialement prévu, vous pouvez la convertir en projet.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Affichage ou accès supérieur aux modèles lors de la conversion vers un projet à l’aide d’un modèle</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour une tâche</p> <p>Afficher les autorisations sur un modèle, en cas de conversion en projet à l’aide d’un modèle</p> <p>Après avoir créé le projet, vous disposez des autorisations de gestion pour le projet.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Observations relatives à la conversion de tâches en projets

* Vous pouvez convertir une tâche en projet vierge ou en projet à l’aide d’un modèle.
* La tâche d’origine est supprimée.
* Toutes les sous-tâches, les problèmes et les notes sont cumulés jusqu’au nouveau projet.
* Les documents, versions de document et BAT sont déplacés vers le nouveau projet.
* L’état et le pourcentage d’achèvement de toutes les sous-tâches et problèmes sont conservés.
* Les utilisateurs partagés de la tâche deviennent des utilisateurs partagés sur le projet.
* La date de début du projet est définie sur la date de début de la tâche.
* Le tableau suivant répertorie les informations du projet et indique s’il est transféré depuis le modèle ou de la tâche :

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Description</td> 
    <td> <p>La description de la tâche est transférée au nouveau projet. </p> <p> S’il n’existe aucune description de la tâche, la description du modèle est transférée au projet. </p> <p>Si le champ Description est vide à la fois pour la tâche et pour le modèle, le champ est vide sur le projet. </p> </td> 
    </tr> 
    <tr> 
    <td>Statut</td> 
    <td> État par défaut sélectionné pour le groupe sur le modèle. Si le modèle n’est pas associé au groupe, l’état du projet est défini sur l’état par défaut défini par l’administrateur Workfront dans la zone Préférences du projet de la section Configuration. Pour plus d’informations, voir <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Configuration des préférences de projet à l’échelle du système</a>

  Les scénarios suivants permettent de mettre à jour l’état du projet :
  <ul>
    <li> Si l’état de la tâche est "Nouveau", l’état du projet est défini sur "Planification".</li>
    <li> Si l’état de la tâche est "En cours", l’état du projet est défini sur "Actuel".</li>
    <li> Si l’état de la tâche est "Terminé", l’état du projet est défini sur "Terminé".</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>Priorité</td> 
    <td>Transfère de la tâche vers le projet, ou le transfère du modèle, si vous en utilisez un dans la conversion. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>L’URL de la tâche est transférée au nouveau projet. </p> <p> Si aucune URL n’est spécifiée dans la tâche, l’URL du modèle est transférée au projet. </p> <p>Si le champ URL est vide à la fois pour le problème et pour le modèle, le champ est vide sur le projet. </p> </td> 
    </tr> 
    <tr> 
    <td>Type de condition du projet</td> 
    <td>Transferts à partir du modèle.</td> 
    </tr> 
    <tr> 
    <td>Statut du projet</td> 
    <td>Correspond à la préférence par défaut au niveau du système, déterminée par l’administrateur Workfront dans la zone Configuration . Pour plus d’informations, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">Définir une condition personnalisée comme condition par défaut pour les projets</a>
    </td> 
    </tr> 
    <tr> 
    <td>Planifier à partir de</td> 
    <td>Transferts à partir du modèle.</td> 
    </tr> 
    <tr> 
    <td>Dates de projets</td> 
    <td> 
      <ul> 
      <li> <p><b>Date de début planifiée</b>: le temps de travail le plus proche basé sur l’heure de travail du planning du modèle doit être présélectionné, en fonction du fuseau horaire du planning du modèle. Ce champ est désactivé si le champ Planifier à partir de est défini sur À partir de la fin. </p> </li> 
      <li> <p><b>Date d’achèvement prévue</b>: le temps de travail le plus proche basé sur l’heure de travail du planning du modèle doit être présélectionné, en fonction du fuseau horaire du planning du modèle. Ce champ est désactivé si le champ Planifier à partir du est défini sur À partir du début. </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>Portfolio</td> 
    <td>Transferts à partir du modèle. Sinon, ce champ est vide.</td> 
    </tr> 
    <tr> 
    <td>Programme</td> 
    <td>Transferts à partir du modèle. Sinon, ce champ est vide.</td> 
    </tr> 
    <tr> 
    <td>Groupe</td> 
    <td><p> Les scénarios suivants existent :</p>
      <ul><li>Si un groupe est spécifié pendant la conversion, il devient le groupe du projet.</li>
      <li>Si vous effectuez une conversion vers un projet à l’aide d’un modèle et qu’un groupe est présent sur le modèle, et que vous ne spécifiez pas de groupe pendant la conversion, le groupe du modèle devient le groupe du nouveau projet.</li>
      <li> S’il n’y a aucun groupe sur le modèle et que vous ne spécifiez pas de groupe pendant la conversion, le groupe du projet du problème d’origine devient le groupe du nouveau projet.</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Entreprise</td>    
    <td>  Transferts à partir du modèle. Sinon, ce champ est vide.</td>

  </tr> 
    <tr> 
    <td>Propriétaire du projet</td> 
    <td>Transferts à partir du champ Propriétaire du modèle sur le modèle. Sinon, elle est définie sur l’utilisateur connecté qui effectue la conversion. </td> 
    </tr> 
    <tr> 
    <td>Sponsor du projet</td> 
    <td>Transferts à partir du champ Modèle de parrainage sur le modèle. Sinon, ce champ est vide.</td> 
    </tr> 
    <tr> 
    <td>Gestionnaire des ressources</td> 
    <td>Transferts à partir du modèle. Sinon, ce champ est vide.</td> 
    </tr> 
    <tr> 
    <td>Paramètres de la tâche</td> 
    <td>Transférer à partir du modèle.</td> 
    </tr> 
    <tr> 
    <td>Paramètres de l'événement</td> 
    <td>Transférer à partir du modèle. </td> 
    </tr> 
    <tr> 
    <td>Accès</td> 
    <td> <p>Transferts depuis la section Accès du modèle. </p> </td> 
    </tr> 
    <tr> 
    <td>Approbations</td> 
    <td>Transférer à partir du modèle. Les validations associées à la tâche sont supprimées lors de la conversion. </td> 
    </tr> 
  </tbody> 
  </table>


## Convertir une tâche en projet

1. Accédez à la tâche que vous souhaitez convertir en projet.
1. Cliquez sur le bouton **Plus** icon ![](assets/more-icon.png), puis **Convertir en projet**.
1. Choisissez l’une des options suivantes :

   * **Nouveau projet**
   * Un modèle dans le **Sélectionner parmi les modèles** section

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Cliquez sur **Continuer** sur la notification qui s’affiche.
1. Dans le **Convertir en projet** , spécifiez les éléments suivants :

   * **Nom**: attribuez un nom à votre projet. Le nom par défaut est le nom de la tâche.
   * (Facultatif) **Description**: décrivez l’objectif de ce projet.
   * (Facultatif et conditionnel) Si vous avez choisi de créer un projet à partir d’un modèle, mettez à jour les champs disponibles dans la variable **Convertir en projet** de la boîte de dialogue

     Pour plus d’informations sur la modification des champs des projets, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Pour mettre à jour les champs de la section Finance de la zone Convertir en projet , vous devez disposer de l’option Modifier l’accès aux données financières de votre niveau d’accès. Si vous disposez de l’option Afficher l’accès aux données financières dans votre niveau d’accès, toutes les informations financières du modèle sont transférées vers le nouveau projet et vous ne pouvez pas les modifier pendant que vous convertissez le problème. Pour plus d’informations, voir [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) et [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Facultatif) Ajoutez **Forms personnalisée** au nouveau projet.

     >[!TIP]
     >
     Si un formulaire personnalisé contenant plusieurs objets associés à la tâche est configuré pour être utilisé avec les tâches et les projets, toutes les informations enregistrées dans le formulaire sont conservées lorsque vous effectuez la conversion.
     >
     >
     Si vous utilisez un modèle pour la conversion et qu’un formulaire personnalisé associé au modèle contient un champ personnalisé également trouvé dans un formulaire personnalisé associé à la tâche, la valeur du champ de la tâche est utilisée pour le nouveau projet. Cependant, si le champ personnalisé est vide sur la tâche, la valeur du modèle est utilisée.

1. Cliquez sur **Enregistrer les modifications**.
