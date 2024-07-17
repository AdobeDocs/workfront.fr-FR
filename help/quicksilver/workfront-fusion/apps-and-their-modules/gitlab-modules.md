---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules GitLab
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion et une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '4070'
ht-degree: 6%

---


# Modules [!UICONTROL GitLab]

Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion et une licence Adobe Workfront.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!UICONTROL GitLab], et les connecter à plusieurs applications et services tiers.

>[!NOTE]
>
>Cet article s’attend à une certaine familiarité avec la documentation de l’API et des fonctionnalités de [!DNL GitLab] en général.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connecter [!DNL GitLab] à [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. Dans un module [!DNL Workfront Fusion] [!DNL Gitlab], cliquez sur **[!UICONTROL Ajouter]** en regard du champ de connexion.
1. Configurez les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td> <p>Saisissez le nom de la connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>Saisissez l’URL de votre instance [!DNL GitLab].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access Token]</td> 
      <td><p>Saisissez votre [!UICONTROL Private Token] ou [!UICONTROL Personal Access Token].</p><p>Pour plus d’informations sur la localisation ou la création d’un jeton d’accès personnel dans [!DNL GitLab], voir "Création d’un jeton d’accès personnel" dans <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">Jetons d’accès personnel</a> dans la documentation [!DNL GitLab].</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Cliquez sur **[!UICONTROL Continuer]**.
1. Cliquez sur **[!UICONTROL Autoriser]** pour créer la connexion et revenir au module.

## Modules [!DNL GitLab] et leurs champs

Lorsque vous configurez des modules [!DNL GitLab], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL GitLab] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Déclencheurs

+++**[!UICONTROL État du build de Watch]**

Ce module de déclenchement instantané démarre un scénario lorsque l’état d’une version change.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Projet que vous souhaitez que le webhook surveille pour les modifications de l’état de création</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Regardez les commentaires commit/MR/issue/fragment]**

Ce module de déclenchement instantané lance un scénario lorsqu’un commentaire est fait sur une validation, une requête de fusion, un problème ou un extrait de code.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Le projet que vous souhaitez que le webhook consulte les commentaires</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Regarder les validations (push)]**

Ce module de déclenchement instantané démarre un scénario lorsqu’une validation est envoyée à un référentiel. Ce module ne lance pas de scénario lorsqu’une balise est envoyée.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Le projet que vous souhaitez que le webhook recherche les validations</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Commentaire du problème de contrôle]**

Ce module de déclenchement instantané démarre un scénario lorsqu’un commentaire est fait sur un problème.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Le projet que vous souhaitez que le webhook recherche les commentaires d’émission</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Problèmes de contrôle]**

Ce module [!UICONTROL déclencheur instantané] démarre un scénario lorsqu’un problème est créé ou lorsqu’un problème existant est mis à jour, fermé ou rouvert.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Projet que vous souhaitez que le webhook recherche les problèmes</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Regarder les requêtes de fusion]**

Ce module de déclenchement instantané démarre un scénario lorsque l’un des événements suivants se produit :

* Une nouvelle requête de fusion est créée.
* Une requête de fusion existante est mise à jour, fusionnée ou fermée.
* Une validation est ajoutée dans la branche source.


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Le projet que vous souhaitez que le webhook recherche les requêtes de fusion</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch merge request comments]**

Ce module de déclenchement instantané démarre un scénario lorsqu’un commentaire est fait sur une requête de fusion.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Le projet que vous souhaitez que le webhook recherche les commentaires de requête de fusion</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL État du pipeline de contrôle]**

Ce module de déclenchement instantané démarre un scénario lorsque l’état d’un pipeline change.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Projet que vous souhaitez que le webhook surveille les modifications de l’état du pipeline</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Surveiller les projets]**

Ce module de déclenchement planifié lance un scénario lorsqu’un nouveau projet est ajouté, dont l’utilisateur authentifié est membre.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitLab] à [!DNL Workfront] Fusion, reportez-vous à la section <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connexion [!DNL GitLab] à [!DNL Workfront] Fusion</a> de cet article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Nbre max. de résultats</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit surveiller pour chaque cycle d’exécution de scénario.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Surveillance des branches du référentiel]**

Ce module de déclenchement planifié lance un scénario lorsqu’une nouvelle branche est ajoutée à un référentiel.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitLab] à [!DNL Workfront] Fusion, reportez-vous à la section <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connexion [!DNL GitLab] à [!DNL Workfront] Fusion</a> de cet article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Nbre max. de résultats</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit surveiller pour chaque cycle d’exécution de scénario.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Regarder les balises du référentiel]**

Ce module de déclenchement instantané démarre un scénario lorsqu’une balise est créée ou supprimée dans un référentiel.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Projet que vous souhaitez que le webhook recherche les balises.</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Regarder les commentaires de fragment de code]**

Ce module de déclenchement instantané démarre un scénario lorsqu’un nouveau commentaire est fait sur un fragment de code.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Le projet que vous souhaitez que le webhook consulte les commentaires</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Outils de surveillance]**

Ce module de déclencheur planifié démarre un scénario lorsqu’un nouvel outil est ajouté. Lorsqu’aucun filtre n’est appliqué, le déclencheur est exécuté lorsqu’un nouveau todo en attente est ajouté.

Pour plus d’informations sur les champs, voir [Obtenir une liste de à faire](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Regardez la page wiki]**

Ce module de déclenchement instantané démarre un scénario lorsqu’une page wiki est créée ou modifiée.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Sélectionnez le webhook que vous souhaitez utiliser pour ce déclencheur ou ajoutez un nouveau webhook. </p><p>Pour ajouter un nouveau webhook, <ol><li>Cliquez sur <b>[!UICONTROL Ajouter]</b> en regard du champ [!UICONTROL webhook].</li><li>Saisissez les informations suivantes : <ul><li>Nom du webhook.</li><li>La connexion que vous souhaitez utiliser pour ce webhook</li><li>Le projet que vous souhaitez que le webhook recherche les pages wiki</li></ul></li><li>Cliquez sur <b>[!UICONTROL Enregistrer]</b> pour enregistrer le webhook et revenir au module. </td> 
   </tr> 
   </tbody> 
</table>

+++

### Actions

+++**[!UICONTROL Requête de fusion Accept]**

Ce module d’action fusionne les modifications envoyées avec la requête de fusion donnée.

Pour plus d’informations sur les champs, voir [Requête de fusion Accept](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Annuler une version]**

Ce module d’action annule un seul build d’un projet.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitLab] à [!DNL Workfront] Fusion, reportez-vous à la section <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connexion [!DNL GitLab] à [!DNL Workfront] Fusion</a> de cet article.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID de projet]</td> 
   <td> <p>Sélectionnez ou mappez le projet qui contient la version que vous souhaitez annuler.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td>Sélectionnez ou mappez la version que vous souhaitez annuler.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Fusionner le message commit]</td> 
   <td> Saisissez ou mappez un message de validation pour la fusion.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Doit supprimer la branche source]</td> 
   <td>Indiquez si vous souhaitez supprimer la branche source une fois la fusion terminée.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Fusionner lorsque la génération réussit]</td> 
   <td>Indiquez si la requête de fusion doit être fusionnée dès que la génération est terminée.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>S’il est présent, ce SHA doit correspondre à l’HEAD de la branche source. S’il ne correspond pas, la fusion échoue.</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Annuler les versions d’un pipeline]**

Ce module d’action annule les versions pour un seul pipeline.

Pour plus d’informations sur les champs, voir [Annuler les tâches d’un pipeline](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Annuler la fusion lorsque le pipeline réussit]**

Si une requête de fusion est définie pour fusionner lorsqu’un pipeline réussit, ce module d’action annule cette action.

Pour plus d’informations sur les champs, voir [Annuler la fusion lorsque le pipeline réussit](https://docs.gitlab.com/ee/api/merge_requests.html) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Cherry pick a commit]**

Ce module d’action sélectionne une validation sur une branche donnée.

Pour plus d’informations sur les champs, voir [Cherry pick a commit](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une nouvelle étiquette]**

Ce module d’action crée un nouveau libellé pour le référentiel donné.

Pour plus d’informations sur les champs, voir [Création d’une étiquette](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer un pipeline]**

Ce module d’action crée un pipeline pour le projet donné.

Pour plus d’informations sur les champs, voir [Création d’un pipeline](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une nouvelle version]**

Ce module d’action ajoute des notes de mise à jour à la balise git existante.

Pour plus d’informations sur les champs, voir [Création d’une version](https://docs.gitlab.com/ee/api/releases/#create-a-release) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une balise]**

Ce module d’action crée une balise dans le référentiel qui pointe vers la référence fournie.

Pour plus d’informations sur les champs, voir [Création d’une balise](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer un todo]**

Ce module d’action crée un outil pour l’utilisateur actuel sur le problème sélectionné. L’utilisateur actuel est l’utilisateur identifié par les informations d’identification sur la connexion utilisée pour ce module.

Pour plus d’informations sur les champs, voir [Création d’un à faire](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer un todo sur une requête de fusion]**

Ce module d’action crée un outil pour l’utilisateur actuel sur la requête de fusion sélectionnée. L’utilisateur actuel est l’utilisateur identifié par les informations d’identification sur la connexion utilisée pour ce module.

Pour plus d’informations sur les champs, voir [Création d’une tâche](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une requête de fusion]**

Ce module d’action crée une requête de fusion sur un projet.

Pour plus d’informations sur les champs, voir [Créer une requête de fusion](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer un fichier dans le référentiel]**

Ce module d’action crée un nouveau fichier dans le référentiel sélectionné.

Pour plus d’informations sur les champs, voir [Création d’un fichier dans le référentiel](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une nouvelle note de problème]**

Ce module d’action crée une note de problème pour un seul problème de projet.

Pour plus d’informations sur les champs, voir [Création d’une note de problème](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une nouvelle note de demande de fusion]**

Ce module d’action crée une note pour une seule requête de fusion.

Pour plus d’informations sur les champs, voir [Création d’une note de demande de fusion](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer un nouveau jalon]**

Ce module d’action crée un nouveau jalon pour un projet.

Pour plus d’informations sur les champs, voir [Création d’un nouveau jalon](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une note de fragment de code]**

Ce module d’action crée une nouvelle note pour un seul fragment de code. Les notes de fragment de code sont des commentaires que les utilisateurs peuvent publier dans un fragment de code.

Pour plus d’informations sur les champs, voir [Création d’une note de fragment de code](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une branche de référentiel]**

Ce module d’action crée une branche de référentiel unique.

Pour plus d’informations sur les champs, voir [Création d’une branche de référentiel](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Créer une variable de build]**

Ce module d’action crée une variable de version.

Pour plus d’informations sur les champs, voir [Création de variable](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Supprimer une requête de fusion]**

Ce module d’action est destiné uniquement aux administrateurs et aux propriétaires de projets. Elle supprime la requête de fusion en question.

Pour plus d’informations sur les champs, voir [Suppression d’une requête de fusion](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Supprimer le fichier existant dans le référentiel]**

Ce module d’action supprime un fichier existant du référentiel.

Pour plus d’informations sur les champs, voir [Suppression d’un fichier existant dans le référentiel](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Supprimer la branche de référentiel]**

Ce module d’action supprime une branche du référentiel.

Pour plus d’informations sur les champs, voir [Suppression de la branche de référentiel](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Modifier le problème]**

Ce module d’action met à jour un problème de projet existant. Cet appel est également utilisé pour marquer un problème comme étant fermé.

Pour plus d’informations sur les champs, voir [Modification du problème](https://docs.gitlab.com/ee/api/issues.html#edit-issue) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Modifier le jalon]**
Ce module d’action met à jour un jalon de projet existant.

Pour plus d’informations sur les champs, voir [Modifier le jalon](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Effacer un build]**

Ce module d’action supprime une version d’un projet (supprime les artefacts de tâche et le journal de la tâche).

Pour plus d’informations sur les champs, voir [Effacer une tâche](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir une liste des tous]**

Ce module de recherche récupère une liste d’éléments à faire.

Pour plus d’informations sur les champs, voir [Obtenir une liste de à faire](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir un seul build]**

Ce module d’action récupère une seule tâche d’un projet.

Pour plus d’informations sur les champs, voir [Obtenir une seule tâche](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir une balise de référentiel unique]**

Ce module d’action récupère une balise de référentiel spécifique déterminée par son nom.

Pour plus d’informations sur les champs, voir [Obtenir une balise de référentiel unique](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir un déploiement spécifique]**

Ce module d’action récupère un déploiement spécifique.

Pour plus d’informations sur les champs, voir [Obtenir un déploiement spécifique](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir tous les problèmes affectés à un seul jalon]**

Ce module de recherche récupère tous les problèmes affectés à un seul jalon de projet.

Pour plus d’informations sur les champs, voir [Obtenir tous les problèmes affectés à un seul jalon](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir un fichier du référentiel]**

Ce module d’action récupère des informations sur un fichier dans le référentiel, comme le nom, la taille ou le contenu.

Pour plus d’informations sur les champs, voir [Obtenir un fichier du référentiel](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir les utilisateurs de projet]**

Ce module de recherche récupère les utilisateurs du projet.

Pour plus d’informations sur les champs, voir [Obtention des utilisateurs de projet](https://docs.gitlab.com/ee/api/projects.html#get-project-users) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir un seul problème]**

Ce module d’action récupère les détails des problèmes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour créer une connexion, voir <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connecter [!DNL GitLab] à Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td> <p>Sélectionnez le projet qui contient le problème dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de problème]</td> 
   <td> <p>Saisissez ou mappez le nom du problème dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Obtenir la note de problème unique]**

Ce module d’action récupère une seule note pour un problème de projet spécifique.

Pour plus d’informations sur les champs, voir [Obtenir une seule note de problème](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir une requête de fusion unique]**

Ce module d’action récupère des informations sur une seule requête de fusion.

Pour plus d’informations sur les champs, voir [Obtenir une requête de fusion unique](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir les modifications de requête de fusion unique]**

Ce module de recherche récupère des informations sur la requête de fusion, y compris ses fichiers et modifications.

Pour plus d’informations sur les champs, voir [Obtenir les modifications de requête de fusion unique](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir des validations de requête de fusion unique]**

Ce module d’action récupère une liste de validations de requête de fusion.

Pour plus d’informations sur les champs, voir [Obtenir les validations de requête de fusion unique](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir la note de demande de fusion unique]**

Ce module d’action renvoie une seule note pour une requête de fusion donnée.

Pour plus d’informations sur les champs, voir [Obtenir une note de demande de fusion unique](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir un jalon]**

Ce module d’action récupère les détails du jalon.

Pour plus d’informations sur les champs, voir [Obtenir un seul jalon](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir un seul projet]**

Ce module d’action récupère les détails du projet.

Pour plus d’informations sur les champs, voir [Obtenir un seul projet](https://docs.gitlab.com/ee/api/projects.html#get-single-project) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir la branche de référentiel unique]**

Ce module d’action récupère les détails de la branche de référentiel.

Pour plus d’informations sur les champs, voir [Obtenir une branche de référentiel unique](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir la note de fragment de code]**

Ce module récupère une seule note pour un extrait de code donné.

Pour plus d’informations sur les champs, voir [Obtenir une seule note de fragment de code](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir les commentaires d’une validation]**

Ce module de recherche récupère les commentaires d’une validation dans un projet.

Pour plus d’informations sur les champs, voir [Obtenir les commentaires d’une validation](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtention de la comparaison d’une validation]**

Ce module d’action récupère la comparaison d’une validation dans un projet.

Pour plus d’informations sur les champs, voir [Obtention de la comparaison d’une validation](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Conserver les artefacts]**

Empêche la suppression des artefacts lorsque l’expiration est définie.

Pour plus d’informations sur les champs, voir [Conserver les artefacts](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Lister toutes les notes de requête de fusion]**

Ce module de recherche récupère une liste de toutes les notes pour une seule requête de fusion.

Pour plus d’informations sur les champs, voir [Liste de toutes les notes de requête de fusion](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Répertorier toutes les notes de fragment de code]**

Ce module obtient une liste de toutes les notes pour un seul fragment de code. Les notes de fragment de code sont des commentaires que les utilisateurs peuvent publier dans un fragment de code.

Pour plus d’informations sur les champs, voir [??](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Lister les builds de validation]**

Ce module de recherche renvoie une liste de versions pour une validation spécifique dans un projet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour créer une connexion, voir <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connecter [!DNL GitLab] à Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet]</td> 
   <td> <p>Sélectionnez le projet contenant la validation pour laquelle vous souhaitez répertorier les versions.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scope]</td> 
   <td> Pour limiter la recherche à créer avec un état spécifique, sélectionnez l’état. Si ce champ est vide, toutes les versions de la validation sont renvoyées.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Problèmes de liste]**

Ce module de recherche renvoie tous les problèmes selon les paramètres de filtre spécifiés.

Pour plus d’informations sur les champs, voir [Problèmes de liste](https://docs.gitlab.com/ee/api/issues.html#list-issues) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des problèmes qui se ferment lors de la fusion]**

Ce module de recherche récupère tous les problèmes qui seraient fermés en fusionnant la requête de fusion fournie.

Pour plus d’informations sur les champs, voir [Problèmes de liste qui se fermeront lors de la fusion](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Étiquettes de liste]**

Ce module de recherche récupère tous les libellés du projet.

Pour plus d’informations sur les champs, voir [Étiquettes de liste](https://docs.gitlab.com/ee/api/labels.html#list-labels) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Lister des requêtes de fusion]**

Ce module de recherche récupère toutes les requêtes de fusion selon les paramètres de filtre.

Pour plus d’informations sur les champs, voir [Requêtes de fusion de liste](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des projets détenus]**

Ce module de recherche récupère les projets dans lesquels l’utilisateur authentifié est défini comme propriétaire.

Pour plus d’informations sur les champs, voir [Liste des projets d’utilisateurs](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des versions de projet]**

Ce module de recherche récupère une liste de versions dans un projet.

Pour plus d’informations sur les champs, voir [Liste des tâches de projet](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des déploiements de projet]**

Ce module de recherche récupère une liste de déploiements dans un projet.

Pour plus d’informations sur les champs, voir [Liste des déploiements de projet](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des notes de problème de projet]**

Ce module de recherche récupère une liste de toutes les notes pour un seul problème.

Pour plus d’informations sur les champs, voir [Liste des notes de problème de projet](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des problèmes de projet]**

Ce module de recherche renvoie tous les problèmes d’un projet spécifié.

Pour plus d’informations sur les champs, voir [Liste des problèmes de projet](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des jalons du projet]**

Ce module de recherche récupère tous les jalons du projet.

Pour plus d’informations sur les champs, voir [Lister les jalons du projet](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Lister les pipelines de projet]**

Ce module de recherche récupère tous les pipelines pour le projet.

Pour plus d’informations sur les champs, voir [Liste des pipelines de projet](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Lister les balises du référentiel de projet]**

Ce module de recherche récupère une liste de balises de référentiel d’un projet, triées par nom dans l’ordre alphabétique inverse.

Pour plus d’informations sur les champs, voir [Liste des balises du référentiel de projet](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des variables de projet]**

Ce module de recherche récupère une liste des variables d’un projet.

Pour plus d’informations sur les champs, voir [Liste des variables de projet](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Liste des projets]**

Ce module de recherche récupère tous les projets dont l’utilisateur authentifié est membre.

Pour plus d&#39;informations sur les champs, voir [Liste de tous les projets](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Répertorier les branches du référentiel]**

Ce module recherche des branches de référentiel par terme de recherche.

Pour plus d’informations sur les champs, voir [Répertorier les branches du référentiel](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Lister des validations de référentiel]**

Ce module de recherche récupère une liste de validations de référentiel dans un projet.

Pour plus d’informations sur les champs, reportez-vous à la section [Liste des validations de référentiel](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) de la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Répertorier les contributeurs de référentiel]**

Ce module de recherche récupère une liste de contributeurs au référentiel.

Pour plus d’informations sur les champs, voir [Contributeurs](https://docs.gitlab.com/ee/api/repositories.html#contributors) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Arborescence de référentiel de liste]**

Ce module de recherche récupère une liste de fichiers et de répertoires de référentiel dans un projet.

Pour plus d’informations sur les champs, voir [Arborescence de référentiel de liste](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Marquer un todo comme fait]**

Ce module d’action marque un seul élément à faire en attente, indiqué par son identifiant pour l’utilisateur actuel, comme indiqué.

Pour plus d’informations sur les champs, voir [Marquer un élément comme fait](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Modifier la note de problème existante]**

Modifie une note existante d’un problème.

Pour plus d’informations sur les champs, voir [Modification d’une note de problème existante](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Modifier la note de demande de fusion existante]**

Modifie la note existante d’une requête de fusion.

Pour plus d’informations sur les champs, voir [Modification d’une note de demande de fusion existante](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Modifier la note de fragment de code existante]**

Ce module d’action modifie une note existante d’un extrait de code.

Pour plus d’informations sur les champs, voir [Modification d’une note de fragment de code existante](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Nouveau problème]**

Ce module d’action crée un problème de projet.

Pour plus d’informations sur les champs, voir [Nouveau numéro](https://www.integromat.com/en/help/app/gitlab) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Lire une version]**

Ce module d’action déclenche une action manuelle pour démarrer une tâche.

Pour plus d’informations sur les champs, voir [Lire une tâche](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Commentaire Post à valider]**

Ce module d’action ajoute un commentaire à une validation.

Pour plus d’informations sur les champs, voir [Commentaire Post à valider](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Supprimer la variable]**

Ce module d’action supprime la variable d’un projet.

Pour plus d’informations sur les champs, voir [Suppression de variable](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Retry a build]**

Ce module d’action tente une nouvelle version dans une validation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour créer une connexion, voir <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connecter [!DNL GitLab] à Workfront Fusion]</a> dans cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de projet]</td> 
   <td> <p>Sélectionnez le projet qui contient le build que vous souhaitez réessayer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td> Sélectionnez la version que vous souhaitez réessayer. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Tâches en échec dans un pipeline]**

Ce module d’action tente à nouveau les versions qui ont échoué dans un pipeline.

Pour plus d’informations sur les champs, voir [Retry jobs in a pipeline](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Obtenir une variable]**

Ce module récupère les détails de la variable spécifique d’un projet.

Pour plus d’informations sur les champs, voir [Afficher les détails de variable](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Mettre à jour une version]**

Ce module d’action met à jour une version.

Pour plus d’informations sur les champs, voir [Mise à jour d’une version](https://docs.gitlab.com/ee/api/releases/#update-a-release) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Mettre à jour la requête de fusion]**

Ce module d’action met à jour une requête de fusion existante. Vous pouvez modifier la branche cible, le titre ou même fermer la version de maintenance.

Pour plus d’informations sur les champs, voir [Mise à jour de la requête de fusion](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) dans la documentation [!DNL GitLab].

+++

+++**[!UICONTROL Mettre à jour une variable]**

Ce module d’action met à jour la variable d’un projet.

Pour plus d’informations sur les champs, voir [Mise à jour de variable](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) dans la documentation [!DNL GitLab].

+++
