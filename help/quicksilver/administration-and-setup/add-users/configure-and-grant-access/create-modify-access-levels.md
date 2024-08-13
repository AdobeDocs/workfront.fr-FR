---
title: Création et modification de niveaux d’accès personnalisés
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur Adobe Workfront, vous pouvez créer des niveaux d’accès personnalisés et les appliquer aux utilisateurs.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '1463'
ht-degree: 10%

---

# Création et modification de niveaux d’accès personnalisés

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

En tant qu’administrateur Adobe Workfront, vous pouvez créer des niveaux d’accès personnalisés et les appliquer aux utilisateurs. Lorsque vous utilisez des niveaux d’accès, il est important de comprendre comment ils fonctionnent ensemble avec les autorisations d’objet que les utilisateurs accordent lorsqu’ils partagent des objets les uns avec les autres. Pour plus d’informations sur les niveaux d’accès, voir :

* [Vue d’ensemble des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Présentation des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs. Pour personnaliser un niveau d&#39;accès, copiez le niveau d&#39;accès par défaut et modifiez la copie. Vous pouvez le faire pour chaque niveau d’accès, à l’exception de l’administrateur système et de l’utilisateur externe.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td>Nouvelle : standard
   <p>ou</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création ou modification d’un niveau d’accès personnalisé

{{step-1-to-setup}}

1. Cliquez sur **Accéder aux niveaux** dans le panneau de gauche.
1. Sélectionnez le niveau d’accès que vous souhaitez copier et personnaliser, puis cliquez sur **Copier**.

   Ou

   Si vous modifiez un niveau d’accès existant (que vous avez copié précédemment), cliquez sur son nom.

1. Dans la zone qui s’affiche, effectuez l’une des opérations suivantes pour commencer à configurer le niveau d’accès personnalisé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>Saisissez le nom de votre niveau d’accès. </p> <p>Si vous venez de copier un niveau d’accès pour en créer un nouveau, le nom par défaut est Nom du niveau d’accès (copie), où Nom du niveau d’accès est le niveau d’accès que vous avez copié.</p> <p><strong>Conseil</strong> : Nous vous recommandons d’inclure le nom d’origine du niveau d’accès dans le nom de la copie. Par exemple, dans la société ACME, une copie du niveau d’accès standard peut être nommée ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description </td> 
      <td>Saisissez une description pour le niveau d’accès. Il est utile d’indiquer ici à quel utilisateur disposant de ce niveau d’accès pourra accéder.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de licence</td> 
      <td>Assurez-vous que la licence sélectionnée ici est celle qui est la plus étroitement associée au type de niveau d'accès que vous créez ou modifiez. La licence sélectionnée détermine les paramètres disponibles pour le niveau d’accès. Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Présentation des nouvelles licences</a> ou <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Présentation des licences</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditionnel) Si **Standard** ou **Plan** est sélectionné dans la zone **Type de licence**, faites défiler l’écran jusqu’à la section **Autoriser l’accès administratif pour** et sélectionnez les autorisations d’accès administratif pour ceux qui auront ce niveau d’accès.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processus d’approbation</td> 
      <td>Créez et gérez des processus d’approbation à utiliser dans l’ensemble du système et pour des groupes spécifiques.<p>Sans cet accès, les utilisateurs peuvent uniquement créer des processus d’approbation ad hoc sur les éléments qu’ils ont accès à gérer.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entreprises</td> 
      <td>Ajoutez de nouvelles entreprises et modifiez les entreprises existantes dans Workfront.<br><p>Sans cet accès, les utilisateurs peuvent uniquement afficher les entreprises existantes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés dans mon groupe</td> 
      <td>Créez et gérez tous les formulaires personnalisés de leur groupe. <br><p>Sans cet accès, les utilisateurs peuvent uniquement joindre des formulaires existants aux objets auxquels ils ont accès pour contribuer ou gérer.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taux de change</td> 
      <td> Ajoutez une nouvelle devise dans Workfront. <p>Sans cet accès, l’utilisateur ne peut ajouter une devise existante qu’à un projet qu’il crée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td>Afficher toutes les dépenses sur les objets dans Workfront.<p>Sans cet accès, l'utilisateur ne peut visualiser que les éléments suivants :</p>
       <ul>
        <li>Dépenses sur les projets, tâches ou problèmes qu'ils gèrent</li>
        <li>Leurs propres dépenses</li>
        <li>Les dépenses de leurs subordonnés</li>
       </ul><p><b>REMARQUE</b> : cela ne permet pas à l’utilisateur de créer de nouveaux types de dépenses.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fonctions</td> 
      <td> Avec cet accès, l’utilisateur est autorisé à effectuer les opérations suivantes : 
       <ul> 
        <li>Affichage et modification des rôles de tâche existants</li> 
        <li>Ajout de nouveaux rôles de tâche</li> 
        <li>Modifier les taux de facturation et de coûts du rôle</li> 
       </ul> 
       <p>Pour obtenir des informations importantes sur l’accès aux données financières disponibles pour un utilisateur Standard ou Planificateur disposant d’un accès administratif aux rôles de tâche, voir <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Utilisateurs standard ou de planificateur disposant d’un accès administratif aux rôles de tâche</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Jalons dans mon groupe</td> 
      <td>Affichez tous les chemins de jalon dans le système sous le menu Chemins de jalon dans Configuration. Les utilisateurs peuvent également modifier ou supprimer les chemins d’accès aux jalons appartenant à l’un de leurs groupes. Les utilisateurs ne peuvent pas gérer (modifier ou supprimer) les chemins d’accès de jalon qui ne sont pas attribués à leur groupe.<p>Sans cet accès, les utilisateurs peuvent uniquement afficher les chemins de jalon existants et les appliquer aux projets qu’ils ont accès à la gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Créez et gérez des notifications de rappel dans Workfront.<p>Sans cet accès, les utilisateurs sont limités à recevoir et afficher des notifications.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Feuilles de temps et heures</td> 
      <td> Les administrateurs de groupe peuvent affecter des profils de feuille de temps aux utilisateurs dans les groupes et sous-groupes qu’ils gèrent. <p>Si cette option n’est pas activée, les administrateurs de groupe ne peuvent pas affecter de profils de feuille de temps à d’autres utilisateurs dans les groupes et sous-groupes qu’ils gèrent, bien qu’ils puissent les créer.</p> <p>Tous les autres utilisateurs disposant d’une licence Standard ou Plan peuvent afficher toutes les heures et les feuilles de temps dans Workfront.</p> <p>Si cette option n’est pas activée, les utilisateurs peuvent afficher les heures uniquement sur :</p> 
       <ul> 
        <li>Projets, tâches ou problèmes qu’ils gèrent</li> 
        <li>Leur propre feuille de temps</li> 
        <li>Une feuille de temps d’une personne qui lui fait rapport</li> 
        <li>Une feuille de temps qu’ils approuvent</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Définir des restrictions supplémentaires**, puis définissez l’une des restrictions suivantes pour le niveau d’accès.

   >[!IMPORTANT]
   >
   >Pour les utilisateurs externes tels que les fournisseurs (toute personne ne faisant pas partie de votre organisation), nous vous recommandons de restreindre l’accès aux tâches, projets, mises à jour, annonces, autres sociétés, équipes et groupes.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ne jamais donner accès au projet complet en cas d'affectation à une tâche ou un événement</td> 
      <td> Permet d’empêcher les utilisateurs affectés à des tâches ou des problèmes d’obtenir des autorisations pour le projet parent, même si les autorisations du projet le permettent.<p>Pour plus d’informations sur la configuration des autorisations sur un projet, reportez-vous à la section <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> de l’article <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifier les projets</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ne jamais hériter l'accès aux documents depuis des projets, des tâches, des événements, etc...</td> 
      <td>Empêche les documents d’hériter des autorisations définies sur leur objet parent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher uniquement les mises à jour dans lesquelles ils ont été inclus dans la conversation</td> 
      <td> Permet aux utilisateurs de n’afficher que les commentaires pour lesquels leur nom ou le nom de leur équipe a été inclus. <p> <p><b>REMARQUE</b> : cela empêche les utilisateurs de s’inscrire aux éléments dans Workfront. Pour plus d’informations sur l’abonnement aux éléments, voir <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Abonnement aux éléments dans Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne jamais autoriser les utilisateurs à supprimer les commentaires </td> 
      <td> Empêche les utilisateurs de supprimer les commentaires qu’ils font sur les éléments.  <p><b>REMARQUE</b> : personne ne peut supprimer les commentaires des autres utilisateurs.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher uniquement les entreprises, les groupes et les équipes auxquels ils appartiennent</td> 
      <td>Permet aux utilisateurs d’afficher et de partager des éléments uniquement avec les entreprises, les groupes et les équipes auxquels ils appartiennent.<p><strong>REMARQUE</strong> : les utilisateurs disposant de licences du demandeur ne peuvent pas afficher les sociétés auxquelles ils n’appartiennent pas, même si cette option est sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne jamais autoriser que les heures prévues ou les heures réelles soient visibles</td> 
      <td>Empêche les utilisateurs de voir les heures prévues et les heures réelles auxquelles ils ont accès. Ils peuvent, toutefois, voir les Heures réelles qu’ils se connectent eux-mêmes ou les heures consignées par une personne qui leur envoie des rapports.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne jamais autoriser les utilisateurs à supprimer les annonces</td> 
      <td>Empêche les utilisateurs de supprimer des annonces dans le Centre d’annonces. Pour plus d’informations, voir <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Envoi d’annonces</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditionnel et facultatif) Si votre système Workfront est configuré pour les utilisateurs appartenant à plusieurs sociétés, limitez la visibilité aux autres utilisateurs en fonction de la société à laquelle ils appartiennent dans la section **Les personnes d’autres sociétés ne doivent afficher que les utilisateurs de**.

   Vous pouvez empêcher les utilisateurs d’afficher uniquement les utilisateurs de leur propre société ou de la société que vous avez désignée comme principale société. L’entreprise principale représente généralement votre compte Workfront où la plupart de vos utilisateurs travaillent. Pour plus d&#39;informations sur l&#39;entreprise principale, voir [Création et modification d&#39;entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Si deux utilisateurs appartiennent à deux sociétés différentes, mais qu’ils peuvent tous deux voir les utilisateurs de la société principale, ils peuvent voir la zone Mises à jour associée à la société principale.

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, passez à l’un des articles répertoriés dans [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), tels que [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cliquer sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à un utilisateur (sauf s’il s’agit d’un niveau d’accès Administrateur système).

   Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Pour plus d’informations sur la manière dont un administrateur d’Adobe affecte un niveau d’accès Administrateur système à un utilisateur, voir [Octroi d’un accès d’administration complet à un utilisateur](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Utilisateurs standard ou planificateurs ayant un accès administratif aux rôles de tâche {#planner-users}

Si vous accordez à un utilisateur Standard ou Planificateur l’accès administratif aux rôles de tâche, le paramètre Modifier la facturation et les taux de coût du rôle est automatiquement activé pour l’utilisateur.

Par la suite, si vous désactivez l’accès administratif aux rôles de tâche pour l’utilisateur, les rôles de tâche sont toujours visibles par l’utilisateur, car le paramètre Modifier les taux de facturation et de coût du rôle est toujours activé.

Si cela se produit et que vous devez supprimer l’accès de l’utilisateur à l’affichage des rôles de tâche, vous devez désactiver le paramètre d’autorisation Modifier la facturation et les taux de coût du rôle de l’utilisateur. Pour obtenir des instructions, voir [Accorder l’accès aux données financières](grant-access-financial.md).
