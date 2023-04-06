---
title: Accorder l’accès au planificateur de scénarios
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur au planificateur de scénarios.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# Accorder l’accès au planificateur de scénarios

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’un utilisateur au planificateur de scénarios, comme expliqué dans la section [Présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Outre l’accès au planificateur de scénarios, un utilisateur disposant d’un niveau d’accès administrateur non système doit également avoir accès aux données financières afin de voir toutes les informations financières contenues dans un plan, telles que les budgets, les coûts et les taux de rôle de travail. Pour plus d’informations, voir [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Professionnel ou supérieur</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Passez en revue ou version ultérieure. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Présentation des licences héritées</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour le planificateur de scénario Adobe Workfront pour accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention du planificateur de scénario Workfront, voir <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Accès nécessaire pour utiliser le planificateur de scénarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Afficher l’accès ou une version ultérieure au planificateur de scénarios</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> <p>Afficher les autorisations ou plus pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Demande d’accès à un plan dans le planificateur de scénarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Configurer l’accès des utilisateurs au planificateur de scénarios à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d’accès, comme expliqué dans la section [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’option située à droite de **Planification du scénario** que vous souhaitez utiliser pour ce niveau d’accès.

   >[!NOTE]
   >
   >Le type de licence Demander ou Externe n’autorise pas l’accès Afficher ou Modifier au planificateur de scénario.

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans la section [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

## Accès au planificateur de scénario par type de licence

Pour plus d’informations sur ce que les utilisateurs de chaque niveau d’accès peuvent faire avec le planificateur de scénario, voir la section [Zone du planificateur de scénario](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accès au planificateur de scénario par paramètre de niveau d’accès

Les informations suivantes peuvent vous aider à comprendre comment utiliser les paramètres de niveau d’accès pour contrôler l’accès des utilisateurs aux informations dans le planificateur de scénarios Workfront.

* [Accès interdit](#no-access)
* [Afficher l’accès](#view-access)
* [Modifier l’accès](#edit-access)

### Accès interdit {#no-access}

Un utilisateur n’ayant pas accès au planificateur de scénarios ne peut pas voir l’icône Scénarios dans le menu principal lorsqu’il est ajouté à son modèle de mise en page, ni afficher les plans et les initiatives qui sont partagés avec lui. Si le lien vers un plan est partagé avec un utilisateur qui n’a pas accès au planificateur de scénario, l’utilisateur ne peut pas afficher ni modifier le plan.

### Afficher l’accès {#view-access}

Les utilisateurs disposant d’un accès en mode Affichage au planificateur de scénario peuvent effectuer les opérations suivantes :

* Voir l’icône Scénarios dans le menu principal ![](assets/esp-icon-in-main-menu.png), mais la zone Plans est vide, sauf si l’utilisateur clique sur un lien de formule partagé par un autre utilisateur.
* Afficher un plan lorsqu’un autre utilisateur partage le lien vers celui-ci.

   Cela inclut toutes les informations sur les rôles d’emploi dans le plan.

   Il inclut également les taux de rôle de l’emploi et les informations de coûts sur le plan si l’utilisateur destinataire a également accès aux données financières. Pour plus d’informations, voir [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Modifier l’accès {#edit-access}

Les utilisateurs disposant de l’accès Modifier au planificateur de scénario peuvent effectuer les opérations suivantes :

* Voir l’icône Scénarios dans le menu principal ![](assets/esp-icon-in-main-menu.png) et l’utiliser pour accéder aux données du plan.
* Créez des plans.
* Affichez, modifiez et supprimez les plans qu’ils créent.
* Afficher, modifier et supprimer les plans d’autres utilisateurs auxquels ils accèdent à l’aide d’un lien partagé.

   Cela inclut toutes les informations sur les rôles de tâche dans un plan.

   Il inclut également les taux de rôle d’emploi et les informations de coûts sur le plan si l’utilisateur destinataire a accès aux données financières. Pour plus d’informations, voir [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
