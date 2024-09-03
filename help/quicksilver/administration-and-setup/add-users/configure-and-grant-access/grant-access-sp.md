---
title: Accorder l’accès au planificateur de scénario
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne au planificateur de scénarios.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 99%

---

# Accorder l’accès au planificateur de scénarios

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne au planificateur de scénarios, comme expliqué dans la section [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Outre l’accès au planificateur de scénarios, une personne disposant d’un niveau d’accès administration non système doit également avoir accès aux données financières afin de voir toutes les informations financières contenues dans un plan, telles que les budgets, les coûts et les taux des fonctions. Pour plus d’informations, voir [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Formule Adobe Workfront*</p> </td> 
   <td>Entreprises ou niveau supérieur</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou niveau supérieur Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Vue d’ensemble des licences</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour le planificateur de scénarios Adobe Workfront pour accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention du planificateur de scénarios Workfront, voir <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Accès nécessaire pour utiliser le planificateur de scénarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Accès Affichage ou niveau supérieur au planificateur de scénarios</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas accès, demandez à votre équipe d’administration Workfront si des restrictions supplémentaires sont définies à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> <p>Autorisations d’affichage ou niveau supérieur pour un plan</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Demander l’accès à un plan dans le planificateur de scénarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configurer l’accès des personnes au planificateur de scénarios à l’aide d’un niveau d’accès personnalisé

1. Commencez à créer ou modifier le niveau d’accès, comme expliqué dans la section [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Cliquez sur l’option située à droite du **Planificateur de scénarios** que vous souhaitez utiliser pour ce niveau d’accès.

   >[!NOTE]
   >
   >Le type de licence Demande ou Externe n’autorise pas l’accès Affichage ou Modification au planificateur de scénarios.

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et domaines dans le niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), comme [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.

## Accéder au planificateur de scénarios selon le type de licence

Pour plus d’informations sur ce que les utilisateurs et utilisatrices de chaque niveau d’accès peuvent faire avec le planificateur de scénarios, voir la section [Zone du planificateur de scénarios](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) dans l’article [Fonctionnalités disponibles pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Accéder au planificateur de scénarios selon les paramètres de niveau d’accès

Les informations suivantes peuvent vous aider à comprendre comment utiliser les paramètres de niveau d’accès pour contrôler l’accès des personnes aux informations dans le planificateur de scénarios Workfront.

* [Pas d’accès](#no-access)
* [Accès Affichage](#view-access)
* [Accès en modification](#edit-access)

### Pas d’accès {#no-access}

Une personne n’ayant pas accès au planificateur de scénarios ne peut pas voir l’icône Scénarios dans le menu principal lorsqu’il est ajouté à son modèle de disposition, ni afficher les plans et les initiatives qui sont partagés avec elle. Si le lien vers un plan est partagé avec une personne qui n’a pas accès au planificateur de scénarios, la personne ne peut pas afficher ni modifier le plan.

### Accès en affichage {#view-access}

Les personne disposant d’un accès en mode Affichage au planificateur de scénarios peuvent effectuer les opérations suivantes :

* Voir l’icône Scénarios dans le menu principal ![](assets/esp-icon-in-main-menu.png), mais la zone Plans est vide, sauf si la personne clique sur un lien de formule partagé par une autre personne.
* Afficher un plan lorsqu’une autre personne partage le lien vers celui-ci.

  Cela inclut toutes les informations sur les fonctions dans le plan.

  Cela inclut également les taux des fonctions et les informations de coûts sur le plan si la personne destinataire a également accès aux données financières. Pour plus d’informations, voir [Accorder l&#39;accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Accès en modification {#edit-access}

Les personnes diposant de l’accès Modification au planificateur de scénarios peuvent effectuer les opérations suivantes :

* Voir l’icône Scénarios dans le menu principal ![](assets/esp-icon-in-main-menu.png) et l’utiliser pour accéder aux données du plan.
* Créez des plans.
* Affichez, modifiez et supprimez les plans créés.
* Affichez, modifiez et supprimez les plans d’autres utilisateurs et utilisatrices accessibles à l’aide d’un lien partagé.

  Cela inclut toutes les informations relatives aux fonctions contenues dans un plan.

  Cela comprend également les taux liés aux fonctions et les informations de coûts sur le plan si l’utilisateur ou l’utilisatrice destinataire a accès aux données financières. Pour plus d’informations, consultez [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
