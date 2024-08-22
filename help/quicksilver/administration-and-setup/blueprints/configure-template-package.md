---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configuration d’un plan directeur
description: Vous pouvez configurer les détails du modèle de projet ou de la structure organisationnelle avant d’installer le plan directeur.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1856'
ht-degree: 3%

---

# Configurer un plan directeur

Vous pouvez configurer les détails d’un plan directeur avant de l’installer. Les types de plan directeur de modèle de projet et de structure organisationnelle nécessitent généralement que certaines préférences soient définies et que certaines propriétés soient mappées. D’autres types de plan directeur peuvent ne pas nécessiter de configuration et vous les installerez en l’état. Pour plus d’informations sur l’installation, voir [Installation d’un plan directeur](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouvelle : standard</p>
   <p>ou</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuration d’un plan directeur de modèle de projet

1. Recherchez le plan directeur que vous souhaitez utiliser.
1. Cliquez sur **[!UICONTROL Installer]**, puis sélectionnez un environnement :

   <table style="table-layout:auto">
        <tr>
        <td><strong>Production</strong></td>
        <td>La production est votre environnement en ligne.</td>
    </tr>
    <tr>
        <td><strong>Aperçu de sandbox</strong></td>
        <td>L’aperçu sandbox est un environnement de test qui sert de réplique à votre environnement en ligne et qui est actualisé chaque week-end par Workfront.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 et 2</strong></td>
        <td>L’environnement de test d’actualisation personnalisée est un environnement de test distinct que vous actualisez manuellement. L’obtention de l’environnement de test d’actualisation personnalisée entraîne des frais supplémentaires.</td>
    </tr>
   </table>

1. Passez aux sections suivantes :

   * [[!UICONTROL Préférences de modèle]](#template-preferences)
   * [[!UICONTROL Mapping du rôle]](#role-mapping)
   * [[!UICONTROL Mapping de l&#39;équipe]](#team-mapping)
   * [[!UICONTROL Mappage de société]g](#company-mapping)
   * [[!UICONTROL Mappage de groupe]](#group-mapping)

## [!UICONTROL Préférences de modèle] {#template-preferences}

Choisissez le mode d’installation du modèle.

Vous pouvez également désigner la propriété du modèle avant d’installer le plan directeur. Vous pouvez apporter des modifications à ces champs une fois le modèle installé. Pour plus d’informations, voir [Modifier les modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Préférences de modèle] section](assets/Blueprints_TemplatePreferences.png)

1. Dans la section [!UICONTROL Préférences du modèle], indiquez un nouveau nom de modèle.
1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Propriétaire du modèle]<strong></td>
        <td>Cette personne reçoit les autorisations [!UICONTROL Gérer] sur le modèle et devient le propriétaire du projet lorsque le modèle est utilisé pour créer un projet.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Responsable de modèles]</strong></td>
        <td>Il s’agit généralement d’un responsable, d’un cadre ou d’une partie prenante qui a besoin de savoir ce qui se passe avec le projet. Le parrain du projet n’a aucun accès supplémentaire au projet, mais il est ajouté aux notifications par e-mail du projet.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>Il s’agit du portefeuille auquel le projet apparaîtra lors de sa création.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>Il s’agit du programme auquel le projet apparaîtra lors de sa création.</td>
    </tr>
   </table>

1. Indiquez si le modèle est installé comme actif ou inactif.
1. Choisissez si vous souhaitez utiliser les nouvelles préférences de problème définies, si des préférences sont disponibles.

   Cliquez sur **[!UICONTROL Voir Préférences de problème]** pour consulter les préférences spécifiques qui s’installeront avec le plan directeur. Les projets créés à partir du modèle importé utilisent ces préférences pour les nouveaux problèmes ajoutés dans la section [!UICONTROL Problèmes] .

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Groupes de rubriques de file d’attente</strong></td> 
      <td> <p>Les groupes de rubriques de file d’attente définissent le niveau de catégories le plus élevé pour les problèmes ou les requêtes. Les utilisateurs voient les groupes de rubriques comme des options de menu lors de la sélection de l’emplacement d’envoi des requêtes. Un groupe de rubriques peut contenir plusieurs rubriques de file d’attente. Pour plus d’informations, voir <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Création de groupes de sujets</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Rubriques en file d’attente</strong></td> 
      <td> <p>Les rubriques de file d’attente fonctionnent conjointement avec les règles de routage pour affecter des problèmes ou des requêtes. Il s’agit des options de menu que les utilisateurs sélectionnent lorsqu’ils saisissent un problème ou une requête, après avoir sélectionné un groupe de rubriques. Pour plus d’informations, voir <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Créer des rubriques de file d’attente</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Règles de routage</strong></td> 
      <td>Les règles de routage envoient des problèmes ou des requêtes à des rôles de tâche, des utilisateurs ou des équipes spécifiques. Ils peuvent également envoyer les requêtes à des projets spécifiques, autres que celui associé à la file d’attente des requêtes. Pour plus d’informations, voir <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Création de règles de routage</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Exemple :** Les nouvelles préférences de problème de ce plan directeur fournissent quatre rubriques de file d’attente. L’utilisateur sélectionne l’une de ces rubriques lors de la création d’un problème. (Puisqu’il n’existe qu’un seul groupe de rubriques, celui-ci est automatiquement appliqué et l’utilisateur n’a pas à le sélectionner.) Lorsque l’utilisateur termine et envoie le problème, les règles de routage déterminent à quel rôle de tâche ou équipe elle est affectée.
   >![Exemple de préférences de nouveau problème](assets/Blueprints_IssuePrefsDetails.png)
   >![Rubriques de file d’attente pour le nouveau problème](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Problème lié au rôle de tâche](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* L’utilisation des préférences de problème permet de créer de la cohérence dans la manière dont les nouveaux problèmes ou demandes sont capturés sur vos projets.
   >* La définition de ces préférences ne place pas automatiquement les projets créés à partir du modèle dans des files d’attente de requêtes. Pour plus d’informations sur la configuration d’une file d’attente de requêtes, voir [Création d’une file d’attente de requêtes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Tous les plans directeurs ne contiennent pas de nouvelles préférences de problème.


## [!UICONTROL Mapping du rôle] {#role-mapping}

>[!NOTE]
>
>Cette section peut ne pas apparaître dans certains plans directeurs.

Certains modèles comportent des rôles de tâche prescrits. Les rôles de tâche vous aident à affecter les personnes appropriées lorsque le modèle est converti en projet. Vous pouvez personnaliser le mappage des rôles avant d’installer le plan directeur. Cliquez sur **[!UICONTROL Voir la description des rôles]** pour en savoir plus sur les rôles disponibles dans le plan directeur.

Le plan directeur effectue des recherches par nom de rôle pour déterminer si des rôles existants correspondent. La recherche étant sensible à la casse, les noms doivent correspondre exactement. Si aucun rôle existant ne correspond, le plan directeur peut les créer pour vous.

![[!UICONTROL  Section Mappage de rôles]](assets/Blueprints_RoleMapping.png)

1. Si un rôle existe, vous pouvez choisir l’une des options suivantes :

   1. Créez un rôle portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez un rôle existant, puis sélectionnez un rôle dans la zone de sélection.
   1. N’utilisez pas de rôle mappé. Cette option n’est pas recommandée, car certains rôles ne seront pas affectés à certaines tâches.

1. Si aucun rôle n’existe, vous pouvez choisir l’une des options suivantes :

   1. Créez un nouveau rôle. Cette option crée le rôle que le plan directeur recommande.
   1. Créez un rôle portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez un rôle existant, puis sélectionnez un rôle dans la zone de sélection.
   1. N’utilisez pas de rôle mappé. Cette option n’est pas recommandée, car certains rôles ne seront pas affectés à certaines tâches.

>[!NOTE]
>
>Le processus d’installation n’applique pas de rôles à des personnes spécifiques. Vous devez vérifier les personnes qui se trouvent dans ces rôles après avoir installé la solution de plan directeur et affecter des personnes si nécessaire. Pour plus d’informations, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Pour plus d’informations sur les rôles de tâche dans [!DNL Workfront], voir [Création et gestion des rôles de tâche](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Mapping de l&#39;équipe] {#team-mapping}

>[!NOTE]
>
>Cette section peut ne pas apparaître dans certains plans directeurs.

Certains modèles incluent des équipes prescrites. Le travail assigné à une équipe peut être effectué par n’importe quel membre de l’équipe. Vous pouvez personnaliser le mappage des équipes avant d’installer le plan directeur. Cliquez sur **[!UICONTROL Voir la description de l’équipe]** pour en savoir plus sur les équipes disponibles dans le plan directeur.

Le plan directeur effectue des recherches par nom d’équipe pour déterminer si des équipes existantes correspondent. La recherche étant sensible à la casse, les noms doivent correspondre exactement. Si aucune équipe existante ne correspond, le plan directeur peut les créer pour vous.

![[!UICONTROL Section de mappage d’équipe]](assets/Blueprints_TeamMapping.png)

1. Si une équipe existe, vous pouvez choisir l’une des options suivantes :

   1. Créez une nouvelle équipe portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez [!UICONTROL l’équipe existante], puis sélectionnez une équipe dans la zone de sélection.
   1. N’utilisez pas d’équipe mappée. Cette option n’est pas recommandée, car certaines tâches n’auront pas d’équipes affectées.

1. Si aucune équipe n’existe, vous pouvez choisir l’une des options suivantes :

   1. Créez une nouvelle équipe. Cette option crée l’équipe recommandée par le plan directeur.
   1. Créez une nouvelle équipe portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez [!UICONTROL l’équipe existante], puis sélectionnez une équipe dans la zone de sélection.
   1. N’utilisez pas d’équipe mappée. Cette option n’est pas recommandée, car certaines tâches n’auront pas d’équipes affectées.

>[!NOTE]
>
>Le processus d’installation n’ajoute pas de personnes aux équipes. Vous devez vérifier les personnes des équipes après l’installation de la solution de plan directeur et affecter des personnes si nécessaire. Pour plus d’informations, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Pour plus d&#39;informations sur le fonctionnement des équipes dans [!DNL Workfront], voir [Créer et gérer des équipes](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Mappage des entreprises {#company-mapping}

>[!NOTE]
>
>Cette section peut ne pas apparaître dans certains plans directeurs.

Certains plans directeurs comportent des entreprises prescrites. Une entreprise est une entité organisationnelle qui peut représenter votre organisation, un service au sein de l’organisation ou un client avec lequel vous travaillez. Vous pouvez personnaliser la manière dont les entreprises sont mappées avant d’installer le plan directeur. Cliquez sur **[!UICONTROL Voir la description de l’entreprise]** pour en savoir plus sur les entreprises disponibles dans le plan directeur.

Le plan directeur effectue des recherches par nom de société pour déterminer si des entreprises existantes correspondent. La recherche étant sensible à la casse, les noms doivent correspondre exactement. Si aucune entreprise existante ne correspond, le plan directeur peut les créer pour vous. L’entreprise principale du plan directeur est mappée à l’entreprise principale de votre environnement, même si elle ne porte pas le même nom.

![[!UICONTROL Section de mappage d’entreprise]](assets/Blueprints_CompanyMapping.png)

1. Si une société existe, vous pouvez choisir l’une des options suivantes :

   1. Créez une nouvelle société portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez une société existante, puis sélectionnez une société dans la zone de sélection.\

      L’entreprise principale du plan directeur est mappée à l’entreprise principale de votre environnement, même si elle ne porte pas le même nom.
   1. N’utilisez pas de société mappée. Cette option n’est pas recommandée, car les références de société dans d’autres objets seront vides.

1. Si une société n’existe pas, vous pouvez choisir l’une des options suivantes :

   1. Créez une nouvelle société. Cette option crée la société que le plan directeur recommande.
   1. Créez une nouvelle société portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez une société existante, puis sélectionnez une société dans la zone de sélection.
   1. N’utilisez pas de société mappée. Cette option n’est pas recommandée, car les références de société dans d’autres objets seront vides.

>[!NOTE]
>
>Pour configurer les entreprises après l’installation du plan directeur, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Pour plus d’informations sur l’association d’un modèle à une entreprise, voir [Modifier des modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Pour plus d&#39;informations sur le fonctionnement des entreprises dans [!DNL Workfront], voir [Créer et modifier des entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Mappage de groupe] {#group-mapping}

>[!NOTE]
>
>Cette section peut ne pas apparaître dans certains plans directeurs.

Certains plans directeurs comportent des groupes prescrits. Un groupe est un groupe d’utilisateurs qui correspond à la structure de votre service. Les groupes sont similaires aux équipes et aux entreprises de Workfront, mais distincts. Vous pouvez personnaliser le mappage des groupes avant d’installer le plan directeur. Cliquez sur **[!UICONTROL Voir la description des groupes]** pour en savoir plus sur les groupes disponibles dans le plan directeur.

Le plan directeur effectue des recherches par nom de groupe pour déterminer si des groupes existants correspondent. La recherche étant sensible à la casse, les noms doivent correspondre exactement. Si aucun groupe existant ne correspond, le plan directeur peut les créer pour vous.

![[!UICONTROL Section Mapping de groupe]](assets/Blueprints_GroupMapping.png)

1. S’il existe un groupe, vous pouvez sélectionner **[!UICONTROL Remap Group]** et choisir l’une des options suivantes :

   1. **[!UICONTROL Créez un groupe portant un nom différent]**, puis saisissez le nom à attribuer à ce groupe. Les références au groupe dans la définition de plan directeur seront associées à ce nouveau groupe à la place.
   1. **[!UICONTROL Remplacez par un groupe existant]**, puis recherchez et sélectionnez un groupe dans la zone de sélection.

      >[!NOTE]
      >
      >Vous ne pouvez pas renommer un groupe existant.

1. Si un groupe n’existe pas, vous pouvez :

   1. Modifiez le nom du groupe suggéré en le saisissant dans la zone de texte.
   1. Sélectionnez **[!UICONTROL Remap Group]** et choisissez [!UICONTROL Remap Group] (Remplacer par un groupe existant), puis recherchez et sélectionnez un groupe dans la zone de sélection.
   1. Sélectionnez **[!UICONTROL Remap Group]** et choisissez **[!UICONTROL Insérer sous un groupe existant]**, puis recherchez et sélectionnez un groupe dans la zone de sélection. Cette option crée un sous-groupe sous le groupe existant.

>[!NOTE]
>
>Pour configurer les groupes après l’installation du plan directeur, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Pour plus d’informations sur l’utilisation des groupes dans [!DNL Workfront], voir [Présentation des groupes](../../administration-and-setup/manage-groups/groups-overview/groups.md).
