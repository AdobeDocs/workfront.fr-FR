---
title: Octroi aux utilisateurs un accès administratif à certaines zones
description: En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour accorder aux utilisateurs un accès administratif de licence Plan à certaines zones du système.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# Octroi aux utilisateurs un accès administratif à certaines zones

<!--Linked in several places, do not rename or change URL.-->

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un niveau d’accès pour accorder aux utilisateurs un accès administratif de licence Plan à certaines zones du système.

>[!NOTE]
>
>Cela diffère de l’accès administratif complet à Workfront pour un utilisateur, qui est expliqué dans la section [Octroi d’un accès administratif complet à un utilisateur](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)&#x200B;

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Octroi aux utilisateurs du forfait un accès administratif à certaines zones de Workfront

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs. Pour personnaliser un niveau d&#39;accès, copiez le niveau d&#39;accès par défaut et modifiez la copie. (Vous pouvez le faire pour chaque niveau d’accès, à l’exception de l’administrateur système et de l’utilisateur externe.)

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Niveaux d’accès**.
1. Cliquez sur le nom du niveau d’accès que vous souhaitez utiliser pour accorder aux utilisateurs un accès administratif à certaines zones de Workfront.
1. Dans le **Autoriser l’accès administratif pour** , cochez les cases pour accorder l’accès administratif nécessaire.

   Ces options vous permettent d’accorder les fonctionnalités suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processus d’approbation</td> 
      <td><p>Créez et gérez des processus d’approbation à utiliser dans l’ensemble du système et pour des groupes spécifiques.</p><p>Sans cet accès, les utilisateurs peuvent uniquement créer des processus d’approbation ad hoc sur les éléments qu’ils ont accès à gérer.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entreprises</td> 
      <td><p>Ajout de nouvelles entreprises et modification des entreprises existantes dans Workfront</p>
      <p>Sans cet accès, les utilisateurs peuvent uniquement afficher les entreprises existantes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés</td> 
      <td><p>Créez et modifiez (ajoutez, modifiez et supprimez les champs) des formulaires personnalisés dans leur groupe.</p><p>Sans cet accès, les utilisateurs peuvent uniquement joindre des formulaires existants à des objets pour lesquels ils ont accès à la contribution ou à la gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taux de change</td> 
      <td> <p>Ajoutez une nouvelle devise dans Workfront.</p> <p>Sans cet accès, l’utilisateur peut uniquement ajouter une devise existante à un projet qu’il crée.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td><p>Afficher toutes les dépenses sur les objets dans Workfront.</p><p>Cela ne permet pas à l’utilisateur de créer de nouveaux types de dépenses.</p><p>Sans cet accès, l'utilisateur ne peut visualiser que les éléments suivants :</p>
       <ul>
        <li>Dépenses sur les projets, tâches ou problèmes qu'ils gèrent</li>
        <li>Leurs propres dépenses</li>
        <li>Les dépenses de leurs subordonnés</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fonctions</td> 
      <td> <p>Avec cet accès, l’utilisateur est autorisé à effectuer les opérations suivantes :</p> 
       <ul> 
        <li>Affichage et modification des rôles de tâche existants</li> 
        <li>Ajout de nouveaux rôles de tâche</li> 
        <li>Modifier la facturation des rôles et les taux de coûts</li> 
       </ul> <p><b>IMPORTANT</b>: Si vous accordez à un utilisateur du planificateur l’accès administratif aux rôles de tâche, le paramètre d’accès aux données financières Modifier les taux de facturation et de coût du rôle est activé automatiquement pour l’utilisateur. Par la suite, si vous désactivez l’accès administratif aux rôles pour l’utilisateur du planificateur, les rôles de tâche sont toujours visibles par l’utilisateur, car le paramètre Modifier les taux de facturation et de coût du rôle est toujours activé. Si cela se produit et que vous devez supprimer l’accès de l’utilisateur à l’affichage des rôles de tâche, vous devez désactiver le paramètre d’autorisation Modifier la facturation et les taux de coût du rôle de l’utilisateur. Pour obtenir des instructions, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l'accès aux données financières</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Jalons dans mon groupe</td> 
      <td>Affichez tous les chemins de jalon dans le système sous le menu Chemins de jalon dans Configuration. Les utilisateurs peuvent également modifier ou supprimer les chemins d’accès aux jalons appartenant à l’un de leurs groupes. Les utilisateurs ne peuvent pas gérer (modifier ou supprimer) les chemins de jalon qui ne sont attribués à aucun de leurs groupes.<br><p>Sans cet accès, les utilisateurs peuvent uniquement afficher les chemins de jalon existants et les appliquer aux projets qu’ils ont accès à la gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Créez et gérez des notifications de rappel dans Workfront.<br>Sans cet accès, les utilisateurs sont limités à recevoir et afficher des notifications.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Feuilles de temps et heures</td> 
      <td> <p>Permet aux utilisateurs d’afficher toutes les heures et toutes les feuilles de temps dans Workfront.</p> <p>Lorsque cette option est désactivée, les utilisateurs peuvent afficher uniquement les heures suivantes :</p> 
       <ul> 
        <li>Projets, tâches ou problèmes qu’ils gèrent</li> 
        <li>Leur propre feuille de temps</li> 
        <li>Une feuille de temps d’une personne qui lui fait rapport</li> 
        <li>Une feuille de temps qu’ils approuvent</li> 
       </ul> <p><b>NOTE</b>:  <p>Que cette option soit activée ou désactivée, les administrateurs de groupe peuvent créer des profils de feuille de temps pour les groupes et les sous-groupes qu’ils gèrent et les affecter aux membres du groupe dont ils ont accès aux modifications.</p> <p>L’activation de cette option peut fournir un accès trop important à certains administrateurs de groupe, car ils peuvent afficher les feuilles de temps générées par les profils de feuille de temps (et les heures) pour tous les utilisateurs du système, et pas seulement pour ceux des groupes qu’ils gèrent. Vous pouvez désactiver cette option pour les administrateurs de groupe qui n’ont pas besoin de cet accès.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.
1. Attribuez le nouveau niveau d’accès à un utilisateur, comme décrit dans la section [Ajout d’utilisateurs](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Vous pouvez permettre aux utilisateurs d’avoir un accès administratif aux utilisateurs. Pour plus d’informations sur l’accès administratif des utilisateurs afin qu’ils puissent gérer des comptes d’utilisateurs, voir [Accorder l’accès aux utilisateurs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
