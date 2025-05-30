---
product-area: documents
navigation-topic: manage-documents
title: Gérer les versions de documents
description: Vous pouvez gérer plusieurs versions d’un document dans Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: a9dbfe21337be9cd9929f4e982e4979265ca14e1
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 53%

---

# Gérer les versions de documents

<!-- Audited: 5/2025 -->

Vous pouvez gérer plusieurs versions d’un document dans Workfront.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td> 
   <p>Nouvelle : contributeur ou supérieure<p>
   <p>Ou</p>
   <p>Actuelle : demande ou supérieure </p>


</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès en affichage au document</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

* Cet article part du principe que le document a plusieurs versions.

  Si vous avez besoin d’informations sur le chargement de nouvelles versions d’un document dans Workfront, consultez la section [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md).

## Afficher une liste de toutes les versions d’un document

{{step1-to-documents}}

1. Sur la page **Documents**, sélectionnez un document dans la liste.

1. Dans le coin supérieur droit de la page, cliquez sur l’icône **Ouvrir le résumé** ![Ouvrir le résumé](assets/qs-summary-in-new-toolbar-small.png). Le panneau latéral **Résumé du document** s’ouvre.

1. Faites défiler l’écran jusqu’à la section **Versions** pour afficher toutes les versions du document.

## Afficher et gérer les détails d’une version antérieure d’un document

{{step1-to-documents}}

1. Pointez sur le document, puis cliquez sur **Détails du document**.

1. En haut de la page **Détails du document**, cliquez sur le menu déroulant en regard du nom, puis cliquez sur le nom de la version que vous souhaitez afficher et gérer.

   ![ Liste déroulante Version de la page Détails du document ](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   En plus d’afficher les détails de la version, vous pouvez y apporter des modifications, comme son nom, ses métadonnées et ses paramètres de relecture (s’il s’agit d’une épreuve de document).

## Télécharger une seule version du document

{{step1-to-documents}}

1. Sur la page **Documents**, sélectionnez un document dans la liste.

1. Dans le coin supérieur droit de la page, cliquez sur l’icône **Ouvrir le résumé** ![Ouvrir le résumé](assets/qs-summary-in-new-toolbar-small.png). Le panneau latéral **Résumé du document** s’ouvre.

1. Dans la section **Versions**, cliquez sur le menu **Plus** ![Plus](assets/more-icon.png) à droite de la version, puis cliquez sur **Télécharger** dans la liste déroulante qui s’affiche.

   ![Télécharger un seul document](assets/more-versions-350x143.png)

## Télécharger toutes les versions d’un document

{{step1-to-documents}}

1. Sur la page **Documents**, sélectionnez un document dans la liste.

1. Dans le coin supérieur droit de la page, cliquez sur l’icône **Ouvrir le résumé** ![Ouvrir le résumé](assets/qs-summary-in-new-toolbar-small.png). Le panneau latéral **Résumé du document** s’ouvre.

1. Faites défiler l’écran jusqu’à la section **Versions**, puis cliquez sur **Tout télécharger**.

## Supprimer une version du document

Si vous chargez une version d’un document par erreur, ou si une version n’est plus nécessaire, vous pouvez supprimer la version et conserver le document original.

>[!IMPORTANT]
>
>Vous ne pouvez pas récupérer une version du document que vous avez supprimée séparément.

Gardez les points suivants à l’esprit lorsque vous envisagez de supprimer une version du document :

* Une seule version peut être supprimée à la fois. Si une version est supprimée, cette action apparaît dans la section Mises à jour du document.
* Si vous chargez une nouvelle version après en avoir supprimé une, la nouvelle version reçoit le numéro séquentiel suivant. Par exemple, s’il existe trois versions d’un document et que vous supprimez la troisième version, le prochain document chargé sera la version 4.
* Les mises à jour du système et les commentaires faits sur une version sont conservés dans Workfront après la suppression de la version.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Pour supprimer une version du document, procédez comme suit :

{{step1-to-documents}}

1. Sur la page **Documents**, sélectionnez le document dans la liste.

1. Dans le coin supérieur droit de la page, cliquez sur l’icône **Ouvrir le résumé** ![Ouvrir le résumé](assets/qs-summary-in-new-toolbar-small.png). Le panneau latéral **Résumé du document** s’ouvre.

1. Faites défiler l’écran jusqu’à la section **Versions** pour afficher toutes les versions du document.
1. Dans la section **Versions**, cliquez sur le menu **Plus** ![Plus](assets/more-icon.png) à droite de la version, puis cliquez sur **Supprimer** dans la liste déroulante qui s’affiche.

   >[!NOTE]
   >
   >* L’option **Supprimer** n’est visible que s’il existe au moins 2 versions.
   >* Si le document est lié à une source extérieure, ce lien est supprimé et le document n’est plus accessible via Workfront.

   ![Supprimer la version du document](assets/more-versions-350x143.png)
