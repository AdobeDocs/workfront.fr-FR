---
title: Gestion des utilisateurs dans Adobe Workfront Planning en tant que produit autonome
description: Cet article décrit comment gérer les utilisateurs et les équipes dans Adobe Workfront Planning lorsque Planning est acheté en tant que produit autonome.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 697499fadf4d5d22292ededed381cb72e53fcae3
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 1%

---


# Gestion des utilisateurs dans Adobe Workfront Planning en tant que produit autonome

>[!IMPORTANT]
>
>Les informations de cet article font référence à Adobe Workfront Planning, lorsqu’il est acheté en tant que produit autonome. Reportez-vous à cet article lorsque votre société a acheté un package Adobe Workfront Planning uniquement sans acheter de package Workfront Workflow.
>
>Pour plus d’informations sur Adobe Workfront Planning lorsqu’il est acheté avec un package Workfront, voir [Prise en main d’Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
>

Vous pouvez gérer les utilisateurs dans Adobe Workfront Planning en tant que produit autonome de la même manière que vous les gérez dans Adobe Workfront.

Les niveaux d’accès que vous pouvez attribuer aux utilisateurs dans Workfront Planning présentent certaines limites.

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning</p></td> 
   <td> 
<p>Tout Workfront Planning sous forme de package autonome</p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Administrateur ou administratrice de planification</p>
   </td> 
  </tr>

</tbody> 
</table>

Pour plus d’informations sur l’accès nécessaire à Workfront en tant que package autonome, voir [Accès nécessaire pour Adobe Workfront Planning en tant que produit autonome](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md).
+++    

## Niveaux d&#39;accès dans Adobe Workfront Planning

Vous pouvez attribuer les niveaux d’accès suivants aux utilisateurs dans Workfront Planning lors de l’achat en tant que produit autonome :

* Administrateur ou administratrice de planification
* Norme de planification

Pour plus d’informations sur les fonctionnalités incluses dans chaque accès, voir [Accès nécessaire pour Adobe Workfront Planning en tant que produit autonome](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md).

Tenez compte des points suivants lorsque vous utilisez des niveaux d’accès dans Workfront Planning en tant que produit autonome :

* Vous ne pouvez pas créer ni modifier des niveaux d&#39;accès dans Workfront Planning. Ils sont préconfigurés.

* Une fois que vous avez ajouté un utilisateur au Adobe Admin Console en tant qu’administrateur pour le produit Workfront, il est automatiquement affecté à ce niveau d’accès dans Workfront Planning et son niveau d’accès ne peut pas être modifié dans Planning.
* Vous ne pouvez attribuer un niveau d&#39;accès Planning Standard aux utilisateurs dans Planning qu&#39;après avoir ajouté les utilisateurs à Admin Console. Il s’agit du seul niveau d’accès que vous pouvez affecter manuellement à un utilisateur.

## Gestion des utilisateurs dans Workfront Planning en tant que produit autonome

1. En tant qu&#39;administrateur de Planning, effectuez l&#39;une des opérations suivantes :

   * Si vous êtes un nouveau client Workfront Planning, vous recevez un e-mail d’Adobe Workfront vous informant que vous disposez désormais d’un compte dans Adobe Workfront. Utilisez le lien contenu dans l’e-mail pour vous connecter à Admin Console.

   * Si vous êtes déjà administrateur Workfront Planning et que vous souhaitez en ajouter d’autres à votre compte, connectez-vous à Admin Console.

   Pour plus d’informations, voir [Gestion des utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

1. Dans Admin Console, commencez à ajouter des utilisateurs dans l’un des onglets suivants :

   * **Administrateurs** : les utilisateurs sont automatiquement créés en tant qu&#39;utilisateurs administrateurs de Planning dans Planning.
   * **Utilisateurs** : vous devez attribuer un niveau d’accès dans Workfront Planning.

1. (Conditionnel) Connectez-vous à Workfront à partir de la page d’accueil d’Adobe CX Enterprise.

   Workfront Planning s’ouvre.
1. Cliquez sur **Menu principal** > **Utilisateurs** > **Nouvel utilisateur**.

   ![Nouvelle zone Utilisateur dans Planning Stand-alone](assets/new-user-box-planning-sta.png)

1. Dans la zone **Nouvel utilisateur**, mettez à jour les informations suivantes :

   * **Prénom(s)** : nom que vous avez ajouté à l’Admin Console.
   * **Nom** : même nom que celui que vous avez ajouté à Admin Console.
   * **Adresse e-mail (nom d’utilisateur)** : adresse e-mail que vous avez ajoutée à Admin Console.
   * **L’utilisateur est actif** : pour indiquer que l’utilisateur est actif et peut se connecter à Workfront Planning et être affecté à des enregistrements, activez le paramètre.
   * **Niveau d&#39;accès** : sélectionnez Planning Standard pour un utilisateur non administrateur. C&#39;est la seule option.

     >[!TIP]
     >
     >L&#39;ajout d&#39;un utilisateur déjà configuré en tant qu&#39;administrateur dans Admin Console ajoute automatiquement le niveau d&#39;accès Administrateur Planning à l&#39;utilisateur. Ce ne peut pas être modifié.

   * **Équipes** : dans le menu déroulant, sélectionnez les équipes à associer à l’utilisateur. Des équipes doivent être créées avant de pouvoir les affecter aux utilisateurs.

     Pour plus d’informations, voir [Gestion des équipes](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md).

1. Cliquez sur **Télécharger maintenant** pour ajouter une image de profil, puis sur **Enregistrer**.

1. Cliquez sur **Enregistrer** ou **Ajouter une personne et en démarrer une autre** pour enregistrer l’utilisateur et en ajouter un autre.

   Les utilisateurs ajoutés recevront un courrier électronique leur permettant de se connecter à Workfront Planning.
1. (Facultatif) Pour modifier un utilisateur existant, effectuez l’une des opérations suivantes :

   * Pointez sur le nom de l’utilisateur dans la liste, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) > **Modifier l’utilisateur**
   * Sélectionnez l’utilisateur dans la liste, puis cliquez sur **Modifier l’utilisateur** dans la barre d’outils bleue en bas de la page.
1. (Facultatif) Pour supprimer un utilisateur, effectuez l’une des opérations suivantes :

   * Pointez sur le nom de l’utilisateur dans la liste, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) > **Supprimer l’utilisateur**
   * Sélectionnez l’équipe dans la liste, puis cliquez sur **Supprimer l’utilisateur** dans la barre d’outils bleue en bas de la page
1. Cliquez sur **Supprimer** pour confirmer.
1. (Facultatif) Pour désactiver un utilisateur, effectuez l’une des opérations suivantes :

   * Pointez sur le nom de l’utilisateur dans la liste, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) > **Désactiver**
   * Sélectionnez l’équipe dans la liste, puis cliquez sur **Désactiver** dans la barre d’outils bleue en bas de la page
1. Cliquez sur **Désactiver** pour confirmer.

   Pour conserver des enregistrements historiques de votre travail, nous vous recommandons de désactiver les utilisateurs au lieu de les supprimer.

