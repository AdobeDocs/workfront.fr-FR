---
title: Octroi de l’accès au planificateur de scénarios
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne au planificateur de scénarios.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 96%

---

# Accorder l’accès au planificateur de scénarios

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour définir l’accès d’une personne au planificateur de scénarios, comme expliqué dans la section [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Outre l’accès au planificateur de scénarios, une personne disposant d’un niveau d’accès administration non système doit également avoir accès aux données financières afin de voir toutes les informations financières contenues dans un plan, telles que les budgets, les coûts et les taux des fonctions. Pour plus d’informations, voir [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Package Adobe Workfront</p> </td> 
   <td>Entreprises ou niveau supérieur</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Léger ou supérieur</p>
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour le planificateur de scénarios Adobe Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou niveau supérieur au planificateur de scénarios</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Autorisations d’objet</p> </td> 
   <td> <p>Autorisations d’affichage ou niveau supérieur pour un plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Une personne n’ayant pas accès au planificateur de scénarios ne peut pas voir l’icône Scénarios dans le menu principal lorsqu’il est ajouté à son modèle de mise en page, ni afficher les plans et les initiatives qui sont partagés avec elle. Si le lien vers un plan est partagé avec une personne qui n’a pas accès au planificateur de scénarios, la personne ne peut pas afficher ni modifier le plan.

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
