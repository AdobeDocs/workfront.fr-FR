---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Partager un tableau de bord
description: Votre administrateur Adobe Workfront autorise les utilisateurs à afficher ou à modifier les tableaux de bord lorsqu’ils attribuent des niveaux d’accès. Outre le niveau d’accès qui est accordé aux utilisateurs, vous pouvez leur accorder des autorisations d’ Affichage ou de Gestion de tableaux de bord spécifiques que vous avez accès au partage.
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 17%

---

# Partager un tableau de bord

Votre administrateur Adobe Workfront autorise les utilisateurs à afficher ou à modifier les tableaux de bord lorsqu’ils attribuent des niveaux d’accès. Pour plus d’informations sur l’octroi de l’accès aux problèmes, voir [Octroi de l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Outre le niveau d’accès qui est accordé aux utilisateurs, vous pouvez leur accorder des autorisations d’ Affichage ou de Gestion de tableaux de bord spécifiques que vous avez accès au partage. Pour plus d’informations sur les niveaux d’accès et les autorisations, voir [Comment les niveaux d’accès et les autorisations fonctionnent ensemble](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.

>[!NOTE]
>
>Un administrateur Workfront peut ajouter ou supprimer des autorisations à n’importe quel élément du système, pour tous les utilisateurs, sans en être le propriétaire.

## Conditions d’accès

Pour partager des objets, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Forfait Adobe Workfront*</strong></td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licence Adobe Workfront*</strong></td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>Afficher l’accès ou une version ultérieure aux Rapports, tableaux de bord et calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Afficher les autorisations ou une version ultérieure du tableau de bord</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Conditions préalables

Le tableau de bord doit être créé avant de pouvoir le partager.

Pour plus d’informations sur la création de tableaux de bord, voir [Création d’un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Observations relatives au partage des tableaux de bord

Outre les considérations ci-dessous, reportez-vous également à la section [Partage de rapports, tableaux de bord et calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Par défaut, le créateur d’un tableau de bord dispose des autorisations Gérer .

* Vous pouvez partager des tableaux de bord que vous créez avec d’autres personnes, équipes, groupes, rôles de travail ou entreprises. Vous pouvez également partager des tableaux de bord créés et qui ont été partagés avec vous.
* Vous pouvez également les partager avec l’ensemble de l’entreprise en la rendant visible à l’échelle du système.
* Vous pouvez partager un tableau de bord individuel ou partager plusieurs tableaux de bord à partir d’une liste.
* Lorsque vous partagez un tableau de bord, les utilisateurs héritent par défaut des autorisations Afficher pour tous les objets de rapport du tableau de bord.

  Pour plus d’informations sur la hiérarchie des objets dans Workfront, voir [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Pour plus d’informations sur l’affichage des autorisations héritées, voir [Affichage des autorisations héritées sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Partager un tableau de bord

Le partage d&#39;un ou de plusieurs tableaux de bord depuis une liste est identique.

1. Accédez à une liste de tableaux de bord et sélectionnez un ou plusieurs tableaux de bord, puis cliquez sur **Partager** ![](assets/share-icon.png).

   Ou

   Cliquez sur le nom d’un tableau de bord, puis sur **Actions du tableau de bord >****Partage**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. Dans le champ **Ajouter des personnes, des équipes, des rôles, des groupes ou des entreprises...**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société avec lequel vous souhaitez partager le tableau de bord, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
1. (Facultatif) Pour rendre le tableau de bord accessible à tous les utilisateurs du système, cliquez sur l’icône **Paramètres** dans le coin supérieur droit de la boîte de dialogue de partage, puis sélectionnez **Rendre ce tableau visible à l’échelle du système**.

1. Cliquer sur **Enregistrer**.
