---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Azure DevOps
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL Azure DevOps] et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1777'
ht-degree: 29%

---

# Modules [!DNL Azure DevOps]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Azure DevOps] et les connecter à plusieurs applications et services tiers.

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

## Conditions préalables

Pour utiliser les modules [!DNL Azure DevOps], vous devez disposer d’un compte [!DNL Azure] DevOps.

## Connecter [!DNL Azure DevOps] à [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. Ajoutez un module [!DNL Azure DevOps] à votre scénario.
1. Cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion] .
1. Dans le champ [!UICONTROL Type de connexion], sélectionnez **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >Le type de connexion [!UICONTROL [!DNL Azure DevOps] (Demander toutes les portées)] sera bientôt obsolète. Par conséquent, nous vous déconseillons de l’utiliser.

1. Renseignez les champs suivants :

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Connection name]</td>
            <td>Saisissez un nom pour la connexion que vous créez.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>Saisissez le nom de l'organisation sous laquelle vous avez créé votre application [!DNL Azure DevOps].</td>
        </tr>
    </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour terminer la configuration de la connexion et continuer la création de votre scénario.

## Modules [!UICONTROL Azure DevOps] et leurs champs

Lorsque vous configurez des modules [!DNL Azure DevOps], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Azure DevOps] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)
* [Recherches](#searches)

### Déclencheurs

#### [!UICONTROL Rechercher des tâches]

Ce module de déclenchement instantané exécute un scénario lorsqu’un enregistrement est ajouté, mis à jour ou supprimé dans [!UICONTROL Azure DevOps].

Le module renvoie les champs standard associés à l’enregistrement, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Sélectionnez ou ajoutez un webhook pour le module.</p> <p>Pour plus d’informations sur les webhooks dans les modules de déclenchement, voir <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant Triggers (webhooks) dans [!DNL Adobe Workfront Fusion]</a>.</p> <p>Pour plus d’informations sur la création d’un webhook, voir <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [Appel API personnalisé](#custom-api-call)
* [Lecture d’enregistrement](#read-record)
* [Création d’un enregistrement](#create-a-record)
* [Mise à jour d’un élément de travail](#update-a-work-item)
* [[!UICONTROL Télécharger une pièce jointe]](#upload-an-attachment)
* [Télécharger une pièce jointe](#download-an-attachment)
* [Lier les éléments de travail]([!UICONTROL #link-work-items])

#### [!UICONTROL Appel API personnalisé]

Ce module d’action vous permet d’effectuer un appel authentifié personnalisé à l’API [!DNL Azure DevOps]. Ainsi, vous pouvez créer une automatisation du flux de données qui ne peut pas être réalisée par les autres modules [!DNL Azure DevOps].

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Azure DevOps] à [!DNL Workfront Fusion], voir <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Azure DevOps] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Base URL]</td> 
   <td> <p>Sélectionnez ou mappez l’URL de base que vous utilisez pour vous connecter à votre compte [!DNL Azure DevOps].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL relative]</td> 
   <td> <p>Saisissez l’URL relative à laquelle vous souhaitez vous connecter pour cet appel API.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemple : </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Sélectionnez ou mappez la version de l’API [!DNL Azure DevOps] à laquelle vous souhaitez vous connecter pour cet appel API. Si aucune version n’est sélectionnée, [!DNL Workfront Fusion] se connecte à l’API [!DNL Azure DevOps] version 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Par exemple : <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :  <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lecture d’enregistrement]

Ce module d’action lit les données d’un seul enregistrement dans [!DNL Azure DevOps].

Vous spécifiez l’identifiant de l’enregistrement.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Azure DevOps] à [!DNL Workfront Fusion], voir <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Azure DevOps] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td> <p>Indiquez si vous souhaitez lire un projet ou un élément de travail.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> : sélectionnez le projet à lire.</p> </li> 
     <li> <p><strong>[!UICONTROL Élément de travail]</strong> : sélectionnez le projet contenant l’élément de travail à lire, puis sélectionnez le type d’élément de travail.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les informations que vous souhaitez inclure dans le lot de sortie pour ce module. Les champs disponibles dépendent du type d’élément de travail.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de l’enregistrement que vous souhaitez lire.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un enregistrement]

Ce module d’action crée un projet ou une tâche.

Le module génère l’identifiant d’objet pour l’élément de travail nouvellement créé, ou l’URL et le code d’état d’un projet nouvellement créé.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Azure DevOps] à [!DNL Workfront Fusion], voir <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Azure DevOps] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’enregistrement]</td> 
   <td> <p>Indiquez si vous souhaitez créer un élément de travail ou un projet.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>Renseignez les champs suivants :</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong> : saisissez ou mappez un nom pour le nouveau projet.</p> </li> 
       <li> <p><strong>[!UICONTROL Description]</strong> : entrez ou mappez une description pour le nouveau projet. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibilité]</strong> : choisissez si vous souhaitez que votre projet soit public ou privé. Les utilisateurs doivent être connectés à votre organisation et avoir accès au projet pour pouvoir interagir avec un projet privé. Les projets publics sont visibles par les utilisateurs qui ne sont pas connectés à votre entreprise.</p> </li> 
       <li> <p><strong>[!UICONTROL Contrôle de version]</strong> : choisissez si vous souhaitez que le projet utilise [!DNL Git] ou [!UICONTROL Team Foundation Version Control (TFCV)] pour le contrôle de version.</p> </li> 
       <li> <p><strong>[!UICONTROL Processus de l’élément de travail]</strong> : sélectionnez le processus de travail à utiliser pour le projet. Les options sont [!UICONTROL Basic], [!UICONTROL Scrum], [!UICONTROL Capability Maturity Model Integration (CMMI)] et [!UICONTROL Agile].</p> <p>Pour plus d'informations sur les processus [!DNL Azure DevOps], voir <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Choose a Process</a> dans la documentation [!DNL Azure DevOps].</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Élément de travail]</strong> </p> <p>Renseignez les champs suivants :</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong> : sélectionnez le projet dans lequel vous souhaitez créer l’élément de travail.</p> </li> 
       <li> <p><strong>[!UICONTROL Type d’élément de travail]</strong> : sélectionnez le type d’élément de travail à créer.</p> </li> 
       <li> <p><strong>[!UICONTROL Autres champs]</strong> : dans ces champs, saisissez la valeur que l’élément de travail doit avoir pour une propriété donnée. Les champs disponibles dépendent du type d’élément de travail.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un élément de travail]

Ce module d’action met à jour un élément de travail existant à l’aide de son identifiant.

Le module renvoie l’identifiant de l’élément de travail mis à jour.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Azure DevOps] à [!DNL Workfront Fusion], voir <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Azure DevOps] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Sélectionnez le projet qui contient l’élément de travail que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’élément de travail]</td> 
   <td> <p>Sélectionnez le type d’élément de travail que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Autres champs]</td> 
   <td>Dans chacun de ces champs, saisissez la valeur que l’élément de travail doit avoir pour une propriété donnée. Les champs disponibles dépendent du type d’élément de travail.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de l’élément de travail]</td> 
   <td>Saisissez ou mappez l’identifiant de l’élément de travail que vous souhaitez mettre à jour.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger une pièce jointe]

Ce module d’action télécharge un fichier et le joint à un élément de travail.

Le module renvoie l’identifiant de la pièce jointe et une URL de téléchargement pour la pièce jointe.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Azure DevOps] à [!DNL Workfront Fusion], voir <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Azure DevOps] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>Sélectionnez le projet dans lequel vous souhaitez charger une pièce jointe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de l’élément de travail]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’élément de travail dans lequel vous souhaitez charger une pièce jointe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Saisissez le texte d’un commentaire à ajouter à la pièce jointe chargée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file] </td> 
   <td>Sélectionnez un fichier source à partir d’un module précédent ou saisissez ou mappez le nom et le contenu du fichier source.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Télécharger une pièce jointe]

Ce module d’action télécharge une pièce jointe.

Le module renvoie le contenu du fichier de la pièce jointe.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Azure DevOps] à [!DNL Workfront Fusion], voir <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Azure DevOps] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL de la pièce jointe]</td> 
   <td> <p>Saisissez ou mappez l’URL de la pièce jointe à télécharger.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lier les éléments de travail]

Ce module d’action relie deux éléments de travail et définit la relation entre eux.

Le module renvoie l’identifiant de l’élément de travail principal et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Azure DevOps] à [!DNL Workfront Fusion], voir <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Azure DevOps] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de l’élément de travail]</td> 
   <td>Saisissez ou mappez l’identifiant de l’élément de travail principal auquel vous souhaitez lier un autre élément de travail.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’élément de travail lié]</td> 
   <td>Saisissez ou mappez l’identifiant de l’élément de travail que vous souhaitez lier à l’élément de travail principal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de lien]</td> 
   <td> <p>Définissez la relation entre les tâches que vous souhaitez lier.</p> <p>Pour plus d’informations, voir <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">Référence du type de lien</a> dans la documentation [!UICONTROL Azure DevOps].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Saisissez ou mappez le texte d’un commentaire. Cela s’avère utile pour expliquer le raisonnement ou l’intention du lien.</td> 
  </tr> 
 </tbody> 
</table>

### Recherches

#### [!UICONTROL Liste des éléments de travail]

Ce module d’action récupère toutes les tâches d’un type spécifique dans un projet [!DNL Azure DevOps].

Le module renvoie l’identifiant de l’élément de travail principal et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!DNL Azure DevOps] à [!DNL Workfront Fusion], voir <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connexion de [!DNL Azure DevOps] à [!UICONTROL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Sélectionnez le projet duquel vous souhaitez récupérer les tâches.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’élément de travail]</td> 
   <td> <p>Sélectionnez le type d’élément de travail que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. Les champs disponibles dépendent du type d’élément de travail que vous souhaitez récupérer. Vous devez sélectionner au moins une propriété.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’éléments de travail renvoyés par [!DNL Workfront Fusion] au cours d’un cycle d’exécution.</td> 
  </tr> 
 </tbody> 
</table>
