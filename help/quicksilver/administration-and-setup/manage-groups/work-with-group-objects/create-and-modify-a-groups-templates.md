---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Création et modification de modèles de projet d’un groupe
description: Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher et travailler avec les modèles de projet associés au groupe et à n’importe lequel de ses sous-groupes.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: 10780ff51d5b1d9d73cb0a6fb0982abc320b0313
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 85%

---

# Créer et modifier les modèles de projet d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher et travailler avec les modèles de projet associés au groupe et à n’importe lequel de ses sous-groupes.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr>
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr>
  <tr> 
   <td>Autorisations d’objet</td>
   <td>Accès en affichage ou de niveau supérieur pour les modèles que vous souhaitez afficher et utiliser.</td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher, utiliser et créer des modèles pour votre groupe à partir de la zone Groupes

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez créer ou modifier des modèles.
1. Dans le panneau de gauche, cliquez sur **Modèles** pour afficher la liste des modèles associés au groupe et à ses éventuels sous-groupes.

   Vous devez avoir accès à l’affichage d’un modèle pour le voir dans cette liste. Pour plus d’informations sur cet accès, voir [Accorder l’accès aux modèles](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ajouter un modèle</td> 
      <td> <p>Cliquez sur <strong>Nouveau modèle</strong>, puis configurez-le à l’aide des options disponibles. Pour plus d’informations sur ces options, voir <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Créer un modèle de projet</a>.</p> <p>Le modèle est automatiquement associé au groupe.</p> <p>Pour plus d’informations sur la manière dont les préférences de groupe s’appliquent aux nouveaux modèles, voir <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Comment les préférences s’appliquent aux modèles et aux tâches des modèles</a> dans cet article.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifier un ou plusieurs modèles</td> 
      <td> <p>Sélectionnez au moins un modèle, cliquez sur l’icône Modifier <img src="assets/edit-icon.png">, puis utilisez l’une des options disponibles pour le configurer. Pour plus d’informations sur ces options, voir <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modifier les modèles de projet</a>.</p> <p>L’icône Modifier n’est disponible que si vous disposez de l’accès en modification à tous les modèles que vous sélectionnez. Pour plus d’informations sur cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Accorder l’accès aux modèles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un ou plusieurs modèles</td> 
      <td> <p>Sélectionnez au moins un modèle, puis cliquez sur l’icône Supprimer <img src="assets/delete.png">.</p> <p>Cette icône n’est disponible que si vous disposez de l’accès en modification à tous les modèles que vous sélectionnez. Pour plus d’informations sur cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Accorder l’accès aux modèles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partager un ou plusieurs modèles</td> 
      <td> <p>Sélectionnez au moins un modèle, cliquez sur l’icône Partager <img src="assets/share-icon.png">, puis cliquez sur l’une des options suivantes dans le menu déroulant :</p> 
       <ul> 
        <li> <p><strong>Modèle</strong> : dans la zone <strong>Accès au modèle</strong> qui s’affiche, ajoutez des noms pour spécifier qui doit avoir accès au modèle.</p> <p>Pour plus d’informations, voir la section <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Partager un modèle</a> dans l’article <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Partager des modèles de projet</a>.</p> </li> 
        <li><strong>Projet</strong> : dans la zone <strong>Accès au projet</strong> qui s’affiche, ajoutez des noms pour spécifier qui doit avoir accès aux projets créés à partir du modèle.</li> 
       </ul> <p>L’icône Partager n’est disponible que si vous disposez de l’accès partagé à tous les modèles que vous sélectionnez. Pour plus d’informations sur cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Accorder l’accès aux modèles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exporter la liste des modèles</td> 
      <td>Cliquez sur <strong>Exporter</strong> <img src="assets/export.png">, puis sélectionnez le format de fichier souhaité pour la liste à exporter.</td> 
     </tr> 
    </tbody> 
   </table>

## Comment les préférences s’appliquent aux modèles et aux tâches des modèles {#how-preferences-apply-to-templates-and-template-tasks}

Lorsque vous créez un modèle de projet, les paramètres énumérés dans les tableaux ci-dessous sont configurés automatiquement par une préférence de projet ou de tâche correspondante.

>[!NOTE]
>
>Une préférence de projet ou de tâche au niveau du groupe ou du système affecte un modèle de projet, selon que vous avez associé ou non le modèle à un groupe lors de sa création.
>
>Si vous l’avez associé à un groupe, c’est la préférence au niveau du groupe qui s’applique Cela se produit dans les cas suivants :
>
>* Vous créez le modèle à partir de la zone Groupes, comme expliqué dans cet article.
>* Vous spécifiez un groupe lorsque vous créez le modèle à l’aide d’un fichier Kickstart.
>* Vous spécifiez un groupe lorsque vous créez le modèle à l’aide de l’API.
>
>Si vous n’avez pas associé le nouveau modèle à un groupe, c’est la préférence de niveau système qui s’applique. Cela se produit dans les cas suivants. (Si vous affectez un groupe au modèle ou à la tâche de modèle plus tard, les préférences du groupe ne s’y appliqueront pas.)
>
>* Vous créez le modèle à partir de la zone Modèles.
>* Vous ne spécifiez pas de groupe lorsque vous créez le modèle à l’aide d’un fichier Kickstart.
>* Vous ne spécifiez pas de groupe lorsque vous créez le modèle à l’aide de l’API.
>

* [Paramètres du modèle de projet configurés par les préférences du projet et de la tâche](#project-template-settings-configured-by-project-and-task-preferences)
* [Paramètres de la tâche de modèle configurés par les préférences de la tâche](#template-task-settings-configured-by-task-preferences)

### Paramètres du modèle de projet configurés par les préférences du projet et de la tâche {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Méthode d'indice de performances</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe « Méthode d’indice de performances » si vous associez le nouveau modèle à un groupe, ou par la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type de condition</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe « Définir automatiquement la condition du projet en fonction du statut de progression » si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Planifier à partir de</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe « Planifier à partir de » si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Congés de l’utilisateur ou de l’utilisatrice</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe « Congés de l’utilisateur » si vous associez le nouveau modèle à un groupe ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type de mise à jour</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe « Les chronologies de projet seront automatiquement recalculées » si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Paramètres de la section Accès</p> </td> 
   <td> <p>Configuré par les préférences de tâche au niveau du groupe dans la section « Accès » si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur les préférences de projet répertoriées dans ce tableau, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Pour plus d’informations sur les préférences de tâche et de problème, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Si vous modifiez le groupe associé à un modèle de projet existant, les paramètres du modèle restent inchangés.
>* Si vous déplacez une tâche de modèle existante vers un autre modèle, les paramètres suivants restent inchangés dans la tâche de modèle, quel que soit le groupe associé au nouveau modèle :
>   * Type de durée
>   * Type de revenus
>   * Type de coût
>
>  Cependant, la tâche du modèle est affectée par le paramètre « Lorsqu’une personne est affectée à une tâche » sur le nouveau modèle. Pour plus d’informations, voir la section [Accès](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) dans l’article [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Lorsqu’un administrateur ou une administratrice enregistre un projet en tant que modèle, tous les paramètres du modèle sont hérités du projet, y compris le groupe.
>
>  Lorsqu’un administrateur ou une administratrice convertit une tâche ou un problème en projet à l’aide d’un modèle, tous les paramètres du modèle sont déterminés par ce qui est déjà enregistré sur le modèle.
>

### Paramètres de la tâche de modèle configurés par les préférences de la tâche {#template-task-settings-configured-by-task-preferences}

Lorsque vous créez une tâche de modèle, certains de ses paramètres sont configurés automatiquement par une préférence de tâche correspondante. Ces paramètres sont énumérés dans le tableau ci-dessous.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Type de durée </p> </td> 
   <td> <p>Configuré par la préférence de tâche au niveau du groupe « Type de durée » si vous associez le modèle à un groupe, ou par la même préférence de tâche et de problème au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type de revenus</p> </td> 
   <td> <p>Configuré par la préférence de tâche au niveau du groupe « Type de revenu » si vous associez le modèle à un groupe, ou par la même préférence de tâche et de problème au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type de coût </p> </td> 
   <td> <p> Configuré par la préférence de tâche au niveau du groupe « Type de coût » si vous associez le modèle à un groupe, ou par la même préférence de tâche et de problème au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur les préférences de tâche répertoriées dans ce tableau, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
