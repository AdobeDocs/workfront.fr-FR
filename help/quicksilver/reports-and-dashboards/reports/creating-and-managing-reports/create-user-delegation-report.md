---
product-area: reporting
keywords: user,delegation,report,delegate,approbation
navigation-topic: create-and-manage-reports
title: Créer un rapport Délégation d’utilisateurs
description: Créer un rapport Délégation d’utilisateurs
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 4%

---

# Créer un rapport Délégation d’utilisateurs

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

Dans Adobe Workfront, les utilisateurs peuvent déléguer les approbations de projet, de tâche et d’émission à d’autres utilisateurs pour s’assurer que leurs approbations sont gérées lorsqu’ils ne sont pas en fonction. Les utilisateurs disposant d’une licence Plan peuvent créer un rapport Délégation d’utilisateurs pour afficher :

* Qui a délégué la tâche, l’émission et l’approbation de projet à un autre utilisateur
* Les utilisateurs qui leur ont délégué la tâche, l’émission et les approbations de projet qui leur sont affectées

* Les dates de début et de fin des délégations

Pour en savoir plus sur la délégation des approbations, voir [Déléguer la demande d’approbation](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations pour les éléments dont les approbations sont déléguées et pour les utilisateurs impliqués dans la délégation</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création d’un rapport de délégation d’utilisateur

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Rapports**.

1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Délégation d’utilisateurs**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   Par défaut, les champs suivants s&#39;affichent dans ce rapport :

   | Champ | Description |
   |---|---|
   | **De l’utilisateur** | Il s’agit de l’utilisateur qui délègue la tâche, les problèmes et les approbations de projet à un autre utilisateur. |
   | **À l’utilisateur** | Il s’agit de l’utilisateur auquel sont déléguées les approbations de tâche, d’émission et de projet. |
   | **Début** | Il s’agit du début de l’heure d’absence du bureau de l’utilisateur qui a effectué les délégations. |
   | **Fin** | Il s’agit de la fin de l’heure d’absence du bureau de l’utilisateur qui a effectué les délégations. |

   {style=&quot;table-layout:auto&quot;}

1. (Facultatif) Dans le créateur de rapports, modifiez les éléments suivants :

   * Colonnes
   * Regroupements
   * Filtres
   * Graphique

   Pour en savoir plus sur ces fonctionnalités, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Une fois le rapport créé, cliquez sur **Enregistrer + Fermer**.

1. Saisissez un nouveau nom dans le champ **Nom du rapport** , puis cliquez sur **Enregistrer le rapport**.

   Le rapport s’affiche.
