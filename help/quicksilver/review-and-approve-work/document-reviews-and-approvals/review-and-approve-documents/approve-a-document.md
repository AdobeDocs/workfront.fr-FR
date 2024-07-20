---
product-area: projects
navigation-topic: approvals
title: Approbation d’un document dans Workfront
description: Si vous êtes affecté en tant qu’approbateur ou approbatrice à un document, vous pouvez prendre votre décision d’approbation de plusieurs façons.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: 3755eb0d384e7274b88fbeafc2affa85f735efbc
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 98%

---

# Approbation d’un document dans Workfront

Si vous êtes affecté en tant qu’approbateur ou approbatrice à un document, vous pouvez prendre votre décision d’approbation de plusieurs façons.

Pour plus d’informations sur la création d’une approbation de document, voir [Créer une demande de révision ou d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus d’approbation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Afficher ou avoir un accès supérieur aux objets associés aux approbations</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher ou avoir des autorisations supérieures sur les objets associés aux approbations</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Approuver un document à partir de l’accueil

1. Cliquez sur l’icône **Accueil** ![](../assets/home-icon-30x29.png) dans le coin supérieur gauche d’Adobe Workfront.

   >[!NOTE]
   >
   >Votre administrateur ou administratrice Workfront peut apporter les modifications suivantes à l’icône Accueil de votre environnement :
   >
   >* La remplacer par une image personnalisée pour illustrer votre entreprise. Dans ce cas, l’icône sera différente de celle présentée dans cet article.
   >
   >* Remplacer la page à laquelle elle est liée par une autre page. Dans ce cas, cliquez sur **Menu Principal** ![](../assets/main-menu-icon.png) dans le coin supérieur droit de la page, puis sur **Accueil**.

1. Cliquez sur **Filtres** en haut à gauche de la page et assurez-vous que **Approbations** est coché.

   Tous les éléments de travail qui nécessitent votre approbation sont répertoriés dans la liste.

   >[!NOTE]
   >
   >Les approbations affectées à des fonctions ou à des groupes ne sont pas répertoriées dans Accueil. Les approbations affectées à des équipes s’affichent dans le regroupement Demande d’équipe de la liste de travail.

1. Cliquez sur l’approbation de document dans la liste pour laquelle vous souhaitez prendre une décision d’approbation. Les informations concernant l’approbation s’affichent sur le côté droit de la page.

1. Cliquez sur l’une des deux options d’approbation suivantes dans le coin supérieur droit de la page :

   * La liste déroulante **Approuver** contient deux options :

      * **Approuver** indique qu’aucune modification n’est nécessaire pour cette version du document et que l’approbation est accordée.

      * **Approuver avec des modifications** indique que de modifications mineures sont toujours requises sur le document, mais que l’approbation est accordée à la condition que ces modifications soient apportées. Si vous sélectionnez cette option, une fenêtre contenant une zone de texte nommée **Étapes suivantes** dans laquelle vous pouvez spécifier les modifications nécessaires pour que le document soit approuvé s’affiche. Vous pouvez saisir ces informations et cliquer sur **Ajouter un message**, ou cliquer sur **Ignorer** pour envoyer la décision de validation sans informations supplémentaires.

   * **Travail nécessaire** indique que la version du document n’est pas approuvée et nécessite des modifications importantes.

   Tenez compte des points suivants lors de l’affichage des approbations de documents dans Accueil :

   * Le nom de l’utilisateur ou de l’utilisatrice qui a demandé l’approbation s’affiche au-dessus du nom du document dans Accueil avec le texte « *Utilisateur A* souhaiterait votre approbation le... », ainsi que sous **Soumis par** dans les informations d’approbation qui s&#39;affichent à droite lorsqu’une approbation est sélectionnée.

   * Une fois qu’une décision a été prise sur une approbation, celle-ci reste affichée dans l’onglet Mes approbations accompagnée du texte « Décision prise » jusqu’à ce que vous cliquiez sur le bouton **Actualiser** ou jusqu’à ce que vous actualisiez la page du navigateur.

## Approuver un document à partir de la page du document

1. Accédez à la page du document en cliquant sur le nom du document.

1. Sélectionnez la version du document en attente d’approbation dans la liste déroulante de la version située en regard du nom du document. La version la plus récente est sélectionnée par défaut.

   Si la version actuellement sélectionnée du document est en attente d’approbation de votre part, les boutons de décision d’approbation s’affichent dans le coin supérieur droit de la page ; si d’autres versions du document sont en attente d’approbation de votre part, le menu déroulant de la version affiche un point rouge.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Cliquez sur l’une des deux options d’approbation suivantes dans le coin supérieur droit de la page :

   * La liste déroulante **Approuver** contient deux options :

      * **Approuver** indique qu’aucune modification n’est nécessaire pour cette version du document et que l’approbation est accordée.

      * **Approuver avec des modifications** indique que de modifications mineures sont toujours requises sur le document, mais que l’approbation est accordée à la condition que ces modifications soient apportées. Si vous sélectionnez cette option, une fenêtre contenant une zone de texte nommée **Étapes suivantes** dans laquelle vous pouvez spécifier les modifications nécessaires pour que le document soit approuvé s’affiche. Vous pouvez saisir ces informations et cliquer sur **Ajouter un message**, ou cliquer sur **Ignorer** pour envoyer la décision de validation sans informations supplémentaires.

   * **Travail nécessaire** indique que la version du document n’est pas approuvée et nécessite des modifications importantes.

## Approuver un document à partir du volet Résumé du document

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.

1. Cliquez sur le document qui doit être approuvé et le volet Résumé du document s’ouvre.

1. Sélectionnez la version du document que vous souhaitez réviser dans la liste déroulante des versions. La version la plus récente est sélectionnée par défaut.

   Si la version actuellement sélectionnée du document est en attente d’approbation, les boutons de décision d’approbation s’affichent dans le coin supérieur droit du volet Résumé du document. Si d’autres versions du document sont en attente d’approbation pour vous, le menu déroulant des versions affiche un point rouge.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Cliquez sur l’une des deux options d’approbation suivantes dans le coin supérieur droit du volet Résumé du document :

   * La liste déroulante **Approuver** contient deux options :

      * **Approuver** indique qu’aucune modification n’est nécessaire pour cette version du document et que l’approbation est accordée.

      * **Approuver avec des modifications** indique que de modifications mineures sont toujours requises sur le document, mais que l’approbation est accordée à la condition que ces modifications soient apportées. Si vous sélectionnez cette option, une fenêtre contenant une zone de texte nommée **Étapes suivantes** dans laquelle vous pouvez spécifier les modifications nécessaires pour que le document soit approuvé s’affiche. Vous pouvez saisir ces informations et cliquer sur **Ajouter un message**, ou cliquer sur **Ignorer** pour envoyer la décision de validation sans informations supplémentaires.

   * **Travail nécessaire** indique que la version du document n’est pas approuvée et nécessite des modifications importantes.