---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules d’épreuve de Workfront
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL Workfront Proof] et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 614fd206ea2c5fe103beb5be8f5ff99c8a45a502
workflow-type: tm+mt
source-wordcount: '3099'
ht-degree: 24%

---

# Modules [!DNL Workfront Proof]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Workfront Proof] et les connecter à plusieurs applications et services tiers.

Cela s’avère utile si vous devez exécuter des tâches actuellement non prises en charge dans la vérification dans [!DNL Workfront] ou dans [!DNL Workfront Proof], telles que la mise à jour des bons à tirer en fonction de certains événements et la recherche des destinataires d’un BAT.

Le connecteur [!DNL Workfront Proof] n’est pas pris en compte dans le nombre d’applications actives disponibles pour votre organisation. Tous les scénarios, même s’ils utilisent uniquement l’application [!DNL Workfront Proof], ne sont pas pris en compte dans le nombre total de scénarios de votre entreprise.

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
   <p>Exigences de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Connecter [!DNL Workfront Proof] à [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre compte [!DNL Workfront Proof] directement à partir de l’intérieur d’un module [!DNL Workfront Fusion].

1. Dans un module [!DNL Workfront Fusion], cliquez sur [!UICONTROL **Ajouter**] en regard du champ [!UICONTROL Connexion]

2. Renseignez les champs suivants :

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>Saisissez un nom pour la connexion.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL connections.environmentType]</td>
                <td>Indiquez s’il s’agit d’un environnement de production ou d’un environnement hors production tel que Aperçu ou Environnement de test.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL connections.authenticationType]</td>
                <td>Indiquez s’il s’agit d’un compte de service ou d’un compte personnel.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Email / Nom d’utilisateur]</td>
                <td>Saisissez le nom d’utilisateur de votre compte [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Password]</td>
                <td>Saisissez le mot de passe de votre compte [!DNL Workfront Proof].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL ID de tenant]</td>
                <td><strong>Remarque</strong> : les clients qui n’utilisent pas BYOK doivent laisser ce champ vide. <p>Saisissez l’identifiant du client pour ce compte. Si vous avez besoin d’aide pour trouver votre ID de tenant, contactez le service clientèle de Workfront.</p></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Domain Extension]</td>
                <td>Saisissez l’extension de l’URL que vous utilisez pour accéder à votre compte. <p>Exemple : <code>com</code> ou <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Production, Aperçu ou Environnement personnalisé]</td>
                <td>Sélectionnez une connexion à un environnement de production, de prévisualisation ou personnalisé.</td>
            </tr>
        </tbody>
    </table>


3. Cliquez sur [!UICONTROL **Continuer**] pour enregistrer la connexion et revenir au module

## Modules [!DNL Workfront Proof] et leurs champs

Lorsque vous configurez des modules [!DNL Workfront Proof], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Workfront Proof] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

* [Bons à tirer](#watch-proofs)
* [Rechercher le résumé du PDF](#watch-for-pdf-summary)
* [[!UICONTROL  {Surveiller l’activité du BAT]](#watch-proof-activity)

#### [!UICONTROL Surveiller Les Bons À Tirer]

Ce module de déclenchement planifié exécute un scénario lorsqu’une personne crée ou prend une décision sur un BAT.

Le module renvoie une liste de tous les enregistrements trouvés pendant la période que vous spécifiez, ainsi que leurs types. Elle renvoie également les valeurs des champs que vous spécifiez. Si le module a trouvé des décisions prises sur le BAT, il inclut les valeurs précédente et actuelle, dans des champs distincts. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Cela se produit dans un intervalle régulièrement planifié que vous spécifiez.

Vous devez disposer des autorisations suffisantes pour accéder au BAT ou aux BAT dans [!DNL Workfront Proof] afin de récupérer ces informations.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Type d’enregistrement</td> 
   <td>Sélectionnez le type d’enregistrement [!DNL Workfront Proof] que le module doit surveiller.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Sorties</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limite</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher le résumé du PDF]

Ce module de déclenchement instantané exécute un scénario lorsqu’une personne crée un résumé du PDF pour un BAT.

Un webhook est requis dans ce module.

Le module renvoie tous les champs standard associés au BAT, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Il crée également un nouvel abonnement d’événement pour les résumés PDF et sort le contenu de l’attribut &quot;pdf_url&quot; envoyé dans la payload. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Vous pouvez sélectionner un webhook existant ou en créer un nouveau. Pour plus d’informations, voir <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheurs instantanés (webhooks) dans [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL  {Surveiller l’activité du BAT]

Ce module de déclenchement exécute un scénario lorsqu’une activité spécifiée se produit sur un BAT.

Le module renvoie tous les champs standard associés au BAT, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Il crée également un nouvel abonnement d’événement pour les résumés de PDF et génère le contenu de l’attribut `pdf_url` envoyé dans la payload. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type d’activité]</td> 
   <td>Indiquez si vous souhaitez regarder une nouvelle décision (y compris les modifications d’état [!UICONTROL BAT]) ou les modifications d’état global du BAT uniquement.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Créer un bon à tirer]](#create-proof)
* [[!UICONTROL Appel API personnalisé]](#custom-api-call)
* [[!UICONTROL Télécharger le bon à tirer]](#download-proof)
* [[!UICONTROL Lire un enregistrement]](#read-a-record)
* [[!UICONTROL Résumé du PDF de requêtes]](#request-pdf-summary)
* [[!UICONTROL Mettre à jour le BAT]](#update-proof)
* [[!UICONTROL Télécharger le fichier]](#upload-file)

#### [!UICONTROL Créer un bon à tirer]

Ce module d’action crée un BAT ou une nouvelle version d’un BAT dans [!DNL Workfront Proof].

Vous spécifiez les paramètres du nouveau BAT et du BAT source si vous créez une nouvelle version.

Le module renvoie l&#39;identifiant de la nouvelle version du BAT ou du BAT. Vous pouvez associer ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL BAT Type]</td> 
   <td> <p>Indiquez si vous souhaitez que le BAT créé dispose d’un workflow de base ou d’un [!UICONTROL Processus automatisé].</p> <p>Renseignez ensuite les champs qui s'affichent pour le type de BAT que vous avez choisi. Par exemple, si vous avez sélectionné [!UICONTROL Processus automatisé], remplissez le champ <strong>[!UICONTROL Étapes de processus]</strong> pour configurer les étapes.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Autoriser le téléchargement du fichier d’origine]</td> 
   <td>Indiquez si vous souhaitez autoriser le téléchargement du fichier d’origine à partir duquel le BAT a été créé.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Indiquez si vous utilisez la visionneuse de BAT classique.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Combiner tous les fichiers en un seul BAT]</td> 
   <td>Activez cette option pour combiner tous les fichiers en un seul BAT multi-page.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Créer une version de BAT]</td> 
   <td>Sélectionnez cette option si vous souhaitez que le module crée une nouvelle version d'un BAT existant. Ensuite, dans le champ <strong>[!UICONTROL Existant Proof ID]</strong> qui affiche, mappe ou saisit l’identifiant unique du BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Étiquette de lien personnalisé]</td> 
   <td>Saisissez ou mappez un libellé pour le lien personnalisé du BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL de lien personnalisé]</td> 
   <td>Saisissez ou mappez l’URL du lien personnalisé.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Notifications électroniques par défaut pour les abonnés]</td> 
   <td>Saisissez l’un des nombres suivants pour indiquer les paramètres de notification par email par défaut suivants que vous souhaitez utiliser pour le BAT créé.
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
   <td>[!UICONTROL Désactiver le résumé Excel]</td> 
   <td>Indiquez si vous souhaitez désactiver la possibilité de télécharger des commentaires de BAT dans un fichier Excel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Désactiver le résumé du PDF]</td> 
   <td>Indiquez si vous souhaitez désactiver la possibilité de télécharger les commentaires BAT dans un fichier de PDF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Désactiver le courrier électronique d’abonnement]</td> 
   <td>Indiquez si vous souhaitez désactiver l'email d'abonnement pour ce BAT.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Activer le lecteur intégré]</td> 
   <td>Indiquez si vous souhaitez activer le lecteur incorporé pour ce BAT.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Activer les abonnements]</td> 
   <td>Indiquez si les personnes qui ne sont pas des participants sont autorisées à souscrire au BAT.<br>Si vous sélectionnez cette option, vous pouvez également sélectionner le rôle par défaut des abonnés, comme décrit dans ce tableau.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Activer la validation des abonnements]</td> 
   <td>Indiquez si vous souhaitez activer la validation des emails d’abonnement. Si cette option est activée, l'abonné doit cliquer sur un lien dans un email pour accéder à un BAT.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Activer l’URL de l’équipe]</td> 
   <td>Indiquez si vous souhaitez que le BAT créé soit masqué ou affiche l’URL de l’équipe.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hachage de fichier] <span style="font-weight: normal;"> ou </span> [!UICONTROL Hachages de fichier]</td> 
   <td>Ajoutez l'identifiant du ou des fichiers à partir desquels vous souhaitez créer un BAT ou des BAT.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Noms de fichier]</td> 
   <td>Ajoutez le ou les noms du fichier pour le BAT créé. Ce champ est obligatoire.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL BAT de verrouillage lorsque toutes les décisions requises sont prises]</td> 
   <td>Indiquez si vous souhaitez que le BAT créé se verrouille une fois toutes les décisions requises prises.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Informer les destinataires de ce BAT]</td> 
   <td>Sélectionnez une option pour indiquer si vous souhaitez que les destinataires soient avertis lors de la création du BAT.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de la preuve]</td> 
   <td>Saisissez le nom du BAT créé. Il s’agit d’un champ obligatoire. Utilisez une barre verticale (|) pour séparer les noms de plusieurs bons à tirer.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID du propriétaire du BAT]</td> 
   <td>Saisissez ou mappez l’identifiant du propriétaire du BAT. Si ce champ n’est pas renseigné, le propriétaire du BAT est défini sur l’utilisateur actuel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference ID]</td> 
   <td>Saisissez l’ID de référence du BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nécessiter une signature électronique]</td> 
   <td>Indiquez si vous souhaitez exiger qu’une personne qui prend une décision sur un BAT envoie une signature électronique.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Nécessite une connexion]</td> 
   <td> <p>Indiquez si vous souhaitez que le BAT créé requiert une connexion. </p> <p>Il s’agit du même paramètre que le paramètre [!UICONTROL Connexion requise] expliqué dans <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configuration des paramètres de BAT] dans [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Resolution ID]</td> 
   <td>Saisissez l'identifiant de la résolution que vous souhaitez utiliser pour votre BAT. Pour obtenir la liste des ID de résolution, consultez la [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">documentation de l’API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Saisissez le type de BAT SWF.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Afficher] [élément]</td> 
   <td>Pour chaque élément, choisissez si vous souhaitez l’afficher dans le BAT.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Saisissez l'identifiant de l'espace de travail dans lequel vous souhaitez créer le BAT. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Destinataires]</td> 
   <td>Ajoutez les adresses email des destinataires que vous souhaitez pour le BAT créé .</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Date limite]</td> 
   <td> <p>Indiquez la date limite de création du BAT. Utilisez le format de date suivant :</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Workfront Proof]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Workfront Proof].

Le module renvoie le code d’état, les en-têtes et le corps. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Method]</td> 
   <td>Définissez l’action de l’appel API. Pour connaître les actions disponibles, reportez-vous à la <a href="https://api.proofhq.com/">documentation de l’API Proof</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Body (XML)]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
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

#### [!UICONTROL Télécharger le bon à tirer]

Ce module d’action télécharge le fichier source d’un BAT particulier que vous identifiez à l’aide de son identifiant.

Vous spécifiez l’identifiant du BAT.

Le module renvoie le contenu du fichier source utilisé pour créer le BAT. Vous pouvez associer ces informations dans les modules suivants du scénario.

Vous devez disposer des autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de récupérer ces informations.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL BAT ID]</td> 
   <td> <p>Saisissez l’identifiant unique du BAT, qui se trouve sur la page [!UICONTROL Proof Details]. Pour plus d’informations, voir <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gérer les détails du BAT dans [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lire un enregistrement]

Ce module d’action lit les données d’un seul BAT dans [!DNL Workfront Proof].

Vous indiquez l’identifiant du BAT et les informations que vous souhaitez obtenir du BAT.

Le module renvoie les valeurs des champs que vous choisissez pour le BAT, ainsi que leurs types. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous devez disposer des autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de récupérer ces informations.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Indiquez si vous souhaitez lire un BAT, des commentaires de BAT ou des réviseurs de BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant unique [!DNL Workfront Proof] de l’enregistrement que vous souhaitez que le module lise.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Résumé du PDF de requêtes]

Ce module d’action demande la synthèse du PDF pour un BAT particulier dans [!DNL Workfront Proof].

Vous spécifiez l’identifiant du BAT.

Le module renvoie des informations récapitulatives pour le PDF. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous devez disposer des autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de récupérer ces informations.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL BAT ID]</td> 
   <td> <p>Saisissez l'identifiant unique [!DNL Workfront Proof] du BAT pour lequel vous souhaitez demander un résumé pour le PDF.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL URL de rappel]</td> 
   <td>Saisissez ou mappez l’URL à laquelle vous souhaitez envoyer la synthèse du PDF.</td> 
  </tr> 
 </tbody> 
</table>

##### Erreur possible

* **Error** : &quot;[!UICONTROL Vous n’avez pas le privilège d’effectuer cette requête. La scène doit contenir au moins un destinataire.]&quot;
* **Solution** : assurez-vous que vous n’êtes pas le seul attribué aux étapes du workflow. Un autre utilisateur doit être affecté aux étapes du workflow.

#### [!UICONTROL Mettre à jour le BAT]

Ce module d&#39;action met à jour un BAT existant dans [!DNL Workfront Proof].

Vous spécifiez l’identifiant du BAT et le type d’enregistrement, ainsi que les champs que vous souhaitez inclure dans la sortie.

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Vous devez disposer des autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de récupérer ces informations.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL BAT ID]</td> 
   <td> <p>Saisissez l’identifiant unique du BAT, qui se trouve sur la page [!UICONTROL Proof Details]. Pour plus d’informations, voir <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Gérer les détails du BAT dans [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date limite]</td> 
   <td> <p>Indiquez la date limite de création du BAT. Utilisez le format de date suivant :</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Notifications électroniques par défaut pour les abonnés]</td> 
   <td>Sélectionnez les paramètres de notification par e-mail par défaut suivants que vous souhaitez utiliser pour le BAT créé.
    <ul>
     <li> [!UICONTROL Tous les nouveaux commentaires et réponses]</li>
     <li>[!UICONTROL Réponses à mes commentaires]</li>
     <li>[!UICONTROL Résumé quotidien]</li>
     <li> [!UICONTROL Résumé horaire]</li>
     <li> [!UICONTROL Décisions uniquement]</li>
     <li> [!UICONTROL Désactivé]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rôle par défaut]</td> 
   <td>Sélectionnez le rôle par défaut du BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Désactiver le courrier électronique d’abonnement]</td> 
   <td>Indiquez si vous souhaitez désactiver l'email d'abonnement pour ce BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Activer les abonnements]</td> 
   <td>Indiquez si les personnes qui ne sont pas des participants sont autorisées à souscrire au BAT.<br>Si vous sélectionnez cette option, vous pouvez également sélectionner le [!UICONTROL Rôle par défaut] pour les abonnés, comme décrit dans ce tableau.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Activer la validation des abonnements]</td> 
   <td>Indiquez si vous souhaitez activer la validation des emails d’abonnement. Si cette option est activée, l'abonné doit cliquer sur un lien dans un email pour accéder à un BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Activer l’URL de l’équipe]</td> 
   <td>Indiquez si vous souhaitez que le BAT créé soit masqué ou affiche l’URL de l’équipe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL BAT de verrouillage lorsque toutes les décisions requises sont prises]</td> 
   <td>Indiquez si vous souhaitez que le BAT créé se verrouille une fois toutes les décisions requises prises.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Message]</td> 
   <td>Saisissez ou mappez un message que vous souhaitez accompagner le BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL BAT ID] </td> 
   <td>Saisissez ou mappez l'identifiant du BAT que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td>Saisissez ou mappez le nom du BAT à mettre à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nécessite une connexion]</td> 
   <td> <p>Indiquez si vous souhaitez que le BAT créé requiert une connexion. </p> <p>Il s’agit du même paramètre que le paramètre [!UICONTROL Connexion requise] expliqué dans <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Configuration des paramètres de BAT] dans [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Afficher les versions comme]</td> 
   <td>Indiquez si vous souhaitez afficher un lien vers d’autres versions de ce BAT.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Entrer ou mapper l’objet du BAT</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger le fichier]

Ce module d’action charge un fichier à utiliser avec le module [!UICONTROL Créer un bon à tirer] dans [!DNL Workfront Proof].

Le module renvoie un identifiant de hachage pour le fichier chargé. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Recherches

* [[!UICONTROL Rechercher]](#search)
* [[!UICONTROL  Liste des modèles de workflow ]](#list-workflow-templates)

#### [!UICONTROL Rechercher]

Ce module de recherche recherche des enregistrements d’un objet dans [!DNL Workfront Proof] qui correspondent à la requête de recherche que vous avez spécifiée.

Le module renvoie l’identifiant du BAT s’il recherche un BAT. Ou elle renvoie les identifiants utilisateur, emails, noms, positions et alias de messagerie des destinataires, s&#39;il recherche des destinataires. Vous pouvez associer ces informations dans les modules suivants du scénario.

Vous devez disposer des autorisations suffisantes pour accéder à l’enregistrement dans [!DNL Workfront Proof] afin de récupérer ces informations.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Rechercher</td> 
   <td> <p>Voir[!UICONTROL ]sélectionnez le type d’enregistrement que le module doit rechercher.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Bon À Tirer]</strong> </p> <p>Saisissez le Nom du BAT du BAT que vous souhaitez rechercher.</p> </li> 
     <li> <p><strong>[!UICONTROL Destinataire]</strong> </p> <p>Saisissez l'adresse email du destinataire que vous souhaitez rechercher.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Result Set]</td> 
   <td>Indiquez si le module recherchera <strong>[!UICONTROL Tous les enregistrements correspondants]</strong> ou uniquement l’ <strong>[!UICONTROL Premier enregistrement correspondant]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Trier Par]</td> 
   <td>Sélectionnez le champ d’après lequel vous souhaitez trier les résultats.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Direction du tri]</td> 
   <td> <p>Indiquez si vous souhaitez trier les résultats par ordre croissant ou décroissant.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL  Liste des modèles de workflow ]

Ce module de recherche répertorie tous les modèles de workflow disponibles.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Workfront Proof] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>Sélectionnez les informations à inclure dans le lot de sortie pour ce module.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de modèles que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>
