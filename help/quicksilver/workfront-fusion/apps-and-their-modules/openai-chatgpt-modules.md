---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules OpenAI (ChatGPT)
description: Dans un scénario Adobe Workfront Fusion, vous pouvez automatiser les workflows qui utilisent OpenAIT (ChatGPT) et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 3a747013-5fb6-4416-8d95-d656dfeeb7db
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '1320'
ht-degree: 23%

---

# Modules [!DNL OpenAI (ChatGPT & DALL-E)]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL OpenAI (ChatGPT & DALL-E)] et les connecter à plusieurs applications et services tiers.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL OpenAI (ChatGPT & DALL-E)], vous devez disposer d&#39;un compte [!DNL OpenAI], incluant une clé API et un ID d&#39;organisation.

## Connexion de [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre compte [!DNL OpenAI (ChatGPT & DALL-E)] directement depuis un module [!DNL OpenAI (ChatGPT & DALL-E)].

1. Dans un module [!DNL OpenAI (ChatGPT & DALL-E)], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Renseignez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Saisissez un nom pour la nouvelle connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Clé API]</td> 
      <td>Vous pouvez localiser votre clé d’API dans les paramètres utilisateur d’OpenAI.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID d’organisation] </td> 
      <td>Vous pouvez trouver votre ID d’organisation sur votre page Paramètres de l’organisation dans OpenAI.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.


## Modules [!DNL OpenAI (ChatGPT & DALL-E)] et leurs champs

Lorsque vous configurez des modules [!DNL OpenAI (ChatGPT & DALL-E)], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL OpenAI (ChatGPT & DALL-E)] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Création d’une fin

>[!IMPORTANT]
>
>Ce module a été abandonné.

<!--

This action module creates a completion for the provided prompt or chat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Enter or map the ID of the model to use. You can use the Get models module to see all of your available models. </td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Temperature]</td> 
   <td> This value must be between 0 and 2, and determines the randomness of the output. Higher values produce output that is more random, while lower values produce more focused output. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating completions in the <a href="https://platform.openai.com/docs/api-reference/completions/create" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### Création d’une modération

Ce module d’action détermine si le texte enfreint la politique de contenu d’OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> Pour chaque exemple de texte à inclure, cliquez sur <b>Ajouter un élément</b> et saisissez ou mappez le texte. Incluez l’échantillon de texte entier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Saisissez ou mappez l’identifiant du modèle à utiliser. Vous pouvez utiliser le module Get models pour afficher tous vos modèles disponibles. </td> 
  </tr> 
 </tbody> 
</table>

### Création d’une modification

Ce module d’action renvoie une version modifiée d’une invite que vous fournissez, en suivant vos instructions.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Saisissez ou mappez l’identifiant du modèle à utiliser. Vous pouvez utiliser le module Get models pour afficher tous vos modèles disponibles. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> Saisissez ou mappez le texte à modifier. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Instruction]</td> 
   <td> Saisissez ou mappez les instructions pour la modification. Exemple : "Corrigez les fautes d’orthographe." </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Paramètres avancés]</td> 
   <td> <p>Pour plus d’informations sur les paramètres avancés facultatifs de ce module, voir les informations sur la création de modifications dans la <a href="https://platform.openai.com/docs/api-reference/edits/create" class="MCXref xref">documentation de l’API OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Création d’une incorporation

Ce module d’action crée un vecteur d’incorporation représentant le texte d’entrée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Saisissez ou mappez l’identifiant du modèle à utiliser. Vous pouvez utiliser le module Get models pour afficher tous vos modèles disponibles. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texte d’entrée à incorporer]</td> 
   <td> Saisissez ou mappez le texte à incorporer. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User ID]</td> 
   <td> Saisissez ou mappez un identifiant unique représentant votre utilisateur final, qui peut aider OpenAI à surveiller et détecter les abus. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Saisissez ou mappez le nombre maximal de modifications que le module doit effectuer au cours de chaque cycle d’exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

### Créer l’achèvement de la conversation

Avec une liste de messages décrivant une conversation, ce module d’action renvoie une réponse.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Saisissez ou mappez l’identifiant du modèle à utiliser. Vous pouvez utiliser le module Get models pour afficher tous vos modèles disponibles. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>Les messages décrivent la conversation jusqu'à présent. Pour chaque message à ajouter, cliquez sur <b>Ajouter un élément</b> et renseignez les éléments suivants :
   <ul>
   <li> <b>Rôle</b> : sélectionnez le rôle de l’auteur de ce message.</li>
   <li> <b>Contenu</b> : entrez ou mappez le contenu de ce message.</li>
   <li> <b>Nom</b> : saisissez ou mappez le nom de l’auteur de ce message. Le nom peut contenir des lettres majuscules et minuscules, des chiffres et des traits de soulignement. La longueur maximale du nom est de 64 caractères.</li>
   </ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Paramètres avancés]</td> 
   <td> <p>Pour plus d’informations sur les paramètres avancés facultatifs de ce module, consultez les informations sur la création de sessions de chat dans la <a href="https://platform.openai.com/docs/api-reference/chat/create" class="MCXref xref">documentation de l’API OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Edit image

This action module makes edits or creates variations of existing images.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to create edits or variations of the image.
   <p>NOTE: Images must be a valid PNG file, less than 4MB, and square. If mask is not provided, the image must have transparency, which will be used as the mask.</p> 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Text description of desired image]</td> 
   <td> <p>If editing an image, enter or map a description of the edits you want to create. Maximum length is 1000 characters.</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating image edits or variations in the <a href="https://platform.openai.com/docs/api-reference/images/createEdit" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### Générer des images

Ce module d’action génère ou manipule des images avec des modèles Dall-E.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description textuelle de l’image désirée]</td> 
   <td> Saisissez ou mappez une description de l’image souhaitée. La longueur maximale de la description est de 1 000 caractères. 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Paramètres avancés]</td> 
   <td> <p>Pour plus d’informations sur les paramètres avancés facultatifs de ce module, voir les informations sur la création d’images dans la <a href="https://platform.openai.com/docs/api-reference/images/create" class="MCXref xref">documentation de l’API OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Obtention de modèles

Ce module répertorie et décrit les différents modèles disponibles dans l’API OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> Indiquez si vous souhaitez obtenir une liste de tous les modèles ou récupérer un modèle spécifique.
    <ul>
    <li><p><b>Modèles de liste </b></p><p>Cette action répertorie les modèles actuellement disponibles et fournit des informations de base sur chacun d’eux, telles que le propriétaire et la disponibilité.</p></li>
    <li><p><b>Récupération du modèle </b></p><p>Saisissez ou mappez l’identifiant du modèle que vous souhaitez récupérer. </p></li>
   </ul>
 </td> 
 </tbody> 
</table>

### Lancer un appel API personnalisé

Ce module d’action est une requête HTTP personnalisée à l’API OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Saisissez un chemin relatif à <code>https://api.openai.com/v1/</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard.</p> <p>Par exemple, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion ajoute automatiquement les en-têtes d’autorisation.</p> </td> 
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

<!--

### Manage Audio

This action modules converts audio to text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to transcribe the audio into the input language, or into English.
   <p>If transcribing into the input language, you can select the language in this module's advanced settings. </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Enter or map the maximum number of edits you want the module to work with during each scenario execution cycle.</td> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating transcriptions in the <a href="https://platform.openai.com/docs/api-reference/audio/createTranscription" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

-->

### Gestion des fichiers

Ce module d’action répertorie, supprime ou récupère des fichiers ou du contenu de fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> Sélectionnez l’action que vous souhaitez effectuer. 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID de fichier]</td> 
   <td> Si vous supprimez un fichier ou que vous récupérez un contenu de fichier ou de fichier, saisissez ou mappez l’identifiant du fichier. 
  </tr> 
</tbody>
</table>

### Gestion des réglages

Gérez des tâches d’optimisation pour personnaliser un modèle en fonction de vos données de formation spécifiques.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL OpenAI (ChatGPT & DALL-E)] à Workfront Fusion, reportez-vous à la section <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connexion [!DNL OpenAI (ChatGPT & DALL-E)] à [!DNL Workfront Fusion]</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sélectionner l’opération]</td> 
   <td> Sélectionnez l’action que vous souhaitez effectuer.
   <ul>
   <li><p>Ajuster un modèle à partir d’un jeu de données</p><p>Saisissez ou mappez une description pour l’image souhaitée.</p>
     <li><p>Obtenir des informations sur une tâche d’optimisation</p><p>Saisissez ou mappez l’identifiant de la tâche.</p>
   <li><p>Annulation d’une tâche d’optimisation</p><p>Saisissez ou mappez l’identifiant de la tâche.</p>
   <li><p>Annulation d’une tâche d’optimisation</p><p>Saisissez ou mappez l’identifiant de la tâche.</p>
   <li><p>Obtenir des mises à jour d’état pour une tâche d’optimisation</p><p>Saisissez ou mappez l’identifiant de la tâche, puis indiquez si vous souhaitez diffuser ces mises à jour.</p>
   <li><p>Suppression d’un modèle affiné</p><p>Saisissez ou mappez l’identifiant du modèle que vous souhaitez supprimer.</p>
 </ul> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID de fichier]</td> 
   <td> Si vous supprimez un fichier ou que vous récupérez un contenu de fichier ou de fichier, saisissez ou mappez l’identifiant du fichier. 
  </tr> 
</tbody>
