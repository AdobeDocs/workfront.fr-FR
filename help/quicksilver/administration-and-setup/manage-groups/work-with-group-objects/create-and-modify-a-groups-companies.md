---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Création et modification d’entreprises d’un groupe
description: Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et travailler avec les entreprises associées au groupe et à l’un de ses sous-groupes.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: ab7877c048ea87180dd518c978b258d266e0f95c
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 0%

---

# Création et modification d’entreprises d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et travailler avec les entreprises associées au groupe et à l’un de ses sous-groupes.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs de Workfront (pour n’importe quel groupe).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur de groupe du groupe ou un administrateur Workfront. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administrateurs de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si vous devez savoir quel plan ou type de licence vous avez, contactez votre administrateur Workfront.

## Affichage, utilisation et création d’entreprises pour votre groupe à partir de la zone Groupes

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez créer ou modifier des sociétés.
1. Dans le panneau de gauche, cliquez sur **Entreprises** pour répertorier les entreprises associées au groupe et les sous-groupes qu’il peut avoir.
1. (Facultatif) Pour ajouter une société, cliquez sur **Ajouter une société**, puis configurez l’entreprise à l’aide des options répertoriées ci-dessous. Lorsque vous avez terminé, cliquez sur **Créer une entreprise**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Section Informations de base</td> 
      <td> 
       <ul> 
        <li> <p><b>Nom de la société</b>: saisissez le nom de la société.</p> </li> 
        <li> <p><b>Est actif</b>: lorsque cette option est activée, les utilisateurs peuvent rechercher la société et la joindre aux projets qu’ils créent et modifient. Une société inactive ne peut pas être jointe aux projets. Cette option est activée par défaut.</p> </li> 
        <li> <p><b>Il s’agit de la société Principal</b>: affecte la société en tant que société principale de votre organisation. L’entreprise principale représente généralement votre compte Workfront où la plupart de vos utilisateurs travaillent.</p> <p>En modifiant leurs niveaux d’accès, vous pouvez limiter les utilisateurs à voir d’autres utilisateurs :</p> 
         <ul> 
          <li>Uniquement dans leur entreprise principale</li> 
          <li> <p>Dans la société associée et la société principale</p> <p>Pour plus d’informations sur les principales fonctionnalités de l’entreprise dans les niveaux d’accès des utilisateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Création ou modification de niveaux d’accès personnalisés</a>.</p> <p>Vous ne pouvez désigner qu’une seule société ou aucune société comme société principale, mais vous ne pouvez pas désigner plusieurs sociétés comme sociétés principales. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Création ou modification de niveaux d’accès personnalisés</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Groupe</b>: s’il existe un groupe qui gère des affaires avec la société, vous pouvez y ajouter le nom du groupe. Cela s’avère utile pour les administrateurs de groupe qui doivent créer des rapports et gérer toutes les entreprises avec lesquelles leurs groupes traitent.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Le système remplit la variable <strong>Groupe</strong> pour la nouvelle société avec le groupe que vous affichez.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si vous disposez d’un accès administratif aux entreprises de votre niveau d’accès, vous pouvez supprimer le groupe de l’entreprise et en affecter un autre, ou laisser l’entreprise sans groupe.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si vous n’avez pas d’accès administratif aux entreprises, la variable <strong>Groupe</strong> est obligatoire et vous pouvez sélectionner uniquement les groupes que vous gérez ou les sous-groupes de ces groupes.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Pour plus d’informations sur l’accès administratif aux entreprises, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </li> 
        <li> <p><b>Membres de la société</b>: ajoutez des utilisateurs existants à la société. Ce faisant, vous associez ces utilisateurs à cette entreprise.</p> <p>Le nombre d’utilisateurs que vous associez à une société est illimité, mais un utilisateur ne peut pas être associé à plusieurs sociétés.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Section Forms personnalisée</td> 
      <td> <p>Si des champs que vous souhaitez ajouter à votre société ne sont pas disponibles dans Workfront, vous pouvez créer un formulaire personnalisé et l’associer à votre société. Vous pouvez joindre ce formulaire à votre société en le sélectionnant dans le menu déroulant. Seules les entreprises actives sont répertoriées dans le menu déroulant. Pour plus d’informations sur la création d’un Forms personnalisé, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Création ou modification d’un formulaire personnalisé</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si vous disposez d’un accès administratif aux entreprises de votre niveau d’accès, vous pouvez également cliquer sur Ajouter d’autres entreprises au bas de la liste. Une ligne supplémentaire permet de configurer rapidement la nouvelle société.

1. (Facultatif) Pour modifier ou supprimer des sociétés, sélectionnez au moins une société, puis utilisez les boutons de la barre d’outils pour la modifier. ![](assets/edit-icon.png) ou supprimer ![](assets/delete.png) c&#39;est le cas.

   Pour plus d’informations sur la modification d’une société, voir la section [Création ou modification d’une entreprise dans Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) dans l’article [Création et modification d’entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Facultatif) Pour exporter la liste des entreprises, cliquez sur l’icône Exporter . ![](assets/export.png), puis sélectionnez le format de fichier souhaité pour la liste exportée.
