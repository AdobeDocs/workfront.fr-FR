---
product-area: projects
navigation-topic: financials
title: Remplacer les taux de facturation au niveau du projet par des taux de facturation au niveau de l’entreprise
description: Remplacer les taux de facturation au niveau du projet par des taux de facturation au niveau de l’entreprise
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 72511f98e05c160e2ca69def8aa3a929ed62bb40
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 100%

---

# Remplacer les taux de facturation au niveau du projet par des taux de facturation au niveau de l’entreprise

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Vous pouvez configurer un projet pour qu’il utilise des taux de facturation au niveau de l’entreprise plutôt qu’au niveau du projet.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets et aux données financières</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour le projet avec les autorisations de gestion financière</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Activer l’option de remplacement des taux de facturation au niveau de l’entreprise

Lorsqu’une entreprise est associée à un projet et que cette option est activée, les modifications apportées aux taux de facturation au niveau de l’entreprise remplacent le taux de facturation défini pour le projet.

Lorsqu’une personne recalcule manuellement les finances du projet, les modifications apportées aux taux de facturation au niveau de l’entreprise sont appliquées. Les calculs de revenus historiques sont également ignorés, à moins qu’ils ne soient marqués comme facturés.

1. Accédez à un projet.
1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png) à côté du nom du projet dans l’en-tête, puis cliquez sur **Modifier**.
1. Dans la section **Finances**, activez l’option **Autoriser le remplacement des taux de facturation au niveau du projet par des taux de facturation au niveau de l’entreprise**.

   >[!CAUTION]
   >
   >L’activation de cette option annule les calculs de revenus historiques, sauf s’ils sont marqués comme facturés. Vous pouvez conserver les calculs historiques des revenus en créant un enregistrement de facturation. Pour plus d’informations, voir l’article [Créer des enregistrements de facturation](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Cliquez sur **Enregistrer les modifications**.

## Mettre à jour les taux de facturation au niveau de l’entreprise et les appliquer à un projet

Après avoir activé l’option de remplacement des taux de facturation au niveau de l’entreprise pour un projet, les modifications apportées aux taux de facturation de l’entreprise s’appliquent au projet chaque fois que les finances sont recalculées.

>[!NOTE]
>
>Les personnes doivent avoir accès aux entreprises dans leur niveau d’accès pour mettre à jour les taux de facturation au niveau de l’entreprise.

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration**.
1. Cliquez sur **Entreprises**.
1. Cliquez sur le nom de l’entreprise associée au projet pour lequel vous avez activé le remplacement des taux de facturation au niveau de l’entreprise.
1. Cliquez sur **Taux de facturation** dans le panneau de gauche.
1. Mettez à jour le **Taux de facturation de l’entreprise** et les dates de début et de fin pour une fonction existante, puis appuyez sur Entrée.

   Pour ajouter un nouveau taux de facturation d’entreprise avec date de validité, sélectionnez un taux de facturation pour la fonction et cliquez sur **Modifier**. Pour plus d’informations sur les taux de facturation de l’entreprise avec date de validité, voir [Remplacer les taux de facturation des fonctions au niveau de l’entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Pour mettre à jour les taux de l’entreprise pour un ou plusieurs projets, effectuez l’une des opérations suivantes :

   * Plusieurs projets :

      1. Accédez à une liste de projets.
      1. Cochez la case correspondant aux projets que vous souhaitez mettre à jour.
      1. Cliquez sur **Modifier**.
      1. Dans la section Paramètres, activez l’option **Recalculer les coûts et les revenus**.
      1. Cliquez sur **Enregistrer les modifications**.

   * Projet unique :

      1. Accédez au projet pour lequel vous avez activé le remplacement par des taux de facturation au niveau de l’entreprise.
      1. Cliquez sur le menu **Plus** ![](assets/qs-more-icon-on-an-object.png) à côté du nom du projet dans l’en-tête, puis cliquez sur **Recalculer finances**.
