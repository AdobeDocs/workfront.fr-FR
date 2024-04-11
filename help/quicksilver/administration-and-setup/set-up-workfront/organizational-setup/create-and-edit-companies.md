---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Création et modification d’entreprises
description: Vous pouvez ajouter des entreprises à [!DNL Adobe Workfront] et les utiliser à des fins de planification financière, de création de rapports, pour définir des autorisations liées à des objets et pour préserver la confidentialité des informations.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 0%

---

# Création et modification d’entreprises

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Une entreprise est une entité organisationnelle dans [!DNL Adobe Workfront] qui peuvent représenter votre organisation, un service au sein de l’organisation ou un client avec lequel vous travaillez. Vous pouvez ajouter des entreprises à [!DNL Workfront] et les utiliser à des fins de planification financière, de création de rapports, pour définir des autorisations liées à des objets et pour préserver la confidentialité des informations.

## Exigences d’accès

Pour gérer les entreprises dans , vous devez disposer des éléments suivants : [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td><p>Actuel : formule [!UICONTROL]</p>
   Ou
   <p>Nouveau : [!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>L’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès [!UICONTROL Administrateur système] qui permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p>Accès administratif pour la gestion des entreprises, ce qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </li> 
    </ul> <p><b>REMARQUE</b>:  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à n’importe quel groupe auquel vous êtes affecté en tant qu’administrateur de groupe.</p> </li> 
      <li> <p>Pour ajouter et supprimer des utilisateurs du [!DNL Workfront] système, vous devez disposer de l’une des fonctionnalités suivantes :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL Administrateur système]. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
        <li> <p>Dans votre niveau d’accès, [!UICONTROL Modifier] doit être sélectionné pour le paramètre [!UICONTROL Utilisateurs] . En outre, pour le paramètre [!UICONTROL Utilisateurs] , sous [!UICONTROL Ajuster vos paramètres] <img src="assets/gear-icon-in-access-levels.png">, l’option [!UICONTROL Créer] et au moins l’une des deux options [!UICONTROL User Admin] doivent être activées. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
       </ul> <p>Pour plus d’informations sur le paramètre Utilisateurs dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Avantages de l’ajout d’utilisateurs à une entreprise {#benefits-of-adding-users-to-a-company}

* Vous pouvez créer un organigramme hiérarchique d’une entreprise en associant les utilisateurs aux rapports directs. Seuls les utilisateurs de la même société peuvent être ajoutés en tant que rapports directs d’un autre utilisateur de cette société.
* En tant que chef de projet, vous pouvez identifier les ressources disponibles au sein de la même entreprise.
* Vous pouvez préserver la confidentialité des informations entre les entreprises en choisissant un ou tous les paramètres suivants :

   * Les utilisateurs de la même société peuvent voir les demandes des autres.

     Pour plus d’informations sur la manière dont une [!DNL Workfront] L’administrateur peut accorder un accès similaire aux demandes en fonction de la société des utilisateurs. Voir la section [Configuration des préférences de tâche et de problème pour toutes les personnes de [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) dans l’article [Configuration des préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Pour plus d’informations sur la manière dont un administrateur de groupe peut accorder un accès similaire aux requêtes en fonction de la société des utilisateurs, voir [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Les utilisateurs ne peuvent afficher que les files d’attente de demandes associées à leurs entreprises. Pour plus d’informations sur la limitation de la visibilité d’une file d’attente de requêtes, voir [Fournir l’accès aux files d’attente de demandes](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Vous pouvez limiter les utilisateurs à afficher uniquement les utilisateurs de leur société ou de leur société et de l’entreprise principale. Pour plus d’informations sur les principales fonctionnalités de l’entreprise concernant la confidentialité des utilisateurs, voir [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Les utilisateurs peuvent limiter la visibilité des mises à jour qu’ils effectuent sur les éléments pour les utilisateurs de leur société uniquement. Pour plus d’informations sur l’établissement d’une mise à jour privée pour une entreprise, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Création ou modification d’une entreprise dans [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Il n’y a pas de limite au nombre d’entreprises que vous pouvez ajouter. Cependant, nous recommandons que vous limitiez le nombre d’entreprises en raison de problèmes pouvant survenir avec les autorisations d’objet. Une trop grande fragmentation peut affecter la visibilité des utilisateurs aux tâches.

Par défaut, la société associée à votre instance de [!DNL Workfront] est déjà créé dans votre [!DNL Workfront] et est la société par Principal de votre organisation. Il porte le même nom que votre nom de client. Pour plus d’informations sur vos clients, voir [!DNL Workfront], voir [Configuration des informations de base pour votre système](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Pour ajouter ou modifier une société :

{#step-1-to-setup}

1. Cliquez sur **[!UICONTROL Entreprises]**.

   Une liste des entreprises s’affiche.
1. Si vous ajoutez une société, cliquez sur **[!UICONTROL Nouvelle entreprise]**.

   Ou

   Si vous modifiez une société existante, sélectionnez-la, puis cliquez sur **[!UICONTROL Modifier]** en haut de la liste des entreprises.

1. Mettez à jour les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Section [!UICONTROL Informations de base]</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Nom de la société]</b>: saisissez le nom de la société.</p> </li> 
        <li> <p><b>[!UICONTROL Est Actif]</b>: lorsque cette option est activée, les utilisateurs peuvent rechercher la société et la joindre aux projets qu’ils créent et modifient. Une société inactive ne peut pas être jointe aux projets. Cette option est activée par défaut.</p> </li> 
        <li> <p><b>[!UICONTROL Il s’agit de la société par Principal]</b>: affecte la société en tant que société principale de votre organisation. L’entreprise principale représente généralement votre [!DNL Workfront] compte où la plupart de vos utilisateurs travaillent.</p> <p>Vous pouvez désigner une société ou aucune société comme entreprise principale, mais vous ne pouvez pas désigner plusieurs sociétés comme sociétés principales. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> <p><b>REMARQUE</b>: en modifiant leurs niveaux d’accès, vous pouvez empêcher les utilisateurs de voir d’autres utilisateurs : uniquement dans leur entreprise principale, ou dans leur entreprise associée et la société principale. Pour plus d’informations sur le fonctionnement de l’entreprise principale avec les niveaux d’accès des utilisateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: s’il existe un groupe qui gère des affaires avec la société, vous pouvez y ajouter le nom du groupe. Cela s’avère utile pour les administrateurs de groupe qui doivent créer des rapports et gérer toutes les entreprises avec lesquelles leurs groupes traitent.</p> <p><b>IMPORTANT</b>: si vous n’associez pas le groupe qui travaillera avec cette société, les administrateurs du groupe ne peuvent pas accéder à la société à moins qu’ils n’aient un accès administratif aux sociétés à leur niveau d’accès. Pour plus d’informations sur la manière dont cet accès est accordé, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Commencez à saisir le nom du groupe, puis appuyez sur <strong>[!UICONTROL Entrée]</strong> lorsqu’il apparaît.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Lorsque vous affectez un groupe à une entreprise, les administrateurs du groupe obtiennent l’accès [!UICONTROL Gérer] à l’entreprise. Pour plus d’informations, voir <a href="#group-administrators-and-companies" class="MCXref xref">Administrateurs de groupe et entreprises</a> dans cet article.</p> </li> 
        <li> <p><b>[!UICONTROL Membres de la société]</b>: ajoutez des utilisateurs existants à la société. Ce faisant, vous associez ces utilisateurs à cette entreprise.</p> <p>Le nombre d’utilisateurs que vous associez à une société est illimité, mais un utilisateur ne peut pas être associé à plusieurs sociétés.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Section [!UICONTROL Forms personnalisé]</td> 
      <td> <p>Si des champs que vous souhaitez ajouter à votre société ne sont pas disponibles dans [!DNL Workfront], vous pouvez créer un formulaire personnalisé et l’associer à votre entreprise. </p> <p>Vous pouvez joindre ce formulaire à votre société en le sélectionnant dans le menu déroulant. Seuls les formulaires personnalisés actifs sont répertoriés dans le menu.</p> <p><strong>Remarque :</strong> Les fonctionnalités de formulaire personnalisées avancées telles que les champs de recherche externe et les champs natifs de Workfront ne sont disponibles que lorsque vous ouvrez l’enregistrement de l’entreprise sur la page de détails, et non dans la boîte de dialogue Modifier l’entreprise . (Dans la liste des sociétés, cliquez sur le nom de la société pour ouvrir les détails.)</p> <p> Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Création ou modification d’un formulaire personnalisé</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Conditionnel) Si vous créez une société, cliquez sur **[!UICONTROL Créer une entreprise]**.

   Ou

   Si vous modifiez une société existante, cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Gestion des appartenances à une entreprise

Pour plus d’informations sur la gestion des adhésions pour une entreprise existante, voir [Gestion des appartenances à une entreprise](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Gestion des taux de facturation

Pour plus d’informations sur le remplacement des taux de facturation au niveau de l’entreprise, voir [Remplacer les taux de facturation des rôles de tâche au niveau de l’entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Présentation du partage d’objets avec les entreprises

Certaines autorisations sont disponibles pour les utilisateurs associés à une entreprise, comme expliqué dans la section . [Avantages de l’ajout d’utilisateurs à une entreprise](#benefits-of-adding-users-to-a-company). Outre ces autorisations, vous pouvez autoriser les utilisateurs à afficher, à contribuer ou à modifier des objets dans [!DNL Workfront] en partageant l’objet avec leur entreprise.

Plutôt que de partager un objet avec un utilisateur individuel à la fois, vous pouvez le partager avec l’ensemble de l’entreprise. Chaque utilisateur de l’entreprise dispose des mêmes autorisations sur cet objet.

Pour plus d’informations sur le partage d’objets, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Administrateurs de groupe et entreprises {#group-administrators-and-companies}

Lorsqu’une [!DNL Workfront] L’administrateur affecte un groupe à une entreprise, les administrateurs du groupe pour le gain du groupe. [!UICONTROL Gérer] accès à l’entreprise dans [!UICONTROL Configuration]. Cela inclut l’accès au [!UICONTROL Entreprises] page [!UICONTROL Configuration], où ils peuvent voir et gérer l’entreprise associée à leur groupe.

Avec cet accès au [!UICONTROL Entreprises] , un administrateur de groupe peut affecter un groupe à une société, mais il doit s’agir d’une société que l’administrateur de groupe a créée. Si le niveau d’accès de l’administrateur du groupe n’est pas configuré avec l’accès administratif aux entreprises, la variable [!UICONTROL Groupe] est obligatoire lorsque l’administrateur du groupe crée la société. Son titre en gras indique :

![Modifier la société](assets/group-admin-add-company.png)

Pour plus d’informations sur la manière dont les utilisateurs accèdent de manière administrative aux entreprises à leur niveau d’accès, voir [Octroi aux utilisateurs un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Pour plus d’informations sur la gestion d’une entreprise dans le [!UICONTROL Configuration] zone, voir [Création ou modification d’une entreprise dans [!DNL Workfront]](#create-or-edit-a-company-in-workfront) dans cet article.
