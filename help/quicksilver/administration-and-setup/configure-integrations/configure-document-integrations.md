---
title: Configuration des intégrations de documents
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer les intégrations de documents pour gérer les documents dans Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 04bdfbdf1fa05082fe12c2ab239e861a6db4ee6e
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configurer les intégrations de documents

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez configurer les intégrations de documents pour gérer les documents dans [!UICONTROL Workfront]. Vous pouvez également configurer [!UICONTROL Workfront] pour que les documents soient stockés uniquement dans les applications de services documentaires et non dans [!UICONTROL Workfront]. Pour plus d’informations, voir [Mettre à jour et lier un document de [!UICONTROL Workfront] à un fournisseur de cloud externe](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) dans [Lier des documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Pour permettre une communication ouverte entre [!DNL Workfront Proof] et les serveurs [!DNL Workfront], vous devrez peut-être ajouter certaines adresses IP à votre liste d’autorisations. Pour plus d’informations, voir [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
       <p>ou</p>
       <p>Actuelle : [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être administrateur ou administratrice [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Intégrations prises en charge

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Vous pouvez configurer les intégrations suivantes pour la gestion des documents :

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  L’établissement d’un lien entre les épreuves de [!DNL Workfront Proof] vous permet de rendre accessibles à [!DNL Workfront] les épreuves qui ont été créées à l’origine à l’intérieur de [!DNL Workfront Proof]. Pour les plans actuels, un plan [!UICONTROL Pro] [!DNL Workfront] ou supérieur est nécessaire pour utiliser cette fonction. Pour les nouveaux plans, cette fonction est disponible pour tous les plans. Pour plus d’informations sur les différents plans disponibles, voir [Plans Workfront](https://www.workfront.com/plans?lang=fr).

* [!DNL Microsoft SharePoint]

  Pour plus d’informations sur l’intégration à [!DNL SharePoint], voir [Configurer l’intégration  [!DNL SharePoint] ](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Fournisseurs tiers de documents en ligne :

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]
   * Quip

  >[!TIP]
  >
  >Vous pouvez vérifier et approuver les documents liés à partir d’un fournisseur de cloud externe de la même manière que vous vérifiez et approuvez les documents téléchargés directement sur [!DNL Workfront].

* D’autres fournisseurs de documents (par le biais d’intégrations de documents personnalisés).

  Pour les plans actuels, un plan [!UICONTROL Pro] [!DNL Workfront] ou supérieur est nécessaire pour utiliser cette fonction. Pour les nouveaux plans, cette fonction est disponible pour tous les plans. Pour plus d’informations sur les différents plans disponibles, voir [Plans Workfront](https://www.workfront.com/plans?lang=fr).

En outre, vous pouvez améliorer votre expérience de document [!DNL Workfront] avec des intégrations DAM tierces. Les administrateurs doivent activer ces fonctionnalités pour que les utilisateurs puissent lier le service à leur compte [!DNL Workfront].

## Configurer les intégrations pour gérer des documents

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Fournisseurs cloud].**

1. (Facultatif) Pour stocker les documents dans une application de services documentaires et non dans [!DNL Workfront], sélectionnez **[!UICONTROL Empêcher les utilisateurs et utilisatrices de stocker des documents dans [!DNL Workfront]].**

1. Sélectionnez les intégrations à activer.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

Si vous paramétrez des intégrations avec [!DNL Workfront DAM], vous pouvez permettre à [!DNL Workfront] d’inclure des métadonnées dans les documents. Pour plus d’informations sur le mappage des métadonnées, voir [Configurer le mappage des métadonnées](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurer les intégrations de documents personnalisés

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Une intégration personnalisée des documents permet aux utilisateurs et utilisatrices de [!DNL Workfront] de lier des fichiers à [!DNL Workfront] à partir de pratiquement n’importe quel système, à condition que ce dernier soit conçu pour fonctionner avec [!DNL Workfront].

Pour mettre l’intégration personnalisée à la disposition des utilisateurs et utilisatrices, vous devez d’abord la créer. Pour plus d’informations sur la création d’intégrations à utiliser avec [!DNL Workfront], voir [API Document Webhooks](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Une fois l’intégration des documents personnalisés réalisée, vous pouvez la mettre à la disposition sur votre site.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Intégration personnalisée]**.

1. Cliquez sur **[!UICONTROL Ajouter une intégration personnalisée]**.
1. Saisissez les informations suivantes pour configurer l’intégration :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Nom de l’intégration personnalisée. Il s’agit du nom que les personnes voient lorsqu’elles utilisent l’intégration dans Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>URL HTTP de base ou HTTP sécurisé pour les appels API. Par exemple, <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>Méthode d’authentification utilisée pour passer des appels API autorisés à l’intégration personnalisée.</p> 
       <ul> 
        <li>Si vous choisissez <strong>[!UICONTROL OAuth]</strong>, passez à l’étape 5.</li> 
        <li>Si vous choisissez <strong>[!UICONTROL ApiKey]</strong>, passez à l’étape 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Le cas échéant) Si vous avez sélectionné l’authentification **[!UICONTROL OAuth]** comme **[!UICONTROL Type d’authentication]**, saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>URL complète utilisée pour l’authentification des utilisateurs et utilisatrices. [!DNL Workfront] dirige les personnes vers cette adresse dans le cadre du processus d’approvisionnement OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>L'URL d'API complète utilisée pour récupérer les jetons OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>ID du client OAuth pour cette intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Secret client OAuth pour cette intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Parameters]</td> 
      <td> <p>Saisissez des valeurs facultatives à ajouter à la chaîne de requête de chaque appel API. Par exemple, access_type=offline.</p> <p>Pour ajouter plusieurs paramètres de requête, cliquez sur <strong>+Ajouter un paramètre de requête</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >L’URI de redirection [!DNL Workfront] qui s’affiche au bas de la page [!UICONTROL Intégration personnalisée] répertorie l’URI utilisé pour enregistrer cette intégration auprès du fournisseur de documents externes.

1. (Le cas échéant) Si vous avez sélectionné l’authentification **[!UICONTROL ApiKey]** comme **[!UICONTROL Type d’authentification]**, saisissez la clé API qui a été émise par le fournisseur de documents personnalisés.

   [!DNL Workfront] utilise cette clé API pour effectuer des appels API autorisés au fournisseur de documents.

1. Cliquez sur **[!UICONTROL Enregistrer]** pour créer l’intégration.

## Utiliser les intégrations de documents

Pour plus d’informations sur la manière dont les personnes peuvent utiliser la relecture, voir [Créer des épreuves](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Pour plus d’informations sur la manière dont les personnes peuvent utiliser les intégrations de documents tierces après les avoir configurées, voir [Lier des documents provenant d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurer [!DNL Workfront] pour envoyer des métadonnées à [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Lors de l’envoi d’un document de [!DNL Workfront] à [!DNL Workfront DAM], vous pouvez également envoyer des informations associées à ce document. Les informations relatives au document sont mappées sur [!DNL Workfront DAM] sous forme de métadonnées.

Les informations ne sont mappées que dans un seul sens, de [!DNL Workfront] à [!DNL Workfront DAM], et ne sont transférées que lorsque le document est chargé sur [!DNL Workfront DAM]. Toute modification future des champs Workfront ne mettra pas à jour les champs de métadonnées dans [!DNL Workfront DAM] une fois que le document aura été chargé.\
Vous pouvez mapper le même champ [!DNL Workfront] sur plusieurs champs [!DNL Workfront DAM], mais vous ne pouvez pas utiliser le même champ [!DNL Workfront DAM] pour plusieurs champs [!DNL Workfront].

Si vous devez configurer plusieurs champs [!DNL Workfront] pour les exporter vers un champ [!DNL Workfront DAM], créez d’abord un champ personnalisé calculé dans [!DNL Workfront] pour afficher tous les champs personnalisés individuels d’un objet. Mappez ensuite le champ [!DNL Workfront] calculé sur un champ [!DNL Workfront DAM].\
Pour plus d’informations sur les champs personnalisés calculés, voir [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Le mappage affecte tous les documents chargés par n’importe quelle personne de [!DNL Workfront] à [!UICONTROL Workfront] DAM.

En tant qu’administrateur ou administratrice [!DNL Workfront], vous devez activer [!DNL Workfront DAM] dans Workfront avant de pouvoir mapper les champs pour le processus de mappage des métadonnées.

Pour configurer [!DNL Workfront] pour envoyer des métadonnées à [!DNL Workfront DAM], procédez comme suit :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

1. Dans le champ **[!UICONTROL Sélectionner le champ source pour le mappage]**, commencez à saisir le nom du champ Workfront que vous souhaitez mapper sur [!DNL Workfront DAM], puis sélectionnez-le lorsqu’il apparaît dans la liste.
1. Dans le champ **[!UICONTROL Sélectionner le champ cible pour le mappage]**, sélectionnez le champ [!DNL Workfront DAM] que vous voulez remplir avec les informations du champ [!DNL Workfront] sélectionné.

   >[!NOTE]
   >
   > Tous les documents envoyés à [!DNL Workfront DAM] par des personnes qui en ont le droit voient leurs métadonnées mises à jour avec les champs [!DNL Workfront] mappés ici, lorsqu’ils sont téléchargés sur [!DNL Workfront DAM].

1. Cliquez sur **[!UICONTROL Ajouter un mappage]**

1. Continuez à ajouter des champs [!UICONTROL Workfront] et des champs [!DNL Workfront DAM] correspondants.

### Supprimer des champs mappés

{{step-1-to-setup}}

1. Développez **[!UICONTROL Documents]**, puis cliquez sur **[!UICONTROL Mappage de métadonnées]**.

1. Dans la liste des champs, sélectionnez l’un des champs à supprimer du mappage des métadonnées.
1. Cliquez sur **[!UICONTROL Supprimer]**.

   Les champs sont supprimés du mappage de métadonnées et les informations qu’ils contiennent ne sont pas transférées à [!DNL Workfront DAM] avec les documents chargés.
