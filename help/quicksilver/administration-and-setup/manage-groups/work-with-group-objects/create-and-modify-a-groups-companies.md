---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Créer et modifier des sociétés d'un groupe
description: Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher les entreprises associées au groupe et à ses sous-groupes et travailler avec elles.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 83%

---

# Créer et modifier les entreprises d’un groupe

Lorsque vous affichez un groupe que vous gérez dans la zone Groupes, vous pouvez afficher les entreprises associées au groupe et à ses sous-groupes et travailler avec elles.

S’il existe des groupes au-dessus de votre groupe, leurs administrateurs et administratrices peuvent également effectuer ces opérations pour votre groupe. Il en va de même pour les administrateurs et administratrices de Workfront (pour n’importe quel groupe).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Vous devez être un administrateur de groupe du groupe ou un administrateur système.</td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher, utiliser et créer des entreprises pour votre groupe à partir de la zone Groupes

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes** ![Groupes](assets/groups-icon.png).

1. Cliquez sur le nom du groupe pour lequel vous souhaitez créer ou modifier des entreprises.
1. Dans le panneau de gauche, cliquez sur **Entreprises** pour répertorier les entreprises associées au groupe et aux sous-groupes qu’il peut avoir.
1. (Facultatif) Pour ajouter une entreprise, cliquez sur **Ajouter une entreprise**, puis configurez l’entreprise à l’aide des options répertoriées ci-dessous. Lorsque vous avez terminé, cliquez sur **Créer une entreprise**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Section Informations de base</td> 
      <td> 
       <ul> 
        <li> <p><b>Nom de l’entreprise</b> : saisissez le nom de l’entreprise.</p> </li> 
        <li> <p><b>Est active</b> : lorsque cette option est activée, il est possible de trouver l’entreprise et de la joindre aux projets créés et modifiés. Une société inactive ne peut pas être jointe aux projets. Cette option est activée par défaut.</p> </li> 
        <li> <p><b>Ceci est l’entreprise principale</b> : désigne l’entreprise comme entreprise principale de votre organisation. L’entreprise principale représente généralement votre compte Workfront où travaillent la plupart de vos utilisateurs et utilisatrices.</p> <p>En modifiant leur niveau d’accès, vous pouvez autoriser les utilisateurs et utilisatrices à voir les autres personnes :</p> 
         <ul> 
          <li>Uniquement dans leur entreprise principale</li> 
          <li> <p>Dans l’entreprise associée et l’entreprise principale</p> <p>Pour plus d’informations sur la fonctionnalité de l’entreprise principale dans les niveaux d’accès des utilisateurs et utilisatrices, voir la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> <p>Vous ne pouvez désigner qu’une seule entreprise comme entreprise principale ou n’en désigner aucune. Pour plus d’informations, voir la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Groupe</b> : s’il existe un groupe qui traite avec l’entreprise, vous pouvez y ajouter le nom du groupe. Cette fonction peut s’avérer utile pour les administrateurs et administratrices de groupes qui doivent créer des rapports et gérer toutes les entreprises avec lesquelles leurs groupes traitent.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Le système remplit le champ <strong>Groupe</strong> de la nouvelle entreprise avec le nom du groupe que vous affichez.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si vous disposez d’un accès administratif aux entreprises de votre niveau d’accès, vous pouvez supprimer le groupe de l’entreprise et en affecter un autre, ou laisser l’entreprise sans groupe.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Si vous ne disposez pas d’un accès administratif aux entreprises, le champ <strong>Groupe</strong> est obligatoire et vous ne pouvez sélectionner que les groupes que vous gérez ou les sous-groupes de ces groupes.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Pour plus d’informations sur l’accès administratif aux entreprises, voir la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Accorder un accès administratif à certaines zones</a>.</p> </li> 
        <li> <p><b>Membres de l’entreprise</b> : ajoutez des personnes à l’entreprise. Ce faisant, vous associez ces utilisateurs et utilisatrices à cette entreprise.</p> <p>Le nombre d’utilisateurs et d’utilisatrices que vous pouvez associer à une entreprise est illimité, mais une personne ne peut pas être associée à plusieurs sociétés.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Section de formulaires personnalisés</td> 
      <td> <p>Si vous souhaitez ajouter des champs à votre société qui ne sont pas disponibles dans Workfront, vous pouvez créer un formulaire personnalisé et l’associer à votre société. Vous pouvez joindre ce formulaire à votre entreprise en le sélectionnant dans le menu déroulant. Seules les entreprises actives sont répertoriées dans le menu déroulant. Pour plus d’informations sur la création de formulaires personnalisés, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Créer un formulaire personnalisé</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Si vous disposez d’un accès administratif aux entreprises de votre niveau d’accès, vous pouvez également cliquer sur Ajouter d’autres entreprises au bas de la liste. Une ligne est ajoutée et permet de configurer rapidement la nouvelle entreprise.

1. (Facultatif) Pour modifier ou supprimer des sociétés, sélectionnez au moins une société, puis utilisez les boutons de la barre d’outils pour la modifier ![icône Modifier](assets/edit-icon.png) ou la supprimer ![icône Supprimer](assets/delete.png).

   Pour plus d’informations sur la modification d’une entreprise, voir la section [Créer ou modifier une entreprise dans Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) dans l’article [Créer et modifier des entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Facultatif) Pour exporter la liste des sociétés, cliquez sur l’icône Exporter ![icône Exporter](assets/export.png), puis sélectionnez le format de fichier souhaité pour la liste exportée.
