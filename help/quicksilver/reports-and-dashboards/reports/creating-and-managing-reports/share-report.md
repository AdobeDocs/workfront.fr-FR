---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Partager un rapport dans Adobe Workfront
description: Votre administrateur ou administratrice Adobe Workfront accorde aux utilisateurs et utilisatrices l’accès à l’affichage ou à la modification des rapports lorsque des niveaux d’accès leur sont attribués. Pour plus d’informations sur l’octroi d’un accès aux problèmes, voir Accorder l’accès aux rapports, tableaux de bord et calendriers.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 100%

---

# Partager un rapport dans Adobe Workfront

Votre administrateur ou administratrice Adobe Workfront accorde aux utilisateurs et utilisatrices l’accès à l’affichage ou à la modification des rapports lorsque des niveaux d’accès leur sont attribués. Pour plus d’informations sur l’octroi d’un accès aux problèmes, voir [Accorder l’accès aux rapports, tableaux de bord et calendriers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

En plus du niveau d’accès accordé aux utilisateurs et utilisatrices, vous pouvez également leur accorder des autorisations pour afficher ou gérer des rapports spécifiques que vous pouvez partager. Pour plus d’informations sur les niveaux d’accès et les autorisations, voir [Comment les niveaux d’accès et les autorisations fonctionnent ensemble](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Les autorisations sont spécifiques à un élément dans Workfront et définissent les actions que vous pouvez effectuer sur cet élément.

>[!NOTE]
>
>Une équipe d’administration Workfront peut ajouter ou supprimer des autorisations à tous les éléments du système, pour toutes les personnes, sans être la personne propriétaire de ces éléments.

## Conditions d’accès

Pour partager des objets, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en affichage ou supérieur aux rapports, tableaux de bord et calendriers</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Afficher ou supérieures sur le rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

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

   ![](assets/qs-report-actions-sharing.png)

1. Dans la zone qui s’affiche, dans le champ **Ajouter des personnes, des équipes, des rôles, des groupes ou des entreprises...**, commencez à saisir le nom de la personne, de l’équipe, de la fonction, du groupe ou de l’entreprise avec lequel vous souhaitez partager le rapport, puis appuyez sur **Entrée** lorsque le nom s’affiche.

1. Pour ajuster le niveau d’accès d’un nom que vous avez ajouté, cliquez sur le menu déroulant à droite du nom, puis choisissez l’une des options ci-dessous.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">L'afficher</td> 
      <td> <p>Permet à la personne destinataire de visualiser le rapport dans la zone <strong>Rapports</strong> <img src="assets/reports-in-main-menu.png"> et de l’exécuter.</p> <p>Vous pouvez cliquer sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que les utilisateurs et les utilisatrices puissent le <strong>Partager</strong> avec n’importe qui dans le système.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le gérer</td> 
      <td> <p>Permet à la personne destinataire de disposer d’un accès complet en modification au rapport.</p> <p>Vous pouvez cliquer sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez que les utilisateurs et les utilisatrices puissent <strong>Supprimer</strong> le rapport du système et le <strong>Partager</strong> avec n’importe qui dans le système.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez les 2 étapes précédentes pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Cliquez sur l’icône **Engrenage** ![](assets/gear-icon-settings-with-dn-arrow.jpg) dans le coin supérieur droit de la zone de partage, puis sélectionnez l’une des options suivantes :

   * **Rendre public pour les utilisateurs et utilisatrices externes :** sélectionnez cette option pour générer une URL qui peut être partagée avec d’autres personnes. Toute personne disposant de l’URL peut accéder au rapport, sans posséder de licence Adobe Workfront.

     >[!CAUTION]
     >
     >Nous avisons la prudence lors du partage d’un objet contenant des informations confidentielles avec des utilisateurs et utilisatrices externes. Cette fonction leur permet d’afficher des informations sans être un utilisateur ou une utilisatrice Workfront ou une personne membre de votre organisation.

     >[!NOTE]
     >
     >Si le rapport comporte une invite que vous partagez publiquement, les personnes qui l’exécutent doivent être connectées à Workfront pour pouvoir exécuter le rapport à l’aide de l’invite. Si elles ne peuvent pas se connecter à Workfront, le rapport s’affiche sans l’invite. Pour plus d’informations sur les limites du partage des rapports avec des invites, consultez la section . [Limites du partage des rapports contenant des invites](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) dans l’article [Ajouter une invite à un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **Rendre visible à l’échelle du système :** sélectionnez cette option pour que tous les utilisateurs et utilisatrices de Workfront ayant accès aux rapports puissent voir le rapport.

1. Cliquer sur **Enregistrer**.
