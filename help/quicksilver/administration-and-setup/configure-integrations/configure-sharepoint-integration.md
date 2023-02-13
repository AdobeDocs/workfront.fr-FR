---
title: Configurez la variable [!DNL SharePoint] integration
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Vous pouvez intégrer des [!DNL Workfront] avec [!DNL SharePoint] En ligne, offrant aux utilisateurs la possibilité de naviguer, de créer des liens et d’ajouter des [!DNL SharePoint] documents dans Workfront. La fonctionnalité fournie est similaire à celle d’autres [!DNL Workfront] intégrations, telles que Google Drive, Box et Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2515'
ht-degree: 0%

---

# Configuration de l’héritage [!DNL SharePoint] integration

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>La nouvelle [!DNL SharePoint] l’intégration a été publiée en production avec la version 22.3 (juillet 2022). Bien que vos utilisateurs puissent toujours accéder aux documents liés par l’intermédiaire de l’ancien [!DNL SharePoint] intégration, ils doivent utiliser la nouvelle [!DNL SharePoint] pour lier des documents à partir de SharePoint.
>
>* La nouvelle intégration de SharePoint ne nécessite pas d’être configurée par un administrateur et peut être configurée par des utilisateurs individuels. Toutefois, pour garantir une transition en douceur vers la nouvelle intégration de SharePoint, un administrateur Workfront doit apporter quelques modifications mineures aux paramètres dans la zone Configuration de Workfront .
   >
   >    Pour plus d’informations et d’instructions, voir [Configuration de l’intégration SharePoint héritée pour un accès continu aux documents](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) dans cet article.
>    
>* Nous recommandons aux utilisateurs de lier des documents qui sont actuellement liés par l’intermédiaire de l’ancien [!DNL SharePoint] par le biais de la nouvelle intégration.
   >    
   >    Pour plus d’informations sur la liaison de documents, voir [Liaison de documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


Vous pouvez intégrer des [!DNL Workfront] avec [!DNL SharePoint Online], ce qui permet aux utilisateurs de naviguer, de créer des liens et d’ajouter des [!DNL SharePoint] documents dans Workfront. La fonctionnalité fournie est similaire à celle d’autres [!DNL Workfront] intégrations, telles que [!DNL Google Drive], [!DNL Box], et [!DNL Dropbox].

Cette intégration n’est compatible qu’avec [!DNL SharePoint Online]. Instances on-premise de [!DNL SharePoint] ne sont pas prises en charge.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Vous devez disposer des autorisations ou des accès nécessaires dans [!DNL SharePoint] pour modifier ou configurer les [!DNL SharePoint].

## Lier des documents par le biais de la nouvelle intégration SharePoint

Les utilisateurs individuels peuvent lier des documents par le biais de la nouvelle [!DNL SharePoint] intégration. L’intégration ne nécessite pas de configuration administrateur. À la place, l’utilisateur se connecte à son [!DNL Microsoft] lors de la liaison d’un document, ce qui permet à l’intégration d’accéder aux documents disponibles dans le [!DNL SharePoint].

La première fois qu’un utilisateur connecte la variable [!DNL Workfront] [!DNL SharePoint] intégration à leur [!DNL SharePoint] , ils verront et accepteront toutes les autorisations de [!DNL Workfront] utilise lors de l’interaction avec leur [!UICONTROL SharePoint] compte . Autorisations de lecture autorisées [!DNL Workfront] pour afficher et accéder aux fichiers sur [!DNL SharePoint], et les autorisations d’écriture permettent à l’utilisateur de charger des fichiers dans [!DNL SharePoint].

Pour obtenir des instructions sur la liaison de documents par le biais de la nouvelle [!DNL SharePoint] intégration, voir [Lier un document externe à [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] l’intégration peut se connecter à une seule [!DNL SharePoint] instance. Par conséquent, un utilisateur peut configurer une intégration pour une [!DNL SharePoint], mais ne peut pas configurer une intégration sur une seconde [!DNL SharePoint], même s’ils disposent d’autorisations pour et des documents sur la deuxième [!DNL SharePoint].
>
>* Un utilisateur a accès aux mêmes sites, collections, dossiers, sous-dossiers et fichiers par l’intermédiaire du [!DNL Workfront] [!DNL SharePoint] intégration comme ils l’ont fait dans leur [!DNL SharePoint] compte .


## Configuration de l’intégration SharePoint héritée pour un accès continu aux documents

Pour vous assurer que vos utilisateurs continuent d’accéder aux documents liés à Workfront par le biais de l’intégration SharePoint héritée, vous devez reconfigurer l’accès à l’intégration SharePoint héritée et tenir le secret client SharePoint à jour.

* [Reconfiguration de l’accès à l’héritage [!DNL SharePoint] integration](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Configuration du secret client pour un accès continu à l’héritage [!DNL SharePoint] integration](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Reconfiguration de l’accès à l’héritage [!DNL SharePoint] integration

Pour vous assurer que vous pouvez accéder aux documents liés par l’intermédiaire de l’ancien [!DNL SharePoint] , tout en veillant à ce que vos utilisateurs ne puissent pas lier de nouveaux documents via cette intégration, procédez comme suit.

>[!NOTE]
>
> * L&#39;héritage [!DNL SharePoint] l’intégration est étiquetée &quot;[!DNL SharePoint].&quot;
> * La nouvelle [!DNL SharePoint] l’intégration est étiquetée &quot;[!UICONTROL [!DNL SharePoint] (API Graph)].&quot;


1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![Configuration](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Sélectionner **[!UICONTROL Documents]** dans le volet de navigation de gauche, puis sélectionnez **[!UICONTROL Fournisseurs cloud]**.
1. Assurez-vous que la variable **[!DNL SharePoint]** et **[!UICONTROL [!DNL SharePoint](API Graph)]** sont toutes les deux activées.
1. Cliquer sur **[!UICONTROL Enregistrer]**.
1. Sélectionner **[!UICONTROL Documents]** dans le volet de navigation de gauche, puis sélectionnez **[!UICONTROL [!DNL SharePoint]Intégration]**.
1. Cochez la case à gauche de la liste pour toutes les intégrations existantes, puis sélectionnez **[!UICONTROL Désactiver]**.


### Configuration du secret client pour un accès continu à l’héritage [!DNL SharePoint] integration

Votre [!DNL SharePoint] Le secret client expire une fois par an. Pour garantir un accès continu aux documents de votre héritage [!DNL SharePoint] intégration, vous devez conserver ses [!DNL SharePoint] Secret client à jour.

>[!IMPORTANT]
>
> Parce que [!DNL SharePoint] Les secrets client sont gérés par [!DNL Microsoft], les fonctionnalités et procédures secrètes du client peuvent changer en fonction des mises à jour apportées à [!DNL SharePoint] made by [!DNL Microsoft]. Toujours vérifier la variable [!DNL Microsoft] documentation pour obtenir les informations les plus récentes sur les procédures et les fonctionnalités d’ [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Générez un nouveau secret client, comme décrit dans [Remplacer un secret client arrivant à expiration dans un [!DNL SharePoint] Module complémentaire](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Copiez ce secret client vers un emplacement sécurisé.
1. Se connecter [!DNL Workfront] en tant qu’administrateur.
1. Dans Workfront, cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint]Intégration]**.
1. Cliquez sur le bouton [!DNL SharePoint] intégration que vous souhaitez mettre à jour, puis cliquez sur **[!UICONTROL Modifier]**.
1. Saisissez le nouveau secret client dans le **[!UICONTROL Secret du client]** champ .
1. Cliquer sur **[!UICONTROL Enregistrer]**.



## Instructions de configuration de l’intégration SharePoint héritée

>[!IMPORTANT]
>
>Cette intégration a été abandonnée. Les instructions ici ne sont fournies qu’à titre indicatif et seront supprimées dans un avenir proche.


Workfront se connecte à [!DNL SharePoint] En ligne à l’aide d’OAuth 2.0, une norme utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs.

Pour configurer OAuth, vous devez créer une [!DNL SharePoint] site et application de site dans [!DNL SharePoint]. Ce processus est décrit dans les sections suivantes.

Pour plus d’informations sur OAuth, voir [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Pour faciliter la copie et le collage d’informations entre [!DNL Workfront] et [!DNL SharePoint] dans ces étapes, nous vous recommandons de garder les deux applications ouvertes dans des onglets distincts.

* [Création et configuration d’une [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site)
* [Octroi d’autorisations d’écriture à l’application de site](#grant-write-permissions-to-the-site-app)
* [Créez un [!DNL Workfront] [!DNL SharePoint] instance d’intégration](#create-a-workfront-sharepoint-integration-instance)
* [Terminer votre intégration](#complete-your-integration)
* [Ajouter des documents](#add-documents)

### Création et configuration d’une [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

Pour [!DNL Workfront] pour vous authentifier auprès de [!DNL SharePoint], [!DNL Workfront] peut utiliser un site maître sur lequel les utilisateurs disposent de la variable [!UICONTROL Contrôle complet] niveau d’autorisation ou des autorisations de gestion spécifiques. Ce site maître agit comme un point d’entrée d’authentification pour [!DNL Workfront].

Pour créer et configurer un [!DNL SharePoint] Site :

1. (Facultatif) Si vous ne souhaitez pas utiliser le site racine de votre entreprise, vous pouvez créer un site maître dans [!DNL SharePoint].

   Pour obtenir des instructions, consultez [Création d’un site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) dans le [!DNL Microsoft] Documentation.

   * Sélectionnez la **[!UICONTROL Site de l’équipe]** lors de la création du site.

1. (Conditionnel) Si vous avez créé un site à l’étape 1, accédez au site que vous venez de créer.

   Ou

   Si vous n’avez pas créé de site à l’étape 1, accédez au site racine de votre entreprise.

1. Ajouter `/_layouts/15/appregnew.aspx` à la fin de l’URL dans la barre de recherche située en haut de la fenêtre du navigateur.
1. Configurez les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL ID client]</p> </td> 
      <td> <p>Cliquez sur <strong>[!UICONTROL Générer]</strong> pour générer un identifiant client. Copiez cet ID vers un emplacement sécurisé. Vous l’utiliserez ultérieurement lorsque vous configurerez la variable [!DNL SharePoint] intégration dans [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Cliquez sur <strong>[!UICONTROL Générer]</strong> pour générer un secret client. Copiez ce secret vers un emplacement sécurisé. Vous l’utiliserez ultérieurement lorsque vous configurerez la variable [!DNL SharePoint] intégration dans [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Titre</p> </td> 
      <td> <p>Saisissez un titre, tel que [!DNL Workfront] Application de site. Les utilisateurs voient ce titre lors de l’ajout de documents.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Domaine de l’application]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Créer]**
1. Passez à la [Octroi d’autorisations d’écriture à l’application de site](#grant-write-permissions-to-the-site-app).

### Octroi d’autorisations d’écriture à l’application de site  {#grant-write-permissions-to-the-site-app}

À ce stade, vous avez créé une application de site et vous l’avez enregistrée dans [!DNL Workfront]. Cette application de site est également connue sous le nom d’entité d’application dans [!DNL SharePoint]. Il réside dans votre client. Les nouvelles applications de site n’ont pas automatiquement accès aux collections de site dans le client. Pour chaque collection de sites, des autorisations doivent être explicitement accordées. Les étapes ci-dessous vous montrent comment accorder une autorisation en écriture à la nouvelle application de site en tant que collection de sites. Répétez ces étapes pour chacune des collections de sites que vous avez ajoutées sous [!UICONTROL Collections de sites visibles] dans les étapes ci-dessus.

Cette application de site doit avoir [!UICONTROL Write] autorisation d’accès à toutes les collections de sites auxquelles les utilisateurs doivent accéder via [!DNL Workfront].

1. Ajoutez &quot;/_layouts/15/appinv.aspx&quot; à l’URL dans [!DNL Sharepoint].

   **Exemple:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configurez les champs suivants

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID d’application]</td> 
      <td> <p>Ajoutez l’ID client que vous avez créé dans <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Création et configuration d’une [!DNL SharePoint] site </a>et cliquez sur <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL Domaine de l’application] / [!UICONTROL URL de redirection]</p> </td> 
      <td> <p>Ces informations sont automatiquement renseignées lorsque vous cliquez sur [!UICONTROL Recherche].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Demande d’autorisation XML]</td> 
      <td> <p>Copiez le code XML suivant dans le champ [!UICONTROL Permission Request XML]. Assurez-vous qu'il est ajouté exactement comme indiqué sans espaces supplémentaires, etc. afin d’éviter les erreurs.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Cliquez sur **[!UICONTROL Créer]**.
1. Dans la boîte de dialogue qui s’affiche, cliquez sur **[!UICONTROL Approuvez-le]**.
1. Vérifiez que l’application de site a accès à la collection de sites en cliquant sur le **[!UICONTROL Autorisations de l’application de collection de sites]** lien dans [!UICONTROL Paramètres du site].
1. Répétez les étapes ci-dessus pour les autres collections de site, puis continuez avec [Créez un [!DNL Workfront] [!DNL SharePoint] instance d’intégration](#create-a-workfront-sharepoint-integration-instance).

### Créez un [!DNL Workfront] [!DNL SharePoint] instance d’intégration {#create-a-workfront-sharepoint-integration-instance}

Lorsque vous avez créé une application de site dans [!DNL SharePoint], vous pouvez désormais copier les informations de l’application de site dans [!DNL Workfront]. L’application de site est une entité d’application qui sert de passerelle par laquelle les demandes OAuth sont envoyées pour accéder aux documents au sein des collections de site.

1. Se connecter [!DNL Workfront] en tant qu’administrateur.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint]Intégration]**.
1. Cliquez sur **[!UICONTROL Ajouter[!DNL SharePoint]]**.
1. Configurez les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Saisissez un nom pour le champ [!DNL SharePoint] intégration. Les utilisateurs voient ce nom lorsqu’ils cliquent sur [!UICONTROL Ajouter] &gt; [!UICONTROL À partir de] 'nom de l’intégration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Instance de l’hôte</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Cela fait référence au site de Principal que les utilisateurs utiliseront pour s’authentifier. Il est probablement identique au domaine [!UICONTROL [!DNL SharePoint] Instance de l’hôte].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Les collections de sites ne sont utilisées que dans les [!DNL SharePoint] Intégration.
       <ul> 
        <li> <p><b>Si vous utilisez le site racine de votre entreprise</b><b>:</b> </p> <p>Entrée <code>/</code></p> </li> 
        <li> <p><b>Si vous utilisez un site maître et des sous-sites :</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] ne recommande plus l’utilisation de sous-sites.</p> <p>Saisissez la racine URL de la collection de sites que vous avez créée dans la section ci-dessus.</p> <p>Il s’agit de la section de l’URL située après .com.</p> <p>Exemple : pour l’URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, le tronc serait <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] ID client]</td> 
      <td>Saisissez l’ID client que vous avez généré dans <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Création et configuration d’une [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client secret]</td> 
      <td>Entrez le secret client que vous avez généré dans <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Création et configuration d’une [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Collections de sites visibles]</td> 
      <td> <b>Important</b> Les collections de sites ne sont utilisées que dans les [!DNL SharePoint] intégration.
       <ul> 
        <li> <p><b> Si vous utilisez le site racine de votre entreprise</b><b>:</b> </p> <p>Entrée <code>/</code></p> </li> 
        <li> <p><b>Si vous utilisez un site maître et des sous-sites :</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] ne recommande plus l’utilisation de sous-sites.</p> <p>Pour chaque sous-site que vous souhaitez ajouter à votre [!DNL SharePoint] intégration, saisissez la racine du sous-site.</p> <p>Exemple : pour l’URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, le tronc serait <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>Si vous souhaitez tester uniquement votre configuration (aucun sous-site), saisissez la racine du site maître. </p> <p>Exemple : pour l’URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, le tronc serait <code>/sites/mysite</code>.</p> <p>Lorsque vous avez testé votre configuration, comme décrit dans <a href="#complete-your-integration" class="MCXref xref">Terminer votre intégration</a>, vous devez supprimer le site maître et accéder aux sous-sites.</p> 
          <ol> 
           <li value="1">Cliquez sur le bouton <strong>[!UICONTROL Menu principal]</strong> icon <img src="assets/main-menu-icon.png"> dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur <strong>[!UICONTROL Configuration]</strong> <img src="assets/gear-icon-settings.png">.<li><p>Dans le panneau de gauche, cliquez sur <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Intégration]</strong>.</p></li><li><p>Cliquez sur le bouton [!DNL SharePoint] intégration que vous configurez, puis cliquez sur Modifier.</p></li><li><p>Supprimez la racine du site maître du champ [!UICONTROL Collections de site visible] .</p></li><li><p>Pour chaque sous-site que vous souhaitez ajouter à votre [!DNL SharePoint] intégration, saisissez la racine du sous-site.</p></li><p>Exemple : pour l’URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, le tronc serait <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**
1. Passez à la [Terminer votre intégration](#complete-your-integration).

### Terminer votre intégration {#complete-your-integration}

La configuration de base est presque terminée.

1. Dans Workfront, cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Cliquez sur **[!UICONTROL Ajouter]**.
1. Cliquez sur **[!UICONTROL De]`<title of your [!DNL SharePoint] site>`** dans la liste déroulante.

   Une boîte de dialogue vous invitant à approuver ce site s’affiche.

   >[!NOTE]
   >
   >Si cette boîte de dialogue n’apparaît pas, votre [!DNL SharePoint] n’est pas configurée correctement.

1. Cliquez sur **[!UICONTROL Approuvez-le]**.

### Ajouter des documents {#add-documents}

Vous pouvez désormais ajouter des documents à partir de votre [!DNL SharePoint] site.

Pour obtenir des instructions, voir [Lier un document externe à [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Liaison de documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Si l&#39;utilisateur qui a lié un dossier n&#39;a plus accès à l&#39;application externe, [!DNL Workfront] ne peut plus accéder au contenu du dossier. Cela peut se produire, par exemple, si l’utilisateur qui avait initialement lié le dossier quitte la société. Pour garantir un accès continu, un utilisateur ayant accès au dossier doit lier à nouveau le dossier.

## Dépannage

* [Problème : Les utilisateurs rencontrent des erreurs d’authentification lors de l’utilisation de la variable [!DNL SharePoint] intégration.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problème : Comme [!DNL Workfront] utilisateur, je ne peux pas configurer une nouvelle [!DNL SharePoint] instance. Lorsque je tente de le faire, une erreur s’affiche.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problème : Lorsque vous tentez de naviguer [!DNL SharePoint] fichiers dans [!DNL Workfront], je ne vois aucune ou toutes mes collections de sites.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problème : Je ne peux pas accéder aux dossiers et documents précédemment liés dans [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problème : Les utilisateurs rencontrent des erreurs d’authentification lors de l’utilisation de la variable [!DNL SharePoint] intégration. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Solutions :

Les utilisateurs doivent être membres d’un groupe disposant des autorisations appropriées pour la variable [!DNL SharePoint] site.

Utilisateurs avec [!UICONTROL Contrôle complet] disposer de toutes les autorisations nécessaires pour [!DNL SharePoint] intégration. Si vous ne souhaitez pas accorder l’accès Contrôle complet à vos utilisateurs, vous devez accorder les autorisations suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Peuvent afficher, ajouter, mettre à jour, supprimer, approuver et personnaliser</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Edit]</p> </td> 
   <td> <p>peut ajouter, modifier et supprimer des listes ; peut afficher, ajouter, mettre à jour et supprimer des éléments et des documents de liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribution]</p> </td> 
   <td> <p>Peuvent afficher, ajouter, mettre à jour et supprimer des éléments et des documents de liste</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Vue uniquement]</p> </td> 
   <td> <p>Peut afficher des pages, des éléments de liste et des documents (les types de document avec des gestionnaires de fichiers côté serveur peuvent être affichés dans le navigateur, mais pas téléchargés).</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur la création et la modification des niveaux d’autorisation, voir [Comment créer et modifier des niveaux d’autorisation](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) dans la documentation de Microsoft.

### Problème : Comme [!DNL Workfront] utilisateur, je ne peux pas configurer une nouvelle [!DNL SharePoint] instance. Lorsque je tente de le faire, une erreur s’affiche. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions :

Cela peut être dû à un certain nombre d’éléments, provenant de l’une ou l’autre des [!DNL Workfront] ou [!DNL SharePoint]Configuration de . Vérifiez que :

* L’identifiant du client, le secret client, l’URL de retour et d’autres champs de configuration sont correctement mappés entre la variable [!DNL Workfront] [!DNL SharePoint] Instance d’intégration et [!DNL SharePoint] Application de site.
* L’utilisateur a [!UICONTROL Contrôle complet] autorisation d’accès à la collection de sites utilisée pour l’authentification.
* L’application de site est répertoriée sous [!UICONTROL Autorisations des applications sur site] pour le [!UICONTROL Collection de sites] utilisé pour l’authentification.

### Problème : Lorsque vous tentez de naviguer [!DNL SharePoint] fichiers dans [!DNL Workfront], je ne vois aucune ou toutes mes collections de sites. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Solutions :

Pour afficher une collection de sites dans [!DNL Workfront], les conditions suivantes doivent être remplies :

* La collection de sites doit être enregistrée dans la variable [!DNL Workfront] [!DNL SharePoint] Instance d’intégration.

   Pour vérifier cela dans [!DNL Workfront]:

   1. Accédez à [!UICONTROL Configuration] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Intégration].
   1. Modifiez la variable [!DNL SharePoint] Informations sur l’instance d’intégration.
   1. Vérifiez que la collection de sites est répertoriée sous [!UICONTROL Collections de sites visibles].

* L’utilisateur doit avoir accès à la collection de sites en mode [!DNL SharePoint].
* Pour vérifier cela dans [!DNL SharePoint], accédez à [!DNL SharePoint], puis ouvrez la collection de sites > [!UICONTROL Paramètres] > [!UICONTROL Autorisations du site].
* Le [!DNL SharePoint] L’application de site doit avoir accès à la collection de sites.

   Pour vérifier cela dans [!DNL SharePoint]:

   1. Accédez à la collection de sites > [!UICONTROL Paramètres] > [!UICONTROL Autorisations des applications sur le site].
   1. Assurez-vous que la variable [!UICONTROL Application de site] utilisé par [!DNL Workfront] est répertorié ici.
   1. (Conditionnel) Si l’application de site n’est pas répertoriée, ajoutez-la à la collection de sites à l’aide de _layouts/15/appinv.aspx.

      Pour plus d’informations sur l’ajout de la collection de sites, voir Octroi d’autorisations d’écriture à l’application de site.

### Problème : Je ne peux pas accéder aux dossiers et documents précédemment liés dans [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Solution :

Si l’utilisateur qui a lié une [!DNL SharePoint] ne peut plus s’authentifier, [!DNL Workfront] ne peut plus accéder au contenu du dossier. Cela peut se produire, par exemple, si l’utilisateur qui avait initialement lié le dossier quitte la société.

Pour garantir un accès continu, un utilisateur ayant accès au dossier doit lier à nouveau le dossier.

Pour plus d’informations sur la liaison de dossiers à partir de fournisseurs externes, voir [Liaison de documents à partir d’applications externes](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problème : Une erreur &quot;404 not found&quot; s’affiche lorsque vous essayez d’ajouter un document à partir de [!DNL Sharepoint]

#### Solution :

Cette erreur peut se produire si l’un des sites configurés dans la variable [!UICONTROL Collections de sites visibles] La liste a été supprimée dans SharePoint. Vérifiez les [!UICONTROL Collections de sites visibles] répertorie tous les sites qui ont été supprimés dans SharePoint.
