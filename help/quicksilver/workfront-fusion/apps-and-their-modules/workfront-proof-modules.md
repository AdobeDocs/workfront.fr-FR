---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Workfront Proof
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL Workfront Proof] et le connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 614fd206ea2c5fe103beb5be8f5ff99c8a45a502
workflow-type: tm+mt
source-wordcount: '3099'
ht-degree: 100%

---

# Modules [!DNL Workfront Proof]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Workfront Proof] et le connecter à plusieurs applications et services tiers.

Cette fonction est utile si vous devez exécuter des tâches qui ne sont actuellement pas prises en charge dans le cadre de la relecture dans [!DNL Workfront] ou [!DNL Workfront Proof], telles que la mise à jour des épreuves en fonction de certains événements et la recherche des destinataires d’une épreuve.

Le connecteur vers [!DNL Workfront Proof] n’est pas pris en compte dans le nombre d’applications actives disponibles pour votre entreprise. Tous les scénarios, même s’ils n’utilisent que l’application [!DNL Workfront Proof], sont comptabilisés dans le nombre total de scénarios de votre entreprise.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td>
  <td> <p>[!UICONTROL Pro] ou version supérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez la section Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connecter [!DNL Workfront Proof] à [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre compte [!DNL Workfront Proof] directement à partir d’un module [!DNL Workfront Fusion].

1. Dans n’importe quel module [!DNL Workfront Fusion], cliquez sur [!UICONTROL **Ajouter**] à côté du champ [!UICONTROL Connexion] 

2. Remplissez les champs suivants :

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>Saisir le nom de la connexion</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL connections.environmentType]</td>
                <td>Sélectionnez s’il s’agit d’un environnement de production ou d’un environnement de non-production tel que Prévisualisation ou Sandbox.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL connections.authenticationType]</td>
                <td>Sélectionnez s’il s’agit d’un compte de service ou d’un compte personnel.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Email / Username]</td>
                <td>Saisissez le nom d’utilisateur ou d’utilisatrice de votre compte [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Password]</td>
                <td>Saisissez le mot de passe de votre compte [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Tenant ID]</td>
                <td><strong>Remarque</strong> : les clientes et clients qui n’utilisent pas BYOK doivent laisser ce champ vide. <p>Saisissez l’identifiant du locataire pour ce compte. Si vous avez besoin d’aide pour trouver votre identifiant de locataire, contactez le service clientèle de Workfront.</p></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Domain Extension]</td>
                <td>Saisissez l’extension de l’URL que vous utilisez pour accéder à votre compte. <p>Exemple : <code>com</code> ou <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Production, Preview, or Custom Environment]</td>
                <td>Sélectionnez une connexion à un environnement de production, de prévisualisation ou personnalisé.</td>
            </tr>
        </tbody>
    </table>


3. Cliquez sur [!UICONTROL **Continuer**] pour enregistrer la connexion et revenir au module.

## Les modules [!DNL Workfront Proof] et leurs champs

Lorsque vous configurez les modules [!DNL Workfront Proof], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Workfront Proof] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

* [Regarder les épreuves](#watch-proofs)
* [Regarder les résumés PDF](#watch-for-pdf-summary)
* [[!UICONTROL Regarder l’activité d’une épreuve]](#watch-proof-activity)

#### [!UICONTROL Regarder les épreuves]

Ce module de déclenchement planifié exécute un scénario lorsque quelqu’un crée ou prend une décision sur une épreuve.

Le module renvoie une liste de tous les enregistrements trouvés au cours de la période spécifiée avec leur type. Il renvoie également les valeurs des champs que vous avez spécifiés. Si le module a trouvé des décisions prises sur l’épreuve, il inclut à la fois la valeur précédente et la valeur actuelle dans des champs séparés. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Cela se produit à un intervalle planifié régulier que vous spécifiez.

Vous devez disposer des autorisations nécessaires pour accéder à la ou aux épreuves dans [!DNL Workfront Proof] afin de pouvoir récupérer ces informations.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir la section  <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type d’enregistrement</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Workfront Proof] que vous voulez que le module regarde.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Sorties</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limite</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder le résumé PDF]

Ce module de déclenchement instantané exécute un scénario lorsque quelqu’un crée un résumé PDF pour une épreuve.

Un webhook est nécessaire pour ce module.

Le module renvoie tous les champs standard associés à l’épreuve, ainsi que tous les champs et valeurs personnalisés auxquels la connexion a accès. Il crée également un nouvel abonnement aux événements pour les résumés PDF et génère le contenu de l’attribut « pdf_url » envoyé dans la payload. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Vous pouvez sélectionner un webhook existant ou en créer un nouveau. Pour plus d’informations, voir <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheurs instantanés (webhooks) sur [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder l’activité d’une épreuve]

Ce module de déclenchement exécute un scénario lorsqu’une activité spécifiée se produit sur une épreuve.

Le module renvoie tous les champs standard associés à l’épreuve, ainsi que tous les champs et valeurs personnalisés auxquels la connexion a accès. Il crée également un nouvel abonnement aux événements pour les résumés PDF et génère le contenu de l’attribut `pdf_url` envoyé dans la payload. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Activity type]</td> 
   <td>Sélectionnez si vous souhaitez regarder toute nouvelle décision (y compris les changements de statut de l’[!UICONTROL proof] ou uniquement les changements de statut de l’épreuve dans son ensemble.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Créer une épreuve]](#create-proof)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Télécharger l’épreuve]](#download-proof)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Demander le résumé du PDF]](#request-pdf-summary)
* [[!UICONTROL Mettre à jour l’épreuve]](#update-proof)
* [[!UICONTROL Charger un fichier]](#upload-file)

#### [!UICONTROL Créer une épreuve]

Ce module d’action crée une nouvelle épreuve ou une nouvelle version d’une épreuve dans [!DNL Workfront Proof].

Vous spécifiez les paramètres de la nouvelle épreuve et de l’épreuve source si vous créez une nouvelle version.

Le module renvoie l’ID de la nouvelle épreuve ou de la nouvelle version de l’épreuve. Vous pouvez mapper cette information dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Type]</td> 
   <td> <p>Indiquez si vous souhaitez que l’épreuve créée ait un workflow de base ou un [!UICONTROL Automated Workflow].</p> <p>Remplissez ensuite les champs qui s’affichent pour le type d’épreuve que vous avez choisi. Par exemple, si vous avez choisi [!UICONTROL Automated Workflow], remplissez le champ <strong>[!UICONTROL Workflow Stages]</strong> pour configurer les étapes.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Allow original file to be downloaded]</td> 
   <td>Indiquez si vous souhaitez autoriser le téléchargement du fichier original à partir duquel l’épreuve a été créée.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Indiquez si vous utilisez la visionneuse d’épreuve classique.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combine all files into single proof]</td> 
   <td>Activez cette option pour combiner tous les fichiers en une seule épreuve multipage.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create a new proof version]</td> 
   <td>Sélectionnez cette option si vous souhaitez que le module crée une nouvelle version d’une épreuve existante. Ensuite, dans le champ <strong>[!UICONTROL Existing Proof ID]</strong> qui s’affiche, mappez ou saisissez l’identifiant unique de l’épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Link Label]</td> 
   <td>Saisissez ou mappez un libellé pour le lien d’épreuve personnalisé.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Link URL]</td> 
   <td>Saisissez ou mappez l’URL du lien personnalisé.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Default email notifications for subscribers]</td> 
   <td>Saisissez l’un des nombres suivants pour indiquer les paramètres de notification par e-mail par défaut que vous souhaitez utiliser pour l’épreuve créée.
    <ul>
     <li><strong>1</strong> - Tous les nouveaux commentaires et réponses</li>
     <li><strong>2</strong> - Réponses à mes commentaires</li>
     <li><strong>3</strong> - Résumé quotidien</li>
     <li><strong>4</strong> - Résumé horaire</li>
     <li><strong>5</strong> - Décisions uniquement</li>
     <li><strong>9</strong> - Désactivé</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable Excel Summary]</td> 
   <td>Indiquez si vous souhaitez désactiver la possibilité de télécharger les commentaires d’épreuves vers un fichier Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable PDF Summary]</td> 
   <td>Indiquez si vous souhaitez désactiver la possibilité de télécharger les commentaires d’épreuves vers un fichier PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Disable Subscription Email]</td> 
   <td>Indiquez si vous souhaitez désactiver l’e-mail d’abonnement pour cette épreuve.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Embed Player]</td> 
   <td>Indiquez si vous souhaitez activer le lecteur incorporé pour cette épreuve.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Subscriptions]</td> 
   <td>Indiquez si les personnes qui ne sont pas inscrites sont autorisées à s’abonner à l’épreuve.<br>Si vous sélectionnez cette option, vous pouvez également sélectionner le rôle par défaut des personnes abonnées, comme décrit dans ce tableau.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Subscriptions Validation]</td> 
   <td>Indiquez si vous souhaitez activer la validation d’abonnement par e-mail. Si cette option est activée, la personne abonnée doit cliquer sur un lien dans un e-mail pour accéder à une épreuve.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Enable Team URL]</td> 
   <td>Choisissez si vous voulez que l’épreuve créée masque ou affiche l’URL de l’équipe.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Hash] <span style="font-weight: normal;">ou</span> [!UICONTROL File Hashes]</td> 
   <td>Ajoutez l’identifiant du ou des fichiers que vous souhaitez utiliser pour créer une ou plusieurs épreuves.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL File Names]</td> 
   <td>Ajoutez le ou les noms de fichiers pour l’épreuve créée. Ce champ est obligatoire.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Lock proof when all required decisions are made]</td> 
   <td>Indiquez si vous souhaitez que l’épreuve créée soit verrouillée une fois que toutes les décisions requises ont été prises.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notify recipients about this proof]</td> 
   <td>Sélectionnez une option pour indiquer si vous voulez informer les personnes destinataires de la création de l’épreuve.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof name]</td> 
   <td>Saisissez un nom pour l’épreuve créée. Ce champ est obligatoire. Utilisez le symbole barre verticale (|) pour séparer les noms des différentes épreuves.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof owner ID]</td> 
   <td>Saisisez ou mappez l’indentifiant de la personne propriétaire de l’épreuve. Si ce champ n’est pas renseigné, la personne actuelle est propriétaire de l’épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference ID]</td> 
   <td>Saisissez l’identifiant de référence de l’épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Require electronic signature]</td> 
   <td>Indiquez si vous souhaitez demander une signature électronique à toute personne prenant une décision sur une épreuve.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Require login]</td> 
   <td> <p>Indiquez si vous souhaitez utiliser l’option de connexion obligatoire pour l’épreuve créée. </p> <p>Ce paramètre est identique au paramètre [!UICONTROL Login Required] expliqué à l’adresse <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configure Proof Settings] dans [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Resolution ID]</td> 
   <td>Saisissez l’identifiant de la résolution que vous souhaitez utiliser pour votre épreuve. Pour une liste des identifiants de résolution, consultez la <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">documentation de l’API</a> [!DNL Workfront Proof].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Saisissez le type d’épreuve SWF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Show] [item]</td> 
   <td>Indiquez si vous souhaitez afficher chaque élément dans l’épreuve.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Saisissez l’identifiant de l’espace de travail dans lequel vous souhaitez créer l’épreuve. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Recipients]</td> 
   <td>Ajoutez les adresses e-mail des personnes à qui vous souhaitez affecter l’épreuve créée.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>Indiquez la date d’échéance pour la relecture de l’épreuve créée. Utilisez le format de date suivant :</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel personnalisé et authentifié à l’API [!DNL Workfront Proof]. Vous pouvez ainsi, automatiser le flux de données d’une façon que les autres modules [!DNL Workfront Proof] ne permettent pas.

Le module renvoie le code d’état, les en-têtes et le corps du texte. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Method]</td> 
   <td>Définissez l’action pour l’appel API. Pour connaître les actions disponibles, voir la <a href="https://api.proofhq.com/">documentation de l’API Workfront Proof</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Body (XML)]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :  <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, mettez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL Télécharger l’épreuve]

Ce module d’action télécharge le fichier source d’une épreuve particulière que vous identifiez à l’aide de son ID.

Vous indiquez l’ID de l’épreuve.

Le module renvoie le contenu du fichier source utilisé pour créer l’épreuve. Vous pouvez mapper cette information dans les modules suivants du scénario.

Vous devez disposer des autorisations nécessaires pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de pouvoir récupérer ces informations.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Saisissez l’ID unique de l’épreuve qui se trouve sur la page [!UICONTROL Proof Details]. Pour plus d’informations, voir <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gérer les détails de l’épreuve dans [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit les données d’une seule épreuve dans [!DNL Workfront Proof].

Vous indiquez l’ID de l’épreuve et les informations que vous souhaitez obtenir de l’épreuve.

Le module renvoie les valeurs des champs que vous avez choisis pour l’épreuve, ainsi que leurs types. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Vous devez disposer d’autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de pouvoir récupérer ces informations.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Indiquez si vous souhaitez lire une épreuve, les commentaires d’une épreuve ou les réviseurs ou réviseuses d’une épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’ID unique [!DNL Workfront Proof] de l’enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Demander le résumé PDF]

Ce module d’action demande le résumé PDF d’une épreuve particulière dans [!DNL Workfront Proof].

Vous indiquez l’ID de l’épreuve.

Le module renvoie les informations du résumé PDF. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Vous devez disposer d’autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de pouvoir récupérer ces informations.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Saisissez l’ID unique [!DNL Workfront Proof] de l’épreuve pour laquelle vous souhaitez demander un résumé PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Callback URL]</td> 
   <td>Saisissez ou mappez l’URL où vous souhaitez que le résumé PDF soit envoyé.</td> 
  </tr> 
 </tbody> 
</table>

##### Erreur possible

* **Erreur** : « [!UICONTROL Vous n’avez pas les privilèges nécessaires pour effectuer cette demande. L’étape doit contenir au moins une personne destinataire.] »
* **Solution** : assurez-vous que vous n’êtes pas la seule personne affectée aux étapes du workflow. Une autre personne doit être affectée aux étapes du workflow.

#### [!UICONTROL Mettre à jour l’épreuve]

Ce module d’action met à jour une épreuve existante dans [!DNL Workfront Proof].

Vous indiquez l’identifiant de l’épreuve et le type d’enregistrement, ainsi que les champs que vous souhaitez inclure dans la sortie.

Le module renvoie tous les champs standard associés à l’enregistrement, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Vous devez disposer d’autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de pouvoir récupérer ces informations.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID]</td> 
   <td> <p>Saisissez l’ID unique de l’épreuve qui se trouve sur la page [!UICONTROL Proof Details]. Pour plus d’informations, voir <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gérer les détails de l’épreuve dans [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>Indiquez la date d’échéance pour la relecture de l’épreuve créée. Utilisez le format de date suivant :</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Default email notifications for subscribers]</td> 
   <td>Sélectionnez l’un des paramètres de notification par e-mail par défaut suivants que vous souhaitez utiliser pour l’épreuve créée.
    <ul>
     <li> [!UICONTROL All new comments and replies]</li>
     <li>[!UICONTROL Replies to my comments]</li>
     <li>[!UICONTROL Daily summary]</li>
     <li> [!UICONTROL Hourly summary]</li>
     <li> [!UICONTROL Decisions only]</li>
     <li> [!UICONTROL Disabled]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Default Role]</td> 
   <td>Sélectionnez le rôle par défaut pour l’épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Disable Subscription Email]</td> 
   <td>Indiquez si vous souhaitez désactiver l’e-mail d’abonnement pour cette épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Subscriptions]</td> 
   <td>Indiquez si les personnes qui ne sont pas inscrites sont autorisées à s’abonner à l’épreuve.<br>Si vous sélectionnez cette option, vous pouvez également sélectionner le [!UICONTROL Default Role] pour les personnes abonnées, comme décrit dans ce tableau.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Subscriptions Validation]</td> 
   <td>Indiquez si vous souhaitez activer la validation d’abonnement par e-mail. Si cette option est activée, la personne abonnée doit cliquer sur un lien dans un e-mail pour accéder à une épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enable Team URL]</td> 
   <td>Choisissez si vous voulez que l’épreuve créée masque ou affiche l’URL de l’équipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lock proof when all required decisions are made]</td> 
   <td>Indiquez si vous souhaitez que l’épreuve créée soit verrouillée une fois que toutes les décisions requises ont été prises.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Message]</td> 
   <td>Saisissez ou mappez le message qui doit accompagner l’épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof ID] </td> 
   <td>Saisissez ou mappez l’identifiant de l’épreuve que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td>Saisissez ou affichez le nom de l’épreuve que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Require login]</td> 
   <td> <p>Indiquez si vous souhaitez utiliser l’option de connexion obligatoire pour l’épreuve créée. </p> <p>Ce paramètre est identique au paramètre [!UICONTROL Login Required] expliqué dans <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configure Proof Settings] dans [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show Versions Like]</td> 
   <td>Indiquez si vous souhaitez afficher un lien vers d’autres versions de cette épreuve.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Saisir ou mapper le sujet de l’épreuve</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Charger fichier]

Ce module d’action charge un fichier à utiliser avec le module [!UICONTROL Créer une épreuve] dans [!DNL Workfront Proof].

Le module renvoie un identifiant de hachage pour le fichier chargé. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Rechercher]](#search)
* [[!UICONTROL Répertorier les modèles de workflows]](#list-workflow-templates)

#### [!UICONTROL Rechercher]

Ce module de recherche recherche les enregistrements dans un objet dans [!DNL Workfront Proof] qui correspondent à la requête que vous avez spécifiée.

Le module renvoie l’identifiant de l’épreuve s’il recherche une épreuve. Il renvoie également les identifiants, les e-mails, les noms, les postes et les alias des e-mail, s’il recherche des destinataires. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous devez disposer d’autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de pouvoir récupérer ces informations.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Rechercher</td> 
   <td> <p>Sé[!UICONTROL ]lectionnez le type d’enregistrement que vous souhaitez que le module recherche.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Proof]</strong> </p> <p>Saisissez le nom de l’épreuve que vous souhaitez rechercher.</p> </li> 
     <li> <p><strong>[!UICONTROL Recipient]</strong> </p> <p>Saisissez l’adresse e-mail de la destinataire ou du destinataire que vous souhaitez rechercher.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Indiquez si le module doit rechercher <strong>[!UICONTROL All Matching Records]</strong> ou seulement <strong>[!UICONTROL First Matching Record]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sort By]</td> 
   <td>Sélectionnez le champ par lequel vous souhaitez trier les résultats.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sorting Direction]</td> 
   <td> <p>Sélectionnez si vous souhaitez trier les résultats par ordre croissant ou décroissant.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier les modèles de workflow]

Ce module de recherche répertorie tous les modèles de workflow disponibles.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations que vous souhaitez inclure dans le bundle de sortie pour ce module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum de modèles que vous souhaitez que le module renvoie au cours de chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>
