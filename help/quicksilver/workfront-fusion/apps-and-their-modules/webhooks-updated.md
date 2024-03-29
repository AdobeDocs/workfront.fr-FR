---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhooks
description: Un webhook est un appel HTTP déclenché par un événement. Vous pouvez utiliser des webhooks pour activer les modules de déclenchement instantanés. Toute application connectée à Internet et autorisant des requêtes HTTP peut envoyer des webhooks à Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1437'
ht-degree: 0%

---

# Webhooks

Un webhook est un appel HTTP déclenché par un événement. Vous pouvez utiliser des webhooks pour activer les modules de déclenchement instantanés. Toute application connectée à Internet et autorisant des requêtes HTTP peut envoyer des webhooks à Adobe Workfront Fusion.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr>
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

&#42;&#42;Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Utilisation d’un webhook dans [!DNL Workfront Fusion]

>[!NOTE]
>
>Pour appeler un webhook tiers (un webhook sortant), utilisez l’un des modules HTTP . Pour plus d’informations, voir [Modules HTTP](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

Pour utiliser un webhook pour connecter une application à [!DNL Workfront Fusion]:

1. Ajoutez la variable **[!UICONTROL Webhooks]** >**[!UICONTROL Webhook personnalisé]** module de déclenchement instantané à votre scénario.

1. Cliquez sur **[!UICONTROL Ajouter]** en regard du champ Webhook et saisissez le nom du nouveau webhook.
1. (Facultatif) Cliquez sur **[!UICONTROL Paramètres avancés]**.
1. Dans le **[!UICONTROL Restrictions d’IP]** , saisissez une liste séparée par des virgules des adresses IP à partir desquelles le module peut accepter les données.
1. Cliquer sur **[!UICONTROL Enregistrer]**

Une fois que vous avez créé un webhook, une URL unique s’affiche. Il s’agit de l’adresse à laquelle le webhook envoie des données. Workfront Fusion valide les données envoyées à cette adresse, puis les transmet pour traitement dans le scénario.

>[!NOTE]
>
>Une fois que vous avez créé un webhook, vous pouvez l’utiliser dans plusieurs scénarios à la fois.

### Configuration de la structure de données du webhook {#configure-the-webhook-s-data-structure}

Afin de reconnaître la structure de données de la payload entrante, [!DNL Workfront Fusion] analyse les données d’exemple que vous envoyez à l’adresse affichée. Vous pouvez fournir les exemples de données en effectuant une modification dans le service ou l’application qui fera appel au webhook pour ce service ou cette application. Par exemple, vous pouvez supprimer un fichier.

Vous pouvez également suivre les étapes ci-dessous pour envoyer les exemples de données via le [!UICONTROL HTTP] > [!UICONTROL Effectuer une requête] module .

1. Créez un scénario avec le **[!UICONTROL HTTP]** > **[!UICONTROL Effectuer une requête]** module

1. Configurez le module avec les valeurs suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Saisissez l’URL du webhook. Cette URL se trouve dans le module [!UICONTROL Webhooks] que vous avez utilisé pour configurer le webhook.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Méthode [!UICONTROL] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Type de corps]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Type de contenu]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Demander du contenu]</td> 
      <td><p>Fichier JSON brut attendu dans le webhook</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. Ouvrez le scénario à l’aide de la commande [!UICONTROL Webhooks] dans un onglet ou une fenêtre de navigateur distinct.
1. Dans le module webhooks, cliquez sur **[!UICONTROL Redéfinir la structure des données]**.

   Il n’est pas nécessaire de dissocier d’autres modules du module webhooks.

1. Basculez vers le scénario avec la méthode [!UICONTROL HTTP] et exécutez-le.
1. Revenez au scénario avec le module Webhooks.

   Un &quot;[!UICONTROL Déterminé]&quot; message signifie que le module a déterminé la structure des données avec succès.

   ![](assets/successfully-determined-350x175.png)

1. Cliquez sur **[!UICONTROL OK]** pour enregistrer la structure de données.

   Les éléments du webhook sont désormais disponibles dans le panneau de mappage pour une utilisation avec les modules suivants dans le scénario.

## File d&#39;attente

Si un webhook reçoit des données et qu’il n’existe pas de scénario principal qui attend ces données, les données sont stockées dans la file d’attente. Une fois le scénario activé, il traite tous les lots en attente dans la file d’attente de manière séquentielle.

>[!IMPORTANT]
>
>Les files d’attente Webhook sont partagées entre les scénarios qui utilisent le même webhook. Si l’un des scénarios est désactivé, toutes les données entrantes sont conservées dans la file d’attente.

## Formats de données entrantes pris en charge

[!DNL Workfront Fusion] prend en charge 3 formats de données entrants : [!UICONTROL Chaîne de requête], [!UICONTROL Données de formulaire] et [!UICONTROL JSON].

[!DNL Workfront Fusion] valide toutes les données entrantes par rapport à la structure de données sélectionnée. Ensuite, selon les paramètres du scénario, les données sont soit stockées dans la file d’attente pour traitement, soit traitées immédiatement.

Si une partie des données n’est pas validée, [!DNL Workfront Fusion] renvoie un code d’état HTTP 400 et spécifie, dans le corps de la réponse HTTP, la raison pour laquelle les données entrantes n’ont pas réussi les contrôles de validation. Si la validation des données entrantes réussit, Workfront Fusion renvoie un &quot;[!UICONTROL 200 acceptés]&quot;.

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

Pour recevoir des fichiers codés avec `multipart/form-data`, vous devez configurer une structure de données avec un `collection` champ de type contenant les champs imbriqués `name`, `mime`, et `data`. Le champ `name` est un `text` et contient le nom du fichier téléchargé. Le `mime` est un `text` saisissez et contient un fichier au format MIME. Le champ `data` est un `buffer` type et contient des données binaires pour le fichier transféré.

Pour plus d’informations sur le format MIME, voir [Modules MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>Si vous souhaitez accéder au fichier JSON d’origine, activez la transmission JSON lors de la configuration du webhook.
>
>1. Cliquez sur **[!UICONTROL Ajouter]** pour ajouter un nouveau webhook.
>1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.
>1. Cliquez sur **[!UICONTROL Diffusion JSON]**.
>

## En-têtes Webhook

Pour accéder aux en-têtes du webhook, activez l’option Obtenir les en-têtes de requête lors de la configuration du webhook.

1. Cliquez sur **[!UICONTROL Ajouter]** pour ajouter un nouveau webhook.
1. Cliquez sur **[!UICONTROL Afficher les paramètres avancés]**.
1. Cliquez sur **[!UICONTROL Obtention des en-têtes de requête]**.

Vous pouvez extraire une valeur d’en-tête spécifique avec la combinaison de `map()` et `get()` fonctions.

>[!INFO]
>
>**Exemple:**
>
>L’exemple ci-dessous illustre une formule qui extrait la valeur de la variable `authorization` de l’en-tête `Headers[]` tableau. La formule est utilisée dans un filtre qui compare la valeur extraite au texte donné pour ne transmettre que les webhooks en cas de correspondance.
>
>![](assets/set-up-a-filter-350x169.png)
>
>Pour plus d’informations sur l’obtention de l’élément d’un tableau avec une clé donnée, voir [Mise en correspondance de l’élément d’un tableau avec une clé donnée](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) dans l’article [Mappage des informations d’un module à un autre dans Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

## Réponse aux webhooks

La réponse par défaut à un appel webhook est le texte &quot;Accepted&quot;. La réponse est renvoyée à l’application qui a appelé le webhook lors de l’exécution du module Custom Webhook.

* [Test de la réponse à un webhook](#test-the-response-to-a-webhook)
* [Exemple de réponse HTML](#html-response-example)
* [Exemple de redirection](#redirect-example)

### Test de la réponse à un webhook

1. Inclure la variable **[!UICONTROL Webhook personnalisé]** dans votre scénario.
1. Ajoutez un nouveau webhook au module .
1. Copiez l’URL du webhook dans le presse-papiers.
1. Exécutez le scénario.

   Icône d’éclair sur la [!UICONTROL Webhook personnalisé] change de module en points de rotation. Cela indique que le module attend désormais l’appel webhook.

1. Ouvrez une nouvelle fenêtre de navigateur, collez l’URL copiée dans la barre d’adresse et appuyez sur **[!UICONTROL Entrée]**.

   Le [!UICONTROL Webhook personnalisé] est déclenché et le navigateur affiche une nouvelle page.

Si vous souhaitez personnaliser la réponse du webhook, utilisez le module Webhook Response.

La configuration du module contient deux champs : [!UICONTROL État] et [!UICONTROL Corps].

* Le [!UICONTROL État] contient des codes d’état de réponse HTTP tels que 2xx pour succès (par exemple, `200` pour OK), 3xx pour Redirection (par exemple, `307` pour la redirection temporaire), 4xx pour les erreurs client (par exemple, `400` pour la demande incorrecte), etc.

* Le [!UICONTROL Corps] contient tout ce qui sera accepté par l’appel du webhook. Il peut s’agir de texte simple, de HTML, de code XML, de code JSON, etc.

  >[!TIP]
  >
  >Nous vous recommandons de définir la variable `Content-Type` en-tête du type MIME correspondant : `text/plain` pour le texte brut, `text/html` pour le HTML, `application/json` pour JSON, `application/xml` pour XML, etc. Pour plus d’informations sur les types MIME, voir [Modules MIME](../../workfront-fusion/apps-and-their-modules/mime.md).

Le délai d’expiration pour l’envoi d’une réponse est de 40 secondes. Si la réponse n’est pas disponible au cours de cette période, Workfront Fusion renvoie un état &quot;200 Accepted&quot;.

### Exemple de réponse HTML

>[!INFO]
>
>**Exemple:**
>
>Configurez la variable [!UICONTROL Réponse Webhook] module comme suit :
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>Code d’état HTTP de réussite 2xx, par exemple 200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>Code HTML</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL En-têtes personnalisés]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>Clé</strong>: Content-type</li> 
&gt;     <li><strong>Valeur</strong>: text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>Cela génère une réponse de HTML qui s’affiche dans un navigateur web :
>
>![](assets/html-response-350x70.png)

### Exemple de redirection

>[!INFO]
>
>**Exemple :** Configurez la variable [!UICONTROL Réponse Webhook] module comme suit :
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>Code d’état HTTP de redirection 3xx, par exemple 303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL En-têtes personnalisés]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong>: Emplacement</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong>: L’URL vers laquelle vous souhaitez rediriger les visiteurs.</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Désactivation de Webhook

Les webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

* Le webhook n’est connecté à aucun scénario depuis plus de 5 jours.
* Le webhook est utilisé uniquement dans les scénarios inactifs, qui sont inactifs depuis plus de 30 jours.

Les webhooks désactivés sont supprimés et désenregistrés automatiquement s’ils ne sont connectés à aucun scénario et sont désactivés depuis plus de 30 jours.


## Dépannage

### Éléments manquants dans le panneau de mappage

Si certains éléments sont manquants dans le panneau de mappage dans la configuration des modules suivant la [!UICONTROL Webhooks] > [!UICONTROL Webhook personnalisé] , cliquez sur le bouton **[!UICONTROL Webhooks] > [!UICONTROL Webhook personnalisé]** pour ouvrir sa configuration, puis cliquez sur **[!UICONTROL Rédéterminer la structure des données]**:

![](assets/redetermine-data-structure-btn-350x195.png)

Suivez ensuite les étapes décrites dans la section [Configuration de la structure de données du webhook](#configure-the-webhook-s-data-structure) dans cet article.
