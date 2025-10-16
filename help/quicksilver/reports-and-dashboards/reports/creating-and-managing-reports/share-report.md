---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Partager un rapport dans Adobe Workfront
description: Votre administrateur ou administratrice Adobe Workfront accorde aux utilisateurs et utilisatrices l’accès à l’affichage ou à la modification des rapports lorsque des niveaux d’accès leur sont attribués. Pour plus d’informations sur l’octroi d’un accès aux problèmes, voir Accorder l’accès aux rapports, tableaux de bord et calendriers.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 72%

---

# Partager un rapport dans Adobe Workfront

<!-- Audited: 11/2024 -->

Votre administrateur ou administratrice Adobe Workfront accorde aux utilisateurs et utilisatrices l’accès à l’affichage ou à la modification des rapports lorsque des niveaux d’accès leur sont attribués. Pour plus d’informations sur l’octroi d’un accès aux problèmes, voir [Accorder l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

En plus du niveau d’accès accordé aux utilisateurs et utilisatrices, vous pouvez également leur accorder des autorisations pour afficher ou gérer des rapports spécifiques que vous pouvez partager. Pour plus d’informations sur les niveaux d’accès et les autorisations, voir [Comment les niveaux d’accès et les autorisations fonctionnent ensemble](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.

>[!NOTE]
>
>Une équipe d’administration Workfront peut ajouter ou supprimer des autorisations à tous les éléments du système, pour toutes les personnes, sans être la personne propriétaire de ces éléments.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
      <p>Léger</p>
      <p>Vérifier</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Afficher l'accès ou supérieur aux rapports, tableaux de bord, calendriers</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures pour le rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Remarques sur le partage de rapports

Outre les considérations ci-dessous, voir également [Partager des rapports, des tableaux de bord et des calendriers](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Vous pouvez partager des rapports que vous créez avec d’autres personnes, équipes, groupes, fonctions ou entreprises. Vous pouvez également partager des rapports que d’autres personnes ont créés et qui ont été partagés avec vous.
* Vous pouvez également les partager avec l’ensemble de votre organisation ou les rendre publics. Rendre un rapport public génère une URL qui peut être partagée avec d’autres personnes.
* Vous pouvez partager un rapport individuel ou plusieurs rapports d’une liste de rapports.

## Façons de partager des rapports

Vous pouvez partager des rapports dans Workfront de la manière suivante :

* Manuellement, comme décrit dans la section [Partager un rapport](#share-a-report) ci-dessous.
* Automatiquement, en héritant des autorisations Afficher d’un tableau de bord qui contient le rapport qui a été partagé. Pour plus d’informations sur l’affichage des autorisations héritées sur les objets, voir [Afficher les autorisations héritées sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Partager un rapport {#share-a-report}

Le partage d’un ou de plusieurs rapports d’une liste est identique.

1. Accédez à la liste des rapports et sélectionnez un ou plusieurs rapports, puis cliquez sur **Partager**.

   Ou

   Cliquez sur le nom d’un rapport, puis sur **Actions du rapport >****Partage**.

   ![](assets/unshimmed-report-actions-sharing.png)

1. Dans la zone qui s’affiche, dans le champ **Ajouter des personnes, des équipes, des rôles, des groupes ou des entreprises...**, commencez à saisir le nom de la personne, de l’équipe, de la fonction, du groupe ou de l’entreprise avec lequel vous souhaitez partager le rapport, puis appuyez sur **Entrée** lorsque le nom s’affiche.

1. Pour ajuster le niveau d’accès d’un nom que vous avez ajouté, cliquez sur le menu déroulant à droite du nom, puis choisissez l’une des options ci-dessous.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">L'afficher</td> 
      <td> <p>Permet à votre destinataire d'accéder au rapport dans la zone <strong>Rapports</strong> et de l'exécuter.</p> <p>Vous pouvez cliquer sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que les utilisateurs et les utilisatrices puissent le <strong>Partager</strong> avec n’importe qui dans le système.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le gérer</td> 
      <td> <p>Permet à la personne destinataire de disposer d’un accès complet en modification au rapport.</p> <p>Vous pouvez cliquer sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que les utilisateurs et les utilisatrices puissent <strong>Supprimer</strong> le rapport du système et le <strong>Partager</strong> avec n’importe qui dans le système.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez les 2 étapes précédentes pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Cliquez sur le menu déroulant **Seules les personnes invitées peuvent accéder** dans la zone de partage, puis choisissez entre les options suivantes :

   * **Seules les personnes invitées peuvent y accéder** Sélectionnez cette option afin que seuls les utilisateurs et utilisatrices ayant obtenu l’accès au rapport puissent l’afficher.

   * **Tout le monde peut afficher le rapport dans le système** Sélectionnez cette option pour que tous les utilisateurs de Workfront ayant accès aux rapports puissent les afficher.

1. (Facultatif) Cliquez sur l’icône **Engrenage** ![Paramètres de l’icône d’engrenage](assets/gear-icon-settings-with-dn-arrow.jpg) dans le coin supérieur droit de la zone de partage, puis sélectionnez éventuellement l’option suivante :

   * **Rendre ceci public pour les utilisateurs externes** Sélectionnez cette option pour générer une URL qui peut être partagée avec d’autres utilisateurs. Toute personne disposant de l’URL peut accéder au rapport, sans posséder de licence Adobe Workfront.

     >[!CAUTION]
     >
     >Nous avisons la prudence lors du partage d’un objet contenant des informations confidentielles avec des utilisateurs et utilisatrices externes. Cette fonction leur permet d’afficher des informations sans être un utilisateur ou une utilisatrice Workfront ou une personne membre de votre organisation.

     >[!NOTE]
     >
     >Si le rapport comporte une invite et que vous le partagez publiquement, les utilisateurs qui exécutent le rapport par le biais du lien de partage public ne pourront pas exécuter le rapport à l’aide de l’invite. Elles verront le rapport sans l’invite qui lui est appliquée, sauf si elles se connectent à Workfront et accèdent au rapport sans utiliser le lien de partage public. Pour plus d’informations sur les limites du partage de rapports avec des invites, consultez la section [Limitations du partage de rapports avec invite](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) dans l’article [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Cliquer sur **Enregistrer**.
