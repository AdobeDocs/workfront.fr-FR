---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organisations et équipes d’Adobe Workfront Fusion
description: Les fonctionnalités dédiées aux organisations et aux équipes d’Adobe Workfront Fusion permettent aux entreprises de contrôler l’accès aux scénarios et aux autres fonctionnalités de Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 063c4a885d43b41ba6ff72ac22a1552486531fa6
workflow-type: ht
source-wordcount: '1239'
ht-degree: 100%

---

# Organisations et équipes d’[!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion]Les fonctionnalités pour les organisations et les équipes permettent aux entreprises de contrôler l’accès aux scénarios et aux autres fonctionnalités dans Fusion.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] forfait*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> 
     <p>Vous devez être un administrateur ou une administratrice de [!DNL Workfront Fusion] pour votre organisation.</p>
     <p>Vous devez être un administrateur ou une administratrice de [!DNL Workfront Fusion] pour votre équipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

<p>Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]licences</a>.</p>


## Organisations

Les utilisateurs et utilisatrices de [!DNL Workfront Fusion] appartiennent à une organisation.

* [Rôles dans l’organisation](#organization-roles)
* [Inviter des utilisateurs à une organisation](#inviting-users-to-an-organization)
* [Passer à une autre organisation](#switch-between-organizations)

### Rôles dans l’organisation

Les rôles suivants sont disponibles au sein d’une organisation :

* **[!UICONTROL Propriétaire]** : la personne propriétaire dispose de toutes les autorisations disponibles dans l’organisation.
* **[!UICONTROL Administration]** : le rôle d’administration permet à une personne de créer et de gérer des équipes et des utilisateurs et utilisatrices pour l’organisation.
* **[!UICONTROL Membre]** : les membres peuvent utiliser [!DNL Workfront Fusion], mais ne peuvent pas apporter de changements organisationnels.
* **[!UICONTROL Comptable]** : un rôle de comptable permet uniquement d’afficher les informations de licence dans le tableau de bord de l’organisation.
* **[!UICONTROL Développement d’applications]** : ce rôle n’est pas encore effectif et sera disponible prochainement. Il est déconseillé d’affecter des personnes à ce rôle pour l’instant.

Pour plus d’informations sur les actions propres à chaque rôle au sein de l’organisation, consultez la section [Rôles au sein de de l’organisation et de l’équipe](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Inviter des utilisateurs à une organisation

Par défaut, la personne propriétaire d’une organisation (ou une personne autorisée) peut inviter une autre personne à rejoindre son organisation.

Pour inviter une personne à rejoindre une organisation, procédez comme suit :

1. Cliquez sur **[!UICONTROL Modifier les détails]** dans le coin supérieur droit de l’écran.
1. Sélectionnez **[!UICONTROL Inviter une nouvelle personne]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Renseignez l’adresse e-mail et le nom de la personne.
1. Sélectionnez un rôle pour la personne. Pour plus d’informations sur les rôles, consultez la section [Rôles dans l’organisation](#organization-roles) de ce document.
1. (Facultatif) Ajoutez une note. Cette note s’affiche dans l’e-mail d’invitation que la personne reçoit.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

[!DNL Fusion] envoie un e-mail d’invitation à l’organisation spécifique et un bouton [!UICONTROL Accepter le rôle].

Lorsque la personne destinataire clique sur le bouton, elle est redirigée vers la page d’invitation, où elle peut accepter l’invitation.

L’invitation expire dans un jour.

>[!NOTE]
>
>Si la personne découvre [!DNL Fusion], [!DNL Fusion] crée automatiquement un compte pour elle et lui envoie un e-mail contenant un mot de passe temporaire avec des instructions pour se connecter et modifier son mot de passe.

### Passer à une autre organisation

Vous pouvez faire partie de plusieurs organisations dans Fusion. Les ressources ne sont pas partagées entre les organisations.

Vous pouvez changer d’organisation dans Adobe Unified Experience en cliquant sur le nom de l’organisation dans le coin supérieur droit et en sélectionnant la nouvelle organisation dans la liste déroulante. Seules les organisations disposant d’un compte Fusion s’affichent dans la liste déroulante, même si vous êtes membre d’autres organisations dans Adobe.

## Équipes

Les équipes sont des groupes de personnes qui partagent l’accès à des ressources spécifiques. Ces éléments peuvent inclure :

* Scénarios
* Connexions
* Webhooks
* Clés
* Magasins de données
* Structures de données
* Paramètres de notification par e-mail

>[!NOTE]
>
>Comme les équipes contrôlent l’accès aux ressources, il est parfois utile qu’une équipe ne comporte qu’un seul membre. Par exemple, les personnes en formation peuvent créer des connexions avec leurs comptes [!DNL Google] individuels. Tout membre de l’équipe peut également se connecter au compte [!DNL Google] individuel, il est donc préférable, dans ce cas, que la personne soit le seul membre d’une équipe de formation.

Les organisations peuvent avoir autant d’équipes que nécessaire et les personnes peuvent appartenir à une ou plusieurs équipes.

Les personnes peuvent sélectionner leur équipe dans la liste déroulante du panneau de navigation de gauche. Les personnes ne voient que les équipes dont elles font partie. La sélection d’une équipe permet à une personnes d’accéder aux ressources de cette équipe.

* [Rôles dans une équipe](#team-roles)
* [Gestion des équipes](#team-management)

### Rôles dans une équipe

Les rôles suivants sont disponibles dans les équipes :

* **[!UICONTROL Administration d’équipe]** : en plus des fonctionnalités des autres rôles d’équipe, le rôle d’administration permet à la personne d’ajouter, de supprimer ou de modifier le rôle d’un membre de l’équipe.
* **[!UICONTROL Membre de l’équipe]** : le rôle de membre de l’équipe permet aux personnes de créer et d’exécuter des scénarios.
* **[!UICONTROL Surveillance de l’équipe]** : le rôle de [!UICONTROL surveillance] permet aux personnes d’accéder aux informations d’exécution pour les scénarios, mais elles ne peuvent pas concevoir de scénarios ni modifier son statut « Actif ».
* **[!UICONTROL Opérateur ou opératrice d’équipe]** : le rôle d’[!UICONTROL Opérateur ou opératrice] permet aux personnes d’afficher les données d’exécution et de modifier le statut « Actif » des scénarios.
* **[!UICONTROL Membre avec restriction de l’équipe]** : ce rôle n’est pas encore effectif et sera disponible prochainement. Il est déconseillé d’affecter des personnes à ce rôle pour l’instant.

Pour plus d’informations sur les actions propres à chaque rôle d’équipe, consultez la section [Rôles dans l’organisation et l’équipe](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Gestion des équipes

* [Créer une équipe](#create-a-team)
* [Définir les options de notification pour l’équipe](#set-team-notification-options)

#### Créer une équipe

Les propriétaires et les administrateurs et administratrices d’organisation peuvent créer des équipes.

Pour créer une équipe, procédez comme suit :

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Organisation]**.
1. Sélectionnez l’onglet **[!UICONTROL Équipe]**.
1. Cliquez sur **[!UICONTROL Ajouter une nouvelle équipe]** dans la liste des équipes.
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

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Équipe]**
1. Sélectionnez l’onglet **[!UICONTROL Options de notification]**.
1. Activez les notifications que vous souhaitez que l’équipe reçoive.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Warning in scenario run]</td> 
      <td> <p>Recevez un e-mail lorsqu’un avertissement se produit dans l’exécution d’un scénario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Errors in scenario run]</td> 
      <td>Recevez un e-mail en cas d’erreur lors de l’exécution d’un scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Scenario deactivation]</p> </td> 
      <td><p>Recevez un e-mail lorsqu’un scénario se désactive.</p><p><b>Note :</b> vous prenez connaissance de la désactivation d’un scénario uniquement lorsque celui-ci a été automatiquement désactivé en raison d’erreurs. Vous ne recevez pas de notifications sur les scénarios qui sont désactivés manuellement.</p><p>Dans certains cas, un scénario peut être désactivé par l’équipe d’ingénierie [!DNL Workfront Fusion], car le scénario cause des problèmes de performances ou autres. Dans ce cas, vous ne recevez pas de notifications dans [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Les modifications apportées aux options de notification sont automatiquement enregistrées.

#### Basculer entre les équipes

Vous pouvez faire partie de plusieurs équipes dans Fusion. Comme les équipes ne partagent pas de ressources, vous devrez peut-être changer d’équipe pour accéder à des scénarios spécifiques ou à d’autres ressources.

Si votre organisation ne figure pas dans Adobe Unified Experience, vous pouvez changer d’équipe en cliquant sur son nom dans le volet de navigation de gauche, puis en sélectionnant une équipe dans la liste déroulante.

Si votre équipe se trouve dans Adobe Unified Experience, vous pouvez sélectionner une nouvelle équipe en cliquant sur son nom dans l’en-tête, puis en sélectionnant une équipe dans la liste déroulante. Cette option est disponible à partir de toutes les pages spécifiques à une équipe spécifique, comme une page de scénario ou la page Connexions.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->