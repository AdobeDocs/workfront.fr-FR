---
product-area: projects
navigation-topic: approvals
title: Approbation d’un document
description: Si vous êtes affecté en tant qu’approbateur à un document, il existe plusieurs façons de prendre votre décision d’approbation.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: e8116a6778d5952ba583cfdfb94b761757adc030
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Approbation d’un document

Si vous êtes affecté en tant qu’approbateur à un document, il existe plusieurs façons de prendre votre décision d’approbation.

Pour plus d’informations sur la création d’une validation de document, voir [Créer une demande d’approbation ou de révision de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus de validation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Consulter ou accéder à des objets associés à des validations</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Consulter ou obtenir des autorisations supérieures aux objets associés aux validations</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Approbation d’un document à partir de l’accueil

1. Cliquez sur le bouton **Accueil** icon ![](../assets/home-icon-30x29.png) dans le coin supérieur gauche d’Adobe Workfront.

   >[!NOTE]
   >
   >Votre administrateur Workfront peut apporter les modifications suivantes à l’icône Accueil de votre environnement :
   >
   >* Remplacez-le par une image personnalisée pour illustrer votre entreprise. Dans ce cas, l’icône sera différente de celle présentée dans cet article.
   >
   >* Remplacez la page qui lui est liée par une autre page. Dans ce cas, cliquez sur le bouton **Menu Principal** ![](../assets/main-menu-icon.png) dans le coin supérieur droit de la page, puis cliquez sur **Accueil**.

1. Cliquez sur **Filtres** en haut à gauche de la page et assurez-vous que **Approbations** est cochée.

   Toutes les tâches qui nécessitent votre approbation sont répertoriées dans la liste.

   >[!NOTE]
   >
   >Les approbations affectées à des rôles de tâche ou à des groupes ne sont pas répertoriées dans Accueil. Les validations affectées aux équipes s’affichent dans le groupe Demande d’équipe de la liste des tâches.

1. Cliquez sur la validation du document dans la liste pour laquelle vous souhaitez effectuer une validation. Les informations concernant l’approbation s’affichent sur le côté droit de la page.

1. Cliquez sur l’une des deux options de validation suivantes dans le coin supérieur droit de la page :

   * La variable **Approuver** la liste déroulante contient deux options :

      * **Approuver** indique qu’aucune modification n’est nécessaire pour cette version du document et que l’approbation est donnée.

      * **Approuver avec des modifications** indique que de petites modifications sont toujours requises dans le document, mais que l’approbation est donnée à la condition que ces modifications soient effectuées. Si vous sélectionnez cette option, une fenêtre contenant une zone de texte nommée **Étapes suivantes** où vous pouvez spécifier les modifications nécessaires pour que le document soit approuvé. Vous pouvez saisir ces informations et cliquer sur **Ajouter un message** ou cliquez sur **Ignorer** pour envoyer la décision de validation sans informations supplémentaires.

   * **Travail nécessaire** indique que la version du document n’est pas approuvée et nécessite des modifications importantes.

   Tenez compte des points suivants lors de l’affichage des approbations de documents dans Accueil :

   * Le nom de l’utilisateur qui a demandé l’approbation s’affiche au-dessus du nom du document dans Accueil avec le texte &quot;*Utilisateur A* Je voudrais votre approbation sur...&quot;, ainsi que sous **Envoyé par** dans les informations de validation qui s&#39;affichent à droite une fois la validation sélectionnée.

   * Une fois qu’une décision a été prise sur une validation, la validation reste dans l’onglet Mes approbations avec le texte &quot;Décision prise&quot; jusqu’à ce que vous cliquiez sur l’onglet **Actualiser** ou jusqu’à ce que vous actualisiez la page du navigateur.

## Approuver un document à partir de la page de document

1. Accédez à la page du document en cliquant sur le nom du document.

1. Sélectionnez la version du document en attente d’approbation dans la liste déroulante des versions située en regard du nom du document. La dernière version est sélectionnée par défaut.

   Si la version actuellement sélectionnée du document est en attente d’approbation, les boutons de décision d’approbation s’affichent dans le coin supérieur droit de la page ; si d’autres versions du document ont été en attente d’approbation pour vous, le menu déroulant de version affiche un point rouge.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Cliquez sur l’une des deux options de validation suivantes dans le coin supérieur droit de la page :

   * La variable **Approuver** la liste déroulante contient deux options :

      * **Approuver** indique qu’aucune modification n’est nécessaire pour cette version du document et que l’approbation est donnée.

      * **Approuver avec des modifications** indique que de petites modifications sont toujours requises dans le document, mais que l’approbation est donnée à la condition que ces modifications soient effectuées. Si vous sélectionnez cette option, une fenêtre contenant une zone de texte nommée **Étapes suivantes** où vous pouvez spécifier les modifications nécessaires pour que le document soit approuvé. Vous pouvez saisir ces informations et cliquer sur **Ajouter un message** ou cliquez sur **Ignorer** pour envoyer la décision de validation sans informations supplémentaires.

   * **Travail nécessaire** indique que la version du document n’est pas approuvée et nécessite des modifications importantes.

## Approuver un document à partir du volet Résumé du document

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.

1. Cliquez sur le document qui doit être approuvé et le volet Résumé du document s’ouvre.

1. Sélectionnez la version du document que vous souhaitez réviser dans la liste déroulante des versions. La dernière version est sélectionnée par défaut.

   Si la version actuellement sélectionnée du document est en attente d’approbation, les boutons de décision d’approbation s’affichent dans le coin supérieur droit du volet Résumé du document ; si d’autres versions du document sont en attente d’approbation pour vous, le menu déroulant Version affiche un point rouge.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Cliquez sur l’une des deux options d’approbation suivantes dans le coin supérieur droit du volet Résumé du document :

   * La variable **Approuver** la liste déroulante contient deux options :

      * **Approuver** indique qu’aucune modification n’est nécessaire pour cette version du document et que l’approbation est donnée.

      * **Approuver avec des modifications** indique que de petites modifications sont toujours requises dans le document, mais que l’approbation est donnée à la condition que ces modifications soient effectuées. Si vous sélectionnez cette option, une fenêtre contenant une zone de texte nommée **Étapes suivantes** où vous pouvez spécifier les modifications nécessaires pour que le document soit approuvé. Vous pouvez saisir ces informations et cliquer sur **Ajouter un message** ou cliquez sur **Ignorer** pour envoyer la décision de validation sans informations supplémentaires.

   * **Travail nécessaire** indique que la version du document n’est pas approuvée et nécessite des modifications importantes.