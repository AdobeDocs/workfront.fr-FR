---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhooks
description: Un webhook est un appel HTTP déclenché par un événement. Vous pouvez utiliser des webhooks pour activer les modules de déclenchement instantanés. Toute application connectée à Internet et autorisant des requêtes HTTP peut envoyer des webhooks à Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 100%

---

# Webhooks

Un webhook est un appel HTTP déclenché par un événement. Vous pouvez utiliser des webhooks pour activer les modules de déclenchement instantanés. Toute application connectée à Internet et autorisant des requêtes HTTP peut envoyer des webhooks à Adobe Workfront Fusion.

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigence du produit hérité : votre organisation doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr>
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

&#42;&#42;Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez la section [[!DNL Adobe Workfront Fusion] Licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Utiliser un webhook dans [!DNL Workfront Fusion]

>[!NOTE]
>
>Pour appeler un webhook tiers (un webhook sortant), vous pouvez utiliser un module HTTP. Pour plus d’informations, consultez la section [Modules HTTP](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

Pour utiliser un webhook pour connecter une application à [!DNL Workfront Fusion], procédez comme suit :

1. Ajoutez le module de déclenchement instantané **[!UICONTROL Webhooks]** >**[!UICONTROL Webhook personnalisé]** à votre scénario.

1. Cliquez sur **[!UICONTROL Ajouter]** en regard du champ Webhook et donnez un nom au nouveau webhook.
1. (Facultatif) Cliquez sur **[!UICONTROL Paramètres avancés]**.
1. Dans le champ **[!UICONTROL Restrictions d’IP]**, saisissez une liste séparée par des virgules des adresses IP à partir desquelles le module peut accepter les données.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

Une fois que vous avez créé un webhook, une URL unique s’affiche. Il s’agit de l’adresse à laquelle le webhook envoie des données. Workfront Fusion valide les données envoyées à cette adresse, puis les transmet pour traitement dans le scénario.

>[!NOTE]
>
>Une fois que vous avez créé un webhook, vous pouvez l’utiliser dans plusieurs scénarios à la fois.

### Configurer la structure de données du webhook {#configure-the-webhook-s-data-structure}

Afin de reconnaître la structure de données du payload entrant, [!DNL Workfront Fusion] analyse les données d’exemple que vous envoyez à l’adresse affichée. Vous pouvez fournir les données d’exemples en effectuant une modification dans le service ou l’application qui fera que ce service ou cette application appellera le webhook. Vous pouvez par exemple supprimer un fichier.

Vous pouvez également suivre les étapes ci-dessous pour envoyer les données d’exemple via le module [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête].

1. Créez un scénario à l’aide du module **[!UICONTROL HTTP]** > **[!UICONTROL Effectuer une requête]**.

1. Configurez le module avec les valeurs suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Saisissez l’URL du webhook. Vous la trouverez dans le module [!UICONTROL Webhooks] que vous avez utilisé pour configurer le webhook.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request content]</td> 
      <td><p>JSON brut attendu dans le webhook</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Ouvrez le scénario à l’aide du module [!UICONTROL Webhooks] dans un onglet ou une fenêtre de navigateur distinct.
1. Dans le module Webhooks, cliquez sur **[!UICONTROL Redéfinir la structure de données]**.

   Il n’est pas nécessaire de dissocier d’autres modules du module Webhooks.

1. Basculez vers le scénario avec le module [!UICONTROL HTTP] et exécutez-le.
1. Revenez au scénario avec le module Webhooks.

   Le message « [!UICONTROL Déterminée avec succès] » signifie que le module a déterminé la structure de données avec succès.

   ![](assets/successfully-determined-350x175.png)

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer la structure de données.

   Les éléments du webhook sont désormais disponibles dans le panneau de mappage pour une utilisation avec les modules suivants du scénario.

## File d&#39;attente

Si un webhook reçoit des données et qu’aucun scénario actif n’attend ces données, les données sont stockées dans la file d’attente. Une fois le scénario activé, il traite tous les lots en attente dans la file d’attente de manière séquentielle.

>[!IMPORTANT]
>
>Les files d’attente de webhook sont partagées entre les scénarios qui utilisent le même webhook. Si l’un des scénarios est désactivé, toutes les données entrantes sont conservées dans la file d’attente.

## Formats de données entrantes pris en charge

[!DNL Workfront Fusion] prend en charge 3 formats de données entrantes : [!UICONTROL Chaîne de requête], [!UICONTROL Données de formulaire] et [!UICONTROL JSON].

[!DNL Workfront Fusion] valide toutes les données entrantes par rapport à la structure de données sélectionnée. Ensuite, en fonction des paramètres du scénario, les données sont soit stockées dans la file d’attente pour traitement, soit traitées immédiatement.

Si une partie des données n’est pas validée, [!DNL Workfront Fusion] renvoie un code d’état HTTP 400 et spécifie, dans le corps de la réponse HTTP, la raison pour laquelle les données entrantes n’ont pas réussi les contrôles de validation. Si la validation des données entrantes réussit, Workfront Fusion renvoie un statut « [!UICONTROL 200 Accepté] ».

* [[!UICONTROL Chaîne de requête]](#query-string)
* [[!UICONTROL Données de formulaire]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL Chaîne de requête]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL Données de formulaire]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### Données de formulaire à plusieurs parties

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

Pour pouvoir recevoir des fichiers codés avec `multipart/form-data`, vous devez configurer une structure de données avec un champ de type `collection` contenant les champs imbriqués `name`, `mime` et `data`. Le champ `name` est de type `text` et contient le nom du fichier chargé. Le champ `mime` est de type `text` et contient un fichier au format MIME. Le champ `data` est de type `buffer` et contient des données binaires pour le fichier transféré.

Pour plus d’informations sur le format MIME, voir [Modules MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>Si vous souhaitez accéder au JSON d’origine, activez la transmission JSON lors de la configuration du webhook.
>
>1. Cliquez sur **[!UICONTROL Ajouter]** pour ajouter un nouveau webhook.
>1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.
>1. Cliquez sur **[!UICONTROL Transmission JSON]**.
>

## En-têtes de webhook

Pour accéder aux en-têtes du webhook, activez l’option Obtenir les en-têtes de requête lors de la configuration du webhook.

1. Cliquez sur **[!UICONTROL Ajouter]** pour ajouter un nouveau webhook.
1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.
1. Cliquez sur **[!UICONTROL Obtenir les en-têtes de requête]**.

Vous pouvez extraire une valeur d’en-tête spécifique avec la combinaison des fonctions `map()` et `get()`.

>[!INFO]
>
>**Exemple :**
>
>L’exemple ci-dessous illustre une formule qui extrait la valeur de l’en-tête `authorization` du tableau `Headers[]`. La formule est utilisée dans un filtre qui compare la valeur extraite au texte donné pour ne transmettre que les webhooks en cas de correspondance.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Pour plus d’informations sur l’obtention de l’élément d’un tableau avec une clé donnée, voir [Mapper l’élément d’un tableau avec une clé donnée](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) dans l’article [Mapper des informations d’un module à un autre dans Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

## Répondre aux webhooks

La réponse par défaut à un appel de webhook est le texte « Accepté ». La réponse est renvoyée à l’application qui a appelé le webhook lors de l’exécution du module webhook personnalisé.

* [Tester la réponse à un webhook](#test-the-response-to-a-webhook)
* [Exemple de réponse HTML](#html-response-example)
* [Exemple de redirection](#redirect-example)

### Tester la réponse à un webhook

1. Incluez le module **[!UICONTROL Webhook personnalisé]** dans votre scénario.
1. Ajoutez un nouveau webhook au module.
1. Copiez l’URL du webhook dans le presse-papiers.
1. Exécutez le scénario.

   L’icône d’éclair sur le module [!UICONTROL Webhook personnalisé] change en symbole de chargement. Cela indique que le module attend désormais l’appel de webhook.

1. Ouvrez une nouvelle fenêtre de navigateur, collez l’URL copiée dans la barre d’adresse et appuyez sur **[!UICONTROL Entrée]**.

   Le module [!UICONTROL Webhook personnalisé] est déclenché et le navigateur affiche une nouvelle page.

Si vous souhaitez personnaliser la réponse du webhook, utilisez le module de réponse webhook.

La configuration du module contient deux champs : [!UICONTROL Statut] et [!UICONTROL Corps].

* Le champ [!UICONTROL Statut] contient des codes de statut de réponse HTTP tels que 2xx pour Succès (par exemple, `200` pour OK), 3xx pour Redirection (par exemple, `307` pour Redirection temporaire), 4xx pour les Erreurs client (par exemple, `400` pour Demande incorrecte), etc.

* Le champ [!UICONTROL Corps] contient tout ce qui sera accepté par l’appel du webhook. Il peut s’agir de texte simple, de code HTML, de code XML, de code JSON, etc.

  >[!TIP]
  >
  >Nous vous recommandons de définir l’en-tête `Content-Type` du type MIME correspondant : `text/plain` pour du texte brut, `text/html` pour HTML, `application/json` pour JSON, `application/xml` pour XML, etc. Pour plus d’informations sur les types MIME, voir [Modules MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

Le délai de temporisation pour l’envoi d’une réponse est de 40 secondes. Si la réponse n’est pas disponible au cours de cette période, Workfront Fusion renvoie un statut « 200 Accepté ».

### Exemple de réponse HTML

>[!INFO]
>
>**Exemple :**
>
>Configurez le module [!UICONTROL Réponse webhook] comme suit :
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>Code de statut HTTP de succès 2xx (par exemple, 200)</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>Code HTML</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Custom headers]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>Clé</strong> : type de contenu</li> 
&gt;     <li><strong>Valeur</strong> : text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>Cette opération génère une réponse HTML qui s’affiche dans un navigateur web :
>
>![](assets/html-response-350x70.png)

### Exemple de redirection

>[!INFO]
>
>**Exemple :** configurez le module [!UICONTROL Réponse webhook] comme suit :
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>Code d’état HTTP de redirection 3xx, par exemple 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Custom headers]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong> : emplacement</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong> : URL vers laquelle vous souhaitez effectuer les redirections.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Désactivation de webhook

Les webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

* Le webhook n’a été connecté à aucun scénario depuis plus de 5 jours.
* Le webhook est utilisé uniquement dans les scénarios inactifs, qui sont inactifs depuis plus de 30 jours.

Les webhooks désactivés sont supprimés et désinscrits automatiquement s’ils ne sont connectés à aucun scénario et s’ils sont restés désactivés pendant plus de 30 jours.


## Dépannage

### Éléments manquants dans le panneau de mappage

Si certains éléments sont manquants dans le panneau de mappage dans la configuration des modules suivant le module [!UICONTROL Webhooks] > [!UICONTROL Webhook personnalisé], cliquez sur le bouton **[!UICONTROL Webhooks] > [!UICONTROL Webhook personnalisé]** pour ouvrir sa configuration, puis cliquez sur **[!UICONTROL Rédéterminer la structure des données]** :

![](assets/redetermine-data-structure-btn-350x195.png)

Suivez ensuite les étapes décrites dans la section [Configuration de la structure de données du webhook](#configure-the-webhook-s-data-structure) dans cet article.
