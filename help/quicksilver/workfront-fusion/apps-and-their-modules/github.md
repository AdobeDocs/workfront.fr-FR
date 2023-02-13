---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules GitHub
description: Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les processus qui utilisent GitHub et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 0%

---

# [!DNL GitHub] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!UICONTROL GitHub], ainsi que de la connecter à plusieurs applications et services tiers.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL GitHub] modules, vous devez disposer d’un [!DNL GitHub] compte .

## Connexion [!DNL GitHub] to [!DNL Workfront Fusion]

Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!UICONTROL Workfront Fusion], voir [Créer une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] et leurs champs.

Lorsque vous configurez [!DNL GitHub] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL GitHub] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)

### Triggers

* [[!UICONTROL Problèmes de contrôle]](#watch-issues)
* [[!UICONTROL Repository]](#watch-repositories)
* [[!UICONTROL Branchements surveillés]](#watch-forks)
* [[!UICONTROL Regarder les commentaires]](#watch-comments)
* [[!UICONTROL Regarder les requêtes de tirage]](#watch-pull-requests)

#### [!UICONTROL Problèmes de contrôle]

Ce module se déclenche lorsqu’un nouveau problème est ajouté ou qu’un problème existant est modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Je veux regarder]</td> 
   <td>Indiquez si vous souhaitez consulter tous les référentiels ou un seul référentiel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Si vous avez choisi de ne regarder les problèmes que dans un seul référentiel, sélectionnez le référentiel à regarder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de problèmes renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Indiquez si vous souhaitez ne surveiller que les nouveaux problèmes ou les nouveaux problèmes et toutes les modifications.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Vous pouvez filtrer les problèmes que vous souhaitez surveiller en fonction de la manière dont vous y êtes associé.</p> 
    <ul> 
     <li>[!UICONTROL Tous les problèmes]</li> 
     <li>[!UICONTROL Uniquement les problèmes qui m’ont été affectés]</li> 
     <li>[!UICONTROL Problèmes uniquement créés par moi]</li> 
     <li>[!UICONTROL Problèmes me mentionnant uniquement]</li> 
     <li>[!UICONTROL Uniquement les problèmes pour lesquels je suis abonné aux mises à jour]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Choisissez si vous souhaitez ne regarder que les problèmes en cours ou uniquement les problèmes fermés. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Ajoutez une balise. Le module recherche les problèmes liés à cette balise.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Repository]

Ce module se déclenche lorsqu’un référentiel est créé ou modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de référentiels renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Indiquez si vous souhaitez rechercher de nouveaux référentiels et toutes les modifications, ou uniquement de nouveaux référentiels.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Branchements surveillés]

Ce module se déclenche lors de la création d’un branchement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel que vous souhaitez surveiller pour les branchements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de branchements renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder les commentaires]

Ce module se déclenche lorsqu’un nouveau commentaire est ajouté ou qu’un commentaire existant est modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel que vous souhaitez regarder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Numéro de problème]</td> 
   <td>Si vous souhaitez limiter la recherche en recherchant uniquement les nouveaux commentaires apportés à un problème spécifique, saisissez le numéro de problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de problèmes renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Choisissez si vous souhaitez ne regarder que les nouveaux commentaires ou les commentaires et toutes les modifications.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder les requêtes de tirage]

Ce module se déclenche lorsqu’une nouvelle requête de tirage est ajoutée ou qu’une requête de tirage existante est modifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel que vous souhaitez regarder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de demandes d’extraction renvoyées]</td> 
   <td>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Indiquez si vous souhaitez surveiller les demandes [!UICONTROL Ouvrir uniquement], [!UICONTROL Uniquement fermées] ou toutes les demandes d’extraction. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Indiquez si vous souhaitez ne surveiller que les nouvelles demandes d’extraction ou les nouvelles demandes d’extraction et toutes les modifications.</td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [[!UICONTROL Recherche d’un problème]](#search-for-an-issue)
* [[!UICONTROL Créer un événement]](#create-an-issue)
* [[!UICONTROL Mettre à jour un problème]](#update-an-issue)
* [[!UICONTROL Obtention d’un problème]](#get-an-issue)
* [[!UICONTROL Ajouter des personnes désignées]](#add-assignees)
* [[!UICONTROL Suppression des personnes désignées]](#remove-assignees)
* [[!UICONTROL Ajout d’étiquettes à un problème]](#add-labels-to-an-issue)
* [[!UICONTROL Supprimer une étiquette d’un problème]](#remove-a-label-from-an-issue)
* [[!UICONTROL Créer un commentaire]](#create-a-comment)
* [[!UICONTROL Lister des commentaires]](#list-comments)

#### [!UICONTROL Recherche d’un problème]

Ce module recherche des problèmes qui correspondent à vos critères de recherche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de problèmes renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera pendant un cycle (nombre de répétitions par exécution de scénario). </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trier par]</td> 
   <td> <p>Sélectionnez le mode de tri des résultats de la recherche.</p> 
    <ul> 
     <li> <p>[!UICONTROL Meilleure correspondance] </p> </li> 
     <li>[!UICONTROL Date de création]</li> 
     <li>[!UICONTROL Date de mise à jour]</li> 
     <li>[!UICONTROL Nombre de commentaires]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Direction du tri]</td> 
   <td> <p>Sélectionnez ascendant ou descendant. </p> <p>Pour les dates, sélectionnez <strong>[!UICONTROL descendant]</strong> renvoie d’abord la date la plus récente. </p> <p>Pour [!UICONTROL au nombre de commentaires], en sélectionnant <strong>[!UICONTROL descendant]</strong> renvoie d’abord le problème avec le plus grand nombre de commentaires.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Saisissez ou mappez votre requête de recherche. Pour obtenir une description détaillée des options de recherche, voir <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">Problèmes de recherche et requêtes d’extraction</a> sur le [!DNL GitHub] site d’aide.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un événement]

Ce module crée un problème dans le référentiel sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel dans lequel vous souhaitez créer un problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cessionnaire]</td> 
   <td>Sélectionnez les personnes que vous souhaitez affecter au problème. Les personnes désignées disponibles incluent toute personne disposant d’autorisations d’écriture sur le référentiel et les membres de l’organisation disposant d’autorisations de lecture sur le référentiel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Sélectionnez le jalon que vous souhaitez associer au nouveau problème. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Sélectionnez les étiquettes à appliquer au nouveau problème. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Saisissez ou mappez un titre pour le nouveau problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Saisissez ou mappez le corps du problème, par exemple une description ou des informations supplémentaires.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un problème]

Ce module met à jour un [!DNL GitHub] problème.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel dans lequel vous souhaitez mettre à jour un problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cessionnaire]</td> 
   <td>Sélectionnez les personnes que vous souhaitez affecter au problème. Les personnes désignées disponibles incluent toute personne disposant d’autorisations d’écriture sur le référentiel et les membres de l’organisation disposant d’autorisations de lecture sur le référentiel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone]</td> 
   <td>Sélectionnez le jalon que vous souhaitez associer au problème. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Sélectionnez les étiquettes à appliquer au problème. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Saisissez ou mappez le numéro du problème que vous souhaitez mettre à jour. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Sélectionnez l’état dans lequel vous souhaitez mettre à jour le problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Saisissez ou mappez un titre pour le problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Saisissez ou mappez le corps du problème, par exemple une description ou des informations supplémentaires.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un problème]

Ce module récupère les détails du problème spécifié

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel contenant le problème sur lequel vous souhaitez récupérer les détails.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Saisissez ou mappez le numéro du problème dont vous souhaitez récupérer les détails. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter des personnes désignées]

Ce module ajoute des personnes désignées au problème spécifié

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel contenant le problème auquel vous souhaitez ajouter les personnes désignées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cessionnaire]</td> 
   <td>Sélectionnez les personnes que vous souhaitez affecter au problème. Les personnes désignées disponibles incluent toute personne disposant d’autorisations d’écriture sur le référentiel et les membres de l’organisation disposant d’autorisations de lecture sur le référentiel. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Saisissez ou mappez le numéro du problème auquel vous souhaitez ajouter des personnes désignées. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression des personnes désignées]

Ce module supprime les personnes désignées du problème spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel contenant le problème à partir duquel vous souhaitez supprimer les personnes désignées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cessionnaire]</td> 
   <td>Sélectionnez les personnes que vous souhaitez supprimer du problème. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Saisissez ou mappez le numéro du problème à partir duquel vous souhaitez supprimer les personnes désignées. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajout d’étiquettes à un problème]

Ce module ajoute des étiquettes à un problème. Les libellés sont définis au niveau du référentiel et ne peuvent être créés que par une personne disposant d’un accès en écriture au référentiel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel contenant le problème auquel vous souhaitez ajouter des libellés.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Sélectionnez les étiquettes à ajouter au problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Saisissez ou mappez le numéro du problème auquel vous souhaitez ajouter des étiquettes.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une étiquette d’un problème]

Ce module supprime un seul libellé d’un problème.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel contenant le problème à partir duquel vous souhaitez supprimer un libellé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels]</td> 
   <td>Sélectionnez le libellé à supprimer du problème.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Saisissez ou mappez le numéro du problème à partir duquel vous souhaitez supprimer un libellé.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un commentaire]

Ce module crée un commentaire sur le problème spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel contenant le problème sur lequel vous souhaitez créer un commentaire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Saisissez ou mappez le numéro du problème sur lequel vous souhaitez créer un commentaire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Saisissez ou mappez le contenu du commentaire.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lister des commentaires]

Ce module répertorie tous les commentaires sur le problème spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL GitHub] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel contenant le problème à partir duquel vous souhaitez répertorier les commentaires.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number]</td> 
   <td>Saisissez ou mappez le numéro du problème à partir duquel vous souhaitez répertorier les commentaires.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Depuis]</td> 
   <td>Le module renvoie les commentaires créés après cette date. Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de commentaires renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] fonctionnera avec pendant un cycle. </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
