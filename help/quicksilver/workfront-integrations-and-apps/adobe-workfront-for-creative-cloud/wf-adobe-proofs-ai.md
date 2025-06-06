---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Charger des épreuves depuis Illustrator
description: Vous pouvez charger vos panoramas d’art en tant que documents pour un examen et une approbation rapides ou simplement les stocker dans Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: e98f27d4-7c07-44cc-8df5-e04472ec946e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 92%

---

# Charger des épreuves à partir d’[!DNL Illustrator]

Vous pouvez charger vos panoramas d’art en tant qu’épreuves directement sur [!DNL Adobe Workfront] pour un examen et une approbation approfondis.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Formule actuelle : [!UICONTROL Pro] ou version ultérieure</p> <p>ou</p> <p>Formule héritée : [!UICONTROL Premium]</p> <p>Pour plus d’informations sur l’accès en relecture avec les différentes formules, voir .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>Formule actuelle : [!UICONTROL Work] ou [!UICONTROL Proof]</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’une licence [!DNL Adobe Creative Cloud] en plus d’une licence [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>[!UICONTROL Manager] ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Modifier l’accès aux [!UICONTROL Documents]</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, consultez la section <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, rôle ou profil d’autorisation d’épreuve dont vous disposez, contactez l’administration [!DNL Workfront] ou [!DNL Workfront Proof].

+++

## Conditions préalables

* Vous devez installer [!DNL Adobe Workfront for design and video] avant de pouvoir charger des épreuves à partir d’[!DNL Illustrator].

  Pour plus d’informations, voir [Installer  [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## Charger une épreuve de base

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![Retour à la liste de travail](assets/go-back-to-work-list-350x314.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger une épreuve.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![icône de document](assets/documents.png) dans la barre de navigation.
1. Cliquez sur **[!UICONTROL Nouveau fichier]** en bas du plug-in.
1. Activez le bouton (bascule) **[!UICONTROL Créer une épreuve]**.
1. (Facultatif) Saisissez un nom pour l’épreuve dans la zone de texte **[!UICONTROL Nom de l’épreuve]**.
1. Dans la section **[!UICONTROL Approbations des épreuves]**, sélectionnez **[!UICONTROL De base]**.
1. (Facultatif) Ajoutez des approbateurs et approbatrices.
1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

   ![Ajouter un commentaire](assets/add-comment.png)

1. Choisissez le **[!UICONTROL type de ressource]** dans le menu déroulant.

1. (Facultatif) Sélectionnez **[!UICONTROL Ajouter un fichier externe]** pour ajouter un fichier à partir de votre ordinateur.
1. Cliquez sur **[!UICONTROL Charger]**, puis configurez les options d’export souhaitées en fonction du type de fichier sélectionné ci-dessus.

   ![Fichiers dans le plug-in](assets/plugin-files-350x307.png)\
   Le document apparaît dans la zone [!UICONTROL Documents] du plug-in et de l’application de bureau.


## Charger une épreuve automatisée

1. Cliquez sur l’icône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![Retour à la liste de travail](assets/go-back-to-work-list-350x314.png)

1. Accédez à l’élément de travail dans lequel vous souhaitez charger une épreuve.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![icône de document](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouveau fichier]** en bas du plug-in.
1. Activez le bouton (bascule) **[!UICONTROL Créer une épreuve]**.
1. (Facultatif) Saisissez un nom pour l’épreuve dans la zone de texte **[!UICONTROL Nom de l’épreuve]**.
1. Dans la section **[!UICONTROL Approbations des épreuves]**, sélectionnez **[!UICONTROL Automatisé]**.
1. (Facultatif) Dans la zone **[!UICONTROL Modèle de workflow]** saisissez le nom d’un modèle de workflow d’épreuve.

{{adjust-proof-settings}}

>[!NOTE]
>
> S’il existe des champs requis vides dans le modèle de workflow, les paramètres d’épreuve automatisés s’ouvrent automatiquement et vous devez renseigner ces champs pour charger l’épreuve.


1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.

   ![Ajouter un commentaire à l’approbation automatisée](assets/add-comment-automated-approval.png)

1. Choisissez le **[!UICONTROL type de ressource]** dans le menu déroulant.
1. (Facultatif) Sélectionnez **[!UICONTROL Ajouter un fichier externe]** pour ajouter un fichier à partir de votre ordinateur.
1. Cliquez sur **[!UICONTROL Charger]**, puis configurez les options d’export souhaitées en fonction du type de ressource sélectionné ci-dessus.
Le document apparaît dans la section [!UICONTROL Documents] du plug-in et de l’application de bureau.

## Charger une nouvelle version d’épreuve

Vous pouvez charger une nouvelle version d’une épreuve. Le plug-in conserve en mémoire le workflow de relecture défini sur la version précédente, mais vous pouvez modifier ce paramètre si vous le souhaitez.

1. Cliquez sur l’cône **[!UICONTROL Menu]** dans le coin supérieur droit, puis sélectionnez **[!UICONTROL Liste de travail]**. Vous pouvez également utiliser le menu pour accéder aux objets parents.

   ![Retour à la liste de travail](assets/go-back-to-work-list-350x314.png)

1. Accédez à l’élément de travail dans lequel vous devez charger un document.
1. Cliquez sur l’icône **[!UICONTROL Document]** ![icône de document](assets/documents.png) dans la barre de navigation.

1. Cliquez sur **[!UICONTROL Nouvelle version]** en bas du plug-in.
1. Activez l’option **[!UICONTROL Créer une épreuve]**.

1. Dans la section *[!UICONTROL *Approbation d’épreuve]&#x200B;**, choisissez &#x200B;** [!UICONTROL De base] **&#x200B; ou &#x200B;** [!UICONTROL Automatique]**.

1. Ajoutez des **[!UICONTROL Réviseurs ou réviseuses]** ou un **[!UICONTROL Modèle de workflow]** en fonction du type d’approbation que vous avez sélectionné lors de l’étape 7.

1. (Facultatif) Saisissez un commentaire dans la zone **[!UICONTROL Mises à jour]**.
1. Choisissez le **[!UICONTROL Type de ressource]** dans le menu déroulant.
1. Cliquez sur **[!UICONTROL Charger]**, puis configurez les options d’export souhaitées en fonction du type de ressource sélectionné ci-dessus.
Le document apparaît dans la zone [!UICONTROL Documents] du plug-in et de l’application de bureau.
