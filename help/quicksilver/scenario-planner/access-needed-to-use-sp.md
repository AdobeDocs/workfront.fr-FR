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
ht-degree: 0%

---

# Accès nécessaire pour utiliser la variable [!DNL Scenario Planner]

La variable [!DNL Scenario Planner] nécessite une licence supplémentaire. Pour plus d’informations sur la variable [!DNL Workfront Scenario Planner], voir [La variable [!DNL Scenario Planner] aperçu](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Sans accès ou autorisations corrects, vous ne pourrez peut-être pas afficher la variable [!UICONTROL Scénarios] area of[!DNL  Adobe Workfront] ou ne gérez pas les plans ou les initiatives de votre entreprise. La gestion des plans et des initiatives comprend la création, la modification et la suppression.

>[!IMPORTANT]
>
>Lors de l’accès [!UICONTROL Scénarios], vous pouvez uniquement afficher et gérer les plans que vous avez créés. Si vous souhaitez permettre à d’autres utilisateurs d’afficher ou de gérer les plans que vous avez créés, vous devez effectuer les opérations suivantes :
>
>* Envoyer un lien vers votre plan à d’autres utilisateurs
>* Partager le plan avec d’autres utilisateurs
>
>  Pour plus d’informations sur le partage d’un plan, voir [Partager un plan dans la [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Lorsqu’un utilisateur est désactivé, ses plans n’ont pas de propriétaire et ne sont pas accessibles, sauf s’ils ont été partagés précédemment avec un lien.

## Accès nécessaire pour afficher et utiliser le [!DNL Adobe Workfront Scenario Planner]

Vous devez vous assurer que toutes les conditions suivantes sont remplies avant d’accéder à la variable [!DNL Workfront Scenario Planner]:

1. Votre entreprise doit avoir l’un des plans Workfront décrits ci-dessous.

   Selon que vous utilisez le nouveau plan Workfront ou le plan actuel, votre entreprise doit disposer de l’une des options suivantes :

   * Pour les nouveaux plans, votre organisation doit disposer de l’une des options suivantes :

      * La variable [!UICONTROL Ultimate] [!DNL Workfront] planifiez. Le planificateur de scénario est inclus dans le plan final.

        Ou

      * La variable [!UICONTROL Sélectionner] ou [!UICONTROL Prime] [!DNL Workfront] planifier, en plus d’acheter une [!DNL Scenario Planner] licence.

   * Pour les plans Workfront actuels, votre organisation doit disposer des deux éléments suivants :

      * Votre entreprise doit acheter un [!DNL Workfront] [!UICONTROL Entreprises] ou supérieur [!DNL Workfront] planifiez. Pour plus d’informations sur la variable [!DNL Workfront] plans, voir [Formules Workfront](https://workfront.com/plans).

      * Votre entreprise doit acheter un [!DNL Workfront Scenario Planner] , en plus d’une [!DNL Workfront] licence. Contactez votre [!DNL Workfront] Représentant du compte pour en savoir plus sur [!DNL Workfront Scenario Planner] licences.

1. Vous devez disposer de l’une des licences Workfront décrites ci-dessous.

   Selon que vous utilisez les nouvelles licences ou les licences actuelles, votre [!DNL Workfront] L’administrateur doit vous attribuer une licence de l’un des types suivants :

   * Pour les nouvelles licences :
      * [!UICONTROL Standard]
      * [!UICONTROL Lumière]

   * Pour les licences actuelles :

      * [!UICONTROL Planifier]
      * [!UICONTROL Travail]
      * [!UICONTROL Réviser]

   >[!NOTE]
   > 
   >* Lors de l’utilisation des nouvelles licences, les utilisateurs disposant d’un [!UICONTROL Contributeur] ou [!UICONTROL Externe] le type de licence ne peut pas accéder au [!DNL Scenario Planner].
   >
   >* Lors de l’utilisation des licences actuelles, les utilisateurs avec un type de licence Demander ou Externe ne peuvent pas accéder au planificateur de scénario.

1. Votre [!DNL Workfront] L’administrateur doit vous indiquer [!UICONTROL Affichage] ou [!UICONTROL Modifier] accès à [!DNL Scenario Planner] dans votre niveau d’accès.

   Pour plus d’informations sur l’octroi de l’accès au [!DNL Workfront Scenario Planner], voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Facultatif et recommandé) Pour afficher ou mettre à jour les informations financières relatives à vos plans et initiatives, votre [!DNL Workfront] L’administrateur doit également vous accorder l’accès [!UICONTROL Données financières] dans votre niveau d’accès. Pour plus d’informations sur l’octroi de données financières à votre niveau d’accès, voir [Accorder l&#39;accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Facultatif) Si vous devez accéder aux plans que vous n’avez pas créés, un créateur de plans doit vous accorder les autorisations appropriées pour y accéder. Pour plus d’informations sur les autorisations nécessaires pour accéder aux plans et initiatives que vous n’avez pas créés, voir la section [Autorisations nécessaires pour accéder aux plans et aux initiatives](#permissions-needed-to-access-plans-and-initiatives) dans cet article.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Accès nécessaire à l’affichage des plans et des initiatives

En plus de votre entreprise qui acquiert la licence appropriée pour la variable [!DNL Workfront Scenario Planner], votre [!DNL Workfront] L’administrateur doit également vous attribuer l’accès et la configuration suivants afin que vous puissiez afficher la variable [!DNL Workfront Scenario Planner] et les informations dans ce domaine :

* Un niveau d’accès avec au moins [!UICONTROL Affichage] accès à [!DNL Scenario Planner].

  Pour plus d’informations sur le niveau d’accès à [!DNL Scenario Planner], voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un niveau d’accès avec au moins [!UICONTROL Affichage] accès à [!UICONTROL Données financières] si vous devez également consulter des informations financières sur le plan et les initiatives. Les budgets, les coûts ou les taux de rôle professionnel constituent quelques exemples d’informations financières.

  Pour plus d’informations sur la variable [!UICONTROL Données financières] niveau d’accès, voir [Accorder l&#39;accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Demandeurs] et [!UICONTROL Externe] Les utilisateurs n’ont pas accès à la fonction [!DNL Scenario Planner].

* Afficher les autorisations du plan. Pour plus d’informations sur les autorisations nécessaires pour accéder aux plans et initiatives que vous n’avez pas créés, voir la section [Autorisations nécessaires pour accéder aux plans et aux initiatives](#permissions-needed-to-access-plans-and-initiatives) dans cet article.

## Accès nécessaire à la gestion des plans et des initiatives

Votre [!DNL Workfront] l’administrateur doit vous attribuer l’accès suivant afin que vous puissiez gérer les plans et leurs informations dans la variable [!DNL Scenario Planner]:

* A [!UICONTROL Planifier] ou [!UICONTROL Travail] type de licence avec l’accès Modifier à la propriété [!DNL Scenario Planner] dans votre niveau d’accès.

  Tous les autres types de licence n’ont pas accès à la gestion des plans.

  Pour plus d’informations sur l’octroi de l’accès à [!DNL Scenario Planner] à partir du niveau d’accès, voir [Accorder l’accès à [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Planifier] type de licence avec [!UICONTROL Modifier] accès à [!UICONTROL Données financières] dans votre niveau d’accès, si vous devez également mettre à jour les informations financières sur le plan.

  Voici quelques exemples d’informations financières que vous pouvez modifier : [!UICONTROL Budget], [!UICONTROL Avantage planifié], et [!UICONTROL Coûts fixes].

  >[!TIP]
  >
  >Uniquement [!UICONTROL Planifier] les titulaires de licence ont [!UICONTROL Modifier] accès à [!UICONTROL Données financières].

  Pour plus d’informations sur la variable [!UICONTROL Données financières] niveau d’accès, voir [Accorder l&#39;accès aux données financières](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Gérez les autorisations d’un plan que vous n’avez pas créé. Pour plus d’informations sur les autorisations nécessaires pour accéder aux plans et initiatives que vous n’avez pas créés, voir la section [Autorisations nécessaires pour accéder aux plans et aux initiatives](#permissions-needed-to-access-plans-and-initiatives) dans cet article.

## Autorisations nécessaires pour accéder aux plans et aux initiatives

Les niveaux d’accès fonctionnent avec les autorisations dans [!DNL Workfront] pour vous donner une visibilité aux plans et initiatives que vous n’avez pas créés. Outre le niveau d’accès correct pour accéder à la variable [!DNL Scenario Planner], vous devez également disposer des autorisations appropriées pour le plan que vous souhaitez afficher ou gérer, si vous n’êtes pas l’auteur de ces plans.

Par défaut, vous n’avez accès qu’aux plans que vous avez créés. Pour afficher les plans créés par d’autres utilisateurs, ils doivent partager leurs plans avec vous. Pour plus d’informations sur le partage de plans, voir [Partager un plan dans la [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Si un utilisateur partage un lien vers un plan sans le partager, vous pouvez demander des autorisations sur le plan. Pour plus d’informations sur la demande d’autorisations pour les plans, voir [Demandez l’accès à un plan dans la [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

