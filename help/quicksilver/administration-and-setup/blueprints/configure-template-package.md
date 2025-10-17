---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configuration d’un plan directeur
description: Vous pouvez configurer les détails du modèle de projet ou de la structure organisationnelle avant d’installer le plan directeur.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1841'
ht-degree: 97%

---

# Configurer un plan directeur

Vous pouvez configurer les détails d’un plan directeur avant de l’installer. Les types de plan directeur de modèle de projet et de structure organisationnelle nécessitent généralement que certaines préférences soient définies et que certaines propriétés soient mappées. D’autres types de plan directeur peuvent ne pas nécessiter de configuration et vous les installerez en l’état. Pour plus d’informations sur l’installation, voir [Installer un plan directeur](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Administrateur ou administratrice Workfront </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer un plan directeur de modèle de projet

1. Recherchez le plan directeur que vous souhaitez utiliser.
1. Cliquez sur **[!UICONTROL Installer]**, puis choisissez un environnement :

   <table style="table-layout:auto">
        <tr>
        <td><strong>Production</strong></td>
        <td>La production est votre environnement en ligne.</td>
    </tr>
    <tr>
        <td><strong>Aperçu de sandbox</strong></td>
        <td>L’environnement de prévisualisation sandbox est un environnement de test qui sert de réplique à votre environnement en ligne et que Workfront actualise chaque week-end.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 et 2</strong></td>
        <td>L’environnement de sandbox à actualisation personnalisée est un environnement de test distinct qui est actualisé manuellement par vos soins. L’obtention du sandbox à actualisation personnalisée entraîne des frais supplémentaires.</td>
    </tr>
   </table>

1. Passez aux sections suivantes :

   * [[!UICONTROL Préférences du modèle]](#template-preferences)
   * [[!UICONTROL Mappage de rôles]](#role-mapping)
   * [[!UICONTROL Mappage d’équipes]](#team-mapping)
   * [[!UICONTROL Mappage d’entreprises]](#company-mapping)
   * [[!UICONTROL Mappage de groupes]](#group-mapping)

## [!UICONTROL Préférences du modèle] {#template-preferences}

Choisissez le mode d’installation du modèle.

Vous pouvez également désigner la propriété du modèle avant d’installer le plan directeur. Vous pouvez apporter des modifications à ces champs une fois le modèle installé. Pour plus d’informations, voir [Modifier des modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Section Préférences de modèle]](assets/Blueprints_TemplatePreferences.png)

1. Dans la section [!UICONTROL Préférences de modèle], indiquez un nouveau nom de modèle.
1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Template owner]<strong></td>
        <td>Cette personne reçoit les autorisations [!UICONTROL Manage] sur le modèle et devient propriétaire du projet lorsque le modèle est utilisé pour créer un projet.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Template sponsor]</strong></td>
        <td>Il s’agit généralement d’une personne responsable, cadre ou partie prenante qui a besoin de savoir ce qui se passe sur le projet. La personne qui sponsorise le projet n’a aucun accès supplémentaire au projet, mais est ajoutée aux notifications par e-mail du projet.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>Il s’agit du portfolio auquel le projet appartiendra après sa création.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>Il s’agit du programme auquel le projet appartiendra après sa création.</td>
    </tr>
   </table>

1. Indiquez si le modèle est installé comme actif ou inactif.
1. Choisissez si vous souhaitez utiliser les nouvelles préférences de problème définies, si des préférences sont disponibles.

   Cliquez sur **[!UICONTROL Voir les préférences de problème]** pour examiner les préférences spécifiques qui seront installées avec le plan directeur. Les projets créés à partir du modèle importé utilisent ces préférences pour les nouveaux problèmes ajoutés dans la section [!UICONTROL Problèmes].

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Groupes de rubriques de file d’attente</strong></td> 
      <td> <p>Les groupes de rubriques de file d’attente définissent le niveau de catégories le plus élevé pour les problèmes ou les demandes. Les personnes affichent les groupes de rubriques comme des options de menu lors de la sélection de l’emplacement de soumission des demandes. Un groupe de rubriques peut contenir plusieurs rubriques de file d’attente. Pour plus d’informations, voir <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Créer des groupes de rubriques</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Rubriques de file d'attente</strong></td> 
      <td> <p>Les rubriques de file d’attente fonctionnent conjointement avec les règles de routage pour affecter des problèmes ou des demandes. Il s’agit des options de menu que les personnes sélectionnent lorsqu’elles saisissent un problème ou une demande, après avoir sélectionné un groupe de rubriques. Pour plus d’informations, voir <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Créer des rubriques de file d’attente</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Règles de routage</strong></td> 
      <td>Les règles de routage envoient des problèmes ou des demandes à des fonctions, des personnes ou des équipes spécifiques. Elles peuvent également envoyer les demandes à des projets spécifiques, autres que celui associé à la file d’attente des demandes. Pour plus d’informations, voir <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Créer des règles de routage</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Exemple :** les nouvelles préférences de problème de ce plan directeur fournissent quatre rubriques de file d’attente. La personne sélectionne l’une de ces rubriques lors de la création d’un problème. (Puisqu&#39;il n&#39;existe qu&#39;un seul groupe de sujets, il est automatiquement appliqué et l&#39;utilisateur n&#39;a pas à le sélectionner.) Lorsque l’utilisateur termine et soumet le problème, les règles de transmission déterminent la fonction ou l’équipe à laquelle il est affecté.
   >![Exemples de préférences de nouveau problème](assets/Blueprints_IssuePrefsDetails.png)
   >![Rubriques de file d’attente pour le nouveau problème](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Problème transmis à la fonction](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* L’utilisation des préférences de problème permet de créer de la cohérence dans la manière dont les nouveaux problèmes ou demandes sont capturés sur vos projets.
   >* La définition de ces préférences ne place pas automatiquement les projets créés à partir du modèle dans des files d’attente de demandes. Pour plus d’informations sur la configuration d’une file d’attente des demandes, voir [Créer une file d’attente des demandes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Tous les plans directeurs ne contiennent pas de préférences de nouveau problème.


## [!UICONTROL Mappage de rôles] {#role-mapping}

>[!NOTE]
>
>Cette section peut ne pas apparaître dans certains plans directeurs.

Certains modèles comportent des fonctions prescrites. Les fonctions vous aident à affecter les personnes appropriées lorsque le modèle est converti en projet. Vous pouvez personnaliser le mappage des rôles avant d’installer le plan directeur. Cliquez sur **[!UICONTROL Voir la description des rôles]** pour en savoir plus sur les rôles disponibles dans le plan directeur.

Le plan directeur effectue des recherches par nom de rôle pour déterminer si des rôles existants correspondent. La recherche respectant la casse, les noms doivent correspondre exactement. Si aucun rôle existant ne correspond, le plan directeur peut les créer pour vous.

![[!UICONTROL Section Mappage des rôles]](assets/Blueprints_RoleMapping.png)

1. Si un rôle existe, vous pouvez choisir l’une des options suivantes :

   1. Créez un rôle portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez un rôle existant, puis sélectionnez un rôle dans la zone de sélection.
   1. N’utilisez pas le rôle mappé. Cette option n’est pas recommandée, car certains rôles ne seront pas affectés à certaines tâches.

1. Si aucun rôle n’existe, vous pouvez choisir l’une des options suivantes :

   1. Créez un rôle. Cette option crée le rôle que le plan directeur recommande.
   1. Créez un rôle portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez un rôle existant, puis sélectionnez un rôle dans la zone de sélection.
   1. N’utilisez pas le rôle mappé. Cette option n’est pas recommandée, car certains rôles ne seront pas affectés à certaines tâches.

>[!NOTE]
>
>Le processus d’installation n’applique pas de rôles à des personnes spécifiques. Vous devez vérifier les personnes qui se trouvent dans ces rôles après avoir installé la solution de plan directeur et affecter des personnes si nécessaire. Pour plus d’informations, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Pour plus d’informations sur les fonctions dans [!DNL Workfront], voir [Créer et gérer des fonctions](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Mappage d’équipes] {#team-mapping}

>[!NOTE]
>
>Cette section peut ne pas apparaître dans certains plans directeurs.

Certains modèles incluent des équipes prescrites. Le travail affecté à une équipe peut être effectué par n’importe quelle personne membre de l’équipe. Vous pouvez personnaliser le mappage des équipes avant d’installer le plan directeur. Cliquez sur **[!UICONTROL Voir les descriptions de l’équipe]** pour en savoir plus sur les équipes disponibles dans le plan directeur.

Le plan directeur effectue des recherches par nom d’équipe pour déterminer si des équipes existantes correspondent. La recherche respectant la casse, les noms doivent correspondre exactement. Si aucune équipe existante ne correspond, le plan directeur peut les créer pour vous.

![[!UICONTROL Section Mappage d’équipes]](assets/Blueprints_TeamMapping.png)

1. Si une équipe existe, vous pouvez choisir l’une des options suivantes :

   1. Créez une équipe portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez [!UICONTROL équipe existante], puis sélectionnez une équipe dans la zone de sélection.
   1. N’utilisez pas l’équipe mappée. Cette option n’est pas recommandée, car certaines tâches n’auront pas d’équipes affectées.

1. Si aucune équipe n’existe, vous pouvez choisir l’une des options suivantes :

   1. Créez une nouvelle équipe. Cette option crée l’équipe recommandée par le plan directeur.
   1. Créez une équipe portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez [!UICONTROL équipe existante], puis sélectionnez une équipe dans la zone de sélection.
   1. N’utilisez pas l’équipe mappée. Cette option n’est pas recommandée, car certaines tâches n’auront pas d’équipes affectées.

>[!NOTE]
>
>Le processus d’installation n’ajoute pas de personnes aux équipes. Vous devez vérifier les personnes des équipes après l’installation de la solution de plan directeur et affecter des personnes si nécessaire. Pour plus d’informations, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Pour plus d’informations sur le fonctionnement des équipes dans [!DNL Workfront], voir [Créer et gérer des équipes](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Mapping d’entreprises {#company-mapping}

>[!NOTE]
>
>Cette section peut ne pas apparaître dans certains plans directeurs.

Certains plans directeurs comportent des entreprises prescrites. Une entreprise est une entité organisationnelle qui peut représenter votre organisation, un service au sein de l’organisation ou un client ou une cliente avec lequel vous travaillez. Vous pouvez personnaliser le mappage des entreprises avant d’installer le plan directeur. Cliquez sur **[!UICONTROL Voir la description des entreprises]** pour en savoir plus sur les entreprises disponibles dans le plan directeur.

Le plan directeur effectue des recherches par nom d’entreprise pour déterminer si des entreprises existantes correspondent. La recherche respectant la casse, les noms doivent correspondre exactement. Si aucune entreprise existante ne correspond, le plan directeur peut les créer pour vous. L’entreprise principale du plan directeur est mappée à l’entreprise principale de votre environnement, même si elle ne porte pas le même nom.

Section ![[!UICONTROL Mappage d’entreprises]](assets/Blueprints_CompanyMapping.png)

1. Si une entreprise existe, vous pouvez choisir l’une des options suivantes :

   1. Créez une entreprise portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez une entreprise existante, puis sélectionnez une entreprise dans la zone de sélection.\

      L’entreprise principale du plan directeur est mappée à l’entreprise principale de votre environnement, même si elle ne porte pas le même nom.
   1. N’utilisez pas l’entreprise mappée. Cette option n’est pas recommandée, car les références de l’entreprise dans d’autres objets seront vides.

1. Si aucune entreprise n’existe, vous pouvez choisir l’une des options suivantes :

   1. Créez une nouvelle entreprise. Cette option crée l’entreprise que le plan directeur recommande.
   1. Créez une entreprise portant un nom différent, puis saisissez le nom dans la zone de texte.
   1. Utilisez une entreprise existante, puis sélectionnez une entreprise dans la zone de sélection.
   1. N’utilisez pas l’entreprise mappée. Cette option n’est pas recommandée, car les références de l’entreprise dans d’autres objets seront vides.

>[!NOTE]
>
>Pour configurer les entreprises après l’installation du plan directeur, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Pour plus d’informations sur l’association d’un modèle à une entreprise, voir [Modifier des modèles de projet](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Pour plus d’informations sur le fonctionnement des entreprises dans [!DNL Workfront], voir [Créer et modifier des entreprises](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Mapper des entreprises] {#group-mapping}

>[!NOTE]
>
>Cette section peut ne pas apparaître dans certains plans directeurs.

Certains plans directeurs comportent des groupes prescrits. Un groupe est un groupe d’utilisateurs et utilisatrices qui correspond à la structure de votre service. Les groupes sont similaires aux équipes et aux entreprises de Workfront, mais distincts. Vous pouvez personnaliser le mappage des groupes avant d’installer le plan directeur. Cliquez sur **[!UICONTROL Voir la description des groupes]** pour en savoir plus sur les groupes disponibles dans le plan directeur.

Le plan directeur effectue des recherches par nom de groupe pour déterminer si des groupes existants correspondent. La recherche respectant la casse, les noms doivent correspondre exactement. Si aucun groupe existant ne correspond, le plan directeur peut les créer pour vous.

Section ![[!UICONTROL Mapper des groupes] &#x200B;](assets/Blueprints_GroupMapping.png)

1. Si un groupe existe, vous pouvez sélectionner **[!UICONTROL Remapper un groupe]** et sélectionnez l’une des options suivantes :

   1. **[!UICONTROL Créez un groupe portant un nom différent]**, puis saisissez le nom à affecter à ce groupe. Les références au groupe dans la définition de plan directeur seront associées à ce nouveau groupe à la place.
   1. **[!UICONTROL Remplacez par un groupe existant]**, puis recherchez et sélectionnez un groupe dans la zone de sélection.

      >[!NOTE]
      >
      >Vous ne pouvez pas renommer un groupe existant.

1. Si un groupe n’existe pas, vous pouvez :

   1. Modifiez le nom du groupe suggéré en le saisissant dans la zone de texte.
   1. Sélectionnez **[!UICONTROL Remapper un groupe]** et choisissez [!UICONTROL Remplacer par un groupe existant], puis recherchez et sélectionnez un groupe dans la zone de sélection.
   1. Sélectionner **[!UICONTROL Remapper un groupe]** et choisissez **[!UICONTROL Insérer sous un groupe existant]**, puis recherchez et sélectionnez un groupe dans la zone de sélection. Cette option crée un sous-groupe sous le groupe existant.

>[!NOTE]
>
>Pour configurer les groupes après l’installation du plan directeur, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Pour plus d’informations sur l’utilisation des groupes dans [!DNL Workfront], voir [Vue d’ensemble des groupes](../../administration-and-setup/manage-groups/groups-overview/groups.md).
