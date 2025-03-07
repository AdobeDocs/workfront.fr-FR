---
title: Créer et modifier des niveaux d'accès personnalisés
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des niveaux d’accès personnalisés et les appliquer aux personnes.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 3e48bebde0171c13b4168d7eb5d693b07cb9e396
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 98%

---

# Créer et modifier des niveaux d’accès personnalisés

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez créer des niveaux d’accès personnalisés et les appliquer aux personnes. Lorsque vous utilisez des niveaux d’accès, il est important de comprendre comment ils fonctionnent avec les autorisations d’objet que les personnes accordent lorsqu’elles partagent des objets les unes avec les autres. Pour plus d’informations sur les niveaux d’accès, voir ce qui suit :

* [Vue d’ensemble des nouveaux niveaux d’accès](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Vue d’ensemble des niveaux d’accès](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs et utilisatrices. Pour personnaliser un niveau d’accès, copiez le niveau d’accès par défaut et modifiez la copie. Vous pouvez le faire pour chaque niveau d’accès, à l’exception d’administrateur ou administratrice système et d’utilisateur ou utilisatrice externe.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Nouveau : Standard
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer ou modifier un niveau d’accès personnalisé

{{step-1-to-setup}}

1. Cliquez sur **Niveaux d’accès** dans le panneau de gauche.
1. Sélectionnez le niveau d’accès à copier et personnaliser, puis cliquez sur **Copier**.

   Ou

   Si vous modifiez un niveau d’accès existant (que vous avez copié précédemment), cliquez sur son nom.

1. Dans la zone qui s’affiche, effectuez l’une des opérations suivantes pour commencer à configurer le niveau d’accès personnalisé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom</td> 
      <td> <p>Saisissez le nom de votre niveau d’accès. </p> <p>Si vous venez de copier un niveau d’accès pour en créer un nouveau, le nom par défaut est Nom du niveau d’accès (copie), où Nom du niveau d’accès est le niveau d’accès que vous avez copié.</p> <p><strong>Conseil</strong> : nous vous recommandons d’inclure le nom original du niveau d’accès dans le nom de la copie. Par exemple, dans la société ACME, une copie du niveau d’accès standard peut être nommée ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description </td> 
      <td>Saisissez une description pour le niveau d’accès. Il est utile d’indiquer ici à quoi une personne disposant de ce niveau d’accès pourra accéder.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type de licence</td> 
      <td>Assurez-vous que la licence sélectionnée ici est celle qui est la plus étroitement associée au type de niveau d’accès que vous créez ou modifiez. La licence sélectionnée détermine les paramètres disponibles pour le niveau d’accès. Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Vue d’ensemble des nouvelles licences</a> ou <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Vue d’ensemble des licences</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Le cas échéant) Si **Standard** ou **Plan** est sélectionné dans la case **Type de licence**, faites défiler jusqu’à la section **Autoriser l’accès administratif pour** et sélectionnez les autorisations d’accès administratif pour les personnes qui auront ce niveau d’accès.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processus d’approbation</td> 
      <td>Créez et gérez des processus d’approbation à utiliser dans l’ensemble du système et pour des groupes spécifiques.<p>Sans cet accès, les personnes peuvent uniquement créer des processus d’approbation ad hoc sur les éléments pour lesquels elles disposent d’un accès en gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entreprises</td> 
      <td>Ajoutez de nouvelles entreprises et modifiez les entreprises existantes dans Workfront.<br><p>Sans cet accès, les utilisateurs et utilisatrices peuvent uniquement afficher les entreprises existantes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés dans mon groupe</td> 
      <td>Créez et gérez tous les formulaires personnalisés de leur groupe. <br><p>Sans cet accès, les personnes peuvent uniquement joindre des formulaires existants aux objets auxquels elles disposent d’un accès en contribution ou en gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taux de change</td> 
      <td> Ajouter une nouvelle devise dans Workfront <p>Sans cet accès, l’utilisateur et utilisatrice peuvent ajouter une devise existante uniquement à un projet qu’ils créent.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td>Afficher toutes les dépenses sur les objets dans Workfront.<p>Sans cet accès, l’utilisateur et l’utilisatrice ne peuvent afficher que les éléments suivants :</p>
       <ul>
        <li>Dépenses sur les projets, tâches ou problèmes qu’ils gèrent.</li>
        <li>Leurs propres dépenses.</li>
        <li>Les dépenses de leurs subordonnés.</li>
       </ul><p><b>NOTE</b> : cela ne permet pas à l’utilisateur ou utilisatrice de créer de nouveaux types de dépenses.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fonctions</td> 
      <td> Avec cet accès, l’utilisateur et utilisatrice sont autorisés à effectuer les opérations suivantes : 
       <ul> 
        <li>Afficher et modifier des fonctions existantes</li> 
        <li>Ajouter des fonctions</li> 
        <li>Modifier les taux de facturation et de coûts du rôle</li> 
       </ul> 
       <p>Pour obtenir des informations importantes sur l’accès aux données financières disponibles pour un utilisateur ou une utilisatrice standard ou de type planificateur disposant d’un accès administratif aux fonctions, voir <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Utilisateurs et utilisatrices standard ou de type planificateur disposant d’un accès administratif aux fonctions</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Jalons dans mon groupe</td> 
      <td>Affichez tous les chemins de jalons du système sous le menu Chemins de jalons dans Configuration. Les utilisateurs et utilisatrices peuvent également modifier ou supprimer les chemins de jalons appartenant à leurs groupes. Les utilisateurs et utilisatrices ne peuvent pas gérer (modifier ou supprimer) les chemins jalonnés qui ne sont affectés à aucun de leurs groupes.<p>Sans cet accès, les utilisateurs et utilisatrices peuvent uniquement afficher les chemins de jalons existants et les appliquer aux projets pour lesquels ils ont un accès en gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Créez et gérez des notifications de rappel dans Workfront.<p>Sans cet accès, les utilisateurs et utilisatrices peuvent uniquement recevoir et afficher des notifications.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Feuilles de temps et heures</td> 
      <td> Les administrateurs et administratrices de groupes peuvent affecter des profils de feuille de temps aux utilisateurs et utilisatrices dans les groupes et sous-groupes qu’ils gèrent. <p>Si cette option n’est pas activée, les administrateurs et administratrices de groupes ne peuvent pas affecter de profils de feuille de temps à d’autres utilisateurs et utilisatrices dans les groupes et sous-groupes qu’ils gèrent, bien qu’ils puissent les créer.</p> <p>Tous les autres utilisateurs et utilisatrices disposant d’une licence Standard ou Plan peuvent afficher toutes les heures et les feuilles de temps dans Workfront.</p> <p>Si cette option n’est pas activée, les utilisateurs et utilisatrices peuvent afficher les heures uniquement sur :</p> 
       <ul> 
        <li>Les projets, tâches ou problèmes qu’ils gèrent.</li> 
        <li>Leur propre feuille de temps.</li> 
        <li>La feuille de temps d’une personne qui leur est subordonnée.</li> 
        <li>Une feuille de temps qu’ils approuvent.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Définir des restrictions supplémentaires**, puis définissez l’une des restrictions suivantes pour le niveau d’accès.

   >[!IMPORTANT]
   >
   >Pour les utilisateurs et utilisatrices externes tels que les fournisseurs (toute personne ne faisant pas partie de votre organisation), nous vous recommandons de restreindre l’accès aux tâches, projets, mises à jour, annonces, autres entreprises, équipes et groupes.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ne jamais donner accès au projet complet en cas d'affectation à une tâche ou un événement</td> 
      <td> Permet d’empêcher les utilisateurs et utilisatrices affectés à des tâches ou des problèmes d’obtenir également des autorisations pour le projet parent, même si les autorisations du projet le permettent.<p>Pour plus d’informations sur la configuration des autorisations sur un projet, voir la section <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> dans l’article <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Modifier des projets</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ne jamais hériter l'accès aux documents depuis des projets, des tâches, des événements, etc...</td> 
      <td>Empêche les documents d’hériter des autorisations définies sur leur objet parent.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher uniquement les mises à jour dans lesquelles ils ont été inclus dans la conversation</td> 
      <td> Permet aux utilisateurs et utilisatrices de n’afficher que les commentaires pour lesquels leur nom ou le nom de leur équipe a été inclus. <p> <p><b>NOTE</b> : cela empêche les utilisateurs et utilisatrices de s’abonner aux éléments dans Workfront. Pour plus d’informations sur l’abonnement aux éléments, voir <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">S’abonner aux éléments dans Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne jamais autoriser les utilisateurs à supprimer les commentaires </td> 
      <td> Empêche les utilisateurs et utilisatrices de supprimer les commentaires qu’ils font sur les éléments.  <p><b>NOTE</b> : personne ne peut supprimer les commentaires des autres utilisateurs et utilisatrices.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher uniquement les entreprises, les groupes et les équipes auxquels ils appartiennent</td> 
      <td>Permet aux utilisateurs et utilisatrices d’afficher et de partager des éléments uniquement avec les entreprises, les groupes et les équipes auxquels ils appartiennent.<p><strong>REMARQUE </strong> : les utilisateurs disposant de licences de demandeur ou de contributeur ne peuvent pas afficher les sociétés auxquelles ils n’appartiennent pas, même si cette option est sélectionnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne jamais autoriser que les heures prévues ou les heures réelles soient visibles</td> 
      <td>Empêche les personnes de voir les heures prévues et les heures effectives auxquelles elles ont accès. Elles peuvent, toutefois, voir les heures effectives qu’elles consignent elles-mêmes ou les heures consignées par une personne subordonnée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ne jamais autoriser les utilisateurs à supprimer les annonces</td> 
      <td>Empêche les personnes de supprimer des annonces dans le Centre des annonces. Pour plus d’informations, voir <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Envoyer des annonces</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Le cas échéant et facultatif) Si votre système Workfront est configuré pour les personnes appartenant à plusieurs entreprises, limitez la visibilité aux autres personnes en fonction de l’entreprise à laquelle elles appartiennent dans la section **Les personnes d’autres entreprises ne devraient pouvoir visualiser que les utilisateurs et utilisatrices de**.

   Vous pouvez empêcher les personness d’afficher uniquement les utilisateurs et utilisatrices de leur propre entreprise ou de l’entreprise que vous avez désignée comme entreprise principale. L’entreprise principale représente généralement votre compte Workfront où travaillent la plupart de vos utilisateurs et utilisatrices. Pour plus d’informations sur l’entreprise principale, voir [Créer et modifier des entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Si deux personnes appartiennent à deux entreprises différentes, mais qu’elles peuvent toutes deux voir les utilisateurs et utilisatrices de l’entreprise principale, elles peuvent voir la zone Mises à jour associée à l’entreprise principale.

1. (Facultatif) Pour configurer les paramètres d’accès pour d’autres objets et zones du niveau d’accès sur lequel vous travaillez, continuez avec l’un des articles répertoriés dans la section [Configurer l’accès à Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), par exemple [Accorder l’accès aux tâches](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) et [Accorder l’accès aux données financières](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cliquer sur **Enregistrer**.

   Une fois le niveau d’accès créé, vous pouvez l’affecter à une personne (sauf s’il s’agit d’un niveau d’accès administrateur ou administratrice système).

   Pour plus d’informations, voir [Modifier le profil d’une personne](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Pour plus d’informations sur la manière dont un administrateur ou une administratrice d’Adobe affecte un niveau d’accès administrateur ou administratrice système à une personne, voir [Accorder un accès administratif intégral à une personne](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Utilisateurs et utilisatrices standard ou planificateurs et planificatrices ayant un accès administratif aux fonctions {#planner-users}

Si vous accordez à une personne disposant d’une licence Standard ou Planification l’accès administratif aux fonctions, le paramètre Modifier la facturation et les taux de coût du rôle est automatiquement activé pour cette personne.

Par la suite, si vous désactivez l’accès administratif aux fonctions pour la personne, les fonctions sont toujours visibles par elle, car le paramètre Modifier la facturation et le taux de coût du rôle est toujours activé.

Si cela se produit et que vous devez supprimer l’accès de l’utilisateur ou de l’utilisatrice à l’affichage des fonctions, désactivez le paramètre d’autorisation Modifier la facturation et les taux de dépense du rôle pour cette personne. Pour obtenir des instructions, voir [Accorder l’accès aux données financières](grant-access-financial.md).



