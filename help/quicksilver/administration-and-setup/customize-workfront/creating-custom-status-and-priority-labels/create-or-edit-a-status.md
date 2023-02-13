---
title: Création ou modification d’un état
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: En tant qu’administrateur Adobe Workfront, vous pouvez créer des statuts personnalisés pour les projets, les tâches et les problèmes.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 2%

---

# Création ou modification d’un état

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

En tant qu’administrateur Adobe Workfront, vous pouvez créer des statuts personnalisés pour les projets, les tâches et les problèmes. Il peut s’agir d’utilisateurs sur l’ensemble du système Workfront ou de groupes ou sous-groupes spécifiques. Pour plus d’informations sur les états, voir [Présentation des états](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Les administrateurs de groupe peuvent également créer leurs propres états de groupe, à utiliser uniquement par leurs groupes. Pour plus d’informations, voir [Création ou modification d’un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Création ou modification d’un état personnalisé

Vous pouvez ajouter un état personnalisé à utiliser par l’ensemble de votre organisation ou par un seul groupe.

Lorsque vous créez un état personnalisé pour l’ensemble de l’organisation, vous pouvez le configurer afin que tous les groupes du système puissent l’utiliser sans le modifier. Vous pouvez également le configurer afin que les administrateurs de groupe puissent le modifier pour leurs groupes, comme expliqué à la section [Création ou modification d’un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **Statuts**.

1. (Conditionnel) Si vous créez ou modifiez un état pour l’utiliser à l’échelle du système, assurez-vous que **États du système** est sélectionné dans la zone située dans le coin supérieur droit.

   ![](assets/system-statuses-in-upper-rt-corner.jpg)

   Ou

   Si l’état d’un groupe ou d’un sous-groupe est défini, commencez à saisir le nom du groupe dans le coin supérieur droit, puis sélectionnez-le lorsqu’il s’affiche.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Sélectionnez l’onglet du type d’objet (**Projet**, **Tâches** ou **Problèmes**) que vous souhaitez associer à l’état .

1. Si vous créez un état, cliquez sur **Ajouter un nouvel état**.

   Ou

   Si vous modifiez un état existant, passez la souris dessus, puis cliquez sur le bouton **Modifier** qui s’affiche à l’extrême droite.

   ![](assets/custom-status-edit.png)

1. Configurez le statut à l’aide des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du statut</td> 
      <td> <p>Saisissez le nom de l’état. Champ obligatoire.</p> <p>Lorsque vous créez un nom d’état, sachez que d’autres utilisateurs du système peuvent créer un état portant le même nom. Il est recommandé d’utiliser un nom unique afin d’éviter toute confusion lors de la sélection d’états dans Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>(Facultatif) Saisissez une description de l’état. Cela communique son but à ceux qui l'utilisent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Personnalisez la couleur de l’état en cliquant sur le champ de couleur et en sélectionnant une couleur dans le panneau d’échantillon. Vous pouvez également saisir un nombre hexadécimal dans le champ.</p> <p>La couleur d’état s’affiche dans le coin supérieur droit de Workfront lorsqu’un utilisateur affiche l’objet.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Équivaut à</td> 
      <td> <p>Sélectionnez l’une des options de la liste qui décrit le mieux la fonction de l’état. Par exemple, si le nom de l’état est Terminé, l’option à laquelle il correspond doit être Terminé.</p> <p>Chaque état doit correspondre à l’une de ces options, car cela détermine le fonctionnement de l’état.</p> <p>Cette option ne peut pas être modifiée une fois l’état créé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clé</td> 
      <td> <p>Si vous créez un état, saisissez un code ou une abréviation pour le statut ou utilisez celui généré pour vous. Cette clé doit être unique dans Workfront, car elle peut être utilisée à des fins de création de rapports. Si vous essayez de spécifier une clé déjà utilisée dans le système, le champ devient rouge.</p> <p>Il peut s’avérer utile d’utiliser une abréviation reconnaissable par ceux qui l’utiliseront.</p> <p>Cette option ne peut pas être modifiée une fois l’état créé.</p> <p>Vous ne pouvez pas modifier le code clé des états Planification, Actuel et Terminé. Ceci est important si vous créez un rapport en mode texte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer l’état</td> 
      <td> <p>(Statuts des projets et des tâches uniquement)</p> <p>Activez cette option si vous souhaitez que l’état soit masqué aux utilisateurs. Lorsqu’il est désactivé (paramètre par défaut), tous les utilisateurs du système peuvent utiliser l’état .</p> <p>Vous pouvez masquer l’état d’un problème en désactivant les 4 types de problème (rapport de bogues, ordre de modification, problème, requête).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verrouiller pour tous les groupes</td> 
      <td>
       <p>Lorsqu’un état est verrouillé, les utilisateurs du système peuvent le voir et l’utiliser, et les administrateurs de groupe ne peuvent pas le personnaliser pour leurs groupes.</p> 
       <p>Lorsqu’un état est déverrouillé, les administrateurs de groupe peuvent le personnaliser pour leurs groupes individuels.</p>

   <div>
       <p>Vous pouvez utiliser les états verrouillés et déverrouillés dans un processus d’approbation du système. Si vous créez un processus d’approbation du système avec l’état déverrouillé, les utilisateurs de tout le système peuvent associer le processus d’approbation à n’importe quel projet, tâche ou problème du système.</p>
       <p> Dans les scénarios suivants, des messages d’avertissement s’affichent pour vous aider, ainsi que vos utilisateurs, à comprendre les résultats du déverrouillage d’un état :</p>
       <ul>
       <li>Un administrateur déverrouille un état au niveau du système utilisé dans un processus d’approbation. Un message avertit que l’état de déverrouillage de leurs groupes est susceptible d’être supprimé, ce qui empêcherait les membres de ces groupes d’utiliser correctement ce processus d’approbation pour les objets qui leur sont assignés.</li>
       <li>Un utilisateur commence à modifier un processus d’approbation qui utilise l’état déverrouillé. Un message avertit l’utilisateur de l’état déverrouillé afin qu’il puisse déterminer s’il est préférable de le reverrouiller ou de le remplacer.</li>
       <li>Un processus d’approbation au niveau du système avec un état déverrouillé est associé à un objet et l’état a été supprimé pour le groupe affecté à l’objet. Lorsqu’un membre du groupe accède à la section Validations de l’objet, un message explique que le processus d’approbation ne peut pas être lancé pour l’objet.</li>
       </ul>
       <p>Pour plus d’informations sur le verrouillage des états, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">États au niveau du système verrouillés et déverrouillés</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Pour plus d’informations sur la définition de ce statut comme statut par défaut, voir [Utilisation d’états personnalisés comme états par défaut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Pour plus d’informations sur la réorganisation des états d’un groupe, voir [Réorganiser les états au niveau du système et du groupe](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
