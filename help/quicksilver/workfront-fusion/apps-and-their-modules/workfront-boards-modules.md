---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Panoramas Adobe Workfront
description: Vous pouvez utiliser le connecteur des panoramas Adobe Workfront pour automatiser vos processus au sein des panoramas Workfront et les connecter à des applications et services tiers.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 0b4a25f7-a8f1-47f4-8929-7eff82f1dfdc
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2647'
ht-degree: 19%

---

# [!DNL Adobe Workfront] modules de panoramas

>[!NOTE]
>
>Le connecteur de fusion des panoramas est en version bêta. Par conséquent, la prise en charge de ce connecteur est limitée et peut changer en raison du développement futur des panoramas. En outre, des modifications peuvent être apportées à l’API GraphQL sans préavis, ce qui peut avoir une incidence sur votre processus de connecteur Fusion.

Les panoramas Adobe Workfront sont des outils flexibles qui permettent aux équipes de collaborer entre elles. Ils permettent d’accéder à un panorama partagé contenant des colonnes et des cartes.

Vous pouvez utiliser les modules Panoramas Adobe Workfront pour lire ou mettre à jour des enregistrements, effectuer un appel API vers l’API Panoramas Workfront ou déclencher un scénario lorsqu’une action se produit sur un panorama.

Pour obtenir des informations générales sur les panoramas Workfront, consultez la [présentation des panoramas](/help/quicksilver/agile/boards-overview.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>
  <td> <p>Tous</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td>
   <td> <p>Nouveau : Standard</p><p>Ou</p><p>Actuelle : [!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence</td> 
   <td>
   <p>Exigences de licence actuelles : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Exigences en matière de licences héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Conditions préalables

Vous devez avoir configuré un panorama dans Adobe Workfront avant de pouvoir vous y connecter.

## Informations sur l’API des panoramas Adobe Workfront

Le connecteur des panoramas Adobe Workfront utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>1.23.6</td> 
  </tr>
 </tbody> 
 </table>

## Création d’une connexion aux panoramas Workfront

>[!NOTE]
>
>Vous pouvez utiliser une connexion Workfront pour vous connecter aux panoramas Workfront ou créer une connexion à des panoramas Workfront distincte.

Pour créer une connexion aux panoramas Workfront :

1. Dans un module [!DNL Adobe Workfront Boards], cliquez sur **[!UICONTROL Ajouter]** en regard de la zone Connexion.

1. Remplissez les champs suivants :

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Saisissez un nom pour cette connexion.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Environment]</td>
          <td>Indiquez si vous vous connectez à un environnement de production ou hors production.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>Choisissez si vous souhaitez vous connecter à un compte de service ou à un compte personnel.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]<p>(Facultatif)</p></td>
          <td>Saisissez votre [!UICONTROL Client ID] [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] d’[!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]<p>(Facultatif)</p></td>
          <td>Saisissez votre [!UICONTROL Client Secret] [!DNL Adobe]. Vous pouvez le trouver dans la section [!UICONTROL Credentials details] d’[!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Authentication URL]<p>(Facultatif)</p></td>
          <td>Saisissez l’URL que votre instance de Workfront utilisera pour authentifier cette connexion. <p>La valeur par défaut est <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Host prefix]</td>
          <td>Saisissez votre préfixe d’hôte.<p>La valeur par défaut est <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. Cliquez sur **[!UICONTROL Continuer]** pour enregistrer la connexion et revenir au module.

## Modules des panoramas Adobe Workfront et leurs champs

Lorsque vous configurez les modules Panoramas Workfront, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de cela, d’autres champs de panoramas Workfront peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à l’autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [vignette](#cards)
* [Panneaux](#boards)
* [Colonnes](#columns)
* [Balises](#tags)
* [Commentaires](#comments)
* [Autre](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### vignette

* [Ajouter un élément de la liste de contrôle](#add-checklist-item)
* [Ajouter une sous-tâche](#add-subtask)
* [Création d’une carte](#create-a-card)
* [Déplacer une carte](#move-a-card)
* [Lecture d’une carte](#read-a-card)
* [Mettre à jour une carte](#update-a-card)

#### Ajouter un élément de la liste de contrôle

Ce module d’action ajoute un élément de liste de contrôle à la carte spécifiée.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la carte à laquelle vous souhaitez ajouter un élément de liste de contrôle.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Éléments de liste de contrôle]</td> 
   <td>Pour chaque élément de liste de contrôle à ajouter, cliquez sur Ajouter un élément, saisissez le nom de l’élément de liste de contrôle, puis indiquez si l’élément a été terminé.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Ajouter une sous-tâche

Ce module d’action ajoute une sous-tâche à une carte dans les panoramas. La carte doit être une carte connectée. La sous-tâche est également ajoutée à la tâche Workfront représentée par la carte.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de carte parente]</td> 
   <td>Saisissez ou mappez l’identifiant de la carte à laquelle vous souhaitez ajouter une sous-tâche.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama contenant la carte à laquelle vous souhaitez ajouter une sous-tâche.<p>L’identifiant du panorama figure dans l’URL lors de son affichage dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nom pour la nouvelle sous-tâche.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Création d’une carte

Ce module d’action crée une carte sur un panorama Workfront.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama auquel vous souhaitez ajouter une carte.<p>L’identifiant du panorama figure dans l’URL lors de son affichage dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de colonne]</td> 
   <td>Saisissez ou mappez l’identifiant de la colonne à laquelle vous souhaitez ajouter une sous-tâche.<p>L’identifiant de colonne figure dans les informations renvoyées à partir du module Lecture d’un panorama .</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nom pour la nouvelle carte.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Déplacer une carte

Ce module d’action déplace une carte vers une colonne différente sur le même panorama.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la carte que vous souhaitez déplacer.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama qui contient la carte que vous souhaitez déplacer.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de colonne de destination]</td> 
   <td>Saisissez ou mappez l’identifiant de la colonne vers laquelle vous souhaitez déplacer la carte.<p>L’identifiant de colonne figure dans les informations renvoyées à partir du module Lecture d’un panorama .</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pour indexer]</td> 
   <td>Saisissez ou mappez la position que vous souhaitez que la carte occupe dans la nouvelle colonne.<p>Position supérieure dans la colonne de l’index 0.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Lecture d’une carte

Ce module d’action récupère des informations sur une carte spécifique.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la carte que vous souhaitez lire.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Mettre à jour une carte

Ce module d’action met à jour les informations relatives à une carte que vous spécifiez.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la carte à mettre à jour.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama qui contient la carte à mettre à jour.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nouveau nom pour la carte.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Saisissez ou mappez une nouvelle description pour la carte.</p></td> 
  </tr> 
 </tbody> 
</table>

### Panneaux

* [Créer un panorama](#create-a-board)
* [Lire un panorama](#read-a-board)

#### Créer un panorama

Ce module d’action crée un panorama dans Workfront. Vous pouvez spécifier le type de panorama à créer.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom du panorama]</td> 
   <td>Saisissez ou mappez un nom pour le nouveau panorama.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td>Sélectionnez le type de panorama à créer.</td> 
  </tr> 
 </tbody> 
</table>

#### Lire un panorama

Ce module d’action renvoie des informations sur un seul panorama, telles que les cartes, colonnes, balises et membres du panorama.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama pour lequel vous souhaitez récupérer des informations.<p>L’identifiant du panorama figure dans l’URL lors de son affichage dans Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

### Colonnes

* [Création d’une colonne](#create-a-column)
* [Recherche d’une colonne](#search-for-a-column)
* [Mettre à jour une colonne](#update-a-column)

#### Création d’une colonne

Ce module d’action crée une nouvelle colonne sur le panorama spécifié.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama auquel vous souhaitez ajouter une colonne.<p>L’identifiant du panorama figure dans l’URL lors de son affichage dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de colonne]</td> 
   <td>Saisissez ou mappez l'identifiant de la colonne que vous souhaitez mettre à jour.<p>L’identifiant de colonne figure dans les informations renvoyées à partir du module Lecture d’un panorama .</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de la colonne]</td> 
   <td>Saisissez ou mappez un nouveau nom pour la colonne.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite de travaux en cours]</td> 
   <td>Saisissez ou mappez une nouvelle limite de travail en cours pour la colonne.</td> 
  </tr> 
 </tbody> 
</table>

#### Recherche d’une colonne

Ce module de recherche renvoie des informations sur la colonne portant le nom spécifié.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama qui contient la colonne que vous souhaitez récupérer.<p>L’identifiant du panorama figure dans l’URL lors de son affichage dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de colonne]</td> 
   <td>Saisissez ou mappez le nom de la colonne à récupérer.</td> 
  </tr> 
 </tbody> 
</table>

#### Mettre à jour une colonne

Ce module d’action met à jour la limite de nom ou de travail en cours de la colonne spécifiée.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama qui contient la colonne que vous souhaitez récupérer.<p>L’identifiant du panorama figure dans l’URL lors de son affichage dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de colonne]</td> 
   <td>Saisissez ou mappez le nom de la colonne à récupérer.</td> 
  </tr> 
 </tbody> 
</table>

### Balises

* [Ajouter une balise à une carte](#add-card-tag)
* [Création d’une balise](#create-a-tag)

#### Ajouter une balise à une carte

Ce module d’action ajoute une balise à une carte.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la carte à laquelle vous souhaitez ajouter une balise.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama contenant la carte à laquelle vous souhaitez ajouter une balise.<p>L’identifiant du panorama figure dans l’URL lors de son affichage dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la balise à ajouter.<p>Vous trouverez l’ID de balise dans les informations renvoyées à partir du module Lire un panorama .</p></td> 
  </tr> 
 </tbody> 
</table>

#### Création d’une balise

Ce module d’action crée une balise et lui attribue une couleur.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Saisissez ou mappez l’identifiant du panorama pour lequel vous souhaitez créer une balise.<p>L’identifiant du panorama figure dans l’URL lors de son affichage dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de balise]</td> 
   <td>Saisissez ou mappez le nom de la nouvelle balise.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Couleur de balise]</td> 
   <td>Sélectionnez la couleur de cette balise.</td> 
  </tr> 
 </tbody> 
</table>

### Commentaires

* [Créer un commentaire](#create-a-comment)
* [Lire les commentaires de carte](#read-card-comments)

#### Créer un commentaire

Ce module d’action a créé un commentaire sur la carte spécifiée.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la carte à laquelle vous souhaitez ajouter un commentaire.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>Saisissez ou mappez le texte du commentaire à ajouter.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Lire les commentaires de carte

Ce module d’action récupère les commentaires de la carte spécifiée.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la carte pour laquelle vous souhaitez récupérer les commentaires.<p>L’ID de carte figure dans l’URL lors de l’affichage de la carte dans Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Saisissez le nombre maximal de commentaires que le module doit renvoyer dans un cycle d’exécution.</p></td> 
  </tr> 
 </tbody> 
</table>

### Autre

#### Effectuer un appel API personnalisé.

Ce module d’action effectue un appel personnalisé à l’API des panoramas Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
      <td> <p>Vous pouvez utiliser une connexion Workfront existante pour vous connecter aux panoramas Workfront ou vous pouvez utiliser une connexion à des panoramas Workfront spécifique. </p><p>Pour plus d'informations sur la connexion de votre application [!DNL Workfront] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Création d'une connexion aux panoramas Workfront</a> de cet article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Saisissez un chemin relatif vers <code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p><p>Pour la plupart des appels de panorama, la méthode est POST. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Cela détermine le type de contenu de la requête.</p> <p>Par exemple,<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> <p>Pour les panoramas Workfront, cette section est généralement laissée vide.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un graphique JSON incorporé. </p> <p>Exemple :</p><p>Cet exemple met à jour un nom de colonne. Vous pouvez inclure les <code>boardId</code> et <code>columnId</code> comme GUID codés en dur ou mappés à partir d’un module précédent.<p><pre>{

  &quot;query&quot;: &quot;mutation { updateColumn(boardId: \&quot;\&quot;, columnId: \&quot;\&quot;, updateColumnInput: { name: \&quot;\&quot; }) { id name }}&quot;

}</pre><p>Note :  <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
