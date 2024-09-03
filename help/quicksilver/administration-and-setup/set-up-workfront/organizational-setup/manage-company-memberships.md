---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Gérer les adhésions des entreprises
description: Dans la zone [!UICONTROL Entreprises] de la section Configuration, vous pouvez ajouter et supprimer des personnes membres d’une entreprise. Vous pouvez également modifier leur profil d’utilisateur ou d’utilisatrice, leur rappeler de s’inscrire dans le système  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 100%

---

# Gérer les adhésions des entreprises

Dans la zone [!UICONTROL Entreprises] dans [!UICONTROL Configuration], vous pouvez ajouter et supprimer des personnes membres d’une entreprise. Vous pouvez également modifier leur profil d’utilisateur ou d’utilisatrice, leur rappeler de s’inscrire sur [!DNL Workfront], les désactiver sur [!DNL Workfront] et les supprimer du système [!DNL Workfront].

Pour plus d’informations sur la création d’une nouvelle entreprise, voir [Créer et modifier des entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Conditions d’accès

Pour pouvoir gérer des entreprises sur [!DNL Workfront], vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] formule*</p> </td> 
   <td>[!UICONTROL Team] ou niveau supérieur</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Utilisez l’une des configurations suivantes :</p> 
    <ul> 
     <li> <p>Le niveau d’accès [!UICONTROL System Administrator], qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès d’administration complet</a>. </p> </li> 
     <li> <p>L’accès administratif à la gestion des entreprises, qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et utilisatrices un accès administratif à certaines zones</a>.</p> </li> 
    </ul> <p><b>NOTE</b> :  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à un groupe pour lequel vous faites partie de l’équipe d’administration.</p> </li> 
      <li> <p>Pour pouvoir ajouter ou supprimer des utilisateurs et utilisatrices du système [!DNL Workfront], vous devez disposer de l’un des éléments suivants :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL System Administrator]. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès administratif complet</a>. </p> </li> 
        <li> <p>Dans votre niveau d’accès, [!UICONTROL Edit] doit être sélectionné pour le paramètre [!UICONTROL Users]. De même, pour le paramètre [!UICONTROL Users], sous [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png">, l’option [!UICONTROL Create] et au moins l’une des deux options [!UICONTROL User Admin] doivent être activées. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez faire partie de l’équipe d’administration du groupe dont la personne est membre.</p> </li> 
       </ul> <p>Pour plus d’informations sur le paramètre Utilisateurs et utilisatrices dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

## Gérer les adhésions des entreprises

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Entreprises]**.
1. Cliquez sur le nom de l’entreprise.
1. La section **[!UICONTROL Personnes membres de l’entreprise]** étant sélectionnée dans le panneau de gauche, effectuez l’une des opérations suivantes :

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
        <li value="1"> <p>Sélectionnez au moins une personne, puis cliquez sur l’icône [!UICONTROL Comment] <img src="assets/comment-icon.png"> dans la barre d’outils.</p> </li> 
        <li value="2"> <p>Saisissez le commentaire à envoyer aux personnes et à la zone [!UICONTROL Updates] de leurs profils.</p> </li> 
       </ol> </td> 
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
