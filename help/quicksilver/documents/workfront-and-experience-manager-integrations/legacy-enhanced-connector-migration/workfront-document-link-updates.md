---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Migrer des dossiers et des documents liés
description: Vous pouvez utiliser l’API pour migrer les dossiers et documents liés vers Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 100%

---

# Migrer des dossiers et des documents liés

Vous pouvez utiliser l’API pour migrer les dossiers et documents liés vers Adobe Experience Manager Assets.

## Procédure

1. Identifiez tous les documents et dossiers liés au fournisseur externe précédent de stockage de documents, en notant leurs identifiants de document ou de dossier internes Workfront ainsi que l’identifiant de dossier de tout dossier les contenant.

   >[!NOTE]
   >
   > Vous devez rechercher tous les dossiers ou documents découverts pour vérifier qu’ils n’ont pas déjà créé de lien avec le nouveau fournisseur.

1. Recherchez les documents et les dossiers dans le nouveau référentiel par chemin d’accès, puis recherchez leur identité dans le système externe.

1. Créez un mappage de l’ID Workfront interne sur l’ID dans le nouvel entrepôt externe. Vous en avez besoin pour créer un lien à l’étape suivante.

1. Créez un lien vers un nouveau document ou dossier de document dans Workfront, en pointant vers la ressource à son nouvel emplacement via son nouvel ID externe.

   1. **Documents** : ajoutez une nouvelle version du document existant auprès du nouveau fournisseur de documents externe.
   1. **Dossiers** : créez un dossier au même endroit avec le même nom.

>[!CAUTION]
>
>   Ne supprimez pas les dossiers liés existants. Cela pourrait entraîner une perte de données. Pour supprimer les anciens liens de dossier de l’application Workfront, désactivez l’intégration de document personnalisée dans la zone Configuration.


## Exemple de processus de migration de liens

![simplified-link-flow](assets/links-flow-simplified.png)

## Informations sur l’API

Pour plus d’informations sur les API Workfront de cette section, voir [Documentation destinée à l’équipe de développement : documents](https://developer.workfront.com/documents.html).

### Rechercher tous les documents

Rechercher tous les **documents (DOCU)** associés au **fournisseur de documents** du **providerType** avec **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[Référence API DOCS](https://developer.workfront.com/documents.html#get-/docu/search)

### Rechercher tous les dossiers

Recherchez tous les **dossiers de documents (DOCFDR)** liés au fournisseur de document du **providerType** avec **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API DOCS : (points d’entrée du dossier de documents non actuellement couverts à l’adresse developer.workfront.com)

### Lier les documents

Lier les **documents (DOCU)** de **fournisseur de documents externe** du **providerType** avec **documentProviderID**.

>[!IMPORTANT]
>
>Les documents sont temporairement stockés. En d’autres termes, vous avez accès à toutes les versions du document. Lorsque vous créez le lien, vous pouvez spécifier l’ID du document existant. Vous n’avez donc qu’à écrire une nouvelle version dans ce document, les données étant hébergées en externe auprès du nouveau fournisseur. Cet ID du document est identique à l’ID du document figurant sur le lien de document que vous remplacez. Il s’agit du même document conceptuel. Vous indiquez simplement que les octets de cette nouvelle version sont stockés auprès d’un fournisseur différent.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API DOCS : (points d’entrée de lien interne non actuellement couverts à l’adresse developer.workfront.com)

### Lier des dossiers

Liez les **dossiers de documents (DOCFDR)** de **fournisseur de documents externe** du **providerType** avec **documentProviderID**.

>[!IMPORTANT]
>
>Pour les liens de dossier, contrairement aux liens de document, vous avez besoin du « documentFolderId » du dossier de Workfront dans lequel vous souhaitez placer votre nouveau lien. Il s’agit probablement du même dossier parent que le dossier lié que nous copions.

>[!CAUTION]
>
>Les dossiers ne sont pas stockés temporairement. Ne supprimez pas les anciens dossiers. Désactivez l’intégration du document personnalisée dans la zone de configuration pour supprimer les anciens dossiers.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API DOCS : (points d’entrée de lien interne non actuellement couverts à l’adresse developer.workfront.com)

## Termes importants

* **Document** : ressource numérique dans Workfront

* **Dossier de documents** : conteneur pour les ressources numériques dans Workfront

* **ID du document** : ID interne Workfront d’une ressource numérique

* **ID du dossier de documents** : ID interne Workfront pour un dossier de ressources numériques

* **ID de fournisseur de documents** : identifiant associé à des fournisseurs de documents spécifiques

>[!IMPORTANT]
>
> Pour tout type de fournisseur de documents donné, un client ou une cliente peut avoir plusieurs instances connectées. Par exemple, plusieurs référentiels AEM peuvent être liés. Ou plusieurs instances Google Drive liées. L’ID de fournisseur de documents indique l’instance spécifique du type de connexion que nous voulons remplacer ou changer.

* **Type de fournisseur de stockage de documents (également « Type d’intégration externe »)** : type d’intégration du fournisseur de stockage de documents prise en charge par Workfront. Soit via une intégration dédiée, soit via une « intégration personnalisée ».

* **Types de fournisseurs de stockage de documents actuels (providerType)** :

  ```
  ATTASK
  BOX
  GOOGLE
  SHAREPOINT
  WEBDAM
  WORKFRONTDAM
  INFERNO
  WIDEN
  DROPBOX
  DROPBOX_BUSINESS
  ONEDRIVE
  QUIP
  WEBHOOKS
  AEM
  MOCK
  ```

* **Document lié** : ressource numérique hébergée par un fournisseur externe de stockage de documents. Workfront aura son propre « ID de document » interne pour la ressource, mais les octets sont stockés en externe. Pour faciliter cette opération, Workfront stocke également un « ID de document externe » afin de faciliter la localisation de la ressource référencée en externe dans le référentiel distant ou entrepôt.

* **Dossier du document lié** : un conteneur pour les ressources numériques hébergées par un fournisseur externe de stockage de documents. Workfront aura son propre « ID de dossier de document » interne pour la ressource, mais les octets sont stockés en externe. Pour faciliter cette opération, Workfront stocke également un « ID de document externe » afin de faciliter la localisation de la ressource référencée en externe dans le référentiel distant ou entrepôt.

* **ID de document externe : ID attribué lorsque les ressources sont stockées en dehors de Workfront.** Workfront mappe son identifiant interne à l’identifiant utilisé pour localiser la ressource dans le système externe, via ce champ « identifiant de document externe ». Par conséquent, lors de la liaison du document ou du dossier à partir d’un nouvel entrepôt externe, un nouvel identifiant de document externe doit être composé, dans le format approprié, pour que le fournisseur de documents externe identifie le document dans le nouveau référentiel ou le nouvel entrepôt.

  >[!NOTE]
  >
  > Workfront ne dispose pas encore d’une norme pour les identifiants de document externe. Une nouvelle spécification est en cours d’utilisation pour les ID d’AEM, mais pour les autres ID, l’ID de document externe peut prendre différentes formes selon le type de fournisseur.


* **Type d’objet : il s’agit d’un terme d’API uniquement aux fins de ce document.** Il s’agit d’un type d’objet générique dans Workfront avec lequel vous souhaitez interagir. Dans ce cas, vous interagissez avec des documents et des dossiers de type « DOCU » et « DOCFDR » respectivement.

* **Identifiant d’objet** : l’identifiant Workfront interne de l’objet générique avec lequel vous souhaitez interagir. Vous interagissez avec des documents et des dossiers, ce qui correspond respectivement à l’ID de document ou à l’ID de dossier de document.
