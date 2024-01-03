---
title: Personnalisation de la nouvelle page d’accueil à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Vous pouvez utiliser un modèle de mise en page pour configurer ce que voient les utilisateurs lorsqu’ils ouvrent la nouvelle page d’accueil.
author: Nolan
feature: System Setup and Administration
role: Admin
source-git-commit: 511d9b0b61870ccec13aa70c9d4d3232b3e60cd3
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 1%

---

# Personnalisation de la nouvelle page d’accueil à l’aide d’un modèle de mise en page

Vous pouvez utiliser un modèle de mise en page pour configurer ce que voient les utilisateurs lorsqu’ils ouvrent la nouvelle page d’accueil.

Vous pouvez configurer les éléments suivants :

* Les widgets qui s’affichent par défaut dans l’espace de travail et leur mise en page sur la page
* L’arrière-plan sélectionné
* Paramètres de widget spécifiques, notamment les filtres et les groupes disponibles pour les widgets Mes projets, Mes tâches et Mes problèmes, ainsi que leurs paramètres par défaut.

>[!IMPORTANT]
>
>Les choix de modèle de mise en page administrateur décrits sur cette page remplacent les choix de personnalisation de chaque utilisateur.
>
>Lors de l’enregistrement des modifications apportées à un modèle de mise en page, la nouvelle page d’accueil des utilisateurs de ce modèle est modifiée afin qu’elle corresponde au modèle de mise en page. Les sélections de widgets existantes sont alors transférées vers le bas de la page. Bien que les widgets sélectionnés par l’administrateur puissent être repositionnés et redimensionnés par un utilisateur, ils ne peuvent pas être supprimés.

Pour plus d’informations sur la nouvelle page d’accueil, voir [Prise en main du nouvel accueil](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

Pour plus d’informations sur la création de modèles de mise en page, voir [Création et gestion des modèles de mise en page](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Création et modification des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs pour que les modifications que vous avez apportées soient visibles par d’autres utilisateurs. Pour plus d’informations sur l’attribution d’un modèle de mise en page aux utilisateurs, voir [Affecter des utilisateurs à un modèle de mise en page](../use-layout-templates/assign-users-to-layout-template.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur système.
Pour les exécuter pour un groupe, vous devez être un responsable de ce groupe.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnalisation de la nouvelle page d’accueil à l’aide d’un modèle de mise en page

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow.png) under **Personnalisation des éléments affichés par les utilisateurs**, puis cliquez sur **Espace de travail**.

1. Dans les onglets qui s’affichent à droite, cliquez sur **Conception et mise en page** pour choisir et organiser des widgets et l’arrière-plan, ou **Paramètres du widget** pour gérer les paramètres de widgets individuels, tels que les filtres et les groupes disponibles.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Conception et disposition</td> 
      <td>
      <p>Sélectionnez les widgets qui seront présents dans les espaces de travail des utilisateurs, leur position et choisissez un arrière-plan. Notez que même si les utilisateurs ne peuvent pas supprimer les widgets sélectionnés, ils peuvent les déplacer et les redimensionner librement et ajouter des widgets supplémentaires.</p>
      <p>Cet onglet fonctionne essentiellement comme un petit nouvel espace de travail d’accueil. Il peut donc être personnalisé selon les étapes décrites dans la section <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Ajout, modification ou suppression de widgets dans la nouvelle page d’accueil</a>. Sélectionnez des widgets et organisez l’espace de travail comme vous le souhaitez pour les utilisateurs.</p>
      <p>Pour modifier l’arrière-plan, procédez comme suit : <b>Personnalisation de l’arrière-plan</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Prise en main du nouvel accueil</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Paramètres du widget</td> 
      <td>
      <p>Modifiez les paramètres de widgets individuels. Actuellement, seuls trois widgets sont pris en charge :</p>
      <ul>
        <li>Mes projets</li>
        <li>Mes tâches</li>
        <li>Mes problèmes</li>
      </ul>
      <p>Une fois que vous avez sélectionné le widget que vous souhaitez modifier, les options disponibles s’affichent à droite. Actuellement, ces options sont : <b>Filtres</b> et <b>Groupes</b>. Vous pouvez :</p>
      <ul>
        <li><b>Sélectionnez les filtres ou groupes qui seront disponibles pour les utilisateurs :</b><p>Cochez la case en regard de toutes les options de la liste que vous souhaitez que les utilisateurs puissent utiliser. Les options non cochées ne s’affichent pas pour les utilisateurs.</li></p>
        <li><b>Définissez un filtre ou un groupe par défaut pour le widget :</b><p>Passez la souris sur une option pour afficher un bouton permettant de définir cette option comme option par défaut pour les utilisateurs. La valeur par défaut actuelle comporte un badge bleu par défaut à sa droite.</li></p>
        <li><b>Ajoutez un filtre ou un groupe existant à la liste des options disponibles :</b><p>Cliquez sur le bouton représentant le signe plus au bas de chaque liste pour ajouter une option à cette liste. Notez que seuls les filtres ou groupes existants peuvent être ajoutés de cette manière.</li></p>
      </ul>
      </td> 
     </tr>
    </tbody> 
   </table>

1. Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer** dans le coin inférieur gauche.

