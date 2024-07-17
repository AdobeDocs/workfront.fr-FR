---
title: Créer ou modifier un statut
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: En tant qu’administrateur Adobe Workfront, vous pouvez créer des statuts personnalisés pour les projets, les tâches et les problèmes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 42%

---

# Créer ou modifier un statut

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

En tant qu’administrateur Adobe Workfront, vous pouvez créer des statuts personnalisés pour les projets, les tâches et les problèmes. Il peut s’agir d’utilisateurs sur l’ensemble du système Workfront ou de groupes ou sous-groupes spécifiques. Pour plus d’informations sur les états, voir [Présentation des états](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Les administrateurs de groupe peuvent également créer leurs propres états de groupe, à utiliser uniquement par leurs groupes. Pour plus d’informations, voir [Création ou modification de l’état d’un groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td>
     <p>Nouvelle : standard</p>
     <p>ou</p>
     <p>Actuelle : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création ou modification d’un état personnalisé

Vous pouvez ajouter un état personnalisé à utiliser par l’ensemble de votre organisation ou par un seul groupe.

Lorsque vous créez un état personnalisé pour l’ensemble de l’organisation, vous pouvez le configurer afin que tous les groupes du système puissent l’utiliser sans le modifier. Vous pouvez également le configurer afin que les administrateurs de groupe puissent le modifier pour leurs groupes, comme expliqué dans la section [Créer ou modifier un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche et sélectionnez **[!UICONTROL Configuration]** ![icône Configurer](/help/_includes/assets/gear-icon-setup.png).

1. Dans le panneau de gauche, cliquez sur **Préférences du projet** > **États**.

1. (Conditionnel) Si vous créez ou modifiez un état pour l’utiliser à l’échelle du système, assurez-vous que l’option **États du système** est sélectionnée dans la zone située dans le coin supérieur droit.

   ![](assets/system-statuses-in-upper-rt-corner-new.jpg)

   Ou

   Si l’état d’un groupe ou d’un sous-groupe est défini, commencez à saisir le nom du groupe dans le coin supérieur droit, puis sélectionnez-le lorsqu’il s’affiche.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Sélectionnez l’onglet du type d’objet (**Projet**, **Tâche** ou **Problèmes**) que vous souhaitez associer au statut.

1. Si vous créez un état, cliquez sur **Ajouter un nouvel état**.

   Ou

   Si vous modifiez un état existant, passez la souris dessus, puis cliquez sur l’icône **Modifier** qui s’affiche à l’extrême droite.

   ![](assets/custom-status-edit.png)

1. Configurez le statut à l’aide des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom du statut</td> 
      <td> <p>Saisissez un nom pour ce modèle... Il s’agit d’un champ obligatoire.</p> <p>Lorsque vous créez un nom de statut, tenez compte du faut que d’autres personnes du système peuvent créer un statut homographe. Il est recommandé d’utiliser un nom unique afin d’éviter toute confusion lors de la sélection de statuts dans Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>(Facultatif) Fournissez une description du statut. Les personnes qui l’utilisent seront ainsi informées de sa finalité.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Couleur</td> 
      <td> <p>Personnalisez la couleur du statut en cliquant sur le champ de couleur et en sélectionnant une couleur dans le panneau d’échantillon. Vous pouvez également saisir un nombre hexadécimal dans le champ.</p> <p>La couleur de statut s’affiche dans le coin supérieur droit de Workfront lorsqu’une personne affiche l’objet.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Équivaut à</td> 
      <td> <p>Sélectionnez l’une des options de la liste qui décrit le mieux la fonction du statut. Par exemple, si le nom du statut est Terminé, l’option à laquelle il correspond doit être Terminé.</p> <p>Chaque statut doit correspondre à l’une de ces options, car cela détermine le fonctionnement du statut.</p> <p>Cette option ne peut pas être modifiée une fois le statut créé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clé</td> 
      <td> <p>Si vous créez un statut, saisissez un code ou une abréviation pour le statut ou utilisez celui généré pour vous. Cette clé doit être unique dans Workfront, car elle peut être utilisée à des fins de création de rapports. Si vous essayez de spécifier une clé déjà utilisée dans le système, le champ devient rouge.</p> <p>Il peut s’avérer utile d’utiliser une abréviation reconnaissable par les personnes qui l’utiliseront.</p> <p>Cette option ne peut pas être modifiée une fois le statut créé.</p> <p>Vous ne pouvez pas modifier le code clé des statuts Planification, En cours et Terminé. Tenez-en compte lorsque vous créez un rapport en mode texte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer le statut</td> 
      <td> <p>(Statuts des projets et des tâches uniquement)</p> <p>Activez cette option si vous souhaitez que l’état soit masqué aux utilisateurs et utilisatrices. Lorsque cette option est désactivée (paramètre par défaut), tous les utilisateurs du système peuvent utiliser l’état .</p> <p>Vous pouvez masquer l’état d’un problème en désactivant cette option pour les 4 types de problèmes (rapport de bogues, ordre de modification, problème, requête).</p> </td> 
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
       <p>Pour plus d’informations sur les états de verrouillage, voir <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">États verrouillés et déverrouillés au niveau du système</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

   Pour obtenir des instructions sur la façon de faire de cet état un état par défaut, voir [Utilisation d’états personnalisés comme états par défaut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Pour plus d’informations sur la réorganisation des états d’un groupe, voir [Réorganiser les états au niveau du système et du groupe](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
