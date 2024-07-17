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
ht-degree: 27%

---

# Création et modification d’entreprises d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes , vous pouvez afficher et travailler avec les entreprises associées au groupe et à l’un de ses sous-groupes.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs ou administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour l’administration de Workfront (pour n’importe quel groupe).

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan Workfront*</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Vous devez être un administrateur ou une administratrice de groupe pour le groupe ou un administrateur ou une administratrice de Workfront. Pour plus d’informations, consultez les sections <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administrateurs et administratrices de groupe</a> et <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Accorder l’accès administratif complet à une personne</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir votre plan ou type de licence, contactez l’administration de Workfront.

## Affichage, utilisation et création d’entreprises pour votre groupe à partir de la zone Groupes

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **Groupes** ![](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez créer ou modifier des sociétés.
1. Dans le panneau de gauche, cliquez sur **Entreprises** pour répertorier les entreprises associées au groupe et les sous-groupes qu’il peut avoir.
1. (Facultatif) Pour ajouter une société, cliquez sur **Ajouter une société**, puis configurez la société à l’aide des options répertoriées ci-dessous. Lorsque vous avez terminé, cliquez sur **Créer une entreprise**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Section Informations de base</td> 
      <td> 
       <ul> 
        <li> <p><b>Nom de la société</b> : saisissez un nom pour la société.</p> </li> 
        <li> <p><b>Est actif</b> : lorsque cette option est activée, les utilisateurs peuvent trouver l’entreprise et la joindre aux projets qu’ils créent et modifient. Une entreprise inactive ne peut pas être associée aux projets. Cette option est activée par défaut.</p> </li> 
        <li> <p><b>Il s’agit de la société de Principal </b> : affecte la société en tant que société principale de votre organisation. L’entreprise principale représente généralement votre compte Workfront où la plupart de vos utilisateurs travaillent.</p> <p>En modifiant leurs niveaux d’accès, vous pouvez limiter les utilisateurs à voir d’autres utilisateurs :</p> 
         <ul> 
          <li>Uniquement dans leur entreprise principale</li> 
          <li> <p>Dans la société associée et la société principale</p> <p>Pour plus d’informations sur les principales fonctionnalités de l’entreprise dans les niveaux d’accès des utilisateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Création ou modification de niveaux d’accès personnalisés</a>.</p> <p>Vous ne pouvez désigner qu’une seule société ou aucune société comme société principale, mais vous ne pouvez pas désigner plusieurs sociétés comme sociétés principales. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Groupe</b> : s’il existe un groupe qui exerce des activités avec la société, vous pouvez ajouter le nom du groupe ici. Cela s’avère utile pour les administrateurs et administratrices de groupes qui doivent créer des rapports et gérer toutes les entreprises avec lesquelles leurs groupes traitent.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Le système renseigne le champ <strong>Group</strong> pour la nouvelle société avec le groupe que vous affichez.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si vous disposez d’un accès administratif aux entreprises de votre niveau d’accès, vous pouvez supprimer le groupe de l’entreprise et en affecter un autre, ou laisser l’entreprise sans groupe.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si vous ne disposez pas d’un accès administratif aux sociétés, le champ <strong>Groupe</strong> est requis et vous pouvez sélectionner uniquement les groupes que vous gérez ou les sous-groupes de ces groupes.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Pour plus d'informations sur l'accès administratif aux entreprises, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Octroi aux utilisateurs d'un accès administratif à certaines zones</a>.</p> </li> 
        <li> <p><b>Membres de la société</b> : ajoutez des utilisateurs existants à la société. Ce faisant, vous associez ces utilisateurs et utilisatrices à cette entreprise.</p> <p>Le nombre d’utilisateurs et d’utilisatrices que vous associez à une entreprise est illimité, mais un utilisateur ou une utilisatrice ne peut pas être associé à plusieurs entreprises.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Section Forms personnalisée</td> 
      <td> <p>Si des champs que vous souhaitez ajouter à votre société ne sont pas disponibles dans Workfront, vous pouvez créer un formulaire personnalisé et l’associer à votre société. Vous pouvez joindre ce formulaire à votre entreprise en le sélectionnant dans le menu déroulant. Seules les entreprises actives sont répertoriées dans le menu déroulant. Pour plus d’informations sur la création d’un Forms personnalisé, voir <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Création ou modification d’un formulaire personnalisé</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si vous disposez d’un accès administratif aux entreprises de votre niveau d’accès, vous pouvez également cliquer sur Ajouter d’autres entreprises au bas de la liste. Une ligne supplémentaire permet de configurer rapidement la nouvelle société.

1. (Facultatif) Pour modifier ou supprimer des sociétés, sélectionnez au moins une société, puis utilisez les boutons de la barre d’outils pour la modifier ![](assets/edit-icon.png) ou la supprimer ![](assets/delete.png).

   Pour plus d’informations sur la modification d’une société, reportez-vous à la section [Création ou modification d’une société dans Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) de l’article [Créer et modifier des sociétés](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Facultatif) Pour exporter la liste des sociétés, cliquez sur l&#39;icône Exporter ![](assets/export.png), puis sélectionnez le format de fichier souhaité pour la liste exportée.
