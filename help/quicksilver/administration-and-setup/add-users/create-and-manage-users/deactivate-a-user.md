---
title: Désactivation ou réactivation d’un utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: En tant qu’administrateur Workfront, vous pouvez désactiver ou réactiver un utilisateur.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: a907cd9d07a2912d42ae26d69815a05a1006a633
workflow-type: tm+mt
source-wordcount: '1261'
ht-degree: 1%

---

# Désactivation ou réactivation d’un utilisateur

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Si un utilisateur quitte l’entreprise, vous devrez peut-être le supprimer d’Adobe Workfront. Ils ne doivent pas rester actifs dans le système, car cela créerait une confusion pour les autres utilisateurs lorsqu’ils les ajouteraient à des mises à jour ou leur attribueraient un travail. Lorsque vous désactivez un utilisateur, son nom n’est plus visible pour les autres utilisateurs qui recherchent des personnes dans le système.

Les administrateurs peuvent voir les utilisateurs inactifs dans la zone Configuration .

Vous pouvez réactiver un utilisateur à tout moment.

>[!IMPORTANT]
>
>Nous vous recommandons de désactiver les utilisateurs qui ont quitté l’organisation plutôt que de les supprimer. Si un utilisateur est supprimé, tout l’historique de Workfront associé à cet utilisateur est perdu. Cela inclut leurs affectations de travail, leur association aux notes, heures, documents et tous les autres objets qu’ils ont créés une fois.
>
>La désactivation d’un utilisateur dans Workfront supprime les licences de l’utilisateur pour Workfront et la vérification dynamique des balises. En outre, l’utilisateur ne peut plus se voir attribuer une tâche. Lorsqu’un utilisateur est désactivé, sa licence Workfront et sa licence de vérification peuvent être utilisées par un autre utilisateur. Toutes les autres informations du profil de l’utilisateur désactivé restent inchangées.
>
>Pour plus d’informations sur l’impact de la suppression et de la désactivation des utilisateurs, voir [Suppression d’utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Conditions d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>  <p>Nouveau : Standard </p> <p>Ou </p><p>Actuel : formule </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez disposer de l’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p><b>Utilisateurs</b> paramètre de votre niveau d’accès configuré sur <b>Modifier</b> accès, avec <b>Créer</b> et au moins l’une des deux <b>Administration des utilisateurs</b> options activées sous <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>de ces deux options, si Utilisateur <b>Administration (utilisateurs de groupe)</b> est activé, vous devez être administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> <p>Pour plus d’informations sur la variable <b>Utilisateurs</b> paramétrer un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Conditions préalables

Avant de désactiver un administrateur Workfront ou un utilisateur sous licence Standard ou Plan, vous devez associer ses objets et activités à un autre utilisateur.

Pour plus d’informations, voir [À propos de la désactivation des administrateurs Workfront et de la planification des utilisateurs de licences](#about-deactivating-workfront-administrators-and-plan-license-users) dans cet article.

## Désactiver un utilisateur ou une utilisatrice

Lors de la désactivation d’un utilisateur, tenez compte des points suivants :

* L’utilisateur ne pourra pas accéder au système.
* L’utilisateur sera supprimé des liens de révision, ressources, projets et comptes de Frame.io.
   * La réactivation de l’utilisateur ne les ajoute pas automatiquement aux éléments Frame.io . Vous devez réaffecter manuellement l’utilisateur aux projets, tâches et ressources Workfront nécessitant une collaboration Frame.io.
* Toutes les données associées à l’utilisateur seront conservées.
* Vous pouvez attribuer une licence d’utilisateur désactivée à un autre utilisateur.

Pour désactiver un utilisateur :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).

1. Sélectionnez un utilisateur, cliquez sur le bouton **Plus** icon ![](assets/more-icon.png), puis cliquez sur **Désactiver**.

1. Cliquez sur **Désactiver** dans la zone qui s’affiche.

## Planification de la désactivation pour les utilisateurs

En tant que responsable, vous pouvez souhaiter marquer les utilisateurs pour désactivation avant qu’ils ne quittent réellement votre entreprise. Par exemple, si vous travaillez avec un utilisateur contractuellement lié, il se trouve dans votre système pendant une période limitée et vous connaissez sa date de fin. Vous pouvez programmer leur désactivation à cette date.

Les administrateurs de Workfront et les utilisateurs de la licence Plan peuvent voir la date de désactivation dans leur profil utilisateur.

Pour planifier la désactivation d’un utilisateur :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).

1. Sélectionnez le nom de l’utilisateur.

   Ou

   (Facultatif) Sélectionnez plusieurs utilisateurs pour les planifier en vue de leur désactivation en bloc.

1. Cliquez sur l’icône Modifier ![](assets/edit-icon.png).
1. Dans la zone Modifier l’utilisateur qui s’affiche, cliquez sur **Planification des ressources** pour aller dans cette zone.
1. Activez la variable **Planifier la désactivation** .

1. Dans le calendrier qui s’affiche, indiquez la date et l’heure du **Date planifiée de désactivation**.

   >[!NOTE]
   >
   >* Dans la zone de temps, vous pouvez sélectionner uniquement des incréments d’une heure entière, et non des minutes.
   >* Si vous sélectionnez une heure pour le jour en cours qui s’est écoulé, Workfront programmera la désactivation pour le jour suivant à 00h00. L’heure sélectionnée correspond au fuseau horaire de l’ordinateur de l’utilisateur qui planifie la désactivation.

1. Cliquez sur **Enregistrer les modifications**.

   L’utilisateur est désactivé le jour sélectionné après l’heure sélectionnée. Si vous avez sélectionné plusieurs utilisateurs à désactiver en bloc, tous les utilisateurs sélectionnés sont désactivés le jour sélectionné après l’heure sélectionnée.

Nous vous recommandons de créer un rapport pour les utilisateurs que vous avez programmés pour la désactivation, afin de vous tenir informé des utilisateurs qui vont être désactivés. Il n’existe aucune confirmation que la désactivation s’est produite une fois les utilisateurs désactivés.

## Réactiver un utilisateur

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Utilisateurs** ![](assets/users-icon-in-main-menu.png).

1. Sélectionnez un utilisateur, cliquez sur l’icône Plus ![](assets/more-icon.png), puis cliquez sur **Activer**.

1. Attribuer une nouvelle **Niveau d’accès** dans le menu déroulant, puis cliquez sur **Réactiver**.

### Impact de l’examen et de l’approbation des ressources lorsque vous réactivez un utilisateur

Les utilisateurs désactivés perdent l’accès à leurs comptes Frame.io attribués, ainsi qu’aux projets, ressources et liens de révision attribués. Si vous choisissez de réactiver l’utilisateur, vous devez le réaffecter manuellement aux projets, tâches et ressources nécessitant la collaboration Frame.io.

### Impact de la vérification lorsque vous réactivez un utilisateur

Les utilisateurs désactivés perdent leur rôle de vérification par défaut et leur licence de BAT (si vous utilisez un forfait hérité Workfront Premium). Si vous choisissez de réactiver l’utilisateur, vous devez :

* Réaffectez la licence (si vous utilisez un forfait hérité Workfront Premium). Pour plus d’informations sur les plans de vérification Workfront, voir [Accès aux fonctionnalités de vérification dans Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Vérifiez qu’ils disposent du rôle de BAT correct. Les utilisateurs de BAT réactivés se voient attribuer le rôle de BAT par défaut spécifié pour les nouveaux utilisateurs. Voir [Configuration des rôles de vérification par défaut](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) pour plus d’informations.

## À propos de la désactivation des administrateurs Workfront et des utilisateurs de licences Standard ou Plan

Avant de désactiver un administrateur Workfront ou un utilisateur disposant d’une licence Plan, il est important de rechercher les objets et activités Workfront qui impliquent cette personne, puis de les associer à un autre administrateur Workfront ou de planifier un utilisateur de licence selon les besoins.

Ces objets et activités peuvent inclure les éléments suivants :

* Tâches ou problèmes affectés à l’utilisateur
* Projets détenus par l’utilisateur
* Rapports configurés pour s’exécuter avec les droits d’accès de l’utilisateur
* Modèles appartenant à l’utilisateur
* Projets et modèles sur lesquels l’utilisateur a été défini comme gestionnaire de ressources
* Règles de routage de la file d’attente des demandes sur lesquelles l’administrateur Workfront ou l’utilisateur de la licence Plan est le responsable par défaut
* Processus de validation comportant une étape, y compris l’utilisateur (en particulier s’il était le seul approbateur sur l’étape)
* Feuilles de calcul qui répertorient l’utilisateur en tant qu’approbateur
* Profils de feuille de temps qui répertorient l’utilisateur en tant qu’approbateur
* Vérification des processus automatisés qui incluent l’utilisateur

## Impact de la planification des ressources lorsque vous planifiez la désactivation d’un utilisateur

Lorsque vous planifiez la désactivation d’un utilisateur, il n’apparaît plus dans le planificateur de ressources comme étant disponible pour les heures de budget. S’ils restent membres des groupes de ressources, ils apparaissent dans le planificateur de ressources, mais leur disponibilité est définie sur zéro heure à compter de la date de leur désactivation planifiée.

Le planificateur de ressources prend en compte tous les rôles de tâche des utilisateurs et les dates d’achèvement planifiées des tâches et calcule les ressources en conséquence.

Pour plus d’informations sur le planificateur de ressources, voir [Présentation de Resource Planner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
