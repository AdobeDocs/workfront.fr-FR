---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Gérer les appartenances à une entreprise
description: Dans la zone [!UICONTROL Entreprises] de Configuration, vous pouvez ajouter et supprimer des membres d’une entreprise. Vous pouvez également modifier leurs profils utilisateur, leur rappeler de s’enregistrer dans le système  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 23%

---

# Gérer les appartenances à une entreprise

Dans la zone [!UICONTROL Entreprises] de [!UICONTROL Configuration], vous pouvez ajouter et supprimer des membres d’une entreprise. Vous pouvez également modifier leurs profils utilisateur, leur rappeler de s&#39;enregistrer dans [!DNL Workfront], les désactiver dans [!DNL Workfront] et les supprimer du système [!DNL Workfront].

Pour plus d&#39;informations sur la création d&#39;une société, voir [Créer et modifier des sociétés](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Conditions d’accès

Pour gérer les entreprises dans [!DNL Workfront], vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] forfait*</p> </td> 
   <td>[!UICONTROL Team] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurations des niveaux d’accès*</strong> </td> 
   <td> <p>Utilisez l’une des configurations suivantes :</p> 
    <ul> 
     <li> <p>Le niveau d’accès [!UICONTROL System Administrator], qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>. </p> </li> 
     <li> <p>L’accès administratif à la gestion des entreprises, qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones</a>.</p> </li> 
    </ul> <p><b>REMARQUE</b> :  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à un groupe pour lequel vous faites partie de l’équipe d’administration.</p> </li> 
      <li> <p>Pour pouvoir ajouter ou supprimer des personnes du système [!DNL Workfront], vous devez disposer de l’un des éléments suivants :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL System Administrator]. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à une personne un accès administratif complet</a>. </p> </li> 
        <li> <p>Dans votre niveau d’accès, [!UICONTROL Edit] doit être sélectionné pour le paramètre [!UICONTROL Users]. En outre, pour le paramètre [!UICONTROL Utilisateurs] , sous [!UICONTROL Ajuster vos paramètres] <img src="assets/gear-icon-in-access-levels.png"> , l’option [!UICONTROL Créer] et au moins l’une des deux options [!UICONTROL Administration des utilisateurs] doivent être activées. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez faire partie de l’équipe d’administration du groupe dont la personne est membre.</p> </li> 
       </ul> <p>Pour plus d’informations sur le paramètre Utilisateurs et utilisatrices dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux personnes</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre administrateur [!DNL Workfront].

## Gérer les appartenances à une entreprise

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Entreprises]**.
1. Cliquez sur le nom de la société.
1. Avec la section **[!UICONTROL Membres de la société]** sélectionnée dans le panneau de gauche, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ajouter un membre</td> 
      <td> <p>Cliquez sur <b>[!UICONTROL Ajouter un membre]</b>, puis sélectionnez l’une des options suivantes dans le menu déroulant qui s’affiche :</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Nouvel utilisateur]</b> : ajoutez un utilisateur qui n’a pas encore été ajouté à [!DNL Workfront].</p> <p>Pour plus d'informations sur l'ajout d'utilisateurs à [!DNL Workfront], voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajout d'utilisateurs</a> et <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d'un utilisateur</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: ajoutez déjà un utilisateur, existant dans le système, que vous avez accès à la modification.</p> <p><b>IMPORTANT</b> : si l’utilisateur est déjà membre d’une autre société, la nouvelle affectation remplace l’ancienne. L’utilisateur perd l’accès aux éléments partagés avec la société précédente et accède aux éléments partagés avec cette société.</p> </li> 
        <li> <p><b>[!UICONTROL Importer des utilisateurs]</b> : importez un utilisateur en chargeant un fichier d’importation de feuille de calcul. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importer des utilisateurs</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifier les membres</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Sélectionnez au moins un utilisateur, puis cliquez sur l’icône [!UICONTROL Modifier] <img src="assets/edit-icon.png"> dans la barre d’outils.</p> </li> 
        <li value="2"> <p>Configurez les options de la zone <b>[!UICONTROL Modifier l’utilisateur]</b> qui s’affiche.</p> <p>Pour plus d’informations sur ces options, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copier le membre</td> 
      <td> <p>Vous pouvez créer un membre de la société en copiant un membre existant. </p> <p><b>NOTE</b> :  <p>Lorsque vous créez un utilisateur de cette manière, toutes les informations sont copiées de l’utilisateur d’origine vers l’utilisateur nouvellement créé, à l’exception des informations suivantes :</p> 
        <ul> 
         <li>Informations de la section [!UICONTROL Informations personnelles] .</li> 
         <li>[!UICONTROL Lorsque je me connecte, afficher] : l’onglet d’entrée par défaut pour le niveau d’accès est sélectionné dans cette zone.</li> 
         <li>[!UICONTROL Rapports directs]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Sélectionnez l’utilisateur, puis cliquez sur l’icône [!UICONTROL Copier] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>Dans la zone <b>[!UICONTROL New User]</b> qui s’affiche, modifiez les champs disponibles pour le nouvel utilisateur.</p> <p>Pour plus d’informations sur tous les champs associés à un utilisateur, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> </li> 
        <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Ajouter Cet Utilisateur]</strong>.</p> <p>Ou</p> <p>Cliquez sur <strong>[!UICONTROL Ajouter un utilisateur et démarrer un autre]</strong> pour enregistrer le nouvel utilisateur et en ajouter un autre.</p> </li> 
       </ol> <p>Cela crée un nouveau compte dans [!DNL Workfront] pour l’utilisateur.</p> <p>Si vous avez sélectionné l’option permettant d’envoyer une invitation à l’utilisateur, celui-ci doit recevoir un e-mail lui permettant de suivre un lien pour créer son mot de passe [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer les utilisateurs</td> 
      <td> 
       <div> 
        <p>Sélectionnez au moins un utilisateur, cliquez sur <b>[!UICONTROL Supprimer les utilisateurs]</b>, puis sélectionnez l’une des options suivantes dans le menu déroulant qui s’affiche :</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Supprimer de la société]</b> : supprime l’utilisateur ou les utilisateurs de la société.</p> </li> 
         <li> <p><b>[!UICONTROL Supprimer]</b> : supprime le ou les utilisateurs du système [!DNL Workfront].</p> <p><b>IMPORTANT</b> : la suppression d’un utilisateur du système supprime également les informations associées à l’utilisateur que vous souhaitez peut-être conserver. Il est recommandé de désactiver les utilisateurs au lieu de les supprimer. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer un commentaire aux utilisateurs et à leurs zones [!UICONTROL Mises à jour]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Sélectionnez au moins un utilisateur, puis cliquez sur l’icône [!UICONTROL Commentaire] <img src="assets/comment-icon.png"> dans la barre d’outils.</p> </li> 
        <li value="2"> <p>Saisissez le commentaire à envoyer aux utilisateurs et à la zone [!UICONTROL Mises à jour] de leurs profils utilisateur.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exporter la liste des membres de l’entreprise</td> 
      <td> <p>Cliquez sur l'icône [!UICONTROL Exporter] <img src="assets/export.png"> dans la barre d'outils, puis sélectionnez le format souhaité pour le fichier exporté.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactivation des membres du système</td> 
      <td> <p>Sélectionnez au moins un utilisateur, cliquez sur l’icône [!UICONTROL Plus] <img src="assets/more-icon.png"> dans la barre d’outils, puis sélectionnez <b>[!UICONTROL Désactiver]</b>.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Rappel à l’utilisateur pour qu’il s’enregistre dans le système</td> 
      <td> <p> Dans la colonne <b>[!UICONTROL Name]</b>, <b>[!UICONTROL Unregistered]</b> s’affiche en regard du nom de chaque utilisateur non enregistré. Pour rappeler à ces utilisateurs de s’enregistrer dans le système, sélectionnez les utilisateurs, cliquez sur l’icône [!UICONTROL Plus] <img src="assets/more-icon.png"> dans la barre d’outils, puis sélectionnez <b>[!UICONTROL Remind user to register]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
