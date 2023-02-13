---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Partage d’un dossier de document
description: Vous pouvez partager un dossier et son contenu à partir de la zone Documents .
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Partage d’un dossier de document

Vous pouvez partager un dossier et son contenu à partir de la zone Documents .

>[!NOTE]
>
>* Le dossier doit se trouver aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet. Chaque dossier au sixième niveau ou au-dessous hérite de ses configurations de partage à partir du dossier situé directement au-dessus.
>
>  Pour plus d’informations sur l’ajout de sous-dossiers pour créer une hiérarchie de dossiers, voir la section [Création de dossiers et de sous-dossiers](../../documents/organizing-documents/create-documents-folder.md#creating-folders) dans l’article [Création de dossiers de document](../../documents/organizing-documents/create-documents-folder.md).
>
>* Les dossiers intelligents ne peuvent pas être partagés.
>* Si vous configurez les options de partage d’un dossier de documents dans un modèle, puis qu’une personne crée un projet à partir de ce modèle, vos configurations de partage ne sont pas transférées vers le dossier de document dans le nouveau projet.
>* Si vous configurez les options de partage d’un dossier de documents au sein d’une tâche, puis copiez cette dernière, vos configurations de partage ne sont pas transférées vers le dossier de document dans la nouvelle tâche.
>


## Exigences d’accès

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Afficher l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage de l’accès à un objet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Partage d’un dossier

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Documents**.

   Ou

   Une fois l’objet Workfront ouvert, cliquez sur **Documents** dans le panneau de gauche.

1. Sélectionnez le dossier, puis cliquez sur l’icône Partager ![](assets/share-icon.png) dans la barre d’outils.

   Le dossier doit se trouver aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet et ne peut pas être un dossier dynamique.

1. Dans la zone qui s’affiche, sous **Octroyer au dossier l’accès**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle de tâche, du groupe ou de la société avec lequel vous souhaitez partager le dossier, puis appuyez sur **Entrée** lorsque le nom s’affiche.
1. Pour ajuster l’accès de l’utilisateur, de l’équipe, du rôle de tâche, du groupe ou de la société que vous venez d’ajouter, cliquez sur le menu déroulant à droite du nom, puis configurez l’une des options disponibles suivantes, ainsi que l’un de ses paramètres avancés :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">L'afficher</td> 
      <td> <p>Possibilité d’afficher le dossier et son contenu.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li><strong>Télécharger</strong>: Possibilité de télécharger le dossier et son contenu sous la forme d’un fichier ZIP</li> 
        <li> <p><strong>Partager</strong>: Possibilité de partager le dossier avec d’autres personnes du système</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le gérer</td> 
      <td> <p>Possibilité d’afficher et de modifier le dossier et son contenu</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les utilisateurs à effectuer les opérations suivantes :</p> 
       <ul> 
        <li><strong>Supprimer</strong>: Supprimer le dossier et son contenu du système</li> 
        <li><b>Télécharger</b>: Téléchargez le dossier et son contenu sous la forme d’un fichier ZIP.</li> 
        <li><strong>Partager</strong>: Partager le dossier et son contenu avec d’autres utilisateurs du système</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez les étapes 3 à 4 pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Si vous souhaitez que tous les utilisateurs du système puissent afficher le dossier et son contenu, cliquez sur l’icône d’engrenage. ![](assets/gear-icon-settings-with-dn-arrow.jpg) dans le coin supérieur droit de la boîte de partage, puis cliquez sur **Rendez cette visibilité à l’échelle du système.**

   Si vous changez d&#39;avis, vous pouvez cliquer sur **Suppression de l’accès à l’échelle du système** (option par défaut).

## Accès des utilisateurs au contenu d’un dossier partagé avec eux

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Actuellement, lorsque vous partagez un dossier, les destinataires ne voient pas le dossier dans leur zone Documents. Cependant, ils peuvent accéder à ses documents en exécutant un rapport de document.

Pour plus d’informations sur l’exécution d’un rapport, voir la section [Rapport sur les objets](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) dans l’article [Présentation des objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Voir aussi [Création d’un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## Autorisations héritées lorsque vous partagez un objet contenant un dossier

Lorsque vous partagez un objet doté d’un dossier de documents, vos destinataires ont également accès au dossier :

* Si vous accordez à vos destinataires l’accès Affichage à l’objet parent, ils disposent de l’accès Affichage au dossier.
* Si vous accordez à vos destinataires l’accès Contribution ou Gérer à l’objet parent, ils disposent de l’accès Gérer au dossier.
* Si vous accordez un type d’accès (Afficher, Contribuer ou Gérer) à l’objet parent et un autre type au dossier, vos destinataires disposent du meilleur de ces deux types d’accès aux documents du dossier.

   Par exemple, si vous partagez l’objet parent avec l’accès Affichage et le dossier avec l’accès Gestion, vos destinataires auront l’option Gérer pour accéder aux documents du dossier.

   >[!NOTE]
   >
   >Un document joint hérite uniquement des autorisations de l’objet auquel il a été joint. Si vous créez un dossier sur l’objet et que vous déplacez le document dans le dossier, il hérite des autorisations du dossier. Cependant, si vous créez un dossier sur un objet parent ou grand-parent et que vous déplacez le document dans ce dossier, il n’hérite pas des autorisations de ce dossier.

* Si l’option &quot;Ne jamais hériter de l’accès aux documents des projets, tâches, problèmes, etc.&quot; est activée au niveau d’accès du destinataire, celui-ci n’héritera pas des autorisations de documents dans un dossier que vous partagez avec lui. Pour leur donner accès à un document du dossier, vous devez le partager.

   Pour plus d’informations sur l’option &quot;Ne jamais hériter&quot;, voir [Configurer l’accès à Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

   Pour plus d’informations sur le partage d’un document, voir [Partage d’un document](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
