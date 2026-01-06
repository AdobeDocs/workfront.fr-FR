---
title: Partager un portfolio
description: Vous pouvez partager un portfolio avec d’autres personnes si vous disposez des autorisations nécessaires pour y accéder.
author: Courtney
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 46%

---

# Partager un portfolio

Votre administrateur ou administratrice Adobe Workfront peut vous accorder l’accès en afichage ou en modification aux portfolios lors de l’attribution de votre niveau d’accès. Vous devez disposer d’une licence de plan pour avoir accès à la modification d’un portfolio. Pour plus d’informations, voir [Accorder l’accès aux portfolios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

En plus du niveau d’accès qui vous est accordé, vous pouvez également recevoir des autorisations pour consulter ou gérer des portfolios spécifiques de la part de personnes qui peuvent les partager avec vous. Pour plus d’informations sur les niveaux d’accès et les autorisations, voir [Comment les niveaux d’accès et les autorisations fonctionnent ensemble](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Les autorisations sont spécifiques à un élément de Workfront et définissent les actions que les personnes peuvent entreprendre sur cet élément.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Travail ou supérieur</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou supérieur aux objets que vous souhaitez partager.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures pour les objets que vous souhaitez partager.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations sur le partage des portfolios

Outre les considérations ci-dessous, voir également [Vue d’ensemble des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Une équipe d’administration Workfront peut ajouter ou supprimer des autorisations à tous les éléments du système, pour toutes les personnes, sans être la personne propriétaire de ces éléments.

* Le créateur d’un portfolio dispose par défaut des autorisations de niveau Gérer .
* Vous pouvez partager un portfolio individuellement ou plusieurs portfolios en même temps. Le partage d’un portfolio est identique au partage d’autres objets dans Workfront. Pour plus d’informations, voir [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Vous ne pouvez accorder des droits d’affichage ou de gestion qu’aux portfolios.
</span>
* Lorsque vous partagez un portfolio, les utilisateurs héritent par défaut des mêmes autorisations pour tous les objets enfants associés au portfolio.

Pour plus d’informations sur la hiérarchie des objets dans Workfront, voir [Comprendre les objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Vous pouvez supprimer les autorisations héritées du portfolio. Pour plus d’informations sur la suppression des autorisations sur les objets, voir [Supprimer les autorisations sur les objets](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Partager un portfolio

{{step1-to-portfolios}}

1. Sur la page **Portfolios**, sélectionnez le portfolio que vous souhaitez partager. La page du portfolio s’ouvre.

1. À droite du nom du portefeuille, cliquez sur **Partager**. La boîte de dialogue **Partager [Portfolio Name]** s’ouvre.

   ![Bouton Partager le portfolio](assets/share-portfolio-button.png)

1. Dans le champ **Accorder l’accès au portefeuille à**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société avec lequel vous souhaitez partager le portefeuille, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!TIP]
   >
   >Vous pouvez uniquement partager un portfolio avec des utilisateurs actifs, des équipes, des rôles ou des entreprises.


1. (Facultatif) Sélectionnez le menu déroulant **Qui a accès** et sélectionnez le niveau d’accès du portefeuille :

   * **Seules les personnes invitées peuvent y accéder :** seuls les utilisateurs invités au portfolio peuvent y accéder (par défaut).
   * **Tout le monde peut afficher dans le système** : tous les utilisateurs du système peuvent afficher le portfolio sans invitation.

1. Cliquez sur la liste déroulante située à droite du nom de l’utilisateur et sélectionnez son niveau d’autorisation pour ce portfolio :

   * **Afficher** : l’utilisateur peut consulter et partager le portfolio.
   * **Gérer** : l’utilisateur dispose d’un accès complet au portfolio sans droits d’administration, qui sont accordés au niveau d’accès (inclut également toutes les autorisations d’affichage).

1. (Facultatif) Cliquez sur l’icône des options avancées en regard du niveau d’autorisation que vous avez accordé pour configurer des autorisations spécifiques sur le portfolio.

   ![Options d’autorisation avancées configurées](assets/advanced-options-icon.png)

1. (Facultatif) Pour partager rapidement le portfolio à l’aide d’un lien, cliquez sur **Copier le lien** puis transférez-le au destinataire.

1. Cliquer sur **Enregistrer**.

## Partage de portefeuilles en bloc

{{step1-to-portfolios}}

1. Sur la page **Portfolios**, sélectionnez la case à gauche de chaque portfolio à partager, puis cliquez sur l’icône **Partager** ![Icône Partager](assets/share-icon.png) en haut de la page. La boîte de dialogue modale de partage s’ouvre.

   ![Portefeuilles d’actions en masse](assets/bulk-share-portfolios.png)

1. Dans le champ **Accorder l’accès au portefeuille à**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société avec lequel vous souhaitez partager les portefeuilles, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

   >[!TIP]
   >
   >Vous pouvez uniquement partager des portefeuilles avec des utilisateurs actifs, des équipes, des rôles ou des entreprises.


1. (Facultatif) Sélectionnez le menu déroulant **Qui a accès** et sélectionnez le niveau d’accès du portefeuille :

   * **Seules les personnes invitées peuvent y accéder :** seuls les utilisateurs invités dans les portefeuilles peuvent y accéder (par défaut).
   * **Tous les utilisateurs du système peuvent afficher** : tous les utilisateurs du système peuvent afficher les portfolios sans invitation.


1. Cliquez sur la liste déroulante située à droite du nom de l’utilisateur et sélectionnez son niveau d’autorisation pour les portefeuilles :

   * **Afficher** : l’utilisateur peut consulter et partager les portfolios.
   * **Gérer** : l’utilisateur dispose d’un accès complet aux portefeuilles sans droits d’administration, qui sont accordés au niveau d’accès (inclut également toutes les autorisations d’affichage).

1. (Facultatif) Cliquez sur l’icône des options avancées en regard du niveau d’autorisation que vous avez accordé pour configurer des autorisations spécifiques sur les portefeuilles.

   ![Options d’autorisation avancées configurées](assets/advanced-options-icon.png)

1. Cliquer sur **Enregistrer**.


## Autorisations pour les portfolios

Le tableau suivant indique les autorisations que vous pouvez accorder aux personnes lorsque vous les autorisez à afficher ou à gérer un portfolio :

| **Actions** | **Gérer** | **Afficher** |
|---|---|---|
| Modifier les détails du portfolio | ✓ |   |
| Afficher un portfolio | ✓ | ✓ |
| Supprimer un portfolio | ✓ |   |
| Joindre un formulaire personnalisé | ✓ |   |
| Modifier un champ personnalisé | ✓ |   |
| Ajouter ou supprimer un programme&#42; | ✓ |   |
| Ajouter ou supprimer un projet&#42; | ✓ |   |
| Approuver un projet | ✓ |   |
| Optimisation du portfolio&#42; | ✓ |   |
| Ajouter un dossier de documents&#42; | ✓ | ✓ |
| Ajouter un document | ✓ | ✓ |
| Mises à jour / commentaires | ✓ | ✓ |
| Partager | ✓ | ✓ |
| Partager sur le système |   | ✓ |

* Ces autorisations sont contrôlées par le niveau d’accès et les autorisations sur d’autres objets, comme les projets, les programmes, les documents.
