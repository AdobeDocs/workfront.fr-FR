---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organisations et équipes d’Adobe Workfront Fusion
description: Les fonctionnalités d’organisation et d’équipe d’Adobe Workfront Fusion permettent aux entreprises de contrôler l’accès aux scénarios et aux autres fonctionnalités de Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] organisations et équipes

[!DNL Adobe Workfront Fusion]Les fonctionnalités d’ organisation et d’ équipes permettent aux entreprises de contrôler l’accès aux scénarios et aux autres fonctionnalités dans Fusion.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>Workfront Fusion pour l’automatisation et l’intégration du travail,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> 
     <p>Vous devez être un [!DNL Workfront Fusion] administrateur de votre entreprise.</p>
     <p>Vous devez être un [!DNL Workfront Fusion] administrateur de votre équipe.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

<p>**Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] licences</a></p>


## Organisations

[!DNL Workfront Fusion] les utilisateurs appartiennent à une organisation. Votre [!DNL Fusion] La licence détermine le nombre de scénarios et de connecteurs principaux disponibles dans votre entreprise.

[!DNL Fusion] la licence détermine le nombre de scénarios principaux et d’applications principales disponibles pour une entreprise. [!DNL Fusion] affiche le nombre actuel de &quot;Principaux scénarios&quot; et &quot;Principales applications&quot; dans le tableau de bord de l’organisation.

* [Rôles d’organisation](#organization-roles)
* [Invitation d’utilisateurs à une organisation](#inviting-users-to-an-organization)

### Rôles d’organisation

Un utilisateur possède l’un des rôles suivants dans une organisation :

* **[!UICONTROL Propriétaire]**: Le propriétaire dispose de toutes les autorisations disponibles dans l’organisation.
* **[!UICONTROL Administration]**: Le rôle d’administrateur permet à un utilisateur de créer et de gérer des équipes et des utilisateurs pour l’organisation.
* **[!UICONTROL membre]**: Les membres peuvent utiliser [!DNL Workfront Fusion] mais ne peuvent pas apporter de changements organisationnels.
* **[!UICONTROL Comptable]**: Un rôle de comptable permet uniquement aux utilisateurs d’afficher les informations de licence dans le tableau de bord de l’organisation.
* **[!UICONTROL Développeur d’applications]**: La fonctionnalité de ce rôle n’est actuellement pas disponible et sera bientôt disponible. Il est déconseillé d’affecter des utilisateurs à ce rôle pour l’instant.

### Invitation d’utilisateurs à une organisation

Par défaut, le propriétaire d’une organisation (ou un utilisateur autorisé) peut inviter une autre personne à rejoindre son organisation.

Pour inviter un utilisateur à rejoindre une organisation :

1. Cliquez sur **[!UICONTROL Modification des détails]** dans le coin supérieur droit de l’écran.
1. Sélectionner **[!UICONTROL Invitation d’un nouvel utilisateur]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Renseignez l’adresse électronique et le nom de l’utilisateur.
1. Sélectionnez un rôle pour l’utilisateur. Pour plus d’informations sur les rôles, voir [Rôles d’organisation](#organization-roles) dans ce document.
1. (Facultatif) Ajoutez une note. Cette note s’affiche dans le courrier électronique d’invitation que l’utilisateur reçoit.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

[!DNL Fusion] envoie un courrier électronique avec une invitation à l’organisation spécifique et un [!UICONTROL Acceptation Du Rôle] bouton .

![](assets/accept-the-role.png)

Lorsque le destinataire clique sur le bouton, il est redirigé vers la page d’invitation, où il peut accepter l’invitation.

L’invitation expire dans un jour.

>[!NOTE]
>
>Si l’utilisateur découvre [!DNL Fusion], [!DNL Fusion] crée automatiquement un compte à leur intention et envoie un courrier électronique avec un mot de passe temporaire, ce qui demande au nouvel utilisateur de se connecter et de changer son mot de passe.

## Équipes

Les équipes sont des groupes d’utilisateurs qui partagent l’accès à des ressources spécifiques. Ces ressources peuvent inclure :

* Scénarios
* Connexions
* Webhooks
* Clés
* Entrepôts de données
* Structures de données
* Paramètres de notification par e-mail

>[!NOTE]
>
>Comme les équipes contrôlent l’accès aux ressources, il est parfois utile qu’une équipe n’ait qu’un seul membre. Par exemple, les utilisateurs en formation peuvent créer des connexions avec leur individu [!DNL Google] comptes. Tout membre de l’équipe peut également se connecter à la personne [!DNL Google] , il est donc préférable, dans ce cas, que l’utilisateur soit le seul membre d’une équipe de formation.

Les organisations peuvent avoir autant d’équipes que nécessaire et les utilisateurs peuvent appartenir à une ou plusieurs équipes.

Les utilisateurs peuvent sélectionner leur équipe dans la liste déroulante du panneau de navigation de gauche. Les utilisateurs ne voient que les équipes dont ils font partie. La sélection d’une équipe permet à un utilisateur d’accéder aux ressources de cette équipe.

* [Rôles d’équipe](#team-roles)
* [Gestion des équipes](#team-management)

### Rôles d’équipe

Un utilisateur possède l’un des rôles suivants dans chacune de ses équipes :

* **[!UICONTROL Administrateur d’équipe]**: Outre les fonctionnalités des autres rôles d’équipe, le rôle d’administrateur permet à l’utilisateur d’ajouter, de supprimer ou de modifier le rôle d’un membre de l’équipe.
* **[!UICONTROL Membre de l’équipe]**: Le rôle de membre de l’équipe permet aux utilisateurs de créer et d’exécuter des scénarios.
* **[!UICONTROL Surveillance de l’équipe]**: Le [!UICONTROL monitoring] role permet aux utilisateurs d’accéder aux informations d’exécution pour les scénarios, mais ils ne peuvent pas concevoir de scénarios ou modifier leur état &quot;Principal&quot;.
* **[!UICONTROL Opérateur d’équipe]**: Le [!UICONTROL operator] Le rôle permet aux utilisateurs d’afficher les données d’exécution et de modifier l’état &quot;Principal&quot; des scénarios.
* **[!UICONTROL Membre avec restriction de l’équipe]**: La fonctionnalité de ce rôle n’est actuellement pas disponible et sera bientôt disponible. Il est déconseillé d’affecter des utilisateurs à ce rôle pour l’instant.

### Gestion des équipes

* [Création d’une équipe](#create-a-team)
* [Définition des options de notification d’équipe](#set-team-notification-options)

#### Création d’une équipe

Les propriétaires et administrateurs d’organisation peuvent créer des équipes.

Pour créer une équipe :

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Organisation]**
1. Sélectionnez la **[!UICONTROL Équipe]** .
1. Cliquez sur **[!UICONTROL Ajouter une nouvelle équipe]** sous la liste des équipes.
1. Saisissez le nom de la nouvelle équipe, puis cliquez sur **Ajouter**.

#### Définition des options de notification d’équipe

Les options de notification électronique sont définies au niveau de l’équipe.

1. Dans le panneau de navigation de gauche, cliquez sur **[!UICONTROL Équipe]**
1. Sélectionnez la **[!UICONTROL Options de notification]** .
1. Activez les notifications que vous souhaitez que l’équipe reçoive.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Avertissement dans l’exécution du scénario]'</td> 
      <td> <p>Recevez un email lorsqu’un avertissement se produit dans un scénario d’exécution</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Erreurs dans l’exécution du scénario]</td> 
      <td>Recevez un email en cas d'erreur lors de l'exécution d'un scénario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Désactivation du scénario]</p> </td> 
      <td><p>Recevez un email lorsqu’un scénario se désactive.</p><p><b>Remarque :</b> Vous êtes informé de la désactivation d’un scénario uniquement lorsque celui-ci a été automatiquement désactivé en raison d’erreurs. Vous ne recevez pas de notifications sur les scénarios qui sont désactivés manuellement.</p><p>Dans certains cas, un scénario peut être désactivé par la fonction [!DNL Workfront Fusion] équipe d’ingénieurs car le scénario cause des performances ou d’autres problèmes. Dans ce cas, vous ne recevez pas de notifications dans [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Les modifications apportées aux options de notification sont automatiquement enregistrées.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->