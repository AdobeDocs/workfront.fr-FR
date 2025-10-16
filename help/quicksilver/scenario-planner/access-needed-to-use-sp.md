---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Accès nécessaire pour utiliser le planificateur de scénarios
description: Le planificateur de scénarios nécessite une licence distincte d’Adobe Workfront et un accès supplémentaire.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 1b06589a705cf218239ff1273b865c05e4ceb96f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 60%

---

# Accès requis pour utiliser le [!DNL Scenario Planner]

<!--Audited: 04/2024-->

<!--The [!DNL Scenario Planner] has additional license requirements. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).-->

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Sans les accès ou autorisations nécessaires, vous ne pourrez peut-être pas afficher la zone [!UICONTROL Scénarios] d’[!DNL  Adobe Workfront] ou gérer les plans ou les initiatives de votre entreprise. La gestion des plans et des initiatives comprend leur création, leur modification et leur suppression.

## Accès nécessaire pour afficher et utiliser le [!DNL Adobe Workfront Scenario Planner]

Vous devez vous assurer que toutes les conditions suivantes sont remplies avant d’accéder au [!DNL Workfront Scenario Planner] :

1. Votre organisation doit disposer d’un package Workfront Ultimate.

   Le planificateur de scénarios n’est pas disponible pour les packages de workflow Workfront.

   Contactez le représentant de votre compte Workfront si vous renouvelez actuellement Workfront et que vous souhaitez conserver le planificateur de scénarios.

   Si vous êtes un nouveau client, le planificateur de scénarios n’est plus disponible à l’achat.

   <!--Old: 
    Depending on whether you use the new or the current Workfront plan, your organization must have one of the following:
    * For the new plans, your organization must have the  [!UICONTROL Ultimate] [!DNL Workfront] plan. The Scenario Planner is included only in the [!UICONTROL Ultimate] plan. 
    * For the current Workfront plans, your organization must have both of the following: 
      * Your organization must purchase a [!DNL Workfront] [!UICONTROL Business] or higher [!DNL Workfront] plan. 
      
      * Your organization must purchase a [!DNL Workfront Scenario Planner] license, in addition to a [!DNL Workfront] license. Contact your [!DNL Workfront] Account Representative to learn about [!DNL Workfront Scenario Planner] licenses. -->

1. Vous devez disposer de l’une des licences Workfront suivantes :

   * [!UICONTROL Léger] ou supérieur
   * [!UICONTROL Réviseur] ou version ultérieure

   <!--Old: 
      * For the current licenses: 
        * [!UICONTROL Plan]
        * [!UICONTROL Work]
        * [!UICONTROL Review]-->
   <!--Old: 
      >[!NOTE]
      > 
      >* When using the new licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
      >
      >* When using the current licenses, users with a Request or External license type cannot access the Scenario Planner. -->

1. Votre administrateur ou administratrice [!DNL Workfront] doit vous accorder l’accès en [!UICONTROL affichage] ou en [!UICONTROL modification] au [!DNL Scenario Planner].

   Pour plus d’informations sur l’octroi des accès au [!DNL Workfront Scenario Planner], consultez [Accorder l’accès au  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facultatif et recommandé) Pour afficher ou mettre à jour les informations financières relatives à vos plans et initiatives, votre administrateur ou administratrice [!DNL Workfront] doit également vous accorder l’accès aux [!UICONTROL données financières]. Pour plus d’informations sur l’octroi des accès aux données financières, consultez [Accorder l’accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).


<!--1. (Optional) If you need to access plans you didn't create, a plan creator must give you the correct permissions to their plan to access it. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.-->

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

<!--Repetitive from above?? 

## Access needed to view plans and initiatives

In addition to your company acquiring the correct license for the [!DNL Workfront Scenario Planner], your [!DNL Workfront] administrator must also assign you the following access and setup so you can view the [!DNL Workfront Scenario Planner] and the information in this area:

* An access level with at least [!UICONTROL View] access to [!DNL Scenario Planner].

  For information about the access level to [!DNL Scenario Planner], see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* An access level with at least [!UICONTROL View] access to [!UICONTROL Financial Data] if you need to also view financial information about the plan and the initiatives. Some examples of financial information are budgets, costs, or job role rates.

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] and [!UICONTROL External] Users do not have access to view the [!DNL Scenario Planner].

* View permissions to the plan. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

## Access needed to manage plans and initiatives

Your [!DNL Workfront] administrator must assign you the following access so you can manage plans and their information in the [!DNL Scenario Planner]:

* A [!UICONTROL Plan] or [!UICONTROL Work] license type with Edit access to the [!DNL Scenario Planner] in your access level.

  All other license types do not have access to manage plans.

  For information about granting access to [!DNL Scenario Planner] from the Access Level, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] license type with [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level, if you need to also update financial information about the plan.

  Some examples of financial information that you can edit are [!UICONTROL Budget], [!UICONTROL Planned Benefit], and [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Only [!UICONTROL Plan] license holders have [!UICONTROL Edit] access to [!UICONTROL Financial Data].

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Manage permissions to a plan that you didn't create. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

-->

## Autorisations nécessaires pour accéder aux plans et aux initiatives

Les niveaux d’accès fonctionnent avec les autorisations dans [!DNL Workfront] pour vous donner une visibilité sur les plans et les initiatives que vous n’avez pas créés. Outre le niveau d’accès approprié pour accéder au [!DNL Scenario Planner], vous devez également disposer des autorisations appropriées pour les plans que vous souhaitez afficher ou gérer, si vous n’êtes pas le créateur de ces plans.

Tous les utilisateurs, y compris les administrateurs système, n’ont accès qu’aux plans qu’ils ont créés.

Pour afficher les plans créés par d’autres utilisateurs, ils doivent vous les partager comme suit :

* Partager le plan avec vous

  Pour plus d’informations sur le partage de plans, voir [Partager un plan dans le  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

* Envoyer un lien vers un plan qu’ils ont créé

  Si un utilisateur ou une utilisatrice partage un lien vers un plan, mais sans partager le plan, vous pouvez demander des autorisations pour le plan. Pour plus d’informations sur la demande d’autorisations pour les plans, voir [Demander l’accès à un plan dans le  [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

>[!NOTE]
>
>Lorsqu’une personne est désactivée, ses plans n’ont pas de personne propriétaire et ne sont pas accessibles, sauf s’ils ont été partagés précédemment avec un lien.


