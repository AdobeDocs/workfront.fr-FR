---
product-area: projects
navigation-topic: approvals
title: Approuver du travail
description: Approuver du travail
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: c6e3e3d8d4fd6b6916c8fd49983bc3572949acaa
workflow-type: tm+mt
source-wordcount: '1145'
ht-degree: 100%

---

# Approuver du travail

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Si vous êtes une personne chargée de l’approbation, il est essentiel que vous examiniez régulièrement les travaux en attente de votre approbation.

Pour plus d’informations sur la création de processus d’approbation, voir [Créer un processus d’approbation pour des éléments de travail](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Pour plus d’informations sur l’association des approbations à du travail dans Workfront, voir [Associer un processus d’approbation nouveau ou existant à du travail](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès Afficher ou supérieur aux objets associés à des approbations</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Afficher ou supérieures pour les objets associés aux approbations</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Localiser des approbations dans Adobe Workfront

Vous pouvez afficher et gérer les approbations dans différentes zones de Workfront.

Pour plus d’informations sur l’affichage des éléments en attente d’approbation ou des éléments que vous avez soumis pour approbation, consultez la section [Afficher les approbations](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Approuver le travail depuis la zone d’accueil

1. Cliquez sur l’icône **Accueil** ![](assets/home-icon-30x29.png) dans le coin supérieur gauche d’Adobe Workfront.

   >[!NOTE]
   >
   >Votre administrateur ou administratrice Workfront peut apporter les modifications suivantes à l’icône Accueil de votre environnement :
   >
   >   
   >* La remplacer par une image personnalisée pour illustrer votre entreprise. Dans ce cas, l’icône sera différente de celle présentée dans cet article.
   >* Remplacer la page à laquelle elle est liée par une autre page. Dans ce cas, cliquez sur **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de la page, puis sur **Accueil**.

1. Cliquez sur le menu déroulant **Filtrer**.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Sélectionnez **Approbations**.\
   Tous les éléments de travail nécessitant votre approbation s’affichent. 

   >[!NOTE]
   >
   >Les approbations affectées à des fonctions ou à des groupes ne s’affichent pas dans la page d’accueil. Les approbations affectées aux équipes s’affichent dans le regroupement Demande de l’équipe de la liste des tâches.

1. (Facultatif) Vous pouvez modifier l’ordre d’affichage des approbations selon les instructions fournies dans la section « Grouper et trier par date, projet ou priorité » de l’article [Afficher les éléments de la liste de travail dans la zone d’accueil](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. Sélectionnez l’élément pour lequel vous souhaitez prendre une décision d’approbation.

   ![](assets/task-approval-home-350x127.png)

1. Cliquez sur l’une des options disponibles lorsque vous prenez une décision d’approbation dans le panneau de droite. Les options suivantes s’affichent dans le coin supérieur droit de la page, en fonction du type d’élément que vous approuvez :

   * **Projets :** cliquez sur **Approuver** ou **Rejeter**.

   * **Tâches :** cliquez sur **Approuver** ou **Rejeter**.

   * **Problèmes :** cliquez sur **Approuver** ou **Rejeter**.

   * **Feuilles de temps :** cliquez sur **Approuver** ou **Rejeter**.

   * **Documents :** cliquez sur **Approuver**, **Rejeter**, ou **Modifications**.\
     Tenez compte des points suivants lors de l’affichage des approbations :

      * Les approbations d’épreuves s’affichent ici lorsqu’un utilisateur ou une utilisatrice partage une épreuve avec vous, comme décrit dans la section « Partager une épreuve à partir d’un lien » de l’article [Partager une épreuve dans Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * Les approbations d’épreuves ne sont visibles sur la page d’accueil que si votre environnement Workfront est intégré à un compte Workfront Proof Premium. Si vous ne pouvez pas utiliser la relecture comme décrit ici, contactez votre administrateur ou administratrice Workfront.
      * Vous recevez une notification in-app vous informant de l’approbation de l’épreuve.\
        Pour plus d’informations sur les notifications in-app, consultez la section [Afficher et gérer les notifications in-app](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * Le nom de l’utilisateur ou de l’utilisatrice qui a demandé l’approbation est affiché à côté de la miniature de l’image dans la page d’accueil, avec le texte suivant :\
        « *Personne A* souhaite obtenir votre approbation sur... »

        <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

        Si le nom de l’utilisateur ou de l’utilisatrice n’est pas disponible, le texte suivant s’affiche :\
        « Une nouvelle version d’une épreuve est prête à être révisée ».
      * Pour prendre une décision d’approbation sur l’épreuve, cliquez sur **Accéder à l’épreuve**, puis sur **Terminer la vérification**, enfin, cliquez sur l’une des options disponibles. Les options disponibles lors de l’approbation d’une épreuve sont les suivantes : **Approuvé**, **Approuvé avec des modifications**, **Modifications requises**, et **Non pertinent**.

      * Une fois qu’une décision a été prise concernant l’épreuve, celle-ci demeure dans l’onglet « Mes approbations » avec la mention « Décision prise » jusqu’à ce que vous cliquiez sur le bouton **Actualiser** ou jusqu’à ce que vous actualisiez la page du navigateur.

        Pour plus d’informations sur la révision d’une épreuve, consultez la section [Réviser des épreuves dans Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

   * **Accès :** sélectionnez le niveau d’accès à accorder dans le menu déroulant **Modifier l’accès**, puis cliquez sur **Accorder l’accès**. Ou cliquez sur **Ignorer**.

## Ouvrir une épreuve à partir d’un projet, d’une tâche ou d’un problème

Lorsque vous attendez l’approbation d’un projet, d’une tâche ou d’un problème, vous avez la possibilité d’approuver ou de rejeter cette approbation directement à partir du projet, de la tâche ou du problème en question. Vous pouvez également consulter les détails de la procédure d’approbation.

Pour approuver un travail directement à partir d’un projet, d’une tâche ou d’un problème, procédez comme suit :

1. Accédez au projet, à la tâche ou problème qui nécessite votre approbation.

   Les détails concernant le processus d’approbation d’un projet, d’une tâche ou d’un problème s’affichent dans l’en-tête de l’élément.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   Les informations d’approbation suivantes sont disponibles :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Statut</td> 
      <td>Statut actuel du projet, de la tâche ou du problème. Il s’agit du statut actuel de l’élément en attente d’approbation. Le statut est validé une fois que chaque étape du processus d’approbation a été approuvée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Étapes d’approbation</td> 
      <td>Étapes du processus d’approbation. <br>L’étape en cours qui est en attente d’approbation est affichée comme étant « En attente ». Les étapes déjà validées sont marquées comme approuvées, tandis que celles qui n’ont pas encore été approuvées ont le statut « Non démarré ».</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Approuver** ou **Rejeter**, selon que vous souhaitez approuver ou rejeter le processus d’approbation.\
   L’étape d’approbation en attente a désormais été validée, et le processus d’approbation passe à l’étape suivante. Le statut est approuvé lorsque toutes les étapes ont été approuvées.

## Approuver un document directement à partir d’un document

1. Accédez à la zone des documents qui contient le document nécessitant votre approbation.
1. Sélectionnez le document, puis cliquez sur **Approuver**, **Modifier**, ou **Rejeter**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Facultatif) Si une épreuve a été générée pour le document, vous pouvez approuver le document dans l’interface de relecture, comme décrit dans [Approuver un document à partir d’une épreuve](#approve-a-document-from-a-proof).

## Approuver un document à partir d’une notification d’approbation par e-mail

En fonction de vos paramètres de notification, vous pouvez recevoir par e-mail des notifications d’approbation de documents nécessitant votre intervention pour une décision d’approbation. Lorsque vous recevez un e-mail contenant un bouton **Prendre une décision d’approbation**, vous pouvez lancer le processus d’approbation directement à partir de cet e-mail :

1. Dans l’e-mail, cliquez sur **Prendre une décision d’approbation** pour ouvrir la page des détails du document de l’épreuve.
1. Pour accéder au document, effectuez l’une des actions suivantes :

   * Affichez les métadonnées du document.
   * Si une épreuve a été créée pour réviser le document avec des annotations et des commentaires, cliquez sur **Ouvrir l’épreuve** ![](assets/open-proof-icon-qs.png) dans le coin supérieur droit et révisez l’épreuve.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Pour plus d’informations sur la révision des épreuves, consultez la section [Réviser des épreuves dans Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Cliquez sur l’option **Décision** dans le coin supérieur droit pour approuver, approuver avec des modifications ou rejeter le document.

## Approuver un document à partir d’une épreuve {#approve-a-document-from-a-proof}

Vous pouvez approuver un document dans la visionneuse de relecture. Pour plus d’informations, consultez la section [Prendre une décision sur une épreuve dans la visionneuse de relecture](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) dans l’article [Prendre une décision sur une épreuve dans la visionneuse de relecture](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
