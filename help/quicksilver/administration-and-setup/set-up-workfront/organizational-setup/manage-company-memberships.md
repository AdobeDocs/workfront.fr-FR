---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Gérer les appartenances d’entreprise
description: Dans la zone [!UICONTROL Entreprises] de la section Configuration, vous pouvez ajouter et supprimer des personnes membres d’une entreprise. Vous pouvez également modifier leur profil d’utilisateur ou d’utilisatrice, leur rappeler de s’inscrire dans le système  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] .
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 705fc990f2d90ff2102233fc68947fdbe1eb6946
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 92%

---

# Gérer les adhésions des entreprises

Dans la zone [!UICONTROL Entreprises] dans [!UICONTROL Configuration], vous pouvez ajouter et supprimer des personnes membres d’une entreprise. Vous pouvez également modifier leur profil d’utilisateur ou d’utilisatrice, leur rappeler de s’inscrire sur [!DNL Workfront], les désactiver sur [!DNL Workfront] et les supprimer du système [!DNL Workfront].

Pour plus d’informations sur la création d’une nouvelle entreprise, voir [Créer et modifier des entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td><p>Actuel : [!UICONTROL Team] ou version ultérieure</p>
   <p>Ou</p>
   <p>Nouveau : Tous</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licence</p> </td> 
   <td><p>Actuelle : [!UICONTROL Plan]</p>
   <p>Ou</p>
   <p>Nouvelle : [!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong> </td> 
   <td> <p>Utilisez l’une des configurations suivantes :</p> 
    <ul> 
     <li> <p>Le niveau d'accès [!UICONTROL System Administrator], qui permet de modifier n'importe quelle société du système.</p> </li> 
     <li> <p>Accès administratif pour gérer les sociétés, ce qui vous permet de modifier n’importe quelle société du système.</p> </li> 
    </ul> <p><b>NOTE</b> :  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à un groupe pour lequel vous faites partie de l’équipe d’administration.</p> </li> 
      <li> <p>Pour pouvoir ajouter ou supprimer des utilisateurs et utilisatrices du système [!DNL Workfront], vous devez disposer de l’un des éléments suivants :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL System Administrator].</p> </li> 
        <li> <p>Dans votre niveau d’accès, [!UICONTROL Edit] doit être sélectionné pour le paramètre [!UICONTROL Users]. De même, pour le paramètre [!UICONTROL Users], sous [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png">, l’option [!UICONTROL Create] et au moins l’une des deux options [!UICONTROL User Admin] doivent être activées. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez faire partie de l’équipe d’administration du groupe dont la personne est membre.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gérer les adhésions des entreprises

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Entreprises]**.
1. Cliquez sur le nom de l’entreprise.
1. Cliquez sur **[!UICONTROL Membres de la société]** dans le panneau de gauche.
1. Effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ajouter une personne membre</td> 
      <td> <p>Cliquez sur <b>[!UICONTROL Add member]</b>, puis sélectionnez l’une de ces options dans le menu déroulant qui s’affiche :</p> 
       <ul> 
        <li> <p><b>[!UICONTROL New user]</b> : ajoutez une personne qui n’a pas encore été ajoutée à [!DNL Workfront].</p> <p>Pour plus d’informations sur l’ajout de personnes à [!DNL Workfront], voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajouter des personnes</a> et <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’une personne</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: ajoutez une personne existante dans le système, que vous avez le droit de modifier.</p> <p><b>IMPORTANT</b> : si la personne est déjà membre d’une autre entreprise, la nouvelle affectation remplace l’ancienne. La personne perd l’accès aux éléments partagés avec l’entreprise précédente et obtient l’accès aux éléments partagés avec cette entreprise.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b> : importez une personne en chargeant un fichier d’import de feuille de calcul. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importer des personnes</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifier les personnes membres</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Sélectionnez au moins une personne, puis cliquez sur l’icône [!UICONTROL Edit] <img src="assets/edit-icon.png"> dans la barre d’outils.</p> </li> 
        <li value="2"> <p>Configurez les options dans la zone <b>[!UICONTROL Edit User]</b> qui s’affiche.</p> <p>Pour plus d’informations sur ces options, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’une personne</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copier une personne membre</td> 
      <td> <p>Vous pouvez créer une personne membre d’entreprise en copiant une personne membre existante. </p> <p><b>NOTE</b> :  <p>Lorsque vous créez une personne en procédant ainsi, toutes les informations sont copiées à partir de la personne d’origine vers la personne nouvellement créée, à l’exception des éléments suivants :</p> 
        <ul> 
         <li>Les informations de la section [!UICONTROL Personal Info].</li> 
         <li>[!UICONTROL When I log in, show] : l’onglet de destination par défaut pour le niveau d’accès est sélectionné dans cette zone.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Sélectionnez la personne, puis cliquez sur l’icône [!UICONTROL Copy] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>Dans la zone <b>[!UICONTROL New User]</b> qui s’affiche, modifiez les champs disponibles de la nouvelle personne.</p> <p>Pour plus d’informations sur tous les champs associés à une personne, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’une personne</a>.</p> </li> 
        <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Add This User]</strong>.</p> <p>Ou</p> <p>Cliquez sur <strong>[!UICONTROL Add Person User &amp; Start Another]</strong> pour enregistrer la nouvelle personne et en ajouter une autre.</p> </li> 
       </ol> <p>Vous créez ainsi un nouveau compte dans [!DNL Workfront] pour la personne.</p> <p>Si vous avez sélectionné l’option d’envoi d’une invitation à la personne, celle-ci reçoit un e-mail contenant un lien de création de son mot de passe [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer les utilisateurs</td> 
      <td> 
       <div> 
        <p>Sélectionnez au moins une personne, cliquez sur <b>[!UICONTROL Remove users]</b>, puis sélectionnez l’une des options suivantes dans le menu déroulant qui s’affiche :</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remove from company]</b> : supprime la ou les personnes de l’entreprise.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b> : supprime la ou les personnes du système [!DNL Workfront].</p> <p><b>IMPORTANT</b> : la suppression d’une personne du système entraîne également la suppression des informations associées que vous pourriez souhaiter conserver. Nous recommandons de désactiver les personnes plutôt que de les supprimer. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactiver ou réactiver une personne</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer un commentaire aux personnes et à leurs zones [!UICONTROL Updates]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Sélectionnez au moins un utilisateur, puis cliquez sur <b>Envoyer la mise à jour à l’utilisateur</b> dans la barre d’outils.</p> </li> 
        <li value="2"> <p>Saisissez le commentaire à envoyer aux personnes et à la zone [!UICONTROL Updates] de leurs profils.</p>
         <p>Pour plus d’informations, voir <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Envoi de messages directs à d’autres utilisateurs</a>.</p></li> 
       </ol>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exporter la liste des personnes membres de l’entreprise</td> 
      <td> <p>Cliquez sur l’icône [!UICONTROL Export] <img src="assets/export.png"> dans la barre d’outils, puis sélectionnez le format souhaité pour le fichier exporté.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactiver des personnes membres dans le système</td> 
      <td> <p>Sélectionnez au moins une personne, cliquez sur l’icône [!UICONTROL More] <img src="assets/more-icon.png"> dans la barre d’outils, puis sélectionnez <b>[!UICONTROL Deactivate]</b>.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactiver ou réactiver une personne</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Rappeler à une personne de s’enregistrer dans le système</td> 
      <td> <p> Dans la colonne <b>[!UICONTROL Name]</b>, <b>[!UICONTROL Unregistered]</b> s’affiche en regard du nom de chaque personne non enregistrée. Pour rappeler à ces personnes de s’enregistrer dans le système, sélectionnez-les, cliquez sur l’icône [!UICONTROL More] <img src="assets/more-icon.png"> dans la barre d’outils, puis sélectionnez <b>[!UICONTROL Remind user to register]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
