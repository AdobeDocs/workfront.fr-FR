---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules Trello
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent Trello et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '5095'
ht-degree: 6%

---

# Modules [!UICONTROL Trello]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!UICONTROL Trello] et les connecter à plusieurs applications et services tiers.

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

Pour utiliser les modules [!DNL Trello], vous devez disposer d&#39;un compte [!UICONTROL Trello].

## Connectez [!UICONTROL Trello] à [!DNL Workfront Fusion]

Pour plus d&#39;informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir [Création d&#39;une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Modules [!UICONTROL Trello] et leurs champs

Lorsque vous configurez les modules [!UICONTROL Trello], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de cela, d&#39;autres champs [!UICONTROL Trello] peuvent s&#39;afficher, selon des facteurs tels que votre niveau d&#39;accès dans l&#39;application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Panneaux](#boards)
* [Listes](#lists)
* [Vignettes](#cards)
* [Membres](#members)
* [Listes de contrôle](#checklists)
* [Libellés](#labels)
* [Commentaires](#comments)

### Panneaux

+++ **[!UICONTROL Panoramas de contrôle]**

Ce module de déclenchement commence un scénario lorsqu’un nouveau panorama est ajouté.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Le nombre maximal de panoramas [!DNL Workfront Fusion] est renvoyé au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer un panorama]**

Ce module d’action crée un panorama avec les paramètres sélectionnés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez ou mappez un nom pour le nouveau panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>Si nécessaire, saisissez ou mappez la description du panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’organisation]</p> </td> 
   <td> <p>Saisissez ou mappez l’ID de l’organisation. L’ID d’organisation peut être récupéré à l’aide d’un autre module, tel que le module Watch Activities.</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Niveau d’autorisation]</p> </td> 
   <td> <p>Les conseils d’administration disposent de règles de vote et de commentaire différentes pour chaque niveau d’autorisation. Par exemple : si votre panorama est [!UICONTROL Privé] et que vous définissez les règles de vote et de commentaire sur [!UICONTROL Tout], une erreur s’affiche. </p> <p>Le vote et les commentaires sont limités aux groupes suivants pour chaque niveau d’autorisation :</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong> : 
      —&gt;Membres, membres et observateurs</li> 
     <li><strong>[!UICONTROL Pour l’organisation]</strong> : 
      —&gt;Membres, membres et observateurs, membres de l’organisation</li> 
     <li><strong>[!UICONTROL Public]</strong> : 
      —&gt;Membres, membres et observateurs, membres de l’organisation, tous</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Vote]</p> </td> 
   <td> <p>Sélectionnez une option pour spécifier qui peut voter sur ce panorama. Consultez le champ [!UICONTROL Niveau d’autorisation] pour connaître les restrictions de vote pour les niveaux d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>Sélectionnez une option pour spécifier qui peut commenter les cartes de ce panorama. Consultez le champ [!UICONTROL Niveau d’autorisation] pour commenter les limites des niveaux d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invitations]</p> </td> 
   <td> <p>Sélectionnez qui peut inviter d’autres personnes à ce panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Auto-jointure]</p> </td> 
   <td> <p>Choisissez si les membres de l’équipe peuvent se joindre au panorama eux-mêmes ou doivent être invités.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Étiquettes par défaut]</p> </td> 
   <td> <p>Choisissez d’utiliser l’ensemble de libellés par défaut pour le nouveau panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Listes par défaut]</p> </td> 
   <td> <p>Indiquez si vous souhaitez ajouter le jeu de listes par défaut au panorama ([!UICONTROL À Faire], [!UICONTROL À Faire], [!UICONTROL À Faire], [!UICONTROL À Terminer]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID source du panorama]</p> </td> 
   <td> <p>Sélectionnez ou mappez l’identifiant du panorama que vous souhaitez copier dans le nouveau panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Couvertures De Carte]</p> </td> 
   <td> <p>Sélectionnez <strong>[!UICONTROL Oui]</strong> si vous souhaitez activer les couvertures de carte pour le panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Arrière-plan]</p> </td> 
   <td> <p>Sélectionnez la couleur de l’arrière-plan ou de l’arrière-plan personnalisé.</p> <p>Remarque : Les arrière-plans personnalisés sont disponibles uniquement pour les abonnés [!UICONTROL Trello Gold et Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL vieillissement des cartes]</p> </td> 
   <td> <p>Choisissez entre deux modes d’âge des cartes. </p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> : les cartes deviennent progressivement plus transparentes à mesure qu'elles vieillissent. </li> 
     <li><strong>[!UICONTROL Pirate]</strong> : les cartes déchireront, jaunes et craqueront comme une vieille carte pirate au fur et à mesure qu'elles vieillissent.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modifier un panorama]**

Ce module d’action modifie les paramètres d’un panorama existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de panorama]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant unique [!UICONTROL Trello] du panorama que vous souhaitez que le module crée. Vous pouvez récupérer l’ID de panorama à l’aide d’un autre module, tel que le module Panoramas de contrôle.</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouveau nom]</td> 
   <td> <p> Saisissez ou mappez un nouveau nom pour le panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouvelle description]</td> 
   <td> <p> Si nécessaire, saisissez ou mappez une nouvelle description du panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID d’organisation]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant unique [!UICONTROL Trello] du panorama que vous souhaitez que le module modifie. Vous pouvez récupérer l’ID de panorama à l’aide d’un autre module, tel que le module [!DNL Watch Activities].</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL S’abonner] </td> 
   <td> <p>Sélectionnez une option pour indiquer si l’utilisateur intérimaire est abonné au panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Niveau d’autorisation]</p> </td> 
   <td> <p>Les conseils d’administration disposent de règles de vote et de commentaire différentes pour chaque niveau d’autorisation. Par exemple : si votre panorama est [!UICONTROL Privé] et que vous définissez les règles de vote et de commentaire sur [!UICONTROL Tout], une erreur s’affiche. </p> <p>Le vote et les commentaires sont limités aux groupes suivants pour chaque niveau d’autorisation :</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong> : 
      —&gt;Membres, membres et observateurs</li> 
     <li><strong>[!UICONTROL Pour l’organisation]</strong> : 
      —&gt;Membres, membres et observateurs, membres de l’organisation</li> 
     <li><strong>[!UICONTROL Public]</strong> : 
      —&gt;Membres, membres et observateurs, membres de l’organisation, tous</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Vote]</p> </td> 
   <td> <p>Sélectionnez une option pour spécifier qui peut voter sur ce panorama. Consultez le champ [!UICONTROL Niveau d’autorisation] pour connaître les restrictions de vote pour les niveaux d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>Sélectionnez une option pour spécifier qui peut commenter les cartes de ce panorama. Consultez le champ [!UICONTROL Niveau d’autorisation] pour commenter les limites des niveaux d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invitations] </td> 
   <td> <p>Sélectionnez qui peut inviter des personnes à ce panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Auto-jointure]</td> 
   <td> <p> Choisissez si les membres de l’équipe peuvent se joindre au panorama eux-mêmes ou doivent être invités.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Couverture de carte]</td> 
   <td> <p> Indiquez si les couvertures de carte doivent s’afficher sur ce panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arrière-plan] </td> 
   <td> <p>Sélectionnez la couleur de l’arrière-plan ou de l’arrière-plan personnalisé.</p> <p>Remarque : Les arrière-plans personnalisés sont disponibles uniquement pour les abonnés [!UICONTROL Trello Gold et Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background ID]</td> 
   <td> <p> Si vous avez choisi d’utiliser un arrière-plan personnalisé dans le champ [!UICONTROL Arrière-plan] , saisissez ou mappez l’identifiant de l’arrière-plan que vous souhaitez utiliser.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL vieillissement des cartes]</p> </td> 
   <td> <p>Choisissez entre deux modes d’âge des cartes. </p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> : les cartes deviennent progressivement plus transparentes à mesure qu'elles vieillissent. </li> 
     <li><strong>[!UICONTROL Pirate]</strong> : les cartes déchireront, jaunes et craqueront comme une vieille carte pirate au fur et à mesure qu'elles vieillissent.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Flux Calendrier activé]</td> 
   <td> <p> Indiquez si le flux du calendrier est activé ou non.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;nom de l’étiquette de la couleur&gt;]</td> 
   <td> <p> Attribuez un nom au libellé de couleur de votre choix.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>Sélectionnez une option pour indiquer si vous souhaitez archiver (fermer) le panorama. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtenir un panorama]**

Ce module d’action récupère les détails d’un panorama.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de panorama]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant du panorama dont vous souhaitez récupérer les informations.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

Ce module de recherche récupère des informations sur un panorama que vous spécifiez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>Saisissez ou mappez le nom (ou une partie du nom) du panorama dont vous souhaitez obtenir des informations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de panoramas renvoyés]</td> 
   <td> <p> Saisissez le nombre maximal de panoramas [!DNL Workfront Fusion] qui seront renvoyés au cours d’un cycle d’exécution. Cette valeur doit être inférieure ou égale à 1 000.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partiel] </p> </td> 
   <td> <p>Par défaut, ce module recherche les correspondances exactes de chaque mot de votre requête dans le contenu des membres. Lorsque [!UICONTROL Partial] est activé, le module recherche du contenu commençant par n’importe quel mot de votre requête.</p> <p> Par exemple, si vous utilisez le mot "développement" pour rechercher un panorama intitulé "Mon rapport d’état de développement", vous devez rechercher le mot entier par défaut. Si [!UICONTROL Partial] est activé, vous pouvez rechercher "dev", mais pas "development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Panoramas] </td> 
   <td> <p>Entrez "mine" ou mappez une liste d’ID de panorama séparés par des virgules.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archiver ou ne plus archiver un panorama]**

Ce module d’action ferme ou rouvre un panorama que vous spécifiez .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de panorama]</td> 
   <td> <p> Saisissez ou mappez l’identifiant du panorama que vous souhaitez fermer ou rouvrir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archiver ou ne plus archiver]</td> 
   <td> <p> Indiquez si vous souhaitez fermer (archiver) ou rouvrir (ne plus archiver) le panorama.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Attribuer un membre à un panorama]**

Ce module d’action affecte un membre à un panorama que vous spécifiez .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de panorama]</td> 
   <td> <p> Sélectionnez le panorama sur lequel vous souhaitez ajouter un membre.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adresse électronique]</td> 
   <td> <p> Saisissez ou mappez l’adresse électronique du membre à ajouter au panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type de membre]</p> </td> 
   <td> <p>Sélectionnez le type de membre à ajouter au panorama.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong> : un administrateur de panorama peut effectuer toute action sur le panorama.</li> 
     <li><strong>[!UICONTROL Normal]</strong> : un membre normal est simplement membre du conseil d’administration.</li> 
     <li><strong>[!UICONTROL Observer]</strong> : un observateur est membre avec un accès en lecture seule au panorama. <br>Les observateurs ne sont disponibles que pour les équipes disposant de [!UICONTROL Trello Business Class].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom complet]</td> 
   <td> <p> Saisissez le nom complet de l’utilisateur à ajouter au panorama.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Annulation de l’affectation d’un membre d’un panorama]**

Ce module d’action supprime un membre du panorama.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de panorama]</td> 
   <td> <p> Saisissez (mappez ou sélectionnez) l’identifiant du panorama duquel vous souhaitez supprimer l’utilisateur.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Member] </td> 
   <td> <p>Sélectionnez le membre à supprimer du panorama.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listes

+++ **[!UICONTROL Carte-mémoire déplacée vers une liste]**

Ce module de déclenchement s’active lorsqu’une carte est déplacée vers une liste spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>Sélectionnez le panorama qui contient la liste à surveiller pour les cartes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List]</td> 
   <td>Sélectionnez la liste à surveiller pour les cartes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Le nombre maximal de cartes [!DNL Workfront Fusion] est renvoyé au cours d’un cycle d’exécution.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer une liste]**

Ce module d’action crée une liste sur un panorama que vous spécifiez .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de panorama]</td> 
   <td> <p> Saisissez ou mappez l’identifiant du panorama sur lequel vous souhaitez créer une liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez ou mappez un nom pour la nouvelle liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Indiquez si vous souhaitez ajouter la liste en haut ou l’ajouter au bas de la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copier la liste]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la liste que vous souhaitez copier.</p> 
    <ul> 
     <li> <p><strong>Entrez manuellement</strong> </p> <p>Dans le champ <strong>[!UICONTROL List ID]</strong>, saisissez ou mappez l’identifiant de la liste à copier.<br></p> </li> 
     <li> <p><strong>Select</strong> </p> <p>Sélectionnez le panorama qui contient la liste à copier, puis sélectionnez la liste.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modifier une liste]**

Ce module d&#39;action édite une liste existante.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de la liste que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez ou mappez un nouveau nom pour la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de panorama]</td> 
   <td> <p> Faites correspondre ou sélectionnez le panorama sur lequel vous souhaitez déplacer la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Indiquez si vous souhaitez ajouter la liste en haut ou l’ajouter au bas de la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abonné]</td> 
   <td> <p>Activez cette option si vous souhaitez abonner le membre actif à la liste.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtenir une liste]**

Ce module d’action récupère les détails d’une liste spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL List ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant de la liste dont vous souhaitez récupérer les informations.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Vignettes

+++ **[!UICONTROL Carte-attention]**

Ce module de déclenchement est activé lorsqu’une nouvelle carte est ajoutée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objet de contrôle]</td> 
   <td> <p>Sélectionnez l’emplacement à surveiller pour les cartes.</p> 
    <ul> 
     <li><strong>[!UICONTROL Toutes les cartes]</strong> </li> 
     <li> <p><strong>Cartes sur un panorama spécifique</strong> </p> <p>Sélectionnez le panorama à surveiller pour les cartes.</p> </li> 
     <li> <p><strong>[!UICONTROL Cartes sur une liste spécifique]</strong> </p> <p>Sélectionnez le panorama qui contient la liste à surveiller pour les cartes, puis sélectionnez la liste.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Le nombre maximal de cartes [!DNL Workfront Fusion] est renvoyé au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer une carte]**

Ce module d’action crée une carte dans une liste sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrez un ID de liste]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la liste dans laquelle vous souhaitez ajouter une carte.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL List ID]</strong>, saisissez ou mappez l’identifiant de la liste dans laquelle vous souhaitez ajouter une carte.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la liste à copier, puis sélectionnez la liste.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>Pour chaque libellé à ajouter à la carte, saisissez l'identifiant du libellé. L’ID peut être récupéré, par exemple à l’aide du module [!UICONTROL Récupérer les étiquettes] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members]</td> 
   <td>Pour chaque membre que vous souhaitez ajouter à la carte, saisissez l’identifiant du membre. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez le nom de la nouvelle carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Description]</p> </td> 
   <td> <p>Saisissez la description de la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Indiquez si vous souhaitez ajouter la carte en haut ou [!UICONTROL ajouter] la carte au bas de la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Échéance]</td> 
   <td> <p> Saisissez la date d’échéance de la carte. Pour consulter la liste des formats de date et d’heure pris en charge, voir la section <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Échéance terminée]</td> 
   <td> <p> Activez cette option pour marquer que la carte est terminée à la date d’échéance.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File URL]</td> 
   <td> <p>Saisissez ou mappez l’URL d’un fichier que vous souhaitez ajouter en tant que pièce jointe à la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Source file]</p> </td> 
   <td> <p>Saisissez ou mappez les informations d’un fichier à ajouter en tant que pièce jointe à la carte.</p> 
    <ul> 
     <li>[!UICONTROL Nom de fichier] : saisissez ou mappez le nom de fichier, y compris l’extension du fichier.</li> 
     <li> 
     <p>Sélectionner un fichier d’un module précédent ou mapper le nom et les données du fichier</p> 
     <p>Remarque : il existe une limite de chargement des fichiers de 10 Mo par pièce jointe. Cependant, les membres [!UICONTROL Business Class] et [!UICONTROL Trello Gold] ont une limite de 250 Mo pour le téléchargement de fichiers par pièce jointe.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copier la carte]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte à copier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL ID de carte]</strong>, saisissez ou mappez l’ID de la carte que vous souhaitez copier.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à copier, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modifier une carte]**

Ce module d’action modifie une carte existante.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saisir l’ID de carte]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte à modifier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL ID de carte]</strong>, saisissez ou mappez l’ID de la carte à modifier.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à modifier, sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouveau nom]</td> 
   <td> <p>Saisissez ou mappez un nouveau nom pour la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nouvelle description]</p> </td> 
   <td> <p>Saisissez ou mappez une nouvelle description pour la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Déplacer une carte]</p> </td> 
   <td> <p>Sélectionnez le panorama ou le panorama et la liste dans laquelle vous souhaitez déplacer la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>Ajoutez les identifiants des étiquettes à ajouter à la carte. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Indiquez si vous souhaitez ajouter la carte en haut ou [!UICONTROL ajouter] la carte au bas de la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Échéance]</td> 
   <td> <p> Saisissez la date d’échéance de la carte. Pour consulter la liste des formats de date et d’heure pris en charge, voir la section <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Échéance terminée]</td> 
   <td> <p> Si cette option est activée, la carte est marquée comme étant terminée à la date d’échéance.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members] </td> 
   <td> <p>Ajoutez ou mappez l’identifiant de tous les membres que vous souhaitez ajouter à la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de couverture de la pièce jointe]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant de la pièce jointe d’image que vous souhaitez que la carte utilise comme couverture.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL S’abonner] </td> 
   <td> <p>Indiquez si le membre doit être abonné à la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>Sélectionnez une option pour indiquer si vous souhaitez archiver (fermer) la carte. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtenir une carte]**

Ce module d’action récupère les détails d’une carte sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de panorama]</td> 
   <td> <p>Saisissez l’identifiant du panorama qui contient la carte dont vous souhaitez récupérer les détails. Vous pouvez ainsi afficher les noms des champs personnalisés du panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer l’ID de carte]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte dont vous souhaitez récupérer les détails.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL ID de carte]</strong>, saisissez ou mappez l’ID de la carte dont vous souhaitez récupérer les détails.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte dont vous souhaitez récupérer les détails, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Rechercher des cartes]**

Ce module d’action renvoie les cartes qui correspondent à la requête de recherche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>Sélectionnez les panoramas que vous souhaitez parcourir. Si aucun panorama n’est sélectionné, tous les panoramas seront recherchés.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Query]</p> </td> 
   <td> <p>Saisissez la requête de recherche. Vous pouvez affiner votre recherche à l’aide des opérateurs de recherche suivants :</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>Vous pouvez ajouter "-" à n’importe quel opérateur pour effectuer une recherche négative, par exemple <code>[!UICONTROL -has:members]</code> pour rechercher des cartes sans aucun membre affecté.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Renvoie les cartes affectées à un membre. Vous pouvez également utiliser <code>member:</code>. Utilisez <code>@me</code> pour inclure uniquement vos cartes.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Renvoie les cartes étiquetées. Vous pouvez également utiliser <code>label:</code>. Par exemple, <code>label:"FIX IT"</code> renverra des cartes avec le libellé "FIX IT".</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Renvoie les cartes d’un panorama spécifique. Par exemple, <code>board:Trello</code> renverra des cartes sur les panoramas dont le nom contient [!UICONTROL Trello].</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Renvoie les cartes de la liste nommée "name".</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Renvoie les cartes avec des pièces jointes. L’opérateur <code>has</code>: peut également être utilisé avec d’autres attributs, tels que <code>has:description</code>, <code>has:cover</code>, <code>has:members</code> ou <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Renvoie les cartes arrivées à expiration dans les 24 heures. L’opérateur <code>due:</code> peut également être utilisé avec d’autres délais, tels que <code>due:week</code>, <code>due:month</code> ou <code>due:overdue</code>. Vous pouvez également rechercher une période spécifique. Par exemple, l’ajout de <code>due:14</code> à la recherche inclut les cartes qui arriveront au cours des 14 prochains jours.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Renvoie les cartes créées au cours des dernières 24 heures. L’opérateur <code> created:</code> peut également être utilisé avec d’autres délais tels que <code>created:week</code> ou <code>created:month</code>. Vous pouvez également rechercher une période spécifique. Par exemple, l’ajout de <code>created:14</code> à la recherche inclut les cartes créées au cours des 14 derniers jours.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Renvoie les cartes modifiées au cours des dernières 24 heures. L’opérateur <code>edited:</code> peut également être utilisé avec d’autres délais, tels que <code>edited:week</code> ou <code>edited:month</code>. Vous pouvez également rechercher une période spécifique. Par exemple, l’ajout de <code>edited:21</code> à la recherche inclut les cartes modifiées au cours des 21 derniers jours.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Renvoie des cartes qui correspondent au texte des descriptions de carte, des listes de contrôle, des commentaires ou des noms. Par exemple, le commentaire : "FIX IT" renvoie des cartes avec "FIX IT" dans un commentaire.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Renvoie les cartes ouvertes ou archivées. Si aucun n’est spécifié, [!UICONTROL Trello] renvoie les deux types.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>Ne comprend que les cartes sur les tableaux de bord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de cartes renvoyées]</td> 
   <td> <p> Le nombre maximal de cartes [!DNL Workfront Fusion] est renvoyé au cours d’un cycle d’exécution. Cette valeur doit être inférieure ou égale à 1 000.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partiel] </td> 
   <td> <p>Par défaut, ce module recherche les correspondances exactes de chaque mot de votre requête dans le contenu des membres. Lorsque [!UICONTROL Partial] est activé, le module recherche du contenu commençant par n’importe quel mot de votre requête.</p> <p> Par exemple, si vous utilisez le mot "développement" pour rechercher un panorama intitulé "Mon rapport d’état de développement", vous devez rechercher le mot entier par défaut. Si [!UICONTROL Partial] est activé, vous pouvez rechercher "dev", mais pas "development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cards] </td> 
   <td> <p>Ajoutez toutes les cartes que vous souhaitez spécifiquement rechercher.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archiver ou ne plus archiver une carte]**

Ce module d’action archive ou renvoie une carte au panorama.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de carte]</td> 
   <td> <p> Saisissez ou mappez l’identifiant de la carte que vous souhaitez archiver ou renvoyer au panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archiver ou ne plus archiver]</td> 
   <td> <p> Indiquez si vous souhaitez fermer la carte (archiver) ou la renvoyer au panorama (ne plus archiver).</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Ajouter une pièce jointe]**

Ce module d’action ajoute une pièce jointe à la carte sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer l’ID de carte]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte dont vous souhaitez récupérer les détails.</p> 
    <ul> 
     <li> <p><strong>Entrez manuellement</strong> </p> <p>Dans le champ <strong>[!UICONTROL ID de carte]</strong>, saisissez ou mappez l’ID de la carte dont vous souhaitez récupérer les détails.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte dont vous souhaitez récupérer les détails, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type de pièce jointe]</p> </td> 
   <td> <p>Indiquez si vous souhaitez charger directement le fichier ou fournir une URL vers le fichier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Saisissez l’URL du fichier et attribuez un nom à la pièce jointe.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Membres

+++ **[!UICONTROL Attribuer un membre à un panorama]**

Voir &quot;[!UICONTROL Attribuer un membre à un panorama]&quot; sous [Panoramas](#boards).

+++

+++ **[!UICONTROL Annulation de l’affectation d’un membre d’un panorama]**

Voir &quot;[!UICONTROL Annulation de l’affectation d’un membre d’un panorama]&quot; sous [Panoramas](#boards).

+++

+++ **[!UICONTROL Ajouter un membre à une carte]**

Ce module d’action ajoute le membre spécifié à la carte spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Entrer l’ID de carte et l’ID de membre]</p> </td> 
   <td> <p>Choisissez le mode de saisie de l’ID de carte et de l’ID de membre.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Saisissez ou mappez les <strong>[!UICONTROL ID de carte]</strong> et <strong>[!UICONTROL ID de membre]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama contenant la carte à laquelle vous souhaitez ajouter un membre, puis sélectionnez la liste contenant la carte, la carte elle-même et le membre à ajouter à la carte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Recherche de membres]**

Ce module d’action récupère des informations sur les membres [!UICONTROL Trello].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>Saisissez le nom complet ou le nom d’utilisateur de l’utilisateur que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partiel] </td> 
   <td> <p>Par défaut, ce module recherche les correspondances exactes de chaque mot de votre requête dans le contenu des membres. Lorsque [!UICONTROL Partial] est activé, le module recherche du contenu commençant par n’importe quel mot de votre requête.</p> <p> Par exemple, si vous utilisez le mot "développement" pour rechercher un panorama intitulé "Mon rapport d’état de développement", vous devez rechercher le mot entier par défaut. Si [!UICONTROL Partial] est activé, vous pouvez rechercher "dev", mais pas "development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de membres renvoyés]</td> 
   <td> <p> Le nombre maximal de membres [!DNL Workfront Fusion] est renvoyé au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listes de contrôle

+++ **[!UICONTROL Créer une liste de contrôle]**

Ce module d’action crée une liste de contrôle sur la carte sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saisissez un ID de carte]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte dans laquelle vous souhaitez ajouter une liste de contrôle.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL ID de carte]</strong>, saisissez ou mappez l’ID de la carte dans laquelle vous souhaitez ajouter une liste de contrôle.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous souhaitez ajouter une liste de contrôle, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez ou mappez un nom pour la liste de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Indiquez si vous souhaitez ajouter la liste de contrôle en haut ou [!UICONTROL ajouter la liste de contrôle au bas de la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Entrer l’ID de liste de contrôle]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant d’une liste de contrôle source que vous souhaitez copier dans la nouvelle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer un élément de liste de contrôle]**

Ce module d’action ajoute un élément à une liste de contrôle spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer l’ID de liste de contrôle]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la liste de contrôle dans laquelle vous souhaitez ajouter un élément.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Checklist ID]</strong> , saisissez ou mappez l’identifiant de la carte dans laquelle vous souhaitez ajouter une liste de contrôle.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous souhaitez ajouter une liste de contrôle, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte, puis sélectionnez la liste de contrôle.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nom de l’élément]</p> </td> 
   <td> <p>Saisissez ou mappez un nom pour le nouvel élément.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Indiquez si vous souhaitez ajouter l’élément en haut ou [!UICONTROL ajouter] en bas de la liste de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Vérifié]</p> </td> 
   <td> <p>Activez cette option si vous souhaitez ajouter l’élément comme déjà coché.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modifier un élément de liste de contrôle]**

Ce module d’action édite une liste de contrôle existante.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saisissez un ID de carte et un ID d’élément de liste de contrôle]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte et de la liste de contrôle dans laquelle vous souhaitez modifier un élément.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Checklist ID]</strong> , saisissez ou mappez l’identifiant de la carte dans laquelle vous souhaitez ajouter une liste de contrôle.</p> <p>Dans le champ <strong>[!UICONTROL Checklist Item ID]</strong> , saisissez ou mappez l’identifiant de la liste de contrôle.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous souhaitez ajouter une liste de contrôle, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte, puis sélectionnez la liste de contrôle.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Checlist ID]</td> 
   <td>Sélectionnez ou mappez la liste de contrôle vers laquelle vous souhaitez déplacer l’élément de liste de contrôle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nom de l’élément]</p> </td> 
   <td> <p>Saisissez ou mappez un nom pour le nouvel élément.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Indiquez si vous souhaitez ajouter l’élément en haut ou en bas de la liste de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL State]</p> </td> 
   <td> <p>Indiquez si l’élément de liste de contrôle est terminé ou incomplet.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Libellés

+++ **[!UICONTROL Ajouter un libellé à une carte]**

Ce module d’action ajoute un libellé à une carte sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrer l’ID de carte]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte dans laquelle vous souhaitez ajouter une liste de contrôle.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL ID de carte]</strong>, saisissez ou mappez l’ID de la carte dans laquelle vous souhaitez ajouter une liste de contrôle. Dans le champ<strong>[!UICONTROL ID d’étiquette]</strong>, saisissez ou mappez l’ID de l’étiquette que vous souhaitez ajouter.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous souhaitez ajouter une liste de contrôle, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte. </p> <p>Sélectionnez le libellé à ajouter à la carte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Commentaires

+++ **[!UICONTROL Regarder les commentaires]**

Récupère les détails du commentaire lorsqu’un nouveau commentaire se trouve à un emplacement spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objet de contrôle]</td> 
   <td> <p>Sélectionnez l’emplacement à surveiller pour les commentaires.</p> 
    <ul> 
     <li><strong>[!UICONTROL Toutes les cartes] partout{1</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>Sélectionnez le panorama que vous souhaitez consulter pour les commentaires.</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>Sélectionnez le panorama qui contient la liste à regarder pour les commentaires, puis sélectionnez la liste.</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>Sélectionnez le panorama qui contient la carte à surveiller pour les commentaires, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Le nombre maximal de commentaires [!DNL Workfront Fusion] est renvoyé au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer un commentaire dans une carte]**

Ce module d’action ajoute un commentaire à une carte sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saisissez un ID de carte]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte dans laquelle vous souhaitez ajouter un commentaire.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL ID de carte]</strong>, saisissez ou mappez l’ID de la carte dans laquelle vous souhaitez ajouter un commentaire.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama contenant la carte sur laquelle vous souhaitez ajouter un commentaire, puis sélectionnez la liste contenant la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment] </td> 
   <td> <p>Saisissez le commentaire à ajouter à la carte sélectionnée.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Lister des commentaires dans une carte]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour plus d’informations sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Saisissez un ID de carte]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’identifiant de la carte dans laquelle vous souhaitez ajouter un commentaire.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrée manuelle]</strong> </p> <p>Dans le champ <strong>[!UICONTROL ID de carte]</strong>, saisissez ou mappez l’ID de la carte dans laquelle vous souhaitez ajouter un commentaire.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama contenant la carte sur laquelle vous souhaitez ajouter un commentaire, puis sélectionnez la liste contenant la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de commentaires renvoyés]</td> 
   <td> <p> Saisissez le nombre maximal de commentaires [!DNL Workfront Fusion] qui seront renvoyés au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Depuis] </td> 
   <td> <p>Définissez la date de début de la période pendant laquelle le commentaire a été créé. Pour consulter la liste des formats de date et d’heure pris en charge, voir la section <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Avant] </td> 
   <td> <p>Définissez la date de fin de la période pendant laquelle le commentaire a été créé. Pour consulter la liste des formats de date et d’heure pris en charge, voir la section <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL Trello] ID d’objet

* [Comment trouver l’identifiant ou le raccourci d’une carte dans [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [Comment trouver les identifiants d’autres objets dans [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### Comment trouver l&#39;identifiant ou le raccourci d&#39;une carte dans [!DNL Trello]

Si vous souhaitez modifier une carte ou créer un commentaire, vous devez connaître l’identifiant de la carte ou son lien court. Vous pouvez obtenir ces informations à partir de la sortie du déclencheur [!UICONTROL New Card]. Vous pouvez également obtenir le raccourci d’une carte en ouvrant la carte et en cliquant sur le bouton [!UICONTROL Partager] . Le lien court se trouve dans la zone [!UICONTROL Lien vers cette carte], à la fin de l’URL après `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### Comment trouver les identifiants d&#39;autres objets dans [!DNL Trello]

Les ID de panorama, de liste et de commentaire ne peuvent être obtenus qu’à l’aide de déclencheurs. Le site web [!DNL trello.com] n’affiche pas ces identifiants.
