---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Créer et modifier des modèles de projet de groupe
description: Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et utiliser des modèles de projet associés au groupe et à l’un de ses sous-groupes.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 11%

---

# Créer et modifier des modèles de projet de groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et utiliser des modèles de projet associés au groupe et à l’un de ses sous-groupes.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs ou administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de groupe pour le groupe ou un administrateur ou une administratrice de Workfront. Pour plus d’informations, consultez les sections <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à une personne</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher l’accès ou une version ultérieure sur les modèles que vous souhaitez afficher et utiliser</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir votre plan ou type de licence, contactez l’administration de Workfront.

## Affichage, utilisation et création de modèles pour votre groupe à partir de la zone Groupes

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez créer ou modifier des modèles.
1. Dans le panneau de gauche, cliquez sur **Modèles** pour répertorier les modèles associés au groupe et aux sous-groupes qu’il peut avoir.

   Vous devez disposer de l’accès Affichage à un modèle pour l’afficher dans cette liste. Pour plus d’informations sur cet accès, voir [Accorder l’accès aux modèles](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ajouter un modèle</td> 
      <td> <p>Cliquez sur <strong>Nouveau modèle</strong>, puis configurez-le à l’aide des options disponibles. Pour plus d’informations sur ces options, voir <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Création d’un modèle de projet</a>.</p> <p>Le modèle est automatiquement associé au groupe.</p> <p>Pour plus d’informations sur la manière dont les préférences de groupe s’appliquent aux nouveaux modèles, voir <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Comment les préférences s’appliquent aux modèles et aux tâches de modèle</a> dans cet article.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifier un ou plusieurs modèles</td> 
      <td> <p>Sélectionnez au moins un modèle, cliquez sur l’icône Modifier <img src="assets/edit-icon.png">, puis utilisez l’une des options disponibles pour le configurer. Pour plus d’informations sur ces options, voir <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Modifier les modèles de projet</a>.</p> <p>L’icône Modifier n’est disponible que si vous avez accès à l’option Modifier pour tous les modèles que vous sélectionnez. Pour plus d’informations sur cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Accorder l’accès aux modèles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer un ou plusieurs modèles</td> 
      <td> <p>Sélectionnez au moins un modèle, puis cliquez sur l’icône Supprimer <img src="assets/delete.png">.</p> <p>Cette icône n’est disponible que si vous avez accès à l’option Modifier pour tous les modèles que vous sélectionnez. Pour plus d’informations sur cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Accorder l’accès aux modèles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partage d’un ou de plusieurs modèles</td> 
      <td> <p>Sélectionnez au moins un modèle, cliquez sur l’icône Partager <img src="assets/share-icon.png">, puis sur l’une des options suivantes dans le menu déroulant :</p> 
       <ul> 
        <li> <p><strong>Modèle</strong> : dans la zone <strong>Accès au modèle</strong> qui s’affiche, ajoutez des noms pour spécifier qui vous souhaitez avoir accès au modèle lui-même.</p> <p>Pour plus d’informations, reportez-vous à la section <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Partager un modèle</a> de l’article <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Partager des modèles de projet</a>.</p> </li> 
        <li><strong>Projet</strong> : dans la zone <strong>Accès au projet</strong> qui s’affiche, ajoutez des noms pour spécifier qui vous souhaitez avoir accès aux projets créés à partir du modèle.</li> 
       </ul> <p>L’icône Partager n’est disponible que si vous avez accès à l’ensemble des modèles que vous sélectionnez. Pour plus d’informations sur cet accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Accorder l’accès aux modèles</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exporter la liste des modèles</td> 
      <td>Cliquez sur <strong>Export</strong> <img src="assets/export.png">, puis sélectionnez le format de fichier souhaité pour la liste exportée.</td> 
     </tr> 
    </tbody> 
   </table>

## Comment les préférences s’appliquent aux modèles et aux tâches de modèle {#how-preferences-apply-to-templates-and-template-tasks}

Lorsque vous créez un modèle de projet, les paramètres répertoriés dans les tableaux ci-dessous sont automatiquement configurés par une préférence de projet ou de tâche corrélée.

>[!NOTE]
>
>Un projet ou une préférence de tâche au niveau du groupe ou du système affecte un modèle de projet, selon que vous l’avez associé à un groupe lors de sa création.
>
>Si vous l’avez associée à un groupe, la préférence de niveau groupe prend effet. Cela se produit dans les scénarios suivants :
>
>* Vous créez le modèle à partir de la zone Groupes, comme expliqué dans cet article.
>* Vous spécifiez un groupe lors de la création du modèle à l’aide d’un fichier de démarrage rapide.
>* Vous spécifiez un groupe lors de la création du modèle à l’aide de l’API
>
>Si vous n’avez pas associé le nouveau modèle à un groupe, la préférence de niveau système prend effet. Cela se produit dans les scénarios ci-dessous. (Si vous affectez par la suite un groupe à la tâche de modèle ou de modèle, les préférences du groupe ne l’affectent pas.)
>
>* Vous créez le modèle à partir de la zone Modèles .
>* Vous ne spécifiez pas de groupe lors de la création du modèle à l’aide d’un fichier de démarrage rapide.
>* Vous ne spécifiez pas de groupe lors de la création du modèle à l’aide de l’API
>

* [ Paramètres du modèle de projet configurés par les préférences du projet et de la tâche ](#project-template-settings-configured-by-project-and-task-preferences)
* [Paramètres des tâches de modèle configurés par les préférences de tâche](#template-task-settings-configured-by-task-preferences)

### Paramètres du modèle de projet configurés par les préférences du projet et de la tâche {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Méthode d'indice de performances</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe "Méthode d’index de performance" si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type de condition</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe "Définissez automatiquement la condition du projet en fonction de l’état de progression" si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Planification depuis</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe "Planifier à partir de" si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Intervalle d’expiration de l’utilisateur</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe "Délai d’utilisation" si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type de mise à jour</p> </td> 
   <td> <p>Configuré par la préférence de projet au niveau du groupe "Les chronologies de projet seront automatiquement recalculées" si vous associez le nouveau modèle à un groupe ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Accès aux paramètres de section</p> </td> 
   <td> <p>Configuré par les préférences de tâche au niveau du groupe dans la section "Accès" si vous associez le nouveau modèle à un groupe, ou la même préférence de projet au niveau du système si vous ne le faites pas.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur les préférences de projet répertoriées dans ce tableau, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Pour plus d’informations sur la tâche et les préférences de problème, voir [Configuration des préférences de tâche à l’échelle du système et de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Si vous modifiez le groupe associé à un modèle de projet existant, les paramètres du modèle restent les mêmes.
>* Si vous déplacez une tâche de modèle existante vers un autre modèle, les paramètres suivants restent inchangés dans la tâche de modèle, quel que soit le groupe associé au nouveau modèle :>
>   * Type de durée
>   * Type de revenus
>   * Type de coût
>
>  Cependant, la tâche de modèle est affectée par le paramètre &quot;Lorsqu’une personne est affectée à une tâche&quot; sur le nouveau modèle. Pour plus d’informations, reportez-vous à la section [Accès](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) dans l’article [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Lorsqu’un administrateur enregistre un projet en tant que modèle, tous les paramètres du modèle sont hérités du projet, y compris le groupe .
>
>  Lorsqu’un administrateur convertit une tâche ou un problème en projet à l’aide d’un modèle, tous les paramètres du modèle sont déterminés par ce qui a déjà été enregistré sur le modèle.
>

### Paramètres des tâches de modèle configurés par les préférences de tâche {#template-task-settings-configured-by-task-preferences}

Lorsque vous créez une tâche de modèle, certains de ses paramètres sont automatiquement configurés par une préférence de tâche correspondante. Ces paramètres sont répertoriés dans le tableau ci-dessous.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Type de durée </p> </td> 
   <td> <p>Configuré par la préférence de tâche au niveau du groupe "Type de durée" si vous associez le modèle à un groupe, ou la même tâche au niveau du système et si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type de revenus</p> </td> 
   <td> <p>Configuré par la préférence de tâche au niveau du groupe "Type de chiffre d’affaires" si vous associez le modèle à un groupe, ou la même tâche au niveau du système et la même préférence d’émission si vous ne le faites pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type de coût </p> </td> 
   <td> <p> Configuré par la préférence de tâche au niveau du groupe "Type de coût" si vous associez le modèle à un groupe, ou la même tâche au niveau du système et si vous ne le faites pas.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur les préférences de tâche répertoriées dans ce tableau, voir [Configuration des préférences de tâche à l’échelle du système et de problème](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
