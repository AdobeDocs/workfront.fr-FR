---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules Trello
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '5165'
ht-degree: 89%

---

# Modules [!UICONTROL Trello]

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans l’article :
>
>* [Modules Trello](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/trello-modules.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!UICONTROL Trello], et le connecter à de multiples applications et services tiers.

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : si vous disposez du plan de [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter du [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Trello], vous devez disposer d’un compte [!UICONTROL Trello].

## Informations sur l’API Trello

Le connecteur Trello utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td> https://api.trello.com/1</td>
  </tr> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v4.12.37</td> 
  </tr>
 </tbody> 
 </table>

## Connecter [!UICONTROL Trello] à [!DNL Workfront Fusion]

Pour savoir comment connecter votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], voir la section [Créer une connexion à  [!DNL Adobe Workfront Fusion]  - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Modules [!UICONTROL Trello] et leurs champs

Lorsque vous configurez les modules [!UICONTROL Trello], [!DNL Workfront Fusion] affiche les champs énumérés ci-dessous. En plus de ces champs, d’autres champs [!UICONTROL Trello] peuvent s’afficher, en fonction de facteurs tels que votre niveau d’accès à l’application ou au service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir la section [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Panneaux](#boards)
* [Listes](#lists)
* [vignette](#cards)
* [Membres](#members)
* [Listes de contrôle](#checklists)
* [Libellés](#labels)
* [Commentaires](#comments)

### Panneaux

+++ **[!UICONTROL Surveiller les panoramas]**

Ce module déclencheur lance un scénario lorsqu’un nouveau panorama est ajouté.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Nombre maximum de panoramas que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer un panorama]**

Ce module d’action crée un nouveau panorama avec les paramètres sélectionnés.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez ou mappez un nom pour le nouveau panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>Saisissez ou mappez la description du panorama si nécessaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’ID de l’organisation. L’ID de l’organisation peut être récupéré à l’aide d’un autre module, tel que le module Surveiller les activités.</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Permission level]</p> </td> 
   <td> <p>Les panoramas possèdent des règles de vote et de commentaire différentes pour chaque niveau d’autorisation. Par exemple : si votre panorama est [!UICONTROL Private] et que vous définissez les règles de vote et de commentaire sur [!UICONTROL All], vous recevez une erreur. </p> <p>Le vote et les commentaires sont limités aux groupes suivants pour chaque niveau d’autorisation :</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong> : 
--&gt;Personnes membres, Personnes membres et observatrices</li> 
     <li><strong>[!UICONTROL For organization]</strong> : 
--&gt;Personnes membres, Personnes membres et observatrices, Personnes membres de l’organisation</li> 
     <li><strong>[!UICONTROL Public]</strong> : 
--&gt;Personnes membres, Personnes membres et observatrices, Personnes membres de l’organisation, Tous</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>Sélectionnez une option pour spécifier qui peut voter sur ce panorama. Reportez-vous au champ [!UICONTROL Permission level] pour en savoir plus sur les limitations de vote en fonction des niveaux d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>Sélectionnez une option pour spécifier qui peut commenter les cartes de ce panorama. Reportez-vous au champ [!UICONTROL Permission level] pour en savoir plus sur les limitations de commentaires en fonction des niveaux d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invitations]</p> </td> 
   <td> <p>Sélectionnez qui peut inviter d’autres personnes dans ce panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Self-join]</p> </td> 
   <td> <p>Indiquez si les personnes membres de l’équipe peuvent rejoindre le panorama elles-mêmes ou si elles doivent être invitées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Default labels]</p> </td> 
   <td> <p>Choisissez d’utiliser ou non le jeu de libellés par défaut pour le nouveau panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Default lists]</p> </td> 
   <td> <p>Choisissez d’ajouter ou non l’ensemble des listes par défaut au panorama ([!UICONTROL To Do], [!UICONTROL Doing], [!UICONTROL Done]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board source ID]</p> </td> 
   <td> <p>Sélectionnez ou mappez l’ID du panorama que vous souhaitez copier dans le nouveau panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card Covers]</p> </td> 
   <td> <p>Sélectionnez <strong>[!UICONTROL Yes]</strong> si vous souhaitez activer les couvertures de cartes du panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Background]</p> </td> 
   <td> <p>Sélectionnez la couleur de l’arrière-plan ou de l’arrière-plan personnalisé.</p> <p>Note : les arrière-plans personnalisés sont disponibles uniquement pour les personnes abonnées à [!UICONTROL Trello Gold and Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card aging]</p> </td> 
   <td> <p>Choisissez entre deux modes d’expiration des cartes. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong> : les cartes deviennent progressivement plus transparentes à mesure qu’elles vieillissent. </li> 
     <li><strong>[!UICONTROL Pirate]</strong> : les cartes se déchirent, jaunissent et se craquellent comme une vieille carte de pirate à mesure qu’elles vieillissent.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modifier un panorama]**

Ce module d’action permet de modifier les paramètres d’un panorama existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’ID unique [!UICONTROL Trello] du panorama que vous voulez que le module crée. Vous pouvez récupérer l’ID du panorama à l’aide d’un autre module, tel que le module Surveiller les panoramas.</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td> <p> Saisissez ou mappez un nouveau nom pour le panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New description]</td> 
   <td> <p> Saisissez ou mappez une nouvelle description du panorama si nécessaire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>Entrez ou mappez l’identifiant unique [!UICONTROL Trello] du panorama que vous voulez que le module modifie. Vous pouvez récupérer l’identifiant du panorama à l’aide d’un autre module, tel que le module [!DNL Watch Activities].</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>Sélectionnez une option pour indiquer si la personne est abonnée au panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Permission level]</p> </td> 
   <td> <p>Les panoramas possèdent des règles de vote et de commentaire différentes pour chaque niveau d’autorisation. Par exemple : si votre panorama est [!UICONTROL Private] et que vous définissez les règles de vote et de commentaire sur [!UICONTROL All], vous recevez une erreur. </p> <p>Le vote et les commentaires sont limités aux groupes suivants pour chaque niveau d’autorisation :</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong> : 
--&gt;Personnes membres, Personnes membres et observatrices</li> 
     <li><strong>[!UICONTROL For organization]</strong> : 
--&gt;Personnes membres, Personnes membres et observatrices, Personnes membres de l’organisation</li> 
     <li><strong>[!UICONTROL Public]</strong> : 
--&gt;Personnes membres, Personnes membres et observatrices, Personnes membres de l’organisation, Tous</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>Sélectionnez une option pour spécifier qui peut voter sur ce panorama. Reportez-vous au champ [!UICONTROL Permission level] pour en savoir plus sur les limitations de vote en fonction des niveaux d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>Sélectionnez une option pour spécifier qui peut commenter les cartes de ce panorama. Reportez-vous au champ [!UICONTROL Permission level] pour en savoir plus sur les limitations de commentaires en fonction des niveaux d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invitations] </td> 
   <td> <p>Indiquez qui peut inviter des personnes sur ce panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-join]</td> 
   <td> <p> Indiquez si les personnes membres de l’équipe peuvent rejoindre le panorama elles-mêmes ou si elles doivent être invitées.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card covers]</td> 
   <td> <p> Indiquez si les couvertures de cartes doivent être affichées sur ce panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background] </td> 
   <td> <p>Sélectionnez la couleur de l’arrière-plan ou de l’arrière-plan personnalisé.</p> <p>Note : les arrière-plans personnalisés sont disponibles uniquement pour les personnes abonnées à [!UICONTROL Trello Gold and Business Class].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background ID]</td> 
   <td> <p> Si vous avez choisi d’utiliser un arrière-plan personnalisé dans le champ [!UICONTROL Background], saisissez ou mappez l’identifiant de l’arrière-plan que vous souhaitez utiliser.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card aging]</p> </td> 
   <td> <p>Choisissez entre deux modes d’expiration des cartes. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong> : les cartes deviennent progressivement plus transparentes à mesure qu’elles vieillissent. </li> 
     <li><strong>[!UICONTROL Pirate]</strong> : les cartes se déchirent, jaunissent et se fissurent comme une vieille carte de pirate à mesure qu’elles vieillissent.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar feed enabled]</td> 
   <td> <p> Indiquez si le flux de calendrier est activé ou pas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Color&gt; label name]</td> 
   <td> <p> Affectez un nom au libellé de couleur souhaité.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>Sélectionnez une option pour indiquer si vous souhaitez archiver (fermer) le panorama. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtenir un panorama]**

Ce module d’action permet de récupérer les détails d’un panorama.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’identifiant du panorama pour lequel vous souhaitez obtenir des informations.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

Ce module de recherche permet d’obtenir des informations sur un panorama indiqué.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>Saisissez ou mappez le nom (ou une partie du nom) du panorama sur lequel vous souhaitez obtenir des informations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned boards]</td> 
   <td> <p> Saisissez le nombre maximum de panoramas que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution. Cette valeur doit être inférieure ou égale à 1 000.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partial] </p> </td> 
   <td> <p>Par défaut, ce module recherche dans le contenu des personnes membres les correspondances exactes de chaque mot de votre requête. Lorsque [!UICONTROL Partial] est activé, le module recherche le contenu qui commence par n’importe quel mot de votre requête.</p> <p> Par exemple, si vous utilisez le mot « développement » pour rechercher un panorama intitulé « Rapport sur le statut de mon développement », vous devrez, par défaut, rechercher le mot dans son intégralité. Si vous avez activé [!UICONTROL Partial], vous pourrez rechercher « dév » mais pas « veloppement ».</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Boards] </td> 
   <td> <p>Saisissez « À moi » ou mappez une liste d’identifiants de panoramas séparés par des virgules.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archiver ou désarchiver un panorama]**

Ce module d’action ferme ou rouvre un panorama que vous spécifiez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Saisissez ou mappez l’ID du panorama que vous souhaitez fermer ou rouvrir.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive or unarchive]</td> 
   <td> <p> Choisissez de fermer (archiver) ou de rouvrir (désarchiver) le panorama.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Affecter une personne membre à un panorama]**

Ce module d’action affecte une personne membre à un panorama que vous spécifiez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Sélectionnez le panorama dans lequel vous souhaitez ajouter une personne membre.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email address]</td> 
   <td> <p> Saisissez ou mappez l’adresse e-mail de la personne membre que vous souhaitez ajouter au panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Member type]</p> </td> 
   <td> <p>Sélectionnez le type de personne membre que vous souhaitez ajouter au panorama.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong> : un administrateur ou une administratrice de panorama peut effectuer n’importe quelle action sur le panorama.</li> 
     <li><strong>[!UICONTROL Normal]</strong> : une personne membre normale est simplement membre du panorama.</li> 
     <li><strong>[!UICONTROL Observer]</strong> : une personne observatrive est une personne membre ayant un accès en lecture seule au panorama. <br>Les observateurs et observatrices ne sont disponibles que pour les équipes avec [!UICONTROL Trello Business Class].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Full name]</td> 
   <td> <p> Saisissez le nom complet de la personne que vous souhaitez ajouter au panorama.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Retirer l’affectation d’une personne membre à un panorama]**

Ce module d’action permet de supprimer une personne membre d’un panorama.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Saisissez (mappez ou sélectionnez) l’ID du panorama duquel vous voulez supprimer la personne.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Member] </td> 
   <td> <p>Sélectionnez la personne membre que vous souhaitez supprimer du panorama.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listes

+++ **[!UICONTROL Surveiller les cartes ajoutées à une liste]**

Ce module déclencheur s’active lorsqu’un panorama est déplacé vers une liste spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>Sélectionnez le panorama qui contient la liste dont vous souhaitez surveiller les cartes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List]</td> 
   <td>Sélectionnez la liste dont vous souhaitez surveiller les cartes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Nombre maximum de cartes que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer une liste]**

Ce module d’action crée une liste sur un panorama que vous spécifiez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Saisissez ou mappez l’ID du panorama dans lequel vous souhaitez créer une liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez ou mappez un nom pour la nouvelle liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Choisissez si vous souhaitez ajouter la liste en haut ou l’annexer au bas de la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy list]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’ID de la liste à copier.</p> 
    <ul> 
     <li> <p><strong>Saisir manuellement</strong> </p> <p>Dans le champ <strong>[!UICONTROL List ID]</strong>, saisissez ou mappez l’ID de la liste que vous souhaitez copier.<br></p> </li> 
     <li> <p><strong>Sélectionner</strong> </p> <p>Sélectionnez le panorama qui contient la liste que vous souhaitez copier, puis sélectionnez la liste.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modifier une liste]**

Ce module d’action permet de modifier une liste existante.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td> <p> Saisissez ou mappez l’ID de la liste que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez ou mappez un nouveau nom pour la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Mappez ou sélectionnez le panorama où vous souhaitez déplacer la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Choisissez si vous souhaitez ajouter la liste en haut ou l’annexer au bas de la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribed]</td> 
   <td> <p>Activez cette option si vous souhaitez abonner la personne membre active à la liste.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtenir une liste]**

Ce module d’action permet de récupérer les détails d’une liste spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL List ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’ID de la liste pour laquelle vous souhaitez récupérer des informations.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### vignette

+++ **[!UICONTROL Surveiller les cartes]**

Ce module déclencheur est activé lorsqu’une nouvelle carte est ajoutée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched object]</td> 
   <td> <p>Sélectionnez l’emplacement où vous souhaitez surveiller les cartes.</p> 
    <ul> 
     <li><strong>[!UICONTROL All cards]</strong> </li> 
     <li> <p><strong>Cartes sur un panorama spécifique</strong> </p> <p>Sélectionner le panorama dont vous souhaitez surveiller les cartes.</p> </li> 
     <li> <p><strong>[!UICONTROL Cards on specific list]</strong> </p> <p>Sélectionnez le panorama qui contient la liste dont vous souhaitez surveiller les cartes, puis la liste.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Nombre maximum de cartes que [!DNL Workfront Fusion] renvoie au cours d’un cycle d’exécution.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a list ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’ID de la liste dans laquelle vous souhaitez ajouter une carte.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL List ID]</strong>, saisissez ou mappez l’ID de la liste dans laquelle vous souhaitez ajouter une carte.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la liste que vous souhaitez copier, puis sélectionnez la liste.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>Pour chaque libellé que vous souhaitez ajouter à la carte, saisissez l’ID du libellé. L’ID peut être récupéré, par exemple, à l’aide du module [!UICONTROL Retrieve Labels].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members]</td> 
   <td>Saisissez l’ID de chaque personne membre que vous souhaitez ajouter à la carte. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez un nom pour la nouvelle carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Description]</p> </td> 
   <td> <p>Saisissez la description de la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Indiquez si vous souhaitez ajouter la carte en haut ou [!UICONTROL append] la carte en bas de la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due date]</td> 
   <td> <p> Saisissez une date d’échéance pour la carte. Pour une liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due complete]</td> 
   <td> <p> Activez cette option pour marquer que la carte est terminée à la date d’échéance.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File URL]</td> 
   <td> <p>Saisissez ou mappez l’URL d’un fichier que vous souhaitez ajouter en tant que pièce jointe à la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Source file]</p> </td> 
   <td> <p>Saisissez les informations du fichier que vous souhaitez ajouter en tant que pièce jointe à la carte.</p> 
    <ul> 
     <li>[!UICONTROL File name] : saisissez ou mappez le nom du fichier, y compris son extension.</li> 
     <li> 
     <p>Sélectionner un fichier à partir d’un module antérieur, ou mapper le nom et les données du fichier</p> 
     <p>Note : le chargement de fichiers est limité à 10 Mo par pièce jointe. Cependant, les personnes membres de [!UICONTROL Business Class] et [!UICONTROL Trello Gold] ont une limite de chargement de fichiers de 250 Mo par pièce jointe.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy card]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’ID de la carte que vous souhaitez copier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Card ID]</strong>, saisissez ou mappez l’ID de la carte que vous souhaitez copier.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à copier, puis la liste qui contient la carte, et enfin la carte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modifier une carte]**

Ce module d’action permet de modifier une carte existante.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Card ID]</td> 
   <td> <p> Sélectionnez le mode de saisie de l’ID de la carte que vous souhaitez modifier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Card ID]</strong>, saisissez ou mappez l’ID de la carte que vous souhaitez modifier.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte que vous souhaitez modifier, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td> <p>Saisissez ou mappez un nouveau nom pour la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL New description]</p> </td> 
   <td> <p>Saisissez ou mappez une nouvelle description pour la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Move a card]</p> </td> 
   <td> <p>Sélectionnez le panorama ou le panorama et la liste où vous souhaitez déplacer la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>Ajoutez les ID des libellés que vous souhaitez ajouter à la carte. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Indiquez si vous souhaitez ajouter la carte en haut ou [!UICONTROL append] la carte en bas de la liste.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due date]</td> 
   <td> <p> Saisissez une date d’échéance pour la carte. Pour une liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due complete]</td> 
   <td> <p> Si cette option est activée, la carte est marquée comme terminée à la date d’échéance.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members] </td> 
   <td> <p>Ajoutez ou mappez l’ID des personnes membres que vous souhaitez ajouter à la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachment cover ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’ID de l’image jointe que vous souhaitez que la carte utilise comme couverture.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>Indiquez si la personne membre doit être abonnée à la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>Sélectionnez une option pour indiquer si vous souhaitez archiver (fermer) la carte. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Obtenir une carte]**

Ce module d’action permet de récupérer les détails d’une carte sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p>Saisissez l’ID du panorama qui contient la carte dont vous souhaitez récupérer les détails. Cela vous permet de voir les noms des champs personnalisés du panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’ID de la carte dont vous souhaitez récupérer les détails.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Card ID]</strong>, saisissez ou mappez l’ID de la carte dont vous souhaitez récupérer les détails.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte dont vous voulez récupérer les détails, puis la liste qui contient la carte, et enfin la carte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Rechercher des cartes]**

Ce module d’action renvoie les cartes qui correspondent à la requête.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>Sélectionnez les panoramas dans lesquels vous souhaitez effectuer une recherche. Si vous ne sélectionnez aucun panorama, tous les panoramas seront inclus dans la recherche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Query]</p> </td> 
   <td> <p>Saisissez la requête. Vous pouvez affiner votre recherche en utilisant les opérateurs de recherche suivants :</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>Vous pouvez ajouter « - » à n’importe quel opérateur pour effectuer une recherche négative, par exemple <code>[!UICONTROL -has:members]</code> pour rechercher les cartes auxquelles aucune personne membre n’a été affectée.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Renvoie les cartes attribuées à une personne membre. Vous pouvez également utiliser <code>member:</code>. Utilisez <code>@me</code> pour inclure uniquement vos cartes.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Renvoie les cartes étiquetées. Vous pouvez également utiliser <code>label:</code>. Par exemple, <code>label:"FIX IT"</code> renverra les cartes avec le libellé « FIX IT ».</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Renvoie les cartes d’un panorama spécifique. Par exemple, <code>board:Trello</code> renverra des cartes sur des panoramas dont le nom contient [!UICONTROL Trello].</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Renvoie les cartes de la liste nommée « nom ».</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Renvoie les cartes avec des pièces jointes. L’opérateur <code>has</code>: peut également être utilisé avec d’autres attributs, tels que <code>has:description</code>, <code>has:cover</code>, <code>has:members</code> ou <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Renvoie les cartes dont l’échéance est dans les 24 prochaines heures. L’opérateur <code>due:</code> peut également être utilisé avec d’autres délais, tels que <code>due:week</code>, <code>due:month</code> ou <code>due:overdue</code>. Vous pouvez également rechercher une période spécifique. Par exemple, l’ajout de <code>due:14</code> à la recherche inclut les cartes dont l’échéance est dans les 14 prochains jours.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Renvoie les cartes créées au cours des dernières 24 heures. L’opérateur <code> created:</code> peut également être utilisé avec d’autres délais, tels que <code>created:week</code> ou <code>created:month</code>. Vous pouvez également rechercher une période spécifique. Par exemple, l’ajout de <code>created:14</code> à la recherche inclut les cartes créées au cours des 14 derniers jours.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Renvoie les cartes modifiées au cours des dernières 24 heures. L’opérateur <code>edited:</code> peut également être utilisé avec d’autres délais, tels que <code>edited:week</code> ou <code>edited:month</code>. Vous pouvez également rechercher une période spécifique. Par exemple, l’ajout de <code>edited:21</code> à la recherche inclut les cartes modifiées au cours des 21 derniers jours.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Renvoie les cartes correspondant au texte des descriptions, des listes de contrôle, des commentaires ou des noms de cartes. Par exemple, comment:"FIX IT" renverra les cartes dont le commentaire contient « FIX IT ».</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Renvoie les cartes ouvertes ou archivées. Si vous ne spécifiez aucun type, [!UICONTROL Trello] renvoie les deux.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>N’inclut que les cartes sur les panoramas marqués d’une étoile.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned cards]</td> 
   <td> <p> Nombre maximum de cartes que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution. Cette valeur doit être inférieure ou égale à 1 000.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>Par défaut, ce module recherche dans le contenu des personnes membres les correspondances exactes de chaque mot de votre requête. Lorsque [!UICONTROL Partial] est activé, le module recherche le contenu qui commence par n’importe quel mot de votre requête.</p> <p> Par exemple, si vous utilisez le mot « développement » pour rechercher un panorama intitulé « Rapport sur le statut de mon développement », vous devrez, par défaut, rechercher le mot dans son intégralité. Si vous avez activé [!UICONTROL Partial], vous pourrez rechercher « dév » mais pas « veloppement ».</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cards] </td> 
   <td> <p>Ajoutez les cartes que vous souhaitez rechercher spécifiquement.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archiver ou désarchiver une carte]**

Ce module d’action permet d’archiver ou de renvoyer une carte sur le panorama.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card ID]</td> 
   <td> <p> Saisissez ou mappez l’ID de la carte que vous souhaitez archiver ou renvoyer sur le panorama.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive or unarchive]</td> 
   <td> <p> Choisissez de fermer la carte (archiver) ou de la renvoyer sur le panorama (désarcher).</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’ID de la carte dont vous souhaitez récupérer les détails.</p> 
    <ul> 
     <li> <p><strong>Saisir manuellement</strong> </p> <p>Dans le champ <strong>[!UICONTROL Card ID]</strong>, saisissez ou mappez l’ID de la carte dont vous souhaitez récupérer les détails.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte dont vous voulez récupérer les détails, puis la liste qui contient la carte, et enfin la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachment type]</p> </td> 
   <td> <p>Indiquez si vous souhaitez charger le fichier directement ou fournir une URL vers le fichier.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Saisissez l’URL du fichier et donnez un nom à la pièce jointe.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Membres

+++ **[!UICONTROL Affecter une personne membre à un panorama]**

Voir « [!UICONTROL Affecter une personne membre à un panorama] » dans [Panoramas](#boards).

+++

+++ **[!UICONTROL Retirer l’affectation d’une personne membre à un panorama]**

Voir « [!UICONTROL Retirer l’affectation d’une personne membre à un panorama] » dans [Panoramas](#boards).

+++

+++ **[!UICONTROL Ajouter une personne membre à une carte]**

Ce module d’action ajoute la personne membre spécifiée à la carte spécifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Enter card ID and member ID]</p> </td> 
   <td> <p>Choisissez la manière dont vous souhaitez saisir l’ID de la carte et l’ID de la personne membre.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Saisissez ou mappez l’<strong>[!UICONTROL Card ID]</strong> et l’<strong>[!UICONTROL Member ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous souhaitez ajouter une personne membre, puis la liste qui contient la carte, la carte elle-même et enfin, la personne membre que vous souhaitez ajouter à la carte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Rechercher des personnes membres]**

Ce module d’action permet de récupérer des informations sur les personnes membres de [!UICONTROL Trello].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>Saisissez le nom complet ou le nom d’utilisateur ou d’utilisatrice de la personne que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>Par défaut, ce module recherche dans le contenu des personnes membres les correspondances exactes de chaque mot de votre requête. Lorsque [!UICONTROL Partial] est activé, le module recherche le contenu qui commence par n’importe quel mot de votre requête.</p> <p> Par exemple, si vous utilisez le mot « développement » pour rechercher un panorama intitulé « Rapport sur le statut de mon développement », vous devrez, par défaut, rechercher le mot dans son intégralité. Si vous avez activé [!UICONTROL Partial], vous pourrez rechercher « dév » mais pas « veloppement ».</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned members]</td> 
   <td> <p> Nombre maximum de personnes membres que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’ID de la carte sur laquelle vous souhaitez ajouter une liste de contrôle.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Card ID]</strong>, saisissez ou mappez l’ID de la carte à laquelle vous souhaitez ajouter une liste de contrôle.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous voulez ajouter une liste de contrôle, puis la liste qui contient la carte, et enfin la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Saisissez ou mappez un nom pour la liste de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Sélectionnez si vous souhaitez ajouter la liste de contrôle en haut ou [!UICONTROL append the] liste de contrôle en bas de la carte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Enter checklist ID]</p> </td> 
   <td> <p>Saisissez ou mappez l’ID d’une liste de contrôle source que vous souhaitez copier dans la nouvelle liste.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Créer un élément de la liste de contrôle]**

Ce module d’action ajoute un élément à une liste de contrôle spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter checklist ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’ID de la liste de contrôle à laquelle vous souhaitez ajouter un élément.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Checklist ID]</strong>, saisissez ou mappez l’ID de la carte à laquelle vous souhaitez ajouter une liste de contrôle.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous souhaitez ajouter une liste de contrôle, puis la liste qui contient la carte, puis la carte elle-même, et enfin la liste de contrôle.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Item name]</p> </td> 
   <td> <p>Saisissez ou mappez un nom pour le nouvel élément.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Sélectionnez si vous souhaitez ajouter l’élément en haut ou l’[!UICONTROL append] en bas de la liste de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Checked]</p> </td> 
   <td> <p>Activez cette option si vous souhaitez ajouter l’élément comme étant déjà contrôlé.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Modifier un élément de la liste de contrôle]**

Ce module d’action modifie une liste de contrôle existante.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a Card ID and Checklist Item ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’ID de la carte et la liste de contrôle où vous souhaitez modifier un élément.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Checklist ID]</strong>, saisissez ou mappez l’ID de la carte à laquelle vous souhaitez ajouter une liste de contrôle.</p> <p>Dans le champ <strong>[!UICONTROL Checklist Item ID]</strong>, saisissez ou mappez l’ID de la liste de contrôle.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous souhaitez ajouter une liste de contrôle, puis la liste qui contient la carte, puis la carte elle-même, et enfin la liste de contrôle.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Checklist ID]</td> 
   <td>Sélectionnez ou mappez la liste de contrôle vers laquelle vous souhaitez déplacer l’élément de liste de contrôle.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Item name]</p> </td> 
   <td> <p>Saisissez ou mappez un nom pour le nouvel élément.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Indiquez si vous souhaitez ajouter l’élément en haut ou l’ajouter en bas de la liste de contrôle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL State]</p> </td> 
   <td> <p>Indiquez si l’élément de la liste de contrôle est terminé ou non terminé.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Libellés

+++ **[!UICONTROL Ajouter un libellé à une carte]**

Ce module d’action ajoute un libellé à la carte sélectionnée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’ID de la carte sur laquelle vous souhaitez ajouter une liste de contrôle.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Card ID]</strong>, saisissez ou mappez l’identifiant de la carte sur laquelle vous souhaitez ajouter une liste de contrôle. Dans le champ <strong>[!UICONTROL Label ID]</strong>, saisissez ou mappez l’identifiant du libellé que vous souhaitez ajouter.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte à laquelle vous voulez ajouter une liste de contrôle, puis la liste qui contient la carte, et enfin la carte. </p> <p>Sélectionnez le libellé que vous souhaitez ajouter à la carte.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Commentaires

+++ **[!UICONTROL Surveiller les commentaires]**

Récupère les détails du commentaire lorsqu’il y a un nouveau commentaire dans un emplacement indiqué.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched object]</td> 
   <td> <p>Sélectionnez l’emplacement où vous souhaitez surveiller les commentaires.</p> 
    <ul> 
     <li><strong>[!UICONTROL All cards] partout</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>Sélectionnez le panorama dont vous souhaitez surveiller les commentaires.</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>Sélectionnez le panorama qui contient la liste dont vous voulez surveiller les commentaires, puis sélectionnez la liste.</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>Sélectionnez le panorama qui contient la carte dont vous voulez surveiller les commentaires, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Le nombre maximum de commentaires que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’identifiant de la carte sur laquelle vous souhaitez ajouter un commentaire.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Card ID]</strong>, saisissez ou mappez l’identifiant de la carte sur laquelle vous souhaitez ajouter un commentaire.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte sur laquelle vous souhaitez ajouter un commentaire, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment] </td> 
   <td> <p>Saisissez le commentaire que vous souhaitez ajouter à la carte sélectionnée.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Répertorier les commentaires dans une carte]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!UICONTROL Trello] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> Sélectionnez la manière dont vous souhaitez saisir l’identifiant de la carte sur laquelle vous souhaitez ajouter un commentaire.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Dans le champ <strong>[!UICONTROL Card ID]</strong>, saisissez ou mappez l’identifiant de la carte sur laquelle vous souhaitez ajouter un commentaire.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Sélectionnez le panorama qui contient la carte sur laquelle vous souhaitez ajouter un commentaire, puis sélectionnez la liste qui contient la carte, puis sélectionnez la carte.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned comments]</td> 
   <td> <p> Saisissez le nombre maximal de commentaires que [!DNL Workfront Fusion] renverra au cours d’un cycle d’exécution.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since] </td> 
   <td> <p>Définissez la date de début de la période au cours de laquelle le commentaire a été créé. Pour une liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before] </td> 
   <td> <p>Définissez la date de fin de la période au cours de laquelle le commentaire a été créé. Pour une liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## ID d’objets [!UICONTROL Trello]

* [Comment trouver l’ID ou le lien court d’une carte dans  [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [Comment trouver les ID d’autres objets dans  [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### Comment trouver l’ID ou le lien court d’une carte dans [!DNL Trello]

Si vous souhaitez modifier une carte ou créer un commentaire, vous devez connaître l’ID de la carte ou son lien court. Vous pouvez obtenir cette information à partir de la sortie du déclencheur [!UICONTROL Nouvelle carte]. Vous pouvez également obtenir le lien court d’une carte en ouvrant la carte et en cliquant sur le bouton [!UICONTROL Partager]. Le lien court se trouve dans la zone [!UICONTROL Lien vers cette carte], à la fin de l’URL après `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### Comment trouver les ID d’autres objets dans [!DNL Trello]

Les ID du panorama, de la liste et des commentaires ne peuvent être obtenus qu’à l’aide de déclencheurs. Le site web [!DNL trello.com] n’affiche pas ces ID.
