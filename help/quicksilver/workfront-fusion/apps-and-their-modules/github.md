---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Modules GitHub
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les processus qui utilisent GitHub et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1839'
ht-degree: 13%

---

# Modules [!DNL GitHub]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!UICONTROL GitHub], et les connecter à plusieurs applications et services tiers.

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

Pour utiliser les modules [!DNL GitHub], vous devez disposer d&#39;un compte [!DNL GitHub].

## Connecter [!DNL GitHub] à [!DNL Workfront Fusion]

Pour plus d’informations sur la connexion de votre compte [!DNL GitHub] à [!UICONTROL Workfront Fusion], voir [Création d’une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] modules et leurs champs.

Lorsque vous configurez des modules [!DNL GitHub], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL GitHub] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheurs](#triggers)
* [Actions](#actions)

### Déclencheurs

* [[!UICONTROL Problèmes de contrôle]](#watch-issues)
* [[!UICONTROL Repositories Watch]](#watch-repositories)
* [[!UICONTROL Branchements de contrôle]](#watch-forks)
* [[!UICONTROL Regarder les commentaires]](#watch-comments)
* [[!UICONTROL Regarder les requêtes d’extraction]](#watch-pull-requests)

#### [!UICONTROL Problèmes de contrôle]

Ce module se déclenche lorsqu’un nouveau problème est ajouté ou qu’un problème existant est modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle. </td> 
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

#### [!UICONTROL Repositories Watch]

Ce module se déclenche lorsqu’un référentiel est créé ou modifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de référentiels renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Indiquez si vous souhaitez rechercher de nouveaux référentiels et toutes les modifications, ou uniquement de nouveaux référentiels.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Branchements de contrôle]

Ce module se déclenche lors de la création d’un branchement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel que vous souhaitez surveiller pour les branchements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de branchements renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle. </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>Choisissez si vous souhaitez ne regarder que les nouveaux commentaires ou les commentaires et toutes les modifications.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Regarder les requêtes d’extraction]

Ce module se déclenche lorsqu’une nouvelle requête de tirage est ajoutée ou qu’une requête de tirage existante est modifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Repository]</td> 
   <td>Sélectionnez le référentiel que vous souhaitez regarder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de demandes d’extraction renvoyées]</td> 
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle. </td> 
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

* [[!UICONTROL Rechercher un problème]](#search-for-an-issue)
* [[!UICONTROL Créer un problème]](#create-an-issue)
* [[!UICONTROL Mettre à jour un problème]](#update-an-issue)
* [[!UICONTROL Obtenir un problème]](#get-an-issue)
* [[!UICONTROL Ajouter des personnes désignées]](#add-assignees)
* [[!UICONTROL Supprimer les personnes désignées]](#remove-assignees)
* [[!UICONTROL Ajouter des étiquettes à un problème]](#add-labels-to-an-issue)
* [[!UICONTROL Supprimer une étiquette d’un problème]](#remove-a-label-from-an-issue)
* [[!UICONTROL Créer un commentaire]](#create-a-comment)
* [[!UICONTROL Lister des commentaires]](#list-comments)

#### [!UICONTROL Rechercher un problème]

Ce module recherche des problèmes qui correspondent à vos critères de recherche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de problèmes renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] va utiliser au cours d’un cycle (le nombre de répétitions par exécution de scénario). </td> 
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
   <td> <p>Sélectionnez ascendant ou descendant. </p> <p>Pour les dates, la sélection de <strong>[!UICONTROL descendant]</strong> renvoie d’abord la date la plus récente. </p> <p>Pour [!UICONTROL (nombre de commentaires), la sélection de <strong>[!UICONTROL descendant]</strong> renvoie le problème avec le plus grand nombre de commentaires en premier.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Saisissez ou mappez votre requête de recherche. Pour obtenir une description détaillée des options de recherche, voir <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests"> Problèmes de recherche et demandes d’extraction </a> sur le site d’aide [!DNL GitHub].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un problème]

Ce module crée un problème dans le référentiel sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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

Ce module met à jour un problème [!DNL GitHub] existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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

#### [!UICONTROL Obtenir un problème]

Ce module récupère les détails du problème spécifié

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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

#### [!UICONTROL Supprimer les personnes désignées]

Ce module supprime les personnes désignées du problème spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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

#### [!UICONTROL Ajouter des étiquettes à un problème]

Ce module ajoute des étiquettes à un problème. Les libellés sont définis au niveau du référentiel et ne peuvent être créés que par une personne disposant d’un accès en écriture au référentiel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL GitHub] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td>Le module renvoie les commentaires créés après cette date. Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Contrainte de type dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre maximal de commentaires renvoyés]</td> 
   <td>Définissez le nombre maximal de résultats que [!DNL Workfront Fusion] utilisera au cours d’un cycle. </td> 
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
