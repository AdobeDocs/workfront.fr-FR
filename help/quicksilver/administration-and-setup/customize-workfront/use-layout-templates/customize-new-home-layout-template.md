---
title: Personnaliser la nouvelle page d’accueil à l’aide d’un modèle de disposition
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Vous pouvez utiliser un modèle de disposition pour configurer ce que voient les personnes lorsqu’elles ouvrent la nouvelle page d’accueil.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 9de4a3729abe0ea2ee89df0be2974b714e65332a
workflow-type: ht
source-wordcount: '812'
ht-degree: 100%

---

# Personnaliser la nouvelle page d’accueil à l’aide d’un modèle de disposition

Vous pouvez utiliser un modèle de disposition pour configurer ce que voient les personnes lorsqu’elles ouvrent la nouvelle page d’accueil.

Vous pouvez configurer les éléments suivants :

* Les widgets qui s’affichent par défaut dans l’espace de travail et leur disposition sur la page.
* L’arrière-plan sélectionné.
* Les paramètres de widget spécifiques, notamment les filtres et les groupes disponibles pour les widgets Mes projets, Mes tâches et Mes problèmes, ainsi que leurs paramètres par défaut.

>[!IMPORTANT]
>
>Les choix de modèle de disposition de l’équipe d’administration décrits sur cette page remplacent les choix de personnalisation de chaque utilisateur ou utilisatrice.
>
>Lors de l’enregistrement des modifications apportées à un modèle de disposition, la nouvelle page d’accueil des utilisateurs et utilisatrices de ce modèle est modifiée afin qu’elle corresponde au modèle de disposition. Les sélections de widgets existantes sont alors transférées vers le bas de la page. Bien que les widgets sélectionnés par l’équipe d’administration puissent être repositionnés et redimensionnés par un utilisateur ou une utilisatrice, ils ne peuvent pas être supprimés.

Pour plus d’informations sur l’utilisation de la nouvelle page d’accueil, consultez [Commencer avec la nouvelle page d’accueil](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

Pour plus d’informations sur la création de modèles de disposition, voir [Créer et gérer des modèles de disposition](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de disposition, vous devez l’attribuer à des utilisateurs et utilisatricess pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de disposition à des utilisateurs et utilisatrices, voir [Attribuer un modèle de disposition à des utilisateurs et utilisatrices](../use-layout-templates/assign-users-to-layout-template.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.
Pour les exécuter pour un groupe, vous devez être responsable de ce groupe.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas accès, demandez à votre équipe d’administration Workfront si des restrictions supplémentaires sont définies pour votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnaliser la nouvelle page d’accueil à l’aide d’un modèle de disposition

1. Commencez à travailler sur un modèle de disposition, comme décrit dans la section [Créer et gérer des modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow.png) sous **Personnaliser ce que les utilisateurs et utilisatrices voient**, puis cliquez sur l’**espace de travail Accueil**.

1. Dans les onglets qui s’affichent à droite, cliquez sur **Conception et disposition** pour choisir et organiser des widgets et l’arrière-plan, ou **Paramètres des widgets** pour gérer les paramètres de widgets individuels, tels que les filtres et les groupes disponibles.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Conception et disposition</td> 
      <td>
      <p>Sélectionnez les widgets qui seront présents dans les espaces de travail des utilisateurs et utilisatrices, leur position et choisissez un arrière-plan. Notez que même si les personnes ne peuvent pas supprimer les widgets sélectionnés,elles peuvent les déplacer et les redimensionner librement et ajouter des widgets supplémentaires.</p>
      <p>Cet onglet fonctionne essentiellement comme un nouveau petit espace de travail d’accueil. Il peut donc être personnalisé selon les étapes décrites dans la section <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Ajouter, modifier ou supprimer des widgets dans la nouvelle page d’accueil</a>. Sélectionnez des widgets et organisez l’espace de travail comme vous le souhaitez pour les utilisateurs et utilisatrices.</p>
      <p>Pour modifier l’arrière-plan, procédez comme suit : <b>Personnalisation de l’arrière-plan</b> dans <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Commencer avec la nouvelle page d’accueil</a>.</p>
      <p>

>[!NOTE]
>
>Seuls le déplacement ou le redimensionnement des widgets dans le modèle de disposition ne déclenchent pas la mise à jour de la disposition des nouvelles pages d’accueil des utilisateurs et utilisatrices. Cependant, l’ajout ou la suppression d’un widget déclenche une mise à jour des pages des utilisateurs et utilisatrices.

</p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Paramètres du widget</td> 
      <td>
      <p>Modifiez les paramètres de widgets individuels. Actuellement, seuls trois widgets sont pris en charge :</p>
      <ul>
        <li>Mes projets</li>
        <li>Mes tâches</li>
        <li>Mes problèmes</li>
      </ul>
      <p>Une fois que vous avez sélectionné le widget que vous souhaitez modifier, les options disponibles s’affichent à droite. Ces options comprennent <b>Filtres</b>, <b>Colonnes</b> et <b>Groupes</b>. Vous pouvez effectuer les opérations suivantes :</p>
      <ul>
      <li><p><b>Sélectionner et trier les filtres, colonnes ou groupes disponibles pour les utilisateurs et utilisatrices :</b></p>
      <p>Cochez la case en regard de toutes les options de la liste que vous souhaitez que les personnes puissent utiliser. Les options non cochées ne s’affichent pas pour les utilisateurs et utilisatrices. Faites glisser les options de la liste pour définir un ordre.</li></p>
      <p>

>[!IMPORTANT]
>
>Les utilisateurs et utilisatrices doivent au moins disposer de l’option Créer l’accès aux vues pour que la configuration des colonnes de l’équipe d’administration s’applique correctement à leurs nouvelles pages d’accueil.

</p>
      <li><p><b>Définir un filtre ou un groupe par défaut pour le widget :</b></p>
      <p>Passez la souris sur une option pour afficher un bouton permettant de définir cette option comme option par défaut pour les utilisateurs et utilisatrices. La valeur par défaut actuelle comporte un badge bleu Par défaut à sa droite.</li></p>
      <li><p><b>Ajouter un filtre, une colonne ou un groupe existant à la liste des options disponibles :</b></p>
      <p>Cliquez sur le bouton représentant le signe plus au bas de chaque liste pour y ajouter une option. Notez que seuls les filtres, champs (pour les colonnes) ou groupes existants peuvent être ajoutés de cette manière.</p></li>
      </ul>
      <p>

>[!NOTE]
>
>Si vous définissez un filtre ou un regroupement par défaut pour un widget spécifique à l’aide d’un modèle de disposition, il se peut qu’il ne prenne pas effet immédiatement en raison des préférences existantes de la personne. Pour appliquer immédiatement le nouveau filtre ou regroupement, vous ou la personne concernée devrez peut-être réinitialiser les préférences en ajoutant « /resetUser » à la fin de l’URL.

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. Poursuivez la personnalisation du modèle de disposition.

   Ou

   Si vous avez terminé de le personnaliser, cliquez sur **Enregistrer** en bas à gauche.
