---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Accès requis pour utiliser le planificateur de scénarios
description: Le planificateur de scénarios nécessite une licence distincte d’Adobe Workfront et un accès supplémentaire.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: f0f6c2bee98c6cebf8ea9e18bf34262f3c1d6e3a
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 1%

---

# Accès nécessaire pour utiliser le [!DNL Scenario Planner]

[!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur [!DNL Workfront Scenario Planner], voir [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Sans accès ou autorisations corrects, vous ne pourrez peut-être pas afficher la zone [!UICONTROL Scénarios] de[!DNL  Adobe Workfront] ni gérer les plans ou les initiatives pour votre organisation. La gestion des plans et des initiatives comprend la création, la modification et la suppression.

>[!IMPORTANT]
>
>Lors de l’accès à [!UICONTROL Scénarios], vous pouvez uniquement afficher et gérer les plans que vous avez créés. Si vous souhaitez permettre à d’autres utilisateurs d’afficher ou de gérer les plans que vous avez créés, vous devez effectuer les opérations suivantes :
>
>* Envoyer un lien vers votre plan à d’autres utilisateurs
>* Partager le plan avec d’autres utilisateurs
>
>  Pour plus d’informations sur le partage d’un plan, voir [Partager un plan dans le  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Lorsqu’un utilisateur est désactivé, ses plans n’ont pas de propriétaire et ne sont pas accessibles, sauf s’ils ont été partagés précédemment avec un lien.

## Accès nécessaire pour afficher et utiliser le [!DNL Adobe Workfront Scenario Planner]

Vous devez vous assurer que toutes les conditions suivantes sont remplies avant de pouvoir accéder au [!DNL Workfront Scenario Planner] :

1. Votre entreprise doit avoir l’un des plans Workfront décrits ci-dessous.

   Selon que vous utilisez le nouveau plan Workfront ou le plan actuel, votre entreprise doit disposer de l’une des options suivantes :

   * Pour les nouveaux plans, votre organisation doit disposer de l’une des options suivantes :

      * Formule [!UICONTROL Ultimate] [!DNL Workfront]. Le planificateur de scénario est inclus dans le plan final.

        Ou

      * Le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront], en plus d&#39;acheter une licence [!DNL Scenario Planner] distincte.

   * Pour les plans Workfront actuels, votre organisation doit disposer des deux éléments suivants :

      * Votre entreprise doit acheter un abonnement [!DNL Workfront] [!UICONTROL Business] ou supérieur [!DNL Workfront]. Pour plus d’informations sur les [!DNL Workfront] plans, voir [Formules Workfront](https://workfront.com/plans).

      * Votre entreprise doit acheter une licence [!DNL Workfront Scenario Planner] en plus d’une licence [!DNL Workfront]. Contactez votre gestionnaire de compte [!DNL Workfront] pour en savoir plus sur les licences [!DNL Workfront Scenario Planner].

1. Vous devez disposer de l’une des licences Workfront décrites ci-dessous.

   Selon que vous utilisez les nouvelles licences ou les licences actuelles, votre administrateur [!DNL Workfront] doit vous attribuer une licence de l’un des types suivants :

   * Pour les nouvelles licences :
      * [!UICONTROL Standard]
      * [!UICONTROL Light]

   * Pour les licences actuelles :

      * [!UICONTROL Plan]
      * [!UICONTROL Travail]
      * [!UICONTROL Révision]

   >[!NOTE]
   > 
   >* Lors de l’utilisation des nouvelles licences, les utilisateurs avec un type de licence [!UICONTROL Contributor] ou [!UICONTROL External] ne peuvent pas accéder à [!DNL Scenario Planner].
   >
   >* Lors de l’utilisation des licences actuelles, les utilisateurs avec un type de licence Demander ou Externe ne peuvent pas accéder au planificateur de scénario.

1. Votre administrateur [!DNL Workfront] doit vous donner l&#39;accès [!UICONTROL Affichage] ou [!UICONTROL Modifier] à [!DNL Scenario Planner] de votre niveau d&#39;accès.

   Pour plus d&#39;informations sur l&#39;octroi de l&#39;accès à [!DNL Workfront Scenario Planner], voir [Accorder l&#39;accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facultatif et recommandé) Pour afficher ou mettre à jour les informations financières relatives à vos plans et initiatives, votre administrateur [!DNL Workfront] doit également vous accorder l’accès aux [!UICONTROL données financières] de votre niveau d’accès. Pour plus d’informations sur l’octroi de données financières à votre niveau d’accès, voir [Accorder l’accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Facultatif) Si vous devez accéder aux plans que vous n’avez pas créés, un créateur de plans doit vous accorder les autorisations appropriées pour y accéder. Pour plus d’informations sur les autorisations nécessaires pour accéder aux plans et initiatives que vous n’avez pas créés, consultez la section [Autorisations nécessaires pour accéder aux plans et initiatives](#permissions-needed-to-access-plans-and-initiatives) de cet article.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Accès nécessaire à l’affichage des plans et des initiatives

Outre l&#39;acquisition par votre société de la licence appropriée pour [!DNL Workfront Scenario Planner], votre administrateur [!DNL Workfront] doit également vous attribuer l&#39;accès et la configuration suivants afin que vous puissiez afficher le [!DNL Workfront Scenario Planner] et les informations dans ce domaine :

* Un niveau d&#39;accès avec au moins [!UICONTROL Affichage] accès à [!DNL Scenario Planner].

  Pour plus d&#39;informations sur le niveau d&#39;accès à [!DNL Scenario Planner], voir [Accorder l&#39;accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un niveau d’accès avec au moins [!UICONTROL Affichage] accès à [!UICONTROL Données financières] si vous devez également consulter des informations financières sur le plan et les initiatives. Les budgets, les coûts ou les taux de rôle professionnel constituent quelques exemples d’informations financières.

  Pour plus d&#39;informations sur le niveau d&#39;accès [!UICONTROL Données financières], voir [Accorder l&#39;accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] et [!UICONTROL External] Les utilisateurs n&#39;ont pas accès à l&#39;affichage de [!DNL Scenario Planner].

* Afficher les autorisations du plan. Pour plus d’informations sur les autorisations nécessaires pour accéder aux plans et initiatives que vous n’avez pas créés, consultez la section [Autorisations nécessaires pour accéder aux plans et initiatives](#permissions-needed-to-access-plans-and-initiatives) de cet article.

## Accès nécessaire à la gestion des plans et des initiatives

Votre administrateur [!DNL Workfront] doit vous attribuer l’accès suivant afin que vous puissiez gérer les plans et leurs informations dans le [!DNL Scenario Planner] :

* Un type de licence [!UICONTROL Plan] ou [!UICONTROL Work] avec l’accès Modifier à [!DNL Scenario Planner] de votre niveau d’accès.

  Tous les autres types de licence n’ont pas accès à la gestion des plans.

  Pour plus d’informations sur l’octroi de l’accès à [!DNL Scenario Planner] à partir du niveau d’accès, voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un type de licence [!UICONTROL Plan] avec l’accès [!UICONTROL Edit] à [!UICONTROL Financial Data] dans votre niveau d’accès, si vous devez également mettre à jour les informations financières sur le plan.

  [!UICONTROL Budget], [!UICONTROL Avantage planifié] et [!UICONTROL Coûts fixes] sont quelques exemples d’informations financières que vous pouvez modifier.

  >[!TIP]
  >
  >Seuls les titulaires de licence [!UICONTROL Plan] ont un accès [!UICONTROL Modifier] à [!UICONTROL Données financières].

  Pour plus d&#39;informations sur le niveau d&#39;accès [!UICONTROL Données financières], voir [Accorder l&#39;accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Gérez les autorisations d’un plan que vous n’avez pas créé. Pour plus d’informations sur les autorisations nécessaires pour accéder aux plans et initiatives que vous n’avez pas créés, consultez la section [Autorisations nécessaires pour accéder aux plans et initiatives](#permissions-needed-to-access-plans-and-initiatives) de cet article.

## Autorisations nécessaires pour accéder aux plans et aux initiatives

Les niveaux d’accès fonctionnent ensemble avec les autorisations dans [!DNL Workfront] pour vous donner une visibilité sur les plans et initiatives que vous n’avez pas créés. Outre le niveau d’accès correct pour accéder à [!DNL Scenario Planner], vous devez également disposer des autorisations correctes pour le plan que vous souhaitez afficher ou gérer, si vous n’êtes pas le créateur de ces plans.

Par défaut, vous n’avez accès qu’aux plans que vous avez créés. Pour afficher les plans créés par d’autres utilisateurs, ils doivent partager leurs plans avec vous. Pour plus d’informations sur le partage de plans, voir [Partager un plan dans le  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Si un utilisateur partage un lien vers un plan sans le partager, vous pouvez demander des autorisations sur le plan. Pour plus d’informations sur la demande d’autorisations pour les plans, voir [Demande d’accès à un plan dans le  [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

