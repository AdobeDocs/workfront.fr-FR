---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organisations et équipes Adobe Workfront Fusion
description: Les fonctionnalités Organisation et Équipes Adobe Workfront Fusion permettent aux entreprises de contrôler l’accès aux scénarios et aux autres fonctionnalités dans Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 063c4a885d43b41ba6ff72ac22a1552486531fa6
workflow-type: tm+mt
source-wordcount: '1239'
ht-degree: 100%

---

# Organisations et équipes [!DNL Adobe Workfront Fusion]

Les fonctionnalités Organisation et Équipes [!DNL Adobe Workfront Fusion] permettent aux entreprises de contrôler l’accès aux scénarios et aux autres fonctionnalités dans Fusion.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>[!DNL Pro] ou une version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigence de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigence de produit hérité : votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> 
     <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront Fusion] de votre organisation.</p>
     <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront Fusion] de votre équipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

<p>**Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>.</p>


## Organisations

Les utilisateurs et utilisatrices [!DNL Workfront Fusion] appartiennent à une organisation.

* [Rôles d’organisation](#organization-roles)
* [Inviter des utilisateurs et des utilisatrices dans une organisation](#inviting-users-to-an-organization)
* [Basculer entre des organisations](#switch-between-organizations)

### Rôles d’organisation

Un utilisateur ou une utilisatrice possède l’un des rôles suivants dans une organisation :

* **[!UICONTROL Personne propriétaire]** : la personne propriétaire dispose de toutes les autorisations disponibles dans l’organisation.
* **[!UICONTROL Administration]** : le rôle d’administration permet à un utilisateur ou à une utilisatrice de créer et de gérer des équipes ainsi que des utilisateurs et des utilisatrices pour l’organisation.
* **[!UICONTROL Personne membre]** : les personnes membres peuvent utiliser [!DNL Workfront Fusion] mais ne peuvent pas apporter de changements organisationnels.
* **[!UICONTROL Personne comptable]** : le rôle de personne comptable permet uniquement aux utilisateurs et aux utilisatrices d’afficher les informations de licence dans le tableau de bord de l’organisation.
* **[!UICONTROL Développeur ou développeuse d’applications]** : les fonctionnalités de ce rôle ne sont actuellement pas disponibles. Elle seront disponibles ultérieurement. Il est déconseillé d’affecter des utilisateurs et des utilisatrices à ce rôle pour l’instant.

Pour plus d’informations sur les actions spécifiques dont disposent les utilisateurs et les utilisatrices pour chaque rôle d’organisation, voir [Rôles d’organisation et d’équipe](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Inviter des utilisateurs et des utilisatrices dans une organisation

Par défaut, la personne propriétaire d’une organisation (ou une personne autorisée) peut inviter une autre personne à rejoindre son organisation.

Pour inviter un utilisateur ou une utilisatrice à rejoindre une organisation :

1. Cliquez sur **[!UICONTROL Modifier les détails]** dans le coin supérieur droit de l’écran.
1. Sélectionnez **[!UICONTROL Inviter un nouvel utilisateur ou une nouvelle utilisatrice]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Renseignez l’adresse e-mail et le nom de l’utilisateur ou de l’utilisatrice.
1. Sélectionnez un rôle pour l’utilisateur ou l’utilisatrice. Pour plus d’informations sur les rôles, voir [Rôles d’organisation](#organization-roles) dans ce document.
1. (Facultatif) Ajoutez une note. Cette note s’affiche dans l’e-mail d’invitation que l’utilisateur ou l’utilisatrice reçoit.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

[!DNL Fusion] envoie un e-mail comportant une invitation à rejoindre l’organisation spécifique et un bouton [!UICONTROL Accepter le rôle].

Lorsque la personne destinataire clique sur le bouton, celle-ci est redirigée vers la page d’invitation, où elle peut accepter l’invitation.

L’invitation expire après un jour.

>[!NOTE]
>
>Si l’utilisateur ou l’utilisatrice utilise [!DNL Fusion] pour la première fois, [!DNL Fusion] lui crée automatiquement un compte et lui envoie un e-mail avec un mot de passe temporaire, invitant le nouvel utilisateur ou la nouvelle utilisatrice à se connecter et à changer son mot de passe.

### Basculer entre des organisations

Vous pouvez faire partie de plusieurs organisations dans Fusion. Les ressources ne sont pas partagées entre les organisations.

Vous pouvez changer d’organisation dans Adobe Unified Experience en cliquant sur le nom de l’organisation dans le coin supérieur droit et en sélectionnant la nouvelle organisation dans la liste déroulante. Seules les organisations disposant d’un compte Fusion s’affichent dans la liste déroulante, même si vous êtes une personne membre d’autres organisations dans Adobe.

## Équipes

Les équipes sont des groupes d’utilisateurs et d’utilisatrices qui partagent un accès à des ressources spécifiques. Ces ressources peuvent inclure les éléments suivants :

* Scénarios
* Connexions
* Webhooks
* Clés
* Magasins de données
* Structures de données
* Paramètres de notification par e-mail

>[!NOTE]
>
>Étant donné que les équipes contrôlent l’accès aux ressources, il est parfois utile qu’une équipe ne comporte qu’une seule personne membre. Par exemple, les utilisateurs et les utilisatrices en formation peuvent créer des connexions avec leur comptes [!DNL Google] individuels. Toute personne membre de l’équipe peut également se connecter son compte [!DNL Google] individuel, il est donc préférable, dans ce cas, que la personne soit l’unique personne membre d’une équipe de formation.

Les organisations peuvent disposer d’autant d’équipes que nécessaire et les utilisateurs et les utilisatrices peuvent appartenir à une ou plusieurs équipes.

Les utilisateurs et les utilisatrices peuvent sélectionner leur équipe dans la liste déroulante du panneau de navigation de gauche. Les utilisateurs et les utilisatrices ne voient que les équipes dont ils font partie. Sélectionner une équipe permet à un utilisateur ou à une utilisatrice d’accéder aux ressources de cette équipe.

* [Rôles d’équipe](#team-roles)
* [Gestion des équipes](#team-management)

### Rôles d’équipe

Un utilisateur ou une utilisatrice possède l’un des rôles suivants dans chacune de ses équipes :

* **[!UICONTROL Administration d’équipe]** : en plus des fonctionnalités des autres rôles d’équipe, le rôle d’administration permet à l’utilisateur ou à l’utilisatrice d’ajouter, de supprimer ou de modifier le rôle d’une personne membre de l’équipe.
* **[!UICONTROL Personne membre de l’équipe]** : le rôle de personne membre de l’équipe permet aux utilisateurs et aux utilisatrices de créer et d’exécuter des scénarios.
* **[!UICONTROL Surveillance de l’équipe]** : le rôle de [!UICONTROL surveillance] permet aux utilisateurs et aux utilisatrices d’accéder aux informations d’exécution pour les scénarios, mais ils ne peuvent pas concevoir de scénarios ou modifier leur statut « actif ».
* **[!UICONTROL Opérateur ou opératrice d’équipe]** : le rôle d’[!UICONTROL opérateur ou opératrice] permet aux utilisateurs et aux utilisatrices d’afficher les données d’exécution et de modifier le statut « actif » des scénarios.
* **[!UICONTROL Personne membre de l’équipe limitée]** : les fonctionnalités de ce rôle ne sont actuellement pas disponibles. Elles seront disponibles ultérieurement. Il est déconseillé d’affecter des utilisateurs et des utilisatrices à ce rôle pour l’instant.

Pour plus d’informations sur les actions spécifiques dont les utilisateurs et les utilisatrices disposent dans chaque rôle d’équipe, voir [Rôles d’organisation et d’équipe](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Gestion des équipes

* [Créer une équipe](#create-a-team)
* [Définir les options de notification d’équipe](#set-team-notification-options)

#### Créer une équipe

Les personnes propriétaires d’organisation ainsi que les administrateurs et administratrices d’organisation peuvent créer des équipes.

Pour créer une équipe :

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Organisation]**.
1. Sélectionnez l’onglet **[!UICONTROL Équipe]**.
1. Cliquez sur **[!UICONTROL Ajouter une nouvelle équipe]** sous la liste des équipes.
1. Saisissez le nom de la nouvelle équipe, puis cliquez sur **Ajouter**.

#### Définir les options de notification pour l’équipe

>[!NOTE]
>
>Si votre entreprise a migré vers Unified Shell, vous recevez des notifications par le biais de la zone Notifications d’Adobe. Vous devez utiliser l’expérience Unified Shell pour afficher des notifications dans la zone Notifications d’Adobe.
>
>Pour utiliser l’expérience Unified Shell, y compris la zone Notifications d’Adobe, cliquez sur le bouton Essayer la nouvelle interface d’utilisation de Fusion dans le bouton Unified Experience près de la partie supérieure de la page. Ce bouton n’est disponible que si votre entreprise a migré vers Unified Shell.
>
>Pour plus d’informations, consultez la section [Accéder à vos notifications](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md#access-your-notifications) dans [!DNL Adobe Unified Experience] pour [!DNL Workfront Fusion].

Les options de notification par e-mail sont définies au niveau de l’équipe.

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Équipe]**.
1. Sélectionnez l’onglet **[!UICONTROL Options de notification]**.
1. Activez les notifications que vous souhaitez que l’équipe reçoive.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">« [!UICONTROL Warning in scenario run] »</td> 
      <td> <p>Recevez un e-mail lorsqu’un avertissement se produit dans une exécution de scénario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Errors in scenario run]</td> 
      <td>Recevez un e-mail en cas d’erreur lors de l’exécution d’un scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Scenario deactivation]</p> </td> 
      <td><p>Recevez un e-mail lorsqu’un scénario se désactive.</p><p><b>Note :</b> vous recevez une notification vous informant de la désactivation d’un scénario uniquement lorsque celui-ci a été automatiquement désactivé en raison d’erreurs. Vous ne recevez pas de notifications concernant les scénarios qui sont désactivés manuellement.</p><p>Dans certains cas, un scénario peut être désactivé par l’équipe technique [!DNL Workfront Fusion] si le scénario cause des problèmes de performance ou d’autres types de problèmes. Dans ce cas, vous ne recevez pas de notifications dans [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Les modifications apportées aux options de notification sont automatiquement enregistrées.

#### Basculer entre les équipes

Vous pouvez faire partie de plusieurs équipes dans Fusion. Étant donné que les équipes ne partagent pas leurs ressources, vous devrez peut-être changer d’équipe pour accéder à des scénarios spécifiques ou à d’autres ressources.

Si votre organisation ne figure pas dans Adobe Unified Experience, vous pouvez changer d’équipe en cliquant sur le nom de l’équipe dans le volet de navigation de gauche, puis en sélectionnant une équipe dans la liste déroulante.

Si votre équipe se trouve dans Adobe Unified Experience, vous pouvez sélectionner une nouvelle équipe en cliquant sur le nom de l’équipe dans l’en-tête, puis en sélectionnant une équipe dans la liste déroulante. Cette option est disponible à partir de toutes les pages spécifiques à une équipe donnée, comme une page de scénario ou la page Connexions.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->