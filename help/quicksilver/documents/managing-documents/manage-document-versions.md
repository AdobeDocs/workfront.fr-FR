---
product-area: documents
navigation-topic: manage-documents
title: Gérer les versions de documents
description: Vous pouvez gérer plusieurs versions d’un document dans Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 9aa6822c9c1ecade776d4c71b113c1afd997f40c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 100%

---

# Gérer les versions de documents

Vous pouvez gérer plusieurs versions d’un document dans Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en affichage aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès en affichage au document</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Conditions préalables

* Cet article part du principe que le document a plusieurs versions.

  Si vous avez besoin d’informations sur le chargement de nouvelles versions d’un document dans Workfront, consultez la section [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

## Afficher une liste de toutes les versions d’un document

1. Dans le résumé, faites défiler l’écran jusqu’à la section **Toutes les versions**. Vous pouvez y consulter toutes les versions du document.

## Afficher et gérer les détails d’une version antérieure d’un document

1. En haut de la page Détails du document, cliquez sur le menu déroulant en regard du nom, puis sur le nom de la version que vous souhaitez afficher et gérer.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Outre l’affichage des détails de la version, vous pouvez apporter des modifications à la version, telles que son nom, ses métadonnées et ses paramètres de relecture (s’il s’agit d’une épreuve de document).

## Télécharger une seule version du document

1. Dans le résumé, sous **Versions**, cliquez sur le menu Plus ![](assets/more-icon.png) à droite de la version, puis cliquez sur **Télécharger** dans la liste déroulante qui apparaît.

   ![](assets/more-versions-350x143.png)

## Télécharger toutes les versions d’un document

1. Cliquez sur **Détails du document**, puis sélectionnez **Toutes les versions** dans le panneau de gauche.

1. Cliquez sur **Tout télécharger** en haut de la liste.

## Supprimer une version du document

Si vous chargez une version d’un document par erreur, ou si une version n’est plus nécessaire, vous pouvez supprimer la version et conserver le document original.

>[!IMPORTANT]
>
>Vous ne pouvez pas récupérer une version du document que vous avez supprimée séparément.

Gardez les points suivants à l’esprit lorsque vous envisagez de supprimer une version du document :

* Une seule version peut être supprimée à la fois. Si une version est supprimée, cette action apparaît dans les **Mises à jour** du document.
* Si vous chargez une nouvelle version après en avoir supprimé une, la nouvelle version reçoit le numéro séquentiel suivant. Par exemple, s’il existe trois versions d’un document et que vous supprimez la troisième version, le prochain document chargé sera la version 4.
* Les mises à jour du système et les commentaires faits sur une version sont conservés dans Workfront après la suppression de la version.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Pour supprimer une version du document, procédez comme suit :

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**. Recherchez le document dont vous avez besoin.
1. Dans la zone **Version** du résumé, cliquez sur la version, puis sur **Supprimer** dans la liste déroulante qui s’affiche. L’option **Supprimer** n’est visible que s’il existe au moins deux versions.

   Si le document est lié à une source extérieure, ce lien est supprimé et le document n’est plus accessible via Workfront.

   ![](assets/more-versions-350x143.png)
