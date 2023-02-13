---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Gestion des appartenances à une entreprise
description: Dans le [!UICONTROL Entreprises] dans Configuration, vous pouvez ajouter et supprimer des membres d’une société. Vous pouvez également modifier leurs profils d’utilisateur, afin de leur rappeler de s’enregistrer dans [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] système.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Gestion des appartenances à une entreprise

Dans le [!UICONTROL Entreprises] area dans [!UICONTROL Configuration], vous pouvez ajouter et supprimer des membres d’une société. Vous pouvez également modifier leurs profils d’utilisateur, afin de leur rappeler de s’enregistrer dans [!DNL Workfront], désactivez-les dans [!DNL Workfront], puis supprimez-les de la fonction [!DNL Workfront] système.

Pour plus d’informations sur la création d’une société, voir [Création et modification d’entreprises](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Exigences d’accès

Pour gérer les entreprises dans , vous devez disposer des éléments suivants : [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan*</p> </td> 
   <td>[!UICONTROL Team] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>L’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès [!UICONTROL Administrateur système] qui permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p>Accès administratif pour la gestion des entreprises, ce qui vous permet de modifier n’importe quelle entreprise du système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Octroi aux utilisateurs un accès administratif à certaines zones</a>.</p> </li> 
    </ul> <p><b>NOTE</b>:  
     <ul> 
      <li> <p>Vous pouvez également gérer les entreprises associées à n’importe quel groupe auquel vous êtes affecté en tant qu’administrateur de groupe.</p> </li> 
      <li> <p>Pour ajouter et supprimer des utilisateurs du [!DNL Workfront] système, vous devez disposer de l’une des fonctionnalités suivantes :</p> 
       <ul> 
        <li> <p>Niveau d’accès [!UICONTROL Administrateur système]. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
        <li> <p>Dans votre niveau d’accès, [!UICONTROL Modifier] doit être sélectionné pour le paramètre [!UICONTROL Utilisateurs] . En outre, pour le paramètre [!UICONTROL Utilisateurs] , sous [!UICONTROL Ajuster vos paramètres] <img src="assets/gear-icon-in-access-levels.png"> , l’option [!UICONTROL Créer] et au moins l’une des deux options [!UICONTROL User Admin] doivent être activées. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Si vous utilisez l’option [!UICONTROL User Admin (Group Users)], vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
       </ul> <p>Pour plus d’informations sur le paramètre Utilisateurs dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou les configurations de niveau d’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Gestion des appartenances à une entreprise

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Entreprises]**.
1. Cliquez sur le nom de la société.
1. Avec le **[!UICONTROL Membres de la société]** dans le panneau de gauche, effectuez l’une des opérations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ajouter un membre</td> 
      <td> <p>Cliquez sur <b>[!UICONTROL Ajouter un membre]</b>, puis sélectionnez l’une de ces options dans le menu déroulant qui s’affiche :</p> 
       <ul> 
        <li> <p><b>[!UICONTROL Nouvel utilisateur]</b>: Ajouter un utilisateur qui n’a pas encore été ajouté à [!DNL Workfront].</p> <p>Pour plus d’informations sur l’ajout d’utilisateurs à [!DNL Workfront], voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Ajout d’utilisateurs</a> et <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Ajoutez déjà un utilisateur, existant dans le système, que vous avez accès à la modification.</p> <p><b>IMPORTANT</b>: Si l’utilisateur est déjà membre d’une autre société, la nouvelle affectation remplace l’ancienne. L’utilisateur perd l’accès aux éléments partagés avec la société précédente et accède aux éléments partagés avec cette société.</p> </li> 
        <li> <p><b>[!UICONTROL Importer des utilisateurs]</b>: Importez un utilisateur en chargeant un fichier d’importation de feuille de calcul. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importer des utilisateurs</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifier les membres</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Sélectionnez au moins un utilisateur, puis cliquez sur l’icône [!UICONTROL Modifier] <img src="assets/edit-icon.png"> dans la barre d’outils.</p> </li> 
        <li value="2"> <p>Configurez les options du <b>[!UICONTROL Modifier l’utilisateur]</b> qui s’affiche.</p> <p>Pour plus d’informations sur ces options, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copier le membre</td> 
      <td> <p>Vous pouvez créer un membre de la société en copiant un membre existant. </p> <p><b>NOTE</b>:  <p>Lorsque vous créez un utilisateur de cette manière, toutes les informations sont copiées de l’utilisateur d’origine vers l’utilisateur nouvellement créé, à l’exception des informations suivantes :</p> 
        <ul> 
         <li>Informations de la section [!UICONTROL Informations personnelles] .</li> 
         <li>[!UICONTROL Lorsque je me connecte, affichez] : L'onglet d'entrée par défaut pour le niveau d'accès est sélectionné dans cette zone.</li> 
         <li>[!UICONTROL Rapports directs]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Sélectionnez l’utilisateur, puis cliquez sur l’icône [!UICONTROL Copier] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>Dans le <b>[!UICONTROL New User]</b> qui s’affiche, modifiez les champs disponibles pour le nouvel utilisateur.</p> <p>Pour plus d’informations sur tous les champs associés à un utilisateur, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> </li> 
        <li value="3"> <p>Cliquez sur <strong>[!UICONTROL Ajouter Cet Utilisateur]</strong>.</p> <p>Ou</p> <p>Cliquez sur <strong>[!UICONTROL Ajouter un utilisateur et démarrer un autre]</strong> pour enregistrer le nouvel utilisateur et en ajouter un autre.</p> </li> 
       </ol> <p>Cela crée un nouveau compte dans [!DNL Workfront] pour l’utilisateur.</p> <p>Si vous avez sélectionné l’option permettant d’envoyer une invitation à l’utilisateur, celui-ci doit recevoir un e-mail dans lequel il peut suivre un lien pour créer sa [!DNL Workfront] mot de passe.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer les utilisateurs</td> 
      <td> 
       <div> 
        <p>Sélectionnez au moins un utilisateur, puis cliquez sur <b>[!UICONTROL Supprimer des utilisateurs]</b>, puis sélectionnez l’une des options suivantes dans le menu déroulant qui s’affiche :</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Supprimer de la société]</b>: Supprime le ou les utilisateurs de la société.</p> </li> 
         <li> <p><b>[!UICONTROL Supprimer]</b>: Supprime le ou les utilisateurs du [!DNL Workfront] système.</p> <p><b>IMPORTANT</b>: La suppression d’un utilisateur du système supprime également les informations associées à l’utilisateur que vous souhaitez peut-être conserver. Il est recommandé de désactiver les utilisateurs au lieu de les supprimer. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>.</p> </li> 
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
      <td> <p>Cliquez sur l’icône [!UICONTROL Export] <img src="assets/export.png"> dans la barre d’outils, sélectionnez le format souhaité pour le fichier exporté.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Désactivation des membres du système</td> 
      <td> <p>Sélectionnez au moins un utilisateur, cliquez sur l’icône [!UICONTROL Plus] <img src="assets/more-icon.png"> dans la barre d’outils, puis sélectionnez <b>[!UICONTROL Désactiver]</b>.</p> <p>Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Rappel à l’utilisateur pour qu’il s’enregistre dans le système</td> 
      <td> <p> Dans le <b>[!UICONTROL Name]</b> column, <b>[!UICONTROL Unregistered]</b> s’affiche en regard du nom de chaque utilisateur non enregistré. Pour rappeler à ces utilisateurs de s’enregistrer dans le système, sélectionnez les utilisateurs, cliquez sur l’icône [!UICONTROL Plus] . <img src="assets/more-icon.png"> dans la barre d’outils, puis sélectionnez <b>[!UICONTROL Rappeler à l’utilisateur de s’enregistrer]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
