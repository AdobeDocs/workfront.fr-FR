---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Création ou modification du statut d’un groupe
description: En tant qu’administrateur ou administratrice de groupe, vous pouvez créer des statuts personnalisés pour un groupe que vous gérez. Cela permet d’éliminer le besoin de dizaines de statuts personnalisés à l’échelle de l’entreprise et d’accroître l’autonomie de vos hiérarchies de groupe.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 92%

---

# Créer ou modifier un statut de groupe

En tant qu’administrateur ou administratrice de groupe, vous pouvez créer des statuts personnalisés pour un groupe que vous gérez. Cela permet d’éliminer le besoin de dizaines de statuts personnalisés à l’échelle de l’entreprise et d’accroître l’autonomie de vos hiérarchies de groupe.

Vous pouvez également modifier le statut d’un groupe que vous gérez à l’échelle du système si un administrateur ou une administratrice Workfront a déverrouillé le statut.
Pour plus d’informations, voir [Statuts verrouillés et déverrouillés à l’échelle du système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

>[!NOTE]
>
>Les statuts de groupe personnalisés ne peuvent pas être affichés sur un projet lors de l’affichage du projet dans une vue Agile. Seuls les statuts verrouillés par défaut et personnalisés sont visibles lors de l’affichage d’un projet dans une vue Agile. Pour plus d’informations sur la personnalisation d’une vue Agile pour un projet, consultez la section [Créer ou personnaliser une vue Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) dans l’article [Créer ou modifier des vues dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

Pour obtenir des informations générales sur les statuts, voir [Vue d’ensemble des statuts](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
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
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer ou modifier un statut pour un groupe

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe dans lequel vous souhaitez créer ou personnaliser des statuts.
1. Dans le panneau de gauche, cliquez sur **Statuts**.

   Si le groupe que vous affichez est un groupe de niveau supérieur, la liste qui s’affiche comprend les éléments suivants :

   * Statuts verrouillés au niveau du système.
   * Statuts personnalisés déjà créés pour le groupe.

   En outre, si le groupe que vous affichez est un sous-groupe, la liste comprend également :

   * Statuts verrouillés appartenant aux groupes situés au-dessus du sous-groupe.
   * Statuts déverrouillés qui appartenaient aux groupes situés au-dessus du sous-groupe lors de sa création.

     Une fois qu’un sous-groupe est créé, les statuts déverrouillés créés dans les groupes situés au-dessus de lui ne sont pas inclus dans la liste des statuts du sous-groupe. Cependant, si une personne en verrouille un par la suite, il est alors inclus dans la liste des statuts du sous-groupe. Pour plus d’informations, voir [Comment les groupes héritent des statuts](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

1. Sélectionnez l’onglet du type d’objet (**Projet**, **Tâche**, ou **Problèmes**) que vous souhaitez associer au statut.

1. Le cas échéant, si le statut concerne un problème, assurez-vous que la **Liste principale** est sélectionnée.

   ![Liste de Principal &#x200B;](assets/master-list.png)

   Pour plus d’informations sur la personnalisation des autres types de problèmes (rapport de bugs, ordre de modification, problème, requête), voir [Personnaliser les types de problèmes par défaut](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. Le cas échéant, pour créer un statut, cliquez sur **Ajouter un nouveau statut**.

   Ou

   Pour modifier un statut existant, placez le pointeur de la souris sur le statut que vous souhaitez modifier, puis cliquez sur l’option **Modifier** qui s’affiche tout à fait à droite.

   ![Statuts des groupes](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Vous ne pouvez modifier le statut de votre groupe que si :
   >      
   >* Vous gérez le groupe pour lequel le statut a été créé.
   >* Un administrateur ou une administratrice Workfront a déverrouillé le statut au niveau du système.
   >* Un administrateur ou une administratrice d’un groupe situé au-dessus du vôtre a déverrouillé le statut.
   >      
   >      
   >Lorsque vous modifiez un statut existant, vous ne pouvez changer que son nom, sa description et sa couleur.
   >
   >Lorsque vous modifiez un statut verrouillé, vos modifications affectent tous les sous-groupes qui ont hérité du statut de votre groupe.
   >   
   >À l’inverse, la modification d’un statut déverrouillé n’affecte pas les sous-groupes qui ont hérité du statut de votre groupe.

1. Indiquez les informations suivantes.

   Si vous modifiez un statut, seuls les 3 premiers paramètres peuvent être modifiés.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du statut</td> 
      <td> <p>Saisissez le nom du statut. Champ obligatoire.</p> <p>Lorsque vous créez un nom de statut, sachez que d’autres utilisateurs et utilisatrices du système peuvent créer un statut portant le même nom. Il est recommandé d’utiliser un nom unique afin d’éviter toute confusion lors de la sélection de statuts dans Workfront.</p><p>En cas de statuts en double, l’administrateur ou l’administratrice de groupe doit mettre à jour les noms pour les différencier. Le seul élément unique du système est la clé de statut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>(Facultatif) Saisissez une description du statut. Cette action communique sa fonctionnalité aux personnes qui l’utilisent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Personnalisez la couleur du statut en cliquant sur le champ de couleur et en sélectionnant une couleur dans le panneau d’échantillons. Vous pouvez également saisir un nombre hexadécimal dans le champ.</p> <p>La couleur du statut est visible dans le coin supérieur droit de Workfront lorsqu’un utilisateur ou une utilisatrice affiche l’objet.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Équivaut à</td> 
      <td> <p>Sélectionnez l’une des options de la liste qui décrit le mieux la fonction du statut. Par exemple, si le nom du statut est Terminé, l’option à laquelle il correspond doit être Terminé.</p> <p>Chaque statut doit correspondre à l’une de ces options, car celles-ci déterminent le fonctionnement du statut.</p> <p>Cette option ne peut pas être modifiée une fois le statut créé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clé</td> 
      <td> <p>Si vous créez un statut, saisissez un code ou une abréviation pour le statut ou utilisez celui généré pour vous. Cette clé doit être unique dans Workfront, car elle peut être utilisée à des fins de création de rapports. Si vous essayez de spécifier une clé déjà utilisée dans le système, le champ devient rouge.</p> <p>Il peut s’avérer utile d’utiliser une abréviation facilement reconnaissable pour les personnes qui l’utiliseront.</p> <p>Cette option ne peut pas être modifiée une fois le statut créé.</p> <p>Vous ne pouvez pas modifier le code clé des statuts Planification, Actuel et Terminé. Prenez cela en compte lorsque vous créez un rapport en mode texte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer le statut</td> 
      <td> <p>(Statuts des projets et des tâches uniquement)</p> <p>Activez cette option si vous souhaitez que le statut soit masqué aux utilisateurs et utilisatrices. Lorsqu’elle est désactivée (paramètre par défaut), tous les sous-groupes situés sous le groupe peuvent utiliser le statut.</p> <p>Conseil : vous pouvez masquer le statut d’un problème en désactivant les 4 types de problème (rapport de bug, ordre de modification, problème, demande).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller pour tous les groupes</td> 
      <td> 
       <p>Si vous laissez cette option activée, les utilisateurs et utilisatrices de votre groupe et de ses sous-groupes peuvent afficher et utiliser le statut et les administrateurs et administratrices de groupe ne peuvent pas le personnaliser pour les sous-groupes inférieurs.</p> 
       <p>Lorsque cette option est désactivée, les administrateurs et administratrices de groupe peuvent personnaliser le statut des sous-groupes inférieurs.</p> 
       <p><b>REMARQUE</b> : vous pouvez utiliser les statuts verrouillés et déverrouillés dans le cadre d’un processus d’approbation de groupe. Si vous créez un processus d’approbation de groupe avec un statut de groupe déverrouillé, les utilisateurs et utilisatrices peuvent associer le processus d’approbation à n’importe quel projet, tâche ou problème associé au groupe.</p> 
       <p>Pour plus d’informations sur le verrouillage des statuts, voir <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Statuts de groupe verrouillés et déverrouillés</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Le statut est désormais disponible pour tous les projets associés à votre groupe ou sous-groupe. Si vous l’avez verrouillé, il est disponible pour tous les sous-groupes inférieurs.

   Vous pouvez configurer le statut comme statut par défaut pour le groupe. Pour plus d’informations, voir [Utiliser un statut personnalisé comme statut par défaut pour un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Créer un statut personnalisé pour plusieurs groupes

Si vous êtes administrateur ou administratrice de Workfront, vous pouvez créer un statut personnalisé pour plusieurs groupes en créant un statut à l’échelle du système, puis en masquant ce statut dans tous les groupes qui n’en ont pas besoin.

Si vous êtes administrateur ou administratrice de groupe (ou administrateur/administratrice Workfront), vous pouvez créer un statut personnalisé pour plusieurs sous-groupes au sein d’une hiérarchie de groupes gérables en créant un statut pour un groupe de niveau supérieur, puis en masquant ce statut dans des sous-groupes inférieurs qui n’en ont pas besoin.

1. Si vous êtes administrateur ou administratrice Workfront, créez un statut de déverrouillage à l’échelle du système, comme décrit dans la section [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. Dans la zone située dans le coin supérieur droit, supprimez **Statuts du système**, commencez à saisir le nom d’un groupe dans lequel vous souhaitez masquer le statut, puis cliquez sur le nom qui s’affiche.
1. Placez la souris sur le statut que vous souhaitez masquer dans le groupe, puis cliquez sur **Modifier** lorsqu’il apparaît.

   ![Modifier le statut &#x200B;](assets/hover-click-edit.jpg)

1. Activez l’option **Masquer le statut** qui s’affiche.

   ![Masquer le statut](assets/hide-group-status.png)

1. Cliquer sur **Enregistrer**.

   Le statut est grisé et n’est plus visible pour tous les utilisateurs et utilisatrices de ce groupe.

1. Répétez les étapes 3 à 5 pour masquer le statut personnalisé dans tous les autres groupes qui n’en ont pas besoin.

