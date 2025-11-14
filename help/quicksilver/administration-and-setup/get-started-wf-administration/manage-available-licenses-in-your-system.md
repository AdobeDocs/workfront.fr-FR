---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Gestion des licences disponibles dans votre système
description: En tant que membre de l’administration Adobe Workfront, vous pouvez accéder aux informations relatives à votre compte Workfront, y compris le nombre de licences achetées pour votre organisation, et le nombre de ces licences en cours d’utilisation.
author: Lisa, Jenny
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 01a80f6140650ca12aaee14115f79449dcfa2a18
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 97%

---

# Gérer les licences disponibles dans votre système

<!-- Audited: 12/2023 -->

En tant que membre de l’administration Adobe Workfront, vous pouvez accéder aux informations relatives à votre compte Workfront, y compris le nombre de licences achetées pour votre organisation, et le nombre de ces licences en cours d’utilisation.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur ou une administratrice Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


>[!NOTE]
>
>Les instructions suivantes s’appliquent aux packages Select, Prime et Ultimate.
>
>Pour le package Select :
>
>1. Les administrateurs et administratrices système ne peuvent pas définir de limites pour les groupes principaux.
>2. Les administrateurs et administratrices système ne peuvent afficher que le nombre total de licences utilisées par tous les groupes principaux.
>3. Les administrateurs et administratrices de groupes ne peuvent pas du tout accéder à la page Licences.
>
>Pour les packages Prime et Ultimate :
>
>1. Les administrateurs et administratrices système peuvent ajouter des groupes principaux à la page Licences pour afficher l’utilisation des licences de ces groupes. Ils peuvent également définir des limites de licence.
>2. Les administrateurs et administratrices de groupes peuvent accéder à la page Licences et afficher l’utilisation des licences dans les groupes qu’ils gèrent et qui ont été ajoutées à la page Licences par les administrateurs et administratrices système.
>3. Les administrateurs et administratrices de groupes ne peuvent pas afficher d’informations pour d’autres groupes principaux ni ajouter de nombres maximum.

+++

## Afficher les licences de votre organisation

Le nombre de licences utilisées se met à jour automatiquement au fur et à mesure que vous accordez des niveaux d’accès aux utilisateurs et aux utilisatrices que vous ajoutez à Workfront. Pour plus d’informations, voir [Ajouter des utilisateurs et des utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Pour afficher les informations relatives aux licences dans votre système :

{{step-1-to-setup}}

1. En bas du panneau de gauche, cliquez sur **Système** > **Licenses**.

   Pour plus d’informations sur les licences répertoriées sur cette page, voir [Vue d’ensemble des licences](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Les licences Proof ne sont disponibles que pour les clientes et les clients qui ont acheté le module complémentaire payant Workfront Proof en plus de leur licence Workfront. Pour plus d’informations sur ce module complémentaire, voir [Workfront Proof : index des articles](../../workfront-proof/workfront-proof.md).

1. (Le cas échéant) Si le message suivant s’affiche : **Pour définir un nombre maximal, vous devez ajouter un groupe principal.**, ajoutez un groupe principal dans votre système, comme expliqué dans la section [Ajouter ou supprimer un groupe principal sur la page Licences](#add-or-remove-a-home-group-to-the-licenses-page) de cet article.

   >[!NOTE]
   >
   >Pour les nouveaux plans, le plan Select n’autorise pas l’administration à afficher les licences par groupe principal. Vous ne pouvez afficher que le nombre total de licences utilisées. Les plans Prime et Ultimate permettent de définir le nombre maximal de licences par groupe principal.

## Afficher les informations sur les licences des modules complémentaires Workfront

Si votre organisation dispose du module complémentaire payant Workfront Proof, le nombre de licences utilisées et le nombre de licences disponibles sont affichés. Par exemple, **5 des 10 licences Proof** indique que l’organisation utilise actuellement 5 des 10 licences de Workfront Proof qu’elle a achetées.

![Licence pour les modules complémentaires de Workfront](assets/updated-licenses-page.png)

Si votre organisation a acheté Objectifs de Workfront, les informations relatives à la licence de ce produit s’affichent également ici. Dans ce cas, vous pouvez afficher les informations suivantes :

* Nombre total de licences Objectifs Workfront achetées par votre entreprise.
* Nombre de licences Objectifs Workfront associées aux utilisateurs et utilisatrices. Il s’agit du nombre d’utilisateurs et d’utilisatrices à qui accorder au moins l’accès Afficher à Objectifs dans leur niveau d’accès.

Pour plus d’informations sur Objectifs Workfront, voir [Vue d’ensemble d’Objectifs Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md). Pour plus d’informations sur l’accès à Objectifs Workfront, voir [Accorder l’accès à Objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

>[!NOTE]
>
>Workfront vous permet d’attribuer plus de licences Objectifs Workfront que celles que vous avez achetées. Cependant, si vous attribuez plus de licences que ce que votre contrat Objectifs Workfront autorise, une personne responsable de votre compte Workfront vous contactera pour vous informer que votre nombre contractuel est dépassé.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Les utilisateurs et les utilisatrices qui n’ont pas d’accès administratif peuvent utiliser un rapport sur les groupes pour afficher le nombre de licences. Dans l’onglet des rapports, créez un nouveau rapport sur les groupes et ajoutez les colonnes suivantes :
>
>* Limite du type de licence : limite du nombre de travailleurs
>* Limite du type de licence : limite du planificateur
>
>Pour en savoir plus sur la création d’un rapport, voir [Créer un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Afficher les informations sur les attributions mensuelles d’épreuves et de décisions relatives aux documents

>[!IMPORTANT]
>
>Les limites de décision en matière d’épreuves et de documents ne s’appliquent qu’aux utilisateurs et utilisatrices des nouvelles licences. Pour plus d’informations, voir [Vue d’ensemble des nouvelles licences](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

Les décisions concernant les épreuves et les documents sont limitées pour toutes les licences Workfront non payantes. Limites réinitialisées chaque mois selon l’utilisateur ou l’utilisatrice.

Les limites de décision pour chaque licence varient en fonction de votre formule. Vous pouvez afficher votre allocation mensuelle dans Configuration > Licences.

Pour plus d’informations sur les limites de décision en matière d’épreuves et de document, voir [Vue d’ensemble du statut de décision limitée des documents et de l’épreuve pour les utilisateurs et utilisatrices non payants](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![Allocation de décision mensuelle](assets/monthly-decision-allotment.png)

## Ajouter ou supprimer un groupe principal à la page des licences {#add-or-remove-a-home-group-to-the-licenses-page}

Chaque utilisateur ou utilisatrice ne peut être affecté qu’à un seul groupe principal. Workfront fournit un nombre de licences orienté groupe en calculant le nombre de licences allouées et actuellement utilisées dans chaque groupe principal.

Si vous voyez le message **Pour définir un maximum, vous devez ajouter un groupe principal** sur la page des licences, vous devez ajouter au moins un groupe principal sur la page des licences.

>[!IMPORTANT]
>
>* Pour gérer efficacement les licences avec les groupes principaux, nous recommandons de configurer des groupes principaux spécifiques pour les unités commerciales avant de mettre à jour le nombre maximum de licences. Pour plus d’informations, voir [Vue d’ensemble des groupes principaux](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* Vous ne pouvez ajouter que des groupes de niveau supérieur en tant que groupes principaux et non des sous-groupes. Si un sous-groupe est attribué à un utilisateur ou une utilisatrice en tant que groupe principal, sa licence est ajoutée au nombre de licences du groupe de niveau supérieur à ce sous-groupe.
>

Pour ajouter ou supprimer un groupe principal à la page des licences :

{{step-1-to-setup}}

1. En bas du panneau de gauche, cliquez sur **Système** > **Licences**.

1. Cliquez sur **Gérer la liste de groupes**.
1. Commencez à saisir le nom du groupe de niveau supérieur dans la zone **Groupes principaux**.
1. Pour ajouter le groupe, cliquez sur son nom lorsqu’il apparaît.

   Ou

   Pour supprimer le groupe, cliquez sur l’icône X à droite de son nom.

1. Cliquer sur **Enregistrer**.

En tant qu’administrateur ou administratrice Workfront, vous pouvez définir un nombre maximum de licences pour les groupes principaux afin d’empêcher une unité commerciale d’utiliser des licences Workfront achetées pour d’autres unités commerciales. Pour obtenir des instructions, voir [Définir le nombre maximum de licences pour un groupe principal](#set-the-maximum-license-count-for-a-home-group) dans cet article.

## Définir le nombre maximum de licences pour un groupe principal {#set-the-maximum-license-count-for-a-home-group}

En tant qu’administrateur ou administratrice Workfront, vous pouvez définir le nombre maximum de licences pour les groupes principaux de niveau supérieur de votre système. Cela vous permet d’empêcher une unité commerciale d’utiliser des licences Workfront achetées pour d’autres unités commerciales au sein de votre organisation.

Par défaut, le nombre maximum de licences est défini sur N/A, ce qui signifie qu’il n’y a pas de limite.

Les administrateurs et administratrices de groupes peuvent consulter le nombre de licences attribuées et utilisées dans un groupe principal qu’ils gèrent. Pour plus d’informations, voir [Afficher le nombre de licences attribuées et utilisées dans un groupe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Pour définir le nombre maximum de licences pour un groupe principal, procédez comme suit :

{{step-1-to-setup}}

1. En bas du panneau de gauche, cliquez sur **Système** > **Licences**.

1. Localisez le groupe principal dans la liste.
1. Dans la colonne **Max** du groupe, cliquez sur la valeur pour laquelle vous souhaitez définir un maximum.
1. Saisissez le nombre maximum, puis appuyez sur Entrée.

   ![Nombre maximal de licences pour le groupe](assets/updated-max.png)

   >[!NOTE]
   >
   >Pour rétablir la valeur par défaut de la licence maximale d’un groupe, ne saisissez pas 0. Au lieu de cela, supprimez le numéro dans la case. Si la valeur maximale de la licence est définie sur 0, cela signifie qu’aucune licence n’a été attribuée à ce groupe.
