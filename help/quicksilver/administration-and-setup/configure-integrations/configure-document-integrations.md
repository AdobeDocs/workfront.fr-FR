---
title: Configuration des intégrations de documents
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer les intégrations de documents pour gérer les documents dans Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 1%

---

# Configuration des intégrations de documents

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Comme [!DNL Adobe Workfront] administrateur, vous pouvez configurer les intégrations de documents pour gérer les documents dans [!UICONTROL Workfront]. Vous pouvez également configurer [!UICONTROL Workfront] afin que les documents soient stockés uniquement dans les applications Document Services et non dans [!UICONTROL Workfront] elle-même. Pour plus d’informations, voir [Mise à jour et liaison d’un document à partir de [!UICONTROL Workfront] vers un fournisseur cloud externe](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [Liaison de documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Pour permettre une communication ouverte entre [!DNL Workfront Proof] et la variable [!DNL Workfront] serveurs, vous devrez peut-être ajouter certaines adresses IP à votre liste autorisée. Pour plus d’informations, voir [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>Nouveau : [!UICONTROL Standard]</p>
       <p>ou</p>
       <p>Actuel : formule [!UICONTROL]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Intégrations prises en charge

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Vous pouvez configurer les intégrations suivantes pour la gestion des documents :

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Liaison de BAT à partir de [!DNL Workfront Proof] vous permet d’effectuer des bons à tirer créés à l’origine dans [!DNL Workfront Proof] disponible dans [!DNL Workfront]. Pour les plans actuels, une [!UICONTROL Pro] [!DNL Workfront] Cette fonctionnalité nécessite une formule ou une valeur supérieure. Pour les nouveaux plans, cette fonctionnalité est disponible avec tous les plans. Pour plus d’informations sur les différents plans disponibles, voir [Formules Workfront](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  Pour plus d’informations sur l’intégration à [!DNL SharePoint], voir [Configurez la variable [!DNL SharePoint] integration](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Fournisseurs de documents cloud tiers :

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

     <!--Quip-->
  >[!TIP]
  >
  >Vous pouvez BAT et approuver les documents liés depuis un fournisseur cloud externe de la même manière que vous testez et approuvez les documents téléchargés directement vers [!DNL Workfront].

* Autres fournisseurs de documents (par le biais d’intégrations de documents personnalisées).

  Pour les plans actuels, une [!UICONTROL Pro] [!DNL Workfront] Cette fonctionnalité nécessite une formule ou une valeur supérieure. Pour les nouveaux plans, cette fonctionnalité est disponible avec tous les plans. Pour plus d’informations sur les différents plans disponibles, voir [Formules Workfront](https://www.workfront.com/plans).

En outre, vous pouvez améliorer votre [!DNL Workfront] Expérience de document avec un système de gestion des actifs numériques (DAM) natif ou avec des intégrations de gestion des actifs numériques tierces. Les administrateurs doivent activer ces fonctionnalités pour que les utilisateurs puissent lier le service à leurs [!DNL Workfront] compte . Pour plus d’informations sur la gestion des ressources numériques Workfront, voir [Gestion de documents avec [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configuration d’intégrations pour gérer des documents

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Fournisseurs cloud].**

1. (Facultatif) Pour stocker des documents dans une application Document Services et non dans [!DNL Workfront], sélectionnez **[!UICONTROL Empêcher les utilisateurs de stocker des documents dans [!DNL Workfront]].**

1. Sélectionnez les intégrations à activer.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

Si vous configurez des intégrations avec [!DNL Workfront DAM], vous pouvez activer [!DNL Workfront] pour inclure des métadonnées avec des documents. Pour plus d’informations sur le mappage des métadonnées, voir [Configuration du mappage des métadonnées](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configuration des intégrations de documents personnalisés

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Une intégration de document personnalisée permet [!DNL Workfront] utilisateurs pour lier des fichiers à [!DNL Workfront] de pratiquement tous les systèmes, à condition que le système soit conçu pour fonctionner avec [!DNL Workfront].

Pour que l’intégration personnalisée soit disponible pour les utilisateurs, vous devez d’abord créer l’intégration. Pour plus d’informations sur la création d’intégrations à utiliser avec [!DNL Workfront], voir [API Document Webhooks](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Une fois l’intégration de document personnalisé créée, vous pouvez la rendre disponible pour les utilisateurs de votre site.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Intégration personnalisée]**.

1. Cliquez sur **[!UICONTROL Ajout d’une intégration personnalisée]**.
1. Saisissez les informations suivantes pour configurer l’intégration :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Nom de l’intégration personnalisée. Il s’agit du nom que les utilisateurs voient lors de l’utilisation de l’intégration dans Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de l’API de base] </td> 
      <td>URL HTTP de base ou HTTP sécurisée pour les appels API. Par exemple, <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>Méthode d’authentification à utiliser lors d’appels API autorisés à l’intégration personnalisée.</p> 
       <ul> 
        <li>Si vous choisissez <strong>[!UICONTROL OAuth]</strong>, passez à l’étape 5.</li> 
        <li>Si vous choisissez <strong>[!UICONTROL ApiKey]</strong>, passez à l’étape 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditionnel) Si vous avez sélectionné **[!UICONTROL OAuth]** l’authentification pour la **[!UICONTROL Type d’authentification]**, saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>URL complète utilisée pour l’authentification de l’utilisateur. [!DNL Workfront] accède aux utilisateurs à cette adresse dans le cadre du processus d’approvisionnement OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>L'URL d'API complète utilisée pour récupérer les jetons OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID client]</td> 
      <td>Identifiant du client OAut pour cette intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Secret client OAut pour cette intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Paramètres de requête]</td> 
      <td> <p>Saisissez les valeurs facultatives à ajouter à la chaîne de requête de chaque appel API. Par exemple, access_type=offline.</p> <p>Pour ajouter plusieurs paramètres de requête, cliquez sur <strong>+Ajouter le paramètre de requête</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >La variable [!DNL Workfront] URI de redirection qui s’affiche au bas de la page [!UICONTROL Intégration personnalisée] page répertorie l’URI utilisé pour enregistrer cette intégration auprès du fournisseur de documents externe.

1. (Conditionnel) Si vous avez sélectionné **[!UICONTROL ApiKey]** l’authentification pour la **[!UICONTROL Type d’authentification]**, saisissez la clé API émise par le fournisseur de documents personnalisé.

   [!DNL Workfront] utilise cette clé d’API pour effectuer des appels d’API autorisés au fournisseur de documents.

1. Cliquez sur **[!UICONTROL Enregistrer]** pour créer l’intégration.

## Utilisation des intégrations de documents

Pour plus d’informations sur la manière dont les utilisateurs peuvent utiliser [!DNL Workfront DAM], voir [Gestion de documents avec [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Pour plus d’informations sur l’utilisation du correctif par les utilisateurs, voir [Créer un bon à tirer](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Pour plus d’informations sur l’utilisation des intégrations de documents tiers par les utilisateurs après leur configuration, voir [Liaison de documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurer [!DNL Workfront] pour envoyer des métadonnées à [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Lors de l’envoi d’un document à partir de [!DNL Workfront] to [!DNL Workfront DAM], vous pouvez également envoyer des informations associées à ce document. Les informations sur le document sont mappées sur [!DNL Workfront DAM] comme métadonnées.

Les informations sont mappées à sens unique uniquement, à partir de [!DNL Workfront] to [!DNL Workfront DAM] et il n’est transféré que lorsque le document est téléchargé vers [!DNL Workfront DAM]. Les modifications futures apportées aux champs Workfront ne mettront pas à jour les champs de métadonnées dans [!DNL Workfront DAM] une fois le document téléchargé.\
Vous pouvez mapper la même [!DNL Workfront] champ à divers [!DNL Workfront DAM] , mais vous ne pouvez pas utiliser le même [!DNL Workfront DAM] champ pour plusieurs [!DNL Workfront] des champs.

Si vous devez configurer plusieurs [!DNL Workfront] champs à exporter en un [!DNL Workfront DAM] , créez tout d’abord un champ personnalisé calculé dans [!DNL Workfront] pour afficher tous les champs personnalisés d’un objet. Associez ensuite le calcul [!DNL Workfront] champ à un [!DNL Workfront DAM] champ .\
Pour plus d’informations sur les champs personnalisés calculés, voir [Ajout de données calculées à un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Le mappage affecte tous les documents chargés par un utilisateur à partir de [!DNL Workfront] to [!UICONTROL Workfront] DAM.

Comme [!DNL Workfront] administrateur, vous devez activer [!DNL Workfront DAM] dans Workfront avant de pouvoir mapper les champs du processus de mappage des métadonnées.

Pour configurer [!DNL Workfront] pour envoyer des métadonnées à [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

1. Dans le **[!UICONTROL Sélectionner le champ source pour le mappage]** , commencez à saisir le nom du champ Workfront auquel vous souhaitez mapper l’élément [!DNL Workfront DAM], puis sélectionnez-le lorsque vous le verrez dans la liste.
1. Dans le **[!UICONTROL Sélectionner le champ cible pour le mappage]**, sélectionnez la variable [!DNL Workfront DAM] champ que vous souhaitez renseigner avec les informations dans le [!DNL Workfront] champ .

   >[!NOTE]
   >
   > Tous les documents envoyés à [!DNL Workfront DAM] par les utilisateurs qui disposent des droits nécessaires, leurs métadonnées sont mises à jour avec la variable [!DNL Workfront] champs mappés ici, lorsqu’ils sont transférés vers [!DNL Workfront DAM].

1. Cliquez sur **[!UICONTROL Ajouter un mappage]**.

1. Continuer à ajouter d’autres [!UICONTROL Workfront] champs et correspondants [!DNL Workfront DAM] des champs.

### Suppression des champs mappés

{{step-1-to-setup}}

1. Développer **[!UICONTROL Documents]**, puis cliquez sur **[!UICONTROL Mappage des métadonnées]**.

1. Dans la liste des champs, sélectionnez les champs à supprimer du mappage des métadonnées.
1. Cliquez sur **[!UICONTROL Supprimer]**.

   Les champs sont supprimés du mappage des métadonnées et les informations qu’ils contiennent ne sont pas transférées vers [!DNL Workfront DAM] avec les documents téléchargés.
