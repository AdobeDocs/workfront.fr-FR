---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Partager un dossier de documents
description: Vous pouvez partager un dossier et son contenu à partir de la zone Documents.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 99%

---

# Partager un dossier de documents

Vous pouvez partager un dossier et son contenu à partir de la zone Documents.

>[!NOTE]
>
>* Le dossier doit se trouver dans les cinq premiers niveaux de la hiérarchie des dossiers d’un objet. Chaque dossier du sixième niveau ou d’un niveau inférieur hérite ses configurations de partage du dossier qui lui est directement supérieur.
>
>  Pour plus d’informations sur l’ajout de sous-dossiers pour créer une hiérarchie de dossiers, voir la section [Créer des dossiers et des sous-dossiers](../../documents/organizing-documents/create-documents-folder.md#creating-folders) dans l’article [Créer des dossiers de documents](../../documents/organizing-documents/create-documents-folder.md).
>
>* Les dossiers intelligents ne peuvent pas être partagés.
>* Si vous configurez des options de partage pour un dossier de documents dans un modèle et qu’une personne crée ensuite un projet à partir de ce modèle, vos configurations de partage ne sont pas transférées au dossier de documents dans le nouveau projet.
>* Si vous configurez des options de partage pour un dossier de documents dans un élément de travail et que vous copiez ensuite l’élément de travail, vos configurations de partage ne sont pas transférées au dossier de documents dans le nouvel élément de travail.
>

## Conditions d’accès

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
+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Léger ou supérieur</p> 
   <p>Révision ou supérieur</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Afficher l’accès aux documents</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès Afficher à un objet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Partager un dossier

{{step1-to-documents}}

Ou

Lorsqu’un objet Workfront est ouvert, cliquez sur **Documents** dans le panneau de gauche.

1. Sélectionnez le dossier, puis cliquez sur l’icône Partager ![](assets/share-icon.png) dans la barre d’outils.

   Le dossier doit se trouver dans les cinq premiers niveaux de la hiérarchie des dossiers d’un objet et ne peut pas être un dossier intelligent.

1. Dans la zone qui s’affiche, sous **Accorder l’accès au dossier à**, commencez à entrer le nom de l’utilisateur ou de l’utilisatrice, de l’équipe, de la fonction, du groupe ou de l’entreprise avec qui vous souhaitez partager le dossier, puis appuyez sur **Entrée** lorsque le nom s’affiche.
1. Pour ajuster l’accès de l’utilisateur ou de l’utilisatrice, de l’équipe, de la fonction, du groupe ou de la société que vous venez d’ajouter, cliquez sur le menu déroulant à droite du nom, puis configurez l’une des options disponibles suivantes, ainsi que l’un de ses paramètres avancés :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">L'afficher</td> 
      <td> <p>Possibilité d’afficher le dossier et son contenu.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li><strong>Télécharger</strong> : possibilité de télécharger le dossier et son contenu sous forme de fichier ZIP</li> 
        <li> <p><strong>Partager</strong> : possibilité de partager le dossier avec d’autres personnes dans le système</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le gérer</td> 
      <td> <p>Possibilité d’afficher et de modifier le dossier et son contenu</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les utilisateurs et utilisatrices à effectuer les opérations suivantes :</p> 
       <ul> 
        <li><strong>Supprimer</strong> : supprimer le dossier et son contenu du système</li> 
        <li><b>Télécharger</b> : télécharger le dossier et son contenu sous forme de fichier ZIP</li> 
        <li><strong>Partager</strong> : partager le dossier et son contenu avec d’autres utilisateurs et utilisatrices du système</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez les étapes 3-4 pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Si vous souhaitez que tous les utilisateurs et utilisatrices du système puissent consulter le dossier et son contenu, cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings-with-dn-arrow.jpg) dans le coin supérieur droit de la zone de partage, puis sur **Rendre visible à l’échelle du système.**

   Si vous changez d’avis, cliquez sur **Supprimer l’accès à l’échelle du système** (option par défaut).

## Comment les utilisateurs et utilisatrices accèdent au contenu d’un dossier partagé avec eux

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story   <a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Actuellement, lorsque vous partagez un dossier, celui-ci ne s’affiche pas dans la zone Documents des personnes destinataires. Toutefois, elles peuvent accéder à ses documents en exécutant un rapport de document.

Pour plus d’informations sur l’exécution d’un rapport, voir la section [Créer des rapports sur les objets](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) dans l’article [Comprendre les objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Voir également [Créer un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## Autorisations héritées lorsque vous partagez un objet contenant un dossier.

Lorsque vous partagez un objet comportant un dossier de documents, vos personnes destinataires ont également accès à ce dossier :

* Si vous accordez à vos personnes destinataires un accès Afficher à l’objet parent, elles disposeront d’un accès Afficher au dossier.
* Si vous accordez à vos personnes destinataires l’accès Contribuer ou Gérer à l’objet parent, elles disposeront de l’accès Gérer au dossier.
* Si vous accordez un type d’accès (Afficher, Contribuer ou Gérer) à l’objet parent et un autre au dossier, vos personnes destinataires disposeront du type d’accès le plus élevé aux documents contenus dans le dossier

  Par exemple, si vous partagez l’objet parent avec l’accès Afficher et le dossier avec l’accès Gérer, vos personnes destinataires auront accès aux documents du dossier avec l’accès Gérer.

  >[!NOTE]
  >
  >Un document joint n’hérite des autorisations que de l’objet auquel il a été joint. Si vous créez un dossier sur l’objet et que vous déplacez le document dans le dossier, il hérite des autorisations du dossier. En revanche, si vous créez un dossier sur un objet parent ou grand-parent et que vous déplacez le document dans ce dossier, il n’hérite pas des autorisations de ce dossier.

* Si l’option « Ne jamais hériter de l’accès aux documents depuis des projets, des tâches, des problèmes, etc. » est activée dans le niveau d’accès de la personne destinataire, elle n’héritera pas des autorisations sur les documents d’un dossier que vous partagez avec elle. Pour donner accès à un document dans le dossier, vous devez partager le document.

  Pour plus d’informations sur l’option « Ne jamais hériter », voir [Configurer l’accès à Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  Pour plus d’informations sur le partage d’un document, voir [Partager un document](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
