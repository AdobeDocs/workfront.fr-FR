---
product-area: resource-management
navigation-topic: resource-planning
title: Partager la vue utilisateur ou utilisatrice du planificateur de ressources à l’aide d’un lien
description: Adobe Workfront peut générer une URL unique pour la vue utilisateur du planificateur de ressources que vous pouvez incorporer dans un tableau de bord en tant que page externe ou l’ouvrir séparément dans un nouvel onglet du navigateur. Cela s’avère utile lors du partage des informations du planificateur de ressources avec les utilisateurs qui ne disposent pas d’un accès direct à la zone Ressource.
author: Alina
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 15%

---

# Partager la vue utilisateur ou utilisatrice du planificateur de ressources à l’aide d’un lien

Adobe Workfront peut générer une URL unique pour la vue utilisateur du planificateur de ressources que vous pouvez incorporer dans un tableau de bord en tant que page externe ou l’ouvrir séparément dans un nouvel onglet du navigateur. Cela s’avère utile lors du partage des informations du planificateur de ressources avec les utilisateurs qui ne disposent pas d’un accès direct à la zone Ressource.

![](assets/rp-user-view-with-link-highlight-350x49.png)

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Affichage ou accès supérieur à la gestion des ressources, aux projets et aux utilisateurs</p> <p>Afficher l’accès aux données financières pour afficher les informations de coût </p> <p><b>REMARQUE</b> Si vous n’y avez toujours pas accès, demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice de Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage ou autorisations supérieures des projets que vous souhaitez afficher dans le planificateur de ressources</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.


Tenez compte de ce qui suit lors de la génération de l’URL unique pour la vue utilisateur du planificateur de ressources :

* Vous pouvez obtenir une URL unique uniquement pour la vue utilisateur. L’option de génération de l’URL n’existe pas dans les vues de projet ou de rôle.
* Vous pouvez partager l’URL avec d’autres utilisateurs, y compris les utilisateurs sous licence Work and Review.\
  Ils doivent avoir accès à l’affichage d’autres utilisateurs afin d’afficher les informations du planificateur de ressources à partir de l’URL que vous partagez avec eux.
* Les informations suivantes sont enregistrées lorsque vous partagez l’URL avec d’autres utilisateurs :

   * Type de période (semaine, mois, trimestre).
   * Les filtres que vous appliquez.
   * Type d’affichage (Heures ou ETR).

Pour obtenir une URL unique dans la vue utilisateur du planificateur de ressources et la partager avec d’autres utilisateurs :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront.

1. Cliquez sur **Ressource**.
1. Dans , sélectionnez **Afficher par utilisateur**.
1. (Facultatif) Sélectionnez la période d’affichage des informations dans le planificateur de ressources. Sélectionnez l’une des options suivantes :

   * Semaine
   * Mois
   * Trimestre

1. (Facultatif) Choisissez si vous souhaitez afficher les informations par **ETR** ou **Heures**.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. (Facultatif) Appliquez des filtres au planificateur de ressources.\
   Pour plus d’informations sur l’application de filtres, voir [Filtrage des informations dans le planificateur de ressources](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. Cliquez sur l’icône **hyperlien** .\
   ![RP_Storm_generate_URL_with_copy_URL_link.png{1](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. Cliquez sur **Copier l’URL**.\
   Cette opération copie l’URL unique du planificateur de ressources dans la vue utilisateur dans le presse-papiers.

1. (Facultatif) Effectuez l’une des opérations suivantes :  

   * Collez l’URL dans une autre application pour l’envoyer à un autre utilisateur.\
     L’utilisateur doit être connecté à Workfront pour afficher le planificateur de ressources dans la vue Utilisateur.
   * Ouvrez un nouvel onglet ou une nouvelle fenêtre du navigateur et collez le lien que vous avez copié, puis cliquez sur Entrée sur votre clavier pour ouvrir le planificateur de ressources dans un nouvel onglet ou une nouvelle fenêtre.
   * Procédez comme suit :

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. Accédez à **Reporting**>**Tableaux de bord**>**Nouveau tableau de bord**>**Ajouter une page externe.**

      1. Collez le lien que vous avez copié dans le presse-papiers dans le champ **URL** .
      1. Cliquez sur **Enregistrer**, puis **Enregistrer + Fermer**.\
         L’URL est alors incorporée dans le tableau de bord. La vue Utilisateur du planificateur de ressources s’affiche dans un tableau de bord distinct.

1. (Facultatif) Si vous avez incorporé l’URL dans un tableau de bord, pensez à l’ajouter à un modèle de mise en page ou à la partager avec d’autres utilisateurs qui n’ont peut-être pas accès à la zone de gestion des ressources.\
   Pour plus d’informations sur l’ajout de tableaux de bord à un modèle de mise en page, voir [Créer et gérer des modèles de mise en page](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .\
   Pour plus d’informations sur le partage des tableaux de bord, voir [Partager un tableau de bord](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .\
   Lors de l’affichage de l’URL partagée, les utilisateurs peuvent voir les informations avec les paramètres que vous avez initialement appliqués au planificateur de ressources. Ils doivent être connectés à Workfront pour afficher l’URL partagée.\
   ![user_view_dashoard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
