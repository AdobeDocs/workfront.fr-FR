---
product-area: documents
navigation-topic: manage-documents
title: Gestion des versions de document
description: Vous pouvez gérer plusieurs versions d’un document dans Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Gestion des versions de document

Vous pouvez gérer plusieurs versions d’un document dans Workfront.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Afficher l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher l’accès au document</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

* Cet article suppose que le document comporte plusieurs versions.

   Si vous avez besoin d’informations sur le téléchargement de nouvelles versions d’un document vers Workfront, reportez-vous à la section [Télécharger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

## Affichage d’une liste de toutes les versions d’un document

1. Dans le résumé, faites défiler l’écran jusqu’à la vue **Toutes les versions** . Vous pouvez afficher ici toutes les versions du document.

## Affichage et gestion des détails d’une version de document précédente

1. Près de la partie supérieure de la page Détails du document, cliquez dans le menu déroulant en regard du nom, puis cliquez sur le nom de la version que vous souhaitez afficher et gérer.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   En plus d’afficher les détails de la version, vous pouvez apporter des modifications à la version, telles que son nom, ses métadonnées et ses paramètres de vérification (s’il s’agit d’un BAT de document).

## Téléchargement d’une version de document unique

1. Dans le résumé, sous **Versions**, cliquez sur le menu Plus . ![](assets/more-icon.png) à droite de la version, puis cliquez sur **Télécharger** dans la liste déroulante qui s’affiche.

   ![](assets/more-versions-350x143.png)

## Téléchargement de toutes les versions d’un document

1. Cliquez sur **Détails du document**, puis sélectionnez **Toutes les versions** dans le panneau de gauche.

1. Cliquez sur **Tout télécharger** en haut de la liste.

## Suppression d’une version de document

Si vous téléchargez par erreur une version d’un document ou si une version n’est plus nécessaire, vous pouvez supprimer la version et conserver le document d’origine.

>[!IMPORTANT]
>
>Vous ne pouvez pas récupérer une version de document que vous supprimez individuellement.

Gardez ce qui suit à l’esprit lorsque vous envisagez de supprimer une version de document :

* Une seule version peut être supprimée à la fois. Si une version est supprimée, cette action apparaît dans la variable **Mises à jour** dans le document .
* Si vous chargez une nouvelle version après avoir supprimé une version, la nouvelle version reçoit le numéro de séquence suivant. Par exemple, s’il existe 3 versions d’un document et que vous supprimez la version 3, le document téléchargé suivant sera la version 4.
* Les mises à jour système et les commentaires effectués sur une version sont conservés dans Workfront une fois la version supprimée.

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Pour supprimer une version de document :

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.Recherchez le document dont vous avez besoin.
1. Dans le **Version** dans le résumé, cliquez sur la version, puis sur **Supprimer** dans la liste déroulante qui s’affiche. Le **Supprimer** n’est visible que s’il existe au moins deux versions.

   Si le document est lié à une source externe, ce lien est supprimé et le document n’est plus accessible via Workfront.

   ![](assets/more-versions-350x143.png)
