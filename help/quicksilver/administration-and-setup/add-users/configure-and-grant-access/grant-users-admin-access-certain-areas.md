---
title: Octroi aux utilisateurs un accès administratif à certaines zones
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour accorder aux utilisateurs et utilisatrices un accès administratif de licence Plan à certaines zones du système.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 99%

---

# Accorder un accès administratif à certaines zones aux utilisateurs et utilisatrices

<!--Linked in several places, do not rename or change URL.-->

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un niveau d’accès pour accorder aux utilisateurs et utilisatrices un accès administratif de licence Plan à certaines zones du système.

>[!NOTE]
>
>Cela diffère de l’accès administratif complet à Workfront pour un utilisateur ou une utilisatrice, qui est expliqué dans la section [Accorder un accès administratif complet à un utilisateur ou une utilisatrice](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Octroyer aux utilisateurs et utilisatrices du Plan un accès administratif à certaines zones de Workfront

>[!IMPORTANT]
>
>Nous vous recommandons vivement de ne pas modifier les niveaux d’accès intégrés afin que vous puissiez y faire référence après avoir configuré vos utilisateurs et utilisatrices. Pour personnaliser un niveau d’accès, copiez le niveau d’accès par défaut et modifiez la copie. (Vous pouvez procéder ainsi pour chaque niveau d’accès, à l’exception de l’administrateur ou administratrice système et de l’utilisateur ou l’utilisatrice externe.)

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Niveaux d’accès**.
1. Cliquez sur le nom du niveau d’accès que vous souhaitez utiliser pour accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones de Workfront.
1. Dans la section **Autoriser l’accès administratif pour**, cochez les cases pour accorder l’accès administratif nécessaire.

   Ces options vous permettent d’accorder les fonctionnalités suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processus d’approbation</td> 
      <td><p>Créez et gérez des processus d’approbation à utiliser dans l’ensemble du système et pour des groupes spécifiques.</p><p>Sans cet accès, les utilisateurs et utilisatrices peuvent uniquement créer des processus d’approbation ad hoc sur les éléments auxquels ils ont accès pour la gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entreprises</td> 
      <td><p>Ajouter de nouvelles entreprises et modifier des entreprises existantes dans Workfront</p>
      <p>Sans cet accès, les utilisateurs et utilisatrices peuvent uniquement afficher les entreprises existantes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulaires personnalisés dans mon groupe</td> 
      <td><p>Créez et modifiez (ajoutez, modifiez et supprimez les champs) des formulaires personnalisés dans leur groupe.</p><p>Sans cet accès, les utilisateurs et utilisatrices peuvent uniquement joindre des formulaires existants à des objets auxquels ils ont accès pour la contribution ou la gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taux de change</td> 
      <td> <p>Ajouter une nouvelle devise dans Workfront</p> <p>Sans cet accès, l’utilisateur et utilisatrice peuvent uniquement ajouter une devise existante à un projet qu’ils créent.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Frais</td> 
      <td><p>Afficher toutes les dépenses sur les objets dans Workfront.</p><p>Cela ne permet pas à l’utilisateur ou utilisatrice de créer de nouveaux types de dépenses.</p><p>Sans cet accès, l’utilisateur et l’utilisatrice ne peuvent afficher que les éléments suivants :</p>
       <ul>
        <li>Dépenses sur les projets, tâches ou problèmes qu’ils gèrent.</li>
        <li>Leurs propres dépenses.</li>
        <li>Les dépenses de leurs subordonnés.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fonctions</td> 
      <td> <p>Avec cet accès, l’utilisateur et utilisatrice sont autorisés à effectuer les opérations suivantes :</p> 
       <ul> 
        <li>Afficher et modifier des fonctions existantes</li> 
        <li>Ajouter des fonctions</li> 
        <li>Modifier les taux de facturation et de coûts du rôle</li> 
       </ul> <p><b>IMPORTANT</b> : si vous accordez à un utilisateur ou une utilisatrice du planificateur l’accès administratif aux fonctions, le paramètre d’accès aux données financières Modifier les taux de facturation et de coûts du rôle est activé automatiquement pour l’utilisateur ou l’utilisatrice. Par la suite, si vous désactivez l’accès administratif aux fonctions pour l’utilisateur ou l’utilisatrice du planificateur, les fonctions sont toujours visibles par l’utilisateur ou l’utilisatrice, car le paramètre Modifier les taux de facturation et de coûts du rôle est toujours activé. Si cela se produit et que vous devez supprimer l’accès de l’utilisateur ou de l’utilisatrice à l’affichage des fonctions, désactivez le paramètre d’autorisation Modifier la facturation et les taux de dépense du rôle pour cette personne. Pour obtenir des instructions, voir la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Accorder l’accès aux données financières</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Jalons dans mon groupe</td> 
      <td>Affichez tous les chemins de jalons du système sous le menu Chemins de jalons dans Configuration. Les utilisateurs et utilisatrices peuvent également modifier ou supprimer les chemins de jalons appartenant à leurs groupes. Les utilisateurs et utilisatrices ne peuvent pas gérer (modifier ou supprimer) les chemins de jalons qui ne sont affectés à aucun de leurs groupes.<br><p>Sans cet accès, les utilisateurs et utilisatrices peuvent uniquement afficher les chemins de jalons existants et les appliquer aux projets pour lesquels ils ont un accès en gestion.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications de rappel</td> 
      <td>Créez et gérez des notifications de rappel dans Workfront.<br>Sans cet accès, les utilisateurs et utilisatrices peuvent uniquement recevoir et afficher des notifications.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Feuilles de temps et heures</td> 
      <td> <p>Permet d’afficher toutes les heures et les feuilles de temps dans Workfront.</p> <p>Lorsque cette option est désactivée, les utilisateurs et utilisatrices peuvent afficher uniquement les heures suivantes :</p> 
       <ul> 
        <li>Projets, tâches ou problèmes qu’ils gèrent.</li> 
        <li>Leur propre feuille de temps.</li> 
        <li>La feuille de temps d’une personne qui leur est subordonnée.</li> 
        <li>Une feuille de temps qu’ils approuvent.</li> 
       </ul> <p><b>REMARQUE</b> :  <p>Que cette option soit activée ou désactivée, les équipes d’administration de groupe peuvent créer des profils de feuille de temps pour les groupes et les sous-groupes qu’elles gèrent et les affecter aux membres du groupe dont elles ont le droit de modifier le profil.</p> <p>L’activation de cette option peut fournir un accès trop important pour certains administrateurs ou certaines administratrices de groupe, car ils peuvent afficher les feuilles de temps générées par les profils de feuille de temps (et les heures) de toutes les personnes du système, et pas seulement celles des groupes qu’ils gèrent. Vous pouvez désactiver cette option pour les administrateurs et administratrices de groupes qui n’ont pas besoin d’un accès aussi important.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Lorsque vous avez terminé, cliquez sur **Enregistrer**.
1. Affectez le nouveau niveau d’accès à un utilisateur ou une utilisatrice, comme décrit dans la section [Ajouter des utilisateurs et utilisatrices](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Vous pouvez autoriser les utilisateurs et utilisatrices à avoir un accès administratif à d’autres personnes. Pour plus d’informations sur l’attribution d’un accès administratif aux utilisateurs et utilisatrices afin qu’ils puissent gérer des comptes d’autres personnes, voir la section [Accorder l’accès aux utilisateurs et utilisatrices](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
