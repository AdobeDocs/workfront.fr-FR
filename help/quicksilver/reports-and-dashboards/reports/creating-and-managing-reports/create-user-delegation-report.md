---
product-area: reporting
keywords: user,delegation,report,delegate,approbation
navigation-topic: create-and-manage-reports
title: Créer un rapport sur la délégation des utilisateurs et utilisatrices
description: Créer un rapport sur la délégation des utilisateurs et utilisatrices
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 30%

---

# Créer un rapport sur la délégation des utilisateurs et utilisatrices

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

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations pour les éléments dont les approbations sont déléguées et pour les utilisateurs impliqués dans la délégation</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Création d’un rapport de délégation d’utilisateur

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Rapports**.

1. Cliquez sur **Nouveau rapport**, puis sélectionnez **Délégation d’utilisateurs**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   Par défaut, les champs suivants s&#39;affichent dans ce rapport :

   | champ | Description |
   |---|---|
   | **De L’Utilisateur** | Il s’agit de l’utilisateur qui délègue la tâche, les problèmes et les approbations de projet à un autre utilisateur. |
   | **À L’Utilisateur** | Il s’agit de l’utilisateur auquel sont déléguées les approbations de tâche, d’émission et de projet. |
   | **Démarrer** | Il s’agit du début de l’heure d’absence du bureau de l’utilisateur qui a effectué les délégations. |
   | **End** | Il s’agit de la fin de l’heure d’absence du bureau de l’utilisateur qui a effectué les délégations. |

   {style="table-layout:auto"}

1. (Facultatif) Dans le créateur de rapports, modifiez les éléments suivants :

   * Colonnes
   * Regroupements
   * Filtres
   * Graphique

   Pour en savoir plus sur ces fonctionnalités, voir [Création d&#39;un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Une fois la création de votre rapport terminée, cliquez sur **Enregistrer + Fermer**.

1. Saisissez un nouveau nom dans le champ **Nom du rapport**, puis cliquez sur **Enregistrer le rapport**.

   Le rapport s’affiche.
