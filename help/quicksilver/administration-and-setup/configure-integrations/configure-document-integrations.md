---
title: Configurer les intégrations de documents
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez configurer les intégrations de documents pour gérer les documents dans Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 99%

---

# Configurer les intégrations de documents

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

En tant qu’ administrateur ou administratrice [!DNL Adobe Workfront], vous pouvez configurer les intégrations de documents pour gérer les documents dans [!UICONTROL Workfront]. Vous pouvez également configurer [!UICONTROL Workfront] afin que les documents soient stockés uniquement dans les applications de services liés aux docuements et non dans [!UICONTROL Workfront]. Pour plus d’informations, voir [Mettre à jour et lier un document à partir de [!UICONTROL Workfront] vers un fournisseur cloud externe](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) dans [Lier des documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Pour permettre une communication ouverte entre [!DNL Workfront Proof] et les serveurs [!DNL Workfront], vous devrez peut-être ajouter certaines adresses IP à votre liste autorisée. Pour plus d’informations, voir [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
       <p>ou</p>
       <p>Actuelle : [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Intégrations prises en charge

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Vous pouvez configurer les intégrations suivantes pour la gestion des documents :

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  La liaison d’épreuves à partir de [!DNL Workfront Proof] vous permet de rendre des épreuves créés à l’origine dans [!DNL Workfront Proof] disponibles dans [!DNL Workfront]. Pour les formules actuelles, une formule [!UICONTROL Pro] [!DNL Workfront] ou supérieure est nécessaire pour utiliser cette fonctionnalité. Pour les nouvelles formules, cette fonctionnalité est disponible avec toutes les formules. Pour plus d’informations sur les différentes formules disponibles, voir [Formules Workfront](https://www.workfront.com/plans?lang=fr).

* [!DNL Microsoft SharePoint]

  Pour plus d’informations sur l’intégration à [!DNL SharePoint], voir [Configurer l’intégration [!DNL SharePoint] ](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Fournisseurs de documents cloud tiers :

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

     <!--Quip-->

  >[!TIP]
  >
  >Vous pouvez relire et approuver les documents liés depuis un fournisseur cloud externe de la même manière que vous testez et approuvez les documents chargés directement dans [!DNL Workfront].

* Autres fournisseurs de documents (par le biais d’intégrations de documents personnalisées).

  Pour les formules actuelles, une formule [!UICONTROL Pro] [!DNL Workfront] ou supérieure est nécessaire pour utiliser cette fonctionnalité. Pour les nouvelles formules, cette fonctionnalité est disponible avec toutes les formules. Pour plus d’informations sur les différentes formules disponibles, voir [Formules Workfront](https://www.workfront.com/plans?lang=fr).

En outre, vous pouvez améliorer votre expérience de document [!DNL Workfront] avec un système de gestion des ressources numériques (DAM) natif ou avec des intégrations de gestion des ressources numériques tierces. L’équipe d’aministration doit activer ces fonctionnalités pour que les personnes puissent lier le service à leur compte [!DNL Workfront]. Pour plus d’informations sur la gestion des ressources numériques Workfront, voir [Gérer des documents avec  [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configurer des intégrations pour gérer des documents

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Fournisseurs cloud].**

1. (Facultatif) Pour stocker des documents dans une application de services liés aux documents et non dans [!DNL Workfront], sélectionnez **[!UICONTROL Empêcher les utilisateurs et utilisatrices de stocker des documents dans [!DNL Workfront]].**

1. Sélectionnez les intégrations à activer.
1. Cliquer sur **[!UICONTROL Enregistrer]**.

Si vous configurez des intégrations avec [!DNL Workfront DAM], vous pouvez activer [!DNL Workfront] pour inclure des métadonnées avec des documents. Pour plus d’informations sur le mappage des métadonnées, voir [Configurer le mappage des métadonnées](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurer les intégrations de documents personnalisées

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Une intégration de document personnalisée permet aux utilisateurs et utilisatrices [!DNL Workfront] de lier des fichiers à [!DNL Workfront] de pratiquement tous les systèmes, à condition que le système soit compatible avec [!DNL Workfront].

Pour que l’intégration personnalisée soit disponible pour les utilisateurs et utilisatrices, vous devez d’abord créer l’intégration. Pour plus d’informations sur la création d’intégrations à utiliser avec [!DNL Workfront], voir [API Document Webhooks](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Une fois l’intégration de document personnalisé créée, vous pouvez la rendre disponible pour les utilisateurs et utilisatrices de votre site.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Intégration personnalisée]**.

1. Cliquez sur **[!UICONTROL Ajouter une intégration personnalisée]**.
1. Saisissez les informations suivantes pour configurer l’intégration :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Le nom de l’intégration personnalisée. Il s’agit du nom que les utilisateurs et utilisatrices voient lors de l’utilisation de l’intégration dans Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>L’URL HTTP de base ou HTTP sécurisée pour les appels API. Par exemple, <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>La méthode d'authentification utilisée pour passer des appels API autorisés pour l’intégration personnalisée.</p> 
       <ul> 
        <li>Si vous choisissez <strong>[!UICONTROL OAuth]</strong>, passez à l’étape 5.</li> 
        <li>Si vous choisissez <strong>[!UICONTROL ApiKey]</strong>, passez à l’étape 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditionnel) Si vous avez sélectionné l’authentification **[!UICONTROL OAuth]** pour le **[!UICONTROL Type d’authentification]**, saisissez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>L’URL complète utilisée pour l’authentification de l’utilisateur ou l’utilisatrice. [!DNL Workfront] accède aux utilisateurs et utilisatrices à cette adresse dans le cadre du processus d’approvisionnement OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>L'URL d'API complète utilisée pour récupérer les jetons OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>L’identifiant du client OAuth pour cette intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Le secret du client OAuth pour cette intégration.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Parameters]</td> 
      <td> <p>Saisissez les valeurs facultatives à ajouter à la chaîne de requête de chaque appel API. Par exemple, access_type=offline.</p> <p>Pour ajouter plusieurs paramètres de demande, cliquez sur <strong>+Ajouter un paramètre de demande</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >L’URI de redirection [!DNL Workfront] qui s’affiche au bas de la page [!UICONTROL Intégration personnalisée] répertorie l’URI utilisé pour enregistrer cette intégration auprès du fournisseur de documents externe.

1. (Conditionnel) Si vous avez sélectionné l’authentification **[!UICONTROL ApiKey]** pour le **[!UICONTROL Type d’authentification]**, saisissez la clé API émise par le fournisseur de documents personnalisé.

   [!DNL Workfront] utilise cette clé API pour effectuer des appels API autorisés au fournisseur de documents.

1. Cliquez sur **[!UICONTROL Enregistrer]** pour créer l’intégration.

## Utiliser les intégrations de documents

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent utiliser [!DNL Workfront DAM], voir [Gérer des documents avec  [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent utiliser la relecture, voir [Créer des épreuves](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Pour plus d’informations sur la manière dont les utilisateurs et utilisatrices peuvent utiliser des intégrations de documents tierces après leur configuration, voir [Lier des documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurer [!DNL Workfront] pour envoyer des métadonnées à [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Lors de l’envoi d’un document de [!DNL Workfront] à [!DNL Workfront DAM], vous pouvez également envoyer des informations associées à ce document. Les informations sur le document sont mappées sur [!DNL Workfront DAM] en tant que métadonnées.

Les informations sont mappées à sens unique uniquement, de [!DNL Workfront] à [!DNL Workfront DAM], et ne sont transférées que lorsque le document est chargé sur [!DNL Workfront DAM]. Les modifications futures apportées aux champs Workfront ne mettront pas à jour les champs de métadonnées dans [!DNL Workfront DAM] une fois le document chargé.\
Vous pouvez mapper le même champ [!DNL Workfront] sur divers [!DNL Workfront DAM], mais vous ne pouvez pas utiliser le même champ [!DNL Workfront DAM] pour plusieurs champs [!DNL Workfront].

Si vous devez configurer plusieurs champs [!DNL Workfront] à exporter vers un champ [!DNL Workfront DAM], créez tout d’abord un champ personnalisé calculé dans [!DNL Workfront] pour afficher tous les champs personnalisés d’un objet. Mappez ensuite le champ [!DNL Workfront] calculé sur un champ [!DNL Workfront DAM].\
Pour plus d’informations sur les champs personnalisés calculés, voir [Ajouter des données calculées à un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Le mappage affecte tous les documents chargés par un utilisateur ou une utilisatrice de [!DNL Workfront] sur [!UICONTROL Workfront] DAM.

En tant qu’administrateur ou administratrice [!DNL Workfront], vous devez activer [!DNL Workfront DAM] dans Workfront avant de pouvoir mapper les champs du processus de mappage des métadonnées.

Pour configurer [!DNL Workfront] pour envoyer des métadonnées à [!DNL Workfront DAM] :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Mappage des métadonnées]**.

1. Dans le champ **[!UICONTROL Sélectionner le champ source pour le mappage]**, commencez à saisir le nom du champ Workfront que vous souhaitez mapper sur [!DNL Workfront DAM], puis sélectionnez-le lorsque vous le voyez dans la liste.
1. Dans le champ **[!UICONTROL Sélectionner le champ cible pour le mappage]**, sélectionnez le champ [!DNL Workfront DAM] que vous souhaitez renseigner avec les informations du champ [!DNL Workfront] sélectionné.

   >[!NOTE]
   >
   > Les métadonnées de tous les documents envoyés à [!DNL Workfront DAM] par les personnes qui disposent des droits nécessaires sont mises à jour avec la champs [!DNL Workfront] mappés ici, lors du chargement sur [!DNL Workfront DAM].

1. Cliquez sur **[!UICONTROL Ajouter un mappage]**.

1. Continuer à ajouter d’autres champs [!UICONTROL Workfront] et les champs [!DNL Workfront DAM] correspondants.

### Supprimer les champs mappés

{{step-1-to-setup}}

1. Développer **[!UICONTROL Documents]**, puis cliquez sur **[!UICONTROL Mappage de métadonnées]**.

1. Dans la liste des champs, sélectionnez les champs à supprimer du mappage de métadonnées.
1. Cliquez sur **[!UICONTROL Supprimer]**.

   Les champs sont supprimés du mappage de métadonnées et les informations qu’ils contiennent ne sont pas transférées vers [!DNL Workfront DAM] avec les documents chargés.
