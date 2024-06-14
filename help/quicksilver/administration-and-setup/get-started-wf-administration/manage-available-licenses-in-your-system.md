---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Gérer les licences disponibles dans votre système
description: En tant qu’administrateur Adobe Workfront, vous pouvez accéder aux informations sur votre compte Workfront, y compris le nombre de licences achetées pour votre entreprise, ainsi que le nombre de licences en cours d’utilisation.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '1198'
ht-degree: 4%

---

# Gérer les licences disponibles dans votre système

<!-- Audited: 12/2023 -->

En tant qu’administrateur Adobe Workfront, vous pouvez accéder aux informations sur votre compte Workfront, y compris le nombre de licences achetées pour votre entreprise, ainsi que le nombre de licences en cours d’utilisation.

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
    <p>Nouveau : Standard</p>
    <p>ou</p>
    <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> </td> 
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

## Affichage des licences de votre entreprise

Le nombre de licences en cours d’utilisation est automatiquement mis à jour lorsque vous attribuez des niveaux d’accès aux utilisateurs que vous ajoutez à Workfront. Pour plus d’informations, voir [Ajout d’utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Pour afficher les informations de licence dans votre système :

{{step-1-to-setup}}

1. Au bas du panneau de gauche, cliquez sur **Système** > **Licences**.

   Pour plus d’informations sur les licences répertoriées sur cette page, voir [Présentation des licences](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Les licences de BAT sont disponibles uniquement pour les clients qui ont acheté le module complémentaire Workfront Proof payant en plus de leur licence Workfront. Pour plus d’informations sur ce module complémentaire, voir [Workfront Proof : index des articles](../../workfront-proof/workfront-proof.md).

1. (Conditionnel) Si le message s’affiche **Pour définir un maximum, vous devez ajouter un groupe d’accueil.**, ajoutez un groupe d’accueil dans votre système, comme expliqué dans la section . [Ajout ou suppression d’un groupe d’accueil sur la page Licences](#add-or-remove-a-home-group-to-the-licenses-page) dans cet article.

   >[!NOTE]
   >
   >Pour les nouveaux plans, le plan Sélectionner n’autorise pas les administrateurs à afficher les licences par groupe d’accueil. Vous ne pouvez afficher que le nombre total de licences utilisées. Les plans Prime et Ultimate permettent de définir le nombre maximum de licences par groupe d’accueil.

## Affichage des informations sur les licences des modules complémentaires Workfront

Si votre entreprise dispose du module complémentaire Workfront Proof payant, le nombre de licences utilisées et le nombre de licences disponibles s’affichent. Par exemple : **5 sur 10 licences de BAT** indique que l’organisation utilise actuellement 5 des 10 licences Workfront Proof qu’elle a achetées.

![Licence pour les modules complémentaires Workfront](assets/updated-licenses-page.png)

Si votre entreprise a acheté les objectifs Workfront, les informations de licence de ce produit s’affichent également ici. Dans ce cas, vous pouvez afficher les informations suivantes :

* Nombre total de licences Workfront Goals achetées par votre entreprise.
* Nombre de licences Workfront Goals associées aux utilisateurs. Il s’agit du nombre d’utilisateurs à qui accorder au moins l’accès Afficher aux objectifs à leur niveau d’accès.

Pour plus d’informations sur les objectifs de Workfront, voir [Présentation des objectifs d’Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md). Pour plus d’informations sur l’accès aux objectifs Workfront, voir [Accorder l’accès aux objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

>[!NOTE]
>
>Workfront vous permet d’attribuer d’autres licences Workfront Goals que vous avez achetées. Cependant, lorsque vous attribuez plus de licences que ce que votre contrat avec les objectifs de Workfront autorise, un gestionnaire de compte Workfront vous contactera pour vous informer que vous avez dépassé votre numéro contractuel.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Les utilisateurs n’ayant pas d’accès administrateur peuvent utiliser un rapport Groupe pour afficher le nombre de licences. Dans l&#39;onglet Rapport , créez un rapport de groupe et ajoutez les colonnes suivantes :
>
>* Limite du type de licence : limite du traitement
>* Limite de type de licence : limite du planificateur
>
>Pour en savoir plus sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Affichage d’informations sur les allocations mensuelles de BAT et de décision de document

>[!IMPORTANT]
>
>Les limites de décision concernant les BAT et les documents s’appliquent uniquement aux utilisateurs disposant de nouvelles licences. Pour plus d’informations, voir [Présentation des nouvelles licences](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

Les décisions relatives aux BAT et aux documents sont limitées pour toutes les licences Workfront non payantes. Limites réinitialisées chaque mois selon l’utilisateur.

Les limites de décision pour chaque licence varient en fonction du plan sur lequel vous travaillez. Vous pouvez afficher votre allocation mensuelle dans Configuration > Licences.

Pour plus d’informations sur les limites de décision des BAT et des documents, voir [Présentation des documents et des BAT limités pour les utilisateurs non payants](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![Allocations de décision mensuelles](assets/monthly-decision-allotment.png)

## Ajout ou suppression d’un groupe d’accueil sur la page Licences {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

Chaque utilisateur ne peut être affecté qu’à un seul groupe d’accueil. Workfront fournit un nombre de licences orientées groupe en calculant le nombre de licences attribuées et actuellement utilisées dans chaque groupe d’accueil.

Si le message s’affiche **Pour définir un maximum, vous devez ajouter un groupe d’accueil.** sur la page Licences , vous devez ajouter au moins un groupe d’accueil à la page Licences .

>[!IMPORTANT]
>
>* Pour gérer efficacement les licences avec les groupes d’accueil, nous vous recommandons de configurer des groupes d’accueil spécifiques pour les unités opérationnelles avant de mettre à jour le nombre maximal de licences. Pour plus d’informations, voir [Présentation des groupes d’accueil](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* Vous pouvez ajouter uniquement des groupes de niveau supérieur en tant que groupes d’accueil, et non des sous-groupes. Si un sous-groupe est affecté à un utilisateur comme groupe d’accueil, sa licence est ajoutée au nombre de licences du groupe de niveau supérieur au sous-groupe en question.
>

Pour ajouter ou supprimer un groupe d’accueil à la page Licences :

{{step-1-to-setup}}

1. Au bas du panneau de gauche, cliquez sur **Système** > **Licences**.

1. Cliquez sur **Gérer la liste des groupes**.
1. Commencez à saisir le nom du groupe de niveau supérieur dans le champ **Groupes d’accueil** de la boîte.
1. Pour ajouter le groupe, cliquez sur son nom lorsqu’il apparaît.

   Ou

   Pour supprimer le groupe, cliquez sur l’icône X située à droite de son nom.

1. Cliquer sur **Enregistrer**.

En tant qu’administrateur Workfront, vous pouvez définir le nombre maximal de licences pour les groupes d’accueil afin d’empêcher une unité opérationnelle d’utiliser les licences Workfront achetées pour d’autres unités opérationnelles. Pour obtenir des instructions, voir [Définition du nombre maximal de licences pour un groupe d’accueil](#set-the-maximum-license-count-for-a-home-group) dans cet article.

## Définition du nombre maximal de licences pour un groupe d’accueil {#set-the-maximum-license-count-for-a-home-group}

En tant qu’administrateur de Workfront, vous pouvez définir le nombre maximal de licences pour les groupes d’accueil de niveau supérieur de votre système. Cela vous permet d’empêcher une unité opérationnelle d’utiliser des licences Workfront achetées pour d’autres unités opérationnelles de votre entreprise.

Par défaut, le nombre maximal de licences est défini sur N/A, ce qui signifie qu’il n’y a aucune limite.

Les administrateurs de groupe peuvent afficher le nombre de licences attribuées et utilisées dans un groupe d’accueil qu’ils gèrent. Pour plus d’informations, voir [Afficher le nombre de licences attribuées et utilisées dans un groupe](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Pour définir le nombre maximal de licences pour un groupe d’accueil :

{{step-1-to-setup}}

1. Au bas du panneau de gauche, cliquez sur **Système** > **Licences**.

1. Recherchez le Groupe d’accueil dans la liste.
1. Dans le **Max** du groupe, cliquez sur la valeur pour laquelle vous souhaitez définir un maximum.
1. Saisissez le nombre maximal, puis appuyez sur Entrée.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >Pour rétablir la valeur de licence maximale d’un groupe sur la valeur par défaut, ne saisissez pas 0. Supprimez plutôt le numéro dans la zone. La définition de la valeur de licence maximale sur 0 indique qu’aucune licence n’est allouée à ce groupe.
