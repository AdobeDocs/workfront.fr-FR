---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Créer et modifier des sociétés
description: Vous pouvez ajouter des entreprises à  [!DNL Adobe Workfront]  et les utiliser à des fins de planification financière, de création de rapports, pour définir des autorisations liées à des objets et pour préserver la confidentialité des informations.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: b89715649473ba13e1b6b7a250dfed7a468bb4b4
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 92%

---

# Créer et modifier des entreprises

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Une entreprise est une entité organisationnelle dans [!DNL Adobe Workfront] qui peut représenter votre organisation, un service au sein de l’organisation ou une clientèle avec laquelle vous travaillez. Vous pouvez ajouter des entreprises à [!DNL Workfront] et les utiliser à des fins de planification financière, de création de rapports, pour définir des autorisations liées à des objets et pour préserver la confidentialité des informations.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licence</p> </td> 
   <td><p>Actuelle : [!UICONTROL Plan]</p>
   <p>Ou</p>
   <p>Nouvelle : [!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Utilisez l’une des configurations suivantes :</p> 
    <ul> 
     <li> <p>Le niveau d'accès [!UICONTROL System Administrator], qui permet de modifier n'importe quelle société du système.</p> </li> 
     <li> <p>Accès administratif pour gérer les sociétés, ce qui vous permet de modifier n’importe quelle société du système.</p> </li> 
    </ul> <p><b>NOTE</b> :  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à un groupe pour lequel vous faites partie de l’équipe d’administration.</p> </li> 
      <li> <p>Pour pouvoir ajouter ou supprimer des utilisateurs et utilisatrices du système [!DNL Workfront], vous devez disposer de l’un des éléments suivants :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL System Administrator]. </p> </li> 
        <li> <p>Dans votre niveau d’accès, [!UICONTROL Edit] doit être sélectionné pour le paramètre [!UICONTROL Users]. En outre, pour le paramètre [!UICONTROL Users], sous [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png">, l’option [!UICONTROL Create] et au moins l’une des deux options [!UICONTROL User Admin] doivent être activées. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez faire partie de l’équipe d’administration du groupe dont la personne est membre.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Avantages de l’ajout de personnes à une entreprise {#benefits-of-adding-users-to-a-company}

* Vous pouvez créer un organigramme hiérarchique d’une entreprise en associant les personnes aux rapports directs. Seules les personnes de la même entreprise peuvent être ajoutées en tant que rapports directs d’une autre personne de cette entreprise.
* En tant que responsable de projet, vous pouvez identifier les ressources disponibles au sein de la même entreprise.
* Vous pouvez préserver la confidentialité des informations entre les entreprises en choisissant un ou tous les paramètres suivants :

   * Les personnes de la même entreprise peuvent voir les demandes des autres.

     Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut accorder un accès similaire aux demandes en fonction de l’entreprise des utilisateurs et utilisatrices, voir la section [Configuer les préférences de tâche et de problème pour toutes les personnes dans  [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) dans l’article [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Pour plus d’informations sur la manière dont un administrateur ou une administratrice de groupes peut accorder un accès similaire aux demandes en fonction de l’entreprise des utilisateurs et utilisatrices, voir [Configurer les préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Les personnes ne peuvent afficher que les files d’attente de demandes associées à leurs entreprises. Pour plus d’informations sur la limitation de la visibilité d’une file d’attente de demandes, voir [Fournir l’accès aux files d’attente de demandes](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Vous pouvez limiter les personnes à afficher uniquement les utilisateurs et utilisatrices de leur entreprise ou de leur entreprise et de l’entreprise principale. Pour plus d’informations sur les principales fonctionnalités de l’entreprise concernant la confidentialité des personnes, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Les personnes peuvent limiter la visibilité des mises à jour qu’elles effectuent sur les éléments pour les personnes de leur entreprise uniquement. Pour plus d’informations sur l’établissement d’une mise à jour privée pour une entreprise, voir [Mettre à jour le travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Créer ou modifier une entreprise dans [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Il n’y a pas de limite au nombre d’entreprises que vous pouvez ajouter. Cependant, nous recommandons que vous limitiez le nombre d’entreprises en raison de problèmes pouvant survenir avec les autorisations d’objet. Une trop grande fragmentation peut affecter la visibilité des personnes aux éléments de travail.

Par défaut, l’entreprise associée à votre instance [!DNL Workfront] est déjà créée dans votre système [!DNL Workfront] et est l’entreprise principale de votre organisation. Elle porte le même nom que votre nom de client ou cliente. Pour plus d’informations sur votre clientèle dans [!DNL Workfront], voir [Configurer les informations de base pour votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Pour ajouter ou modifier une entreprise, procédez comme suit :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Entreprises]**.

   Une liste des entreprises s’affiche.

1. Si vous souhaitez ajouter une entreprise, cliquez sur **[!UICONTROL Nouvelle entreprise]**.

   Ou

   Si vous modifiez une société existante, sélectionnez-la, puis cliquez sur l’icône **[!UICONTROL Modifier]** ![Modifier](assets/edit-icon.png) en haut de la liste des sociétés.

1. Mettez à jour les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Section [!UICONTROL Basic Info]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b> : saisissez le nom de l’entreprise.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b> : lorsque cette option est activée, les utilisateurs et utilisatrices peuvent rechercher l’entreprise et la joindre aux projets qu’ils créent et modifient. Une société inactive ne peut pas être jointe aux projets. Cette option est activée par défaut.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b> : affecte l’entreprise en tant qu’entreprise principale de votre organisation. L’entreprise principale représente généralement votre compte [!DNL Workfront] où la plupart de vos utilisateurs et utilisatrices travaille.</p> <p>Vous pouvez désigner une entreprise, ou aucune, comme entreprise principale, mais vous ne pouvez pas en désigner plusieurs à la fois. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> <p><b>NOTE</b> : modifier les niveaux d’accès vous permet d’empêcher les utilisateurs et utilisatrices d’afficher d’autres personnes, que ce soit uniquement dans leur entreprise principale ou dans celle-ci ainsi que dans leur entreprise associée. Pour plus d’informations sur le fonctionnement de l’entreprise principale avec les niveaux d’accès des utilisateurs et utilisatrices, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b> : si un groupe traite avec l’entreprise, vous pouvez ajouter le nom du groupe ici. Cette fonction peut s’avérer utile pour les administrateurs et administratrices de groupes qui doivent créer des rapports et gérer toutes les entreprises avec lesquelles leurs groupes traitent.</p> <p><b>IMPORTANT</b> : si vous n’associez pas le groupe qui travaillera avec cette entreprise, les administrateurs et administratrices de groupes ne peuvent pas accéder à l’entreprise à moins que leurs niveaux d’accès comportent un accès administratif aux entreprises. Pour plus d’informations sur la manière dont cet accès est accordé, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Commencez à saisir le nom du groupe, puis appuyez sur <strong>[!UICONTROL Enter]</strong> lorsqu’il apparaît.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Lorsque vous affectez un groupe à une entreprise, les administrateurs et administratrices de groupes obtiennent l’accès [!UICONTROL Manage] à l’entreprise. Pour plus d’informations, voir <a href="#group-administrators-and-companies" class="MCXref xref">Administrateurs et administratrices de groupes et entreprises</a> dans cet article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b> : ajoutez des utilisateurs et utilisatrices existants à l’entreprise. Ce faisant, vous associez ces utilisateurs et utilisatrices à cette entreprise.</p> <p>Le nombre d’utilisateurs et d’utilisatrices que vous pouvez associer à une entreprise est illimité, mais une personne ne peut pas être associée à plusieurs sociétés.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Section [!UICONTROL Custom Forms]</td> 
      <td> <p>Si des champs que vous souhaitez ajouter à votre entreprise ne sont pas disponibles dans [!DNL Workfront], vous pouvez créer un formulaire personnalisé et l’associer à votre entreprise. </p> <p>Vous pouvez joindre ce formulaire à votre entreprise en le sélectionnant dans le menu déroulant. Seuls les formulaires personnalisés actifs sont répertoriés dans le menu.</p> <p><strong>Remarque :</strong> les fonctions avancées de formulaires personnalisés telles que les champs de recherche externe et les champs natifs de Workfront ne sont disponibles que lorsque vous ouvrez l’enregistrement de la société sur la page de détails, et non dans la boîte de dialogue Modifier la société . (Dans la liste des entreprises, cliquez sur le nom de l’entreprise pour ouvrir les détails.)</p> <p> Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Créer un formulaire personnalisé</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Le cas échéant) Si vous créez une entreprise, cliquez sur **[!UICONTROL Créer une entreprise]**.

   Ou

   Si vous modifiez une société existante, cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Gérer les adhésions des entreprises

Pour plus d’informations sur la gestion des appartenances à une entreprise existante, voir [Gérer les appartenances à une entreprise](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Gérer les taux de facturation

Pour plus d’informations sur le remplacement des taux de facturation à l’échelle de l’entreprise, voir [Remplacer les taux de facturation des fonctions à l’échelle de l’entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Vue d’ensemble du partage d’objets avec les entreprises

Certaines autorisations sont disponibles pour les utilisateurs et utilisatrices associés à une entreprise, comme expliqué dans la section [Avantages de l’ajout d’utilisateurs et d’utilisatrices à une entreprise](#benefits-of-adding-users-to-a-company). Outre ces autorisations, vous pouvez permettre aux utilisateurs et utilisatrices d’afficher, de contribuer ou de modifier des objets dans [!DNL Workfront] en partageant l’objet avec leur entreprise.

Plutôt que de partager un objet avec une personne individuelle à la fois, vous pouvez le partager avec l’ensemble de l’entreprise. Chaque utilisateur ou utilisatrice de l’entreprise dispose des mêmes autorisations sur cet objet.

Pour plus d’informations sur le partage d’objets, voir [Vue d’ensemble du partage des autorisations sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Administrateurs et administratrices de groupes et entreprises {#group-administrators-and-companies}

Lorsque l’administration de [!DNL Workfront] affecte un groupe à une entreprise, les administrateurs et administratrices de groupes obtiennent un accès [!UICONTROL Gérer] à l’entreprise dans [!UICONTROL Configuration]. Cela inclut l’accès à la page [!UICONTROL Entreprises] dans [!UICONTROL Configuration], où ils peuvent consulter et gérer l’entreprise associée à leur groupe.

Grâce à l’accès à la page [!UICONTROL Entreprises], un administrateur ou une administratrice de groupes peut affecter un groupe à une entreprise, à condition que celle-ci ait été créée par l’administrateur ou l’administratrice de groupes. Si le niveau d’accès de l’administrateur ou de l’administratrice de groupes n’est pas configuré avec l’accès administratif aux entreprises, le champ [!UICONTROL Groupe] doit être rempli lorsque l’administrateur ou l’administratrice de groupes crée l’entreprise. Son titre en gras indique :

![Modifier l’entreprise](assets/group-admin-add-company.png)

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices obtiennent un accès administratif aux entreprises pour leur niveau d’accès, voir [Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Pour plus d’informations sur la gestion d’une entreprise dans la zone [!UICONTROL Configuration], consultez dans cet article la section [Créer ou modifier une entreprise dans  [!DNL Workfront]](#create-or-edit-a-company-in-workfront).
