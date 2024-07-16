---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Gérer les licences disponibles dans votre système
description: En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez consulter les informations de votre compte Workfront, y compris le nombre de licences détenues par votre entreprise, ainsi que le nombre de licences en cours d’utilisation.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 834d08d8e9896b80d047d00b2008dd9a002a95da
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 87%

---

# Gérer les licences disponibles dans votre système

<!-- Audited: 12/2023 -->

En tant qu’administrateur ou administratrice d’Adobe Workfront, vous pouvez consulter les informations de votre compte Workfront, y compris le nombre de licences détenues par votre entreprise, ainsi que le nombre de licences en cours d’utilisation.

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
    <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être administrateur système ou administrateur de groupe. L’administrateur du groupe a une vue limitée des informations de licence.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

>[!NOTE]
>
>Les déclarations suivantes s&#39;appliquent uniquement aux nouveaux plans.
>
>Pour le plan Select :
>
>1. Les administrateurs système ne peuvent pas définir de limites pour les groupes d’accueil.
>2. Les administrateurs système ne peuvent afficher que le nombre total de licences utilisées pour tous les groupes d’accueil.
>3. Les administrateurs de groupe ne peuvent pas du tout accéder à la page Licences .
>
>Pour les plans Prime et Ultimate :
>
>1. Les administrateurs système peuvent ajouter des groupes d’accueil à la page Licences pour afficher l’utilisation des licences de ces groupes, et ils peuvent également définir des limites de licence.
>2. Les administrateurs de groupe peuvent accéder à la page Licences et afficher l’utilisation des licences dans les groupes qu’ils gèrent et qui ont été ajoutées à la page Licences par les administrateurs système.
>3. Les administrateurs de groupe ne peuvent pas afficher d’informations pour d’autres groupes d’accueil ni ajouter de maximums.

+++

## Afficher les licences de votre entreprise

Le nombre de licences en cours d’utilisation est automatiquement mis à jour lorsque vous attribuez des niveaux d’accès aux nouveaux utilisateurs et utilisatrices de Workfront. Pour plus d’informations, voir [Ajouter des utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Pour afficher les informations de licence dans votre système :

{{step-1-to-setup}}

1. Au bas du panneau de gauche, cliquez sur **Système** > **Licences**.

   Pour plus d’informations sur les licences répertoriées sur cette page, voir [Vue d’ensemble des licences](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Les licences d’épreuve sont disponibles uniquement pour les clientes et clients qui ont acheté le module complémentaire Workfront Proof payant en plus de leur licence Workfront. Pour plus d’informations sur ce module complémentaire, voir [Workfront Proof : index des articles](../../workfront-proof/workfront-proof.md).

1. (Le cas échéant) Si le message suivant s’affiche : **Pour définir un nombre maximal, vous devez ajouter un groupe principal.**, ajoutez un groupe principal dans votre système, comme expliqué dans la section [Ajouter ou supprimer un groupe principal sur la page Licences](#add-or-remove-a-home-group-to-the-licenses-page) de cet article.

   >[!NOTE]
   >
   >Pour les nouveaux plans, le plan Select n’autorise pas l’administration à afficher les licences par groupe principal. Vous ne pouvez afficher que le nombre total de licences utilisées. Les plans Prime et Ultimate permettent de définir le nombre maximal de licences par groupe principal.

## Afficher les informations sur les licences des modules complémentaires Workfront

Si votre entreprise dispose du module complémentaire Workfront Proof payant, le nombre de licences utilisées et le nombre de licences disponibles s’affichent. Par exemple : **5 des 10 licences d’épreuve** indique que l’organisation utilise actuellement 5 des 10 licences Workfront Proof qu’elle a achetées.

![Licence pour les modules complémentaires Workfront](assets/updated-licenses-page.png)

Si votre entreprise a acheté Objectifs Workfront, les informations de licence de ce produit s’affichent également ici. Dans ce cas, vous pouvez afficher les informations suivantes :

* Nombre total de licences Objectifs Workfront achetées par votre entreprise
* Nombre de licences Objectifs Workfront attribuées aux utilisateurs et utilisatrices Il s’agit du nombre d’utilisateurs et d’utilisatrices qui disposent au moins d’un accès en affichage aux objectifs dans leur niveau d’accès.

Pour plus d’informations sur Objectifs Workfront, consultez la section [Vue d’ensemble d’Adobe Objectifs Workfront](../../workfront-goals/goal-management/wf-goals-overview.md). Pour plus d’informations sur l’accès à Objectifs Workfront, consultez la section [Accorder l’accès à Adobe Objectifs Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

>[!NOTE]
>
>Workfront vous permet d’attribuer plus de licences Objectifs Workfront que votre contrat ne le permet. Cependant, lorsque vous attribuez plus de licences que ce que votre contrat Objectifs Workfront prévoit, une personne gestionnaire de compte Workfront vous contactera pour vous informer que vous avez dépassé le quota de votre contrat.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Les utilisateurs et utilisatrices n’ayant pas d’accès d’administratif peuvent utiliser un rapport Groupe pour afficher le nombre de licences. Dans l&#39;onglet Rapport, créez un rapport de groupe et ajoutez les colonnes suivantes :
>
>* Limite du type de licence : limite pour la licence de travail
>* Limite du type de licence : limite pour la licence de plan
>
>Pour en savoir plus sur la création d’un rapport, consultez la section [Créer un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Afficher les informations sur les allocations mensuelles de décision d’épreuve et de document

>[!IMPORTANT]
>
>Les limites de décision concernant les épreuves et les documents s’appliquent uniquement aux personnes disposant de nouvelles licences. Pour plus d’informations, consultez la section [Vue d’ensemble des licences](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

Les décisions relatives aux épreuves et aux documents sont limitées pour toutes les licences Workfront non payantes. Les limites sont réinitialisées chaque mois pour chaque personne.

Les limites de décision pour chaque licence varient en fonction de votre plan. Vous pouvez afficher votre allocation mensuelle dans Configuration > Licences.

Pour plus d’informations sur les limites de décision pour les épreuves et les documents, consultez la section [Vue d’ensemble du statut de décision limitée des documents et de l’épreuve pour les utilisateurs et utilisatrices non payants](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![Allocation de décision mensuelle](assets/monthly-decision-allotment.png)

## Ajouter ou supprimer un groupe principal sur la page Licences {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

Chaque personne ne peut être affectée qu’à un seul groupe principal. Workfront fournit des licences pour les groupes et calcule le nombre de licences attribuées et actuellement utilisées dans chaque groupe principal.

Si le message suivant s’affiche **Pour définir un nombre maximal, vous devez ajouter un groupe principal.** sur la page Licences , vous devez ajouter au moins un groupe principal à la page Licences.

>[!IMPORTANT]
>
>* Pour gérer efficacement les licences avec les groupes principaux, nous vous recommandons de configurer des groupes principaux spécifiques pour chaque unité opérationnelle avant de mettre à jour le nombre maximal de licences. Pour plus d’informations, consultez la [Vue d’ensemble des groupes principaux](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* Vous pouvez ajouter uniquement des groupes de niveau supérieur en tant que groupes principaux, et non des sous-groupes. Si un sous-groupe est affecté à une personne en tant que groupe principal, sa licence est ajoutée au nombre de licences du groupe de niveau supérieur au sous-groupe en question.
>

Pour ajouter ou supprimer un groupe principal de la page Licences :

{{step-1-to-setup}}

1. Au bas du panneau de gauche, cliquez sur **Système** > **Licences**.

1. Cliquez sur **Gérer la liste de groupes**.
1. Commencez à saisir le nom du groupe de niveau supérieur dans la zone **Groupes principaux**.
1. Pour ajouter le groupe, cliquez sur son nom lorsqu’il apparaît.

   Ou

   Pour supprimer le groupe, cliquez sur l’icône X située à droite de son nom.

1. Cliquer sur **Enregistrer**.

En tant qu’administrateur ou administratrice de Workfront, vous pouvez définir le nombre maximal de licences pour les groupes principaux afin d’empêcher une unité opérationnelle d’utiliser les licences Workfront achetées pour d’autres unités opérationnelles. Pour suivre la procédure, consultez la section [Définir le nombre maximal de licences pour un groupe principal](#set-the-maximum-license-count-for-a-home-group) de cet article.

## Définir le nombre maximal de licences pour les groupes principaux {#set-the-maximum-license-count-for-a-home-group}

En tant qu’administrateur ou administratrice de Workfront, vous pouvez définir le nombre maximal de licences pour les groupes principaux de niveau supérieur de votre système. Cela vous permet d’empêcher une unité opérationnelle d’utiliser des licences Workfront destinées à d’autres unités opérationnelles de votre entreprise.

Par défaut, le nombre maximal de licences est défini sur S/O, ce qui signifie qu’il n’y a aucune limite.

Les administrateurs et administratrices de groupe peuvent afficher le nombre de licences attribuées et utilisées dans un groupe principal qu’ils gèrent. Pour plus d’informations, consultez la section [Afficher le nombre de licences attribuées et utilisées dans un groupe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Pour définir le nombre maximal de licences pour un groupe principal, procédez comme suit :

{{step-1-to-setup}}

1. Au bas du panneau de gauche, cliquez sur **Système** > **Licences**.

1. Recherchez le groupe principal dans la liste.
1. Dans la colonne **Max** du groupe, cliquez sur la valeur pour laquelle vous souhaitez définir un maximum.
1. Saisissez le nombre maximal, puis appuyez sur Entrée.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >Pour rétablir la valeur de licence maximale d’un groupe sur la valeur par défaut, ne saisissez pas 0. Supprimez plutôt le nombre dans la zone. La définition de la valeur de licence maximale sur 0 indique qu’aucune licence n’est allouée à ce groupe.
