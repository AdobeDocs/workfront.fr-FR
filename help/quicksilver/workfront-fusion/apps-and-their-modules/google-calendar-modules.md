---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connector
navigation-topic: apps-and-their-modules
title: Modules du calendrier Google
description: Dans un [!DNL Adobe Workfront Fusion] vous pouvez automatiser les workflows qui utilisent le calendrier Google et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3821'
ht-degree: 0%

---

# [!DNL Google Calendar] modules

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!UICONTROL Calendrier Google], ainsi que de la connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, reportez-vous à la section [Création d’un scénario dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, voir [Modules dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser [!DNL Google Calendar] modules, vous devez disposer d’un [!DNL Google] compte .

## [!DNL Google Calendar] modules et leurs champs

Lorsque vous configurez [!DNL Google Calendar] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Google Calendar] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Événements](#events)
* [Calendriers](#calendars)
* [Règles de contrôle d&#39;accès](#access-control-rules)
* [Itérateurs (obsolète)](#iterators-deprecated)
* [Autre](#other)

### Événements

* [[!UICONTROL Surveiller les événements]](#watch-events)
* [[!UICONTROL Recherche d’événements]](#search-events)
* [[!UICONTROL Obtention d’un événement]](#get-an-event)
* [[!UICONTROL Créer un événement]](#create-an-event)
* [[!UICONTROL Mettre à jour un événement]](#update-an-event)
* [[!UICONTROL Suppression d’un événement]](#delete-an-event)


#### [!UICONTROL Surveiller les événements]

Ce module de déclenchement exécute un scénario lorsqu’un nouvel événement est ajouté, mis à jour, supprimé, démarré ou se termine dans le calendrier que vous spécifiez. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendrier] </td> 
   <td> <p>Sélectionnez le calendrier avec lequel le module doit fonctionner.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Événements de contrôle]</td> 
   <td> <p>Indiquez si vous souhaitez voir les événements par date de création, date de mise à jour, date de début ou date de fin.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Afficher les événements supprimés]</td> 
   <td> <p>Activez cette option pour inclure les événements qui ont été supprimés.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] </td> 
   <td> <p>Saisissez le texte à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p> Définissez le nombre maximal d’événements qui [!DNL Workfront Fusion] fonctionne avec pendant un cycle (nombre de répétitions par exécution de scénario). Si la valeur est définie sur une valeur trop élevée, la connexion peut être interrompue du côté du service tiers donné (délai d’expiration). [!DNL Workfront Fusion] n'a aucune influence sur cela. Nous vous recommandons de définir une valeur inférieure et de définir une valeur supérieure pour le nombre maximal de cycles ou d’exécuter le scénario plus fréquemment.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Recherche d’événements]

Ce module d’action recherche un événement dans le calendrier sélectionné.

Vous indiquez le calendrier et les paramètres de la recherche.

Le module renvoie l’identifiant de l’événement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à Adobe Workfront Fusion - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de début]</td> 
   <td> <p> Entrez ou mappez la date de début de l’événement. Ce module récupère également les événements qui commencent avant cette date et qui se produisent toujours à la date de début saisie. </p> <p>Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de fin]</td> 
   <td> <p> Saisissez ou mappez la date de fin de l’événement. </p> <p> Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Événements uniques]</td> 
   <td> <p> Activez cette option pour traiter les événements récurrents comme des instances uniques. Par exemple, si vous disposez d’une réunion hebdomadaire et que cette option est activée, le module renvoie la réunion de chaque semaine sous la forme d’un événement distinct.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Saisissez ou mappez le terme à rechercher. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordre par]</td> 
   <td> <p>Sélectionnez l’ordre des événements renvoyés dans le résultat.</p> 
    <ul> 
     <li><strong>[!UICONTROL Heure de début]</strong>: Classer par date et heure de début (croissant). Cette option n’est disponible que lors de l’interrogation d’événements uniques.</li> 
     <li><strong>[!UICONTROL Heure de mise à jour]</strong>: Classer par heure de dernière modification (ascendant).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limite]</td> 
   <td> <p>Définition du nombre maximal d’événements [!DNL Workfront Fusion] renvoie pendant un cycle d'exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un événement]

Ce module d’action renvoie les métadonnées d’un événement unique dans le calendrier spécifié.

Vous spécifiez le calendrier et l’événement.

Le module renvoie l’identifiant de l’événement et tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendrier]</td> 
   <td> <p>Saisissez ou mappez l’identifiant du calendrier qui contient l’événement que vous souhaitez obtenir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Saisissez l’identifiant d’événement de la variable [!DNL Google Calendar] que vous souhaitez obtenir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un événement]

Ce module d’action crée un événement.

Vous spécifiez le calendrier et les paramètres de l’événement.

Le module renvoie l’identifiant de l’événement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à Adobe Workfront Fusion - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Créer un événement]</td> 
   <td> <p>Sélectionnez le mode de création de l’événement.</p> 
    <ul> 
     <li><b>[!UICONTROL En Détail]</b><p>Cette option vous permet de fournir plus de détails sur l’événement.<br></p></li> 
     <li><b>[!UICONTROL Rapidement]</b><p>Il vous suffit de sélectionner le calendrier et de saisir un nom pour l’événement. Vous pouvez inclure des informations sur l’heure et le lieu dans le nom, et [!DNL Google Calendar] planifiera l’événement pour cet endroit et cette heure.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier dans lequel vous souhaitez que l’événement s’affiche.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color]</td> 
   <td>Sélectionnez la couleur que l’événement affiche dans le calendrier.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom de l’événement]</td> 
   <td> <p> Saisissez ou mappez un nom pour l’événement. </p> <p>Remarque : Si vous avez sélectionné [!UICONTROL Ajout rapide] dans le champ [!UICONTROL Créer un événement] , vous pouvez inclure la date et l’heure de l’événement, et [!DNL Workfront Fusion] crée l’événement pour cette date et cette heure. Exemple: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Si vous avez sélectionné [!UICONTROL Ajout rapide] sans inclure de date et d’heure dans le nom de l’événement, l’événement est créé à partir de l’heure actuelle et dure une heure.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tout le jour]</td> 
   <td>Activez cette option si l’événement est un événement de toute la journée (il ne nécessite pas d’heures de début et de fin).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de début]</td> 
   <td> <p>S’il s’agit d’un événement de toute la journée, saisissez la date de début de l’événement. </p> <p>Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date de fin]</td> 
   <td> <p> S’il s’agit d’un événement de toute la journée, saisissez la date de fin de l’événement. </p> <p>Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description pour l’événement. Ce champ prend en charge le HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Emplacement]</td> 
   <td>Saisissez l’emplacement de l’événement dans le formulaire texte.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utiliser les paramètres de rappel par défaut pour cet événement]</td> 
   <td>Activez cette option pour utiliser les paramètres de rappel par défaut. Si vous définissez un rappel personnalisé dans le champ [!UICONTROL Rappel] , cette valeur est définie sur Non.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reminder] </td> 
   <td> <p>Ajoutez un rappel pour l’événement. Pour chaque rappel, sélectionnez la méthode à retenir et définissez la durée (en minutes) qui précède l’événement à rappeler.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Participants]</td> 
   <td>Ajoutez les participants à l’événement. Pour chaque participant, saisissez ou mappez son nom et son adresse email.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me montrer comme étant]</td> 
   <td>Choisissez si vous souhaitez que les personnes qui consultent votre calendrier vous voient comme occupé ou Disponible pendant cet événement.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibilité] </td> 
   <td> <p>Sélectionnez la visibilité de cet événement. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Par Défaut]</b></p> <p>La visibilité de l’événement est définie dans les paramètres du calendrier.</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>Tous ceux avec qui le calendrier est partagé peuvent voir cet événement.</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>Seuls les participants peuvent voir cet événement.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Envoi d’une notification sur la création de l’événement]</td> 
   <td> <p>Choisissez d’envoyer des notifications sur la création d’un événement à tous les invités, à ceux qui ne sont pas[!DNL Google Calendar] les invités, ou personne.</p> <p>Conseil : Il est recommandé d’utiliser l’option [!UICONTROL Aucun] uniquement pour les cas pratiques de migration.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Les invités peuvent modifier l’événement]</td> 
   <td> <p>Activez cette option si vous souhaitez que les invités puissent modifier cet événement.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Périodicité]</td> 
   <td>Ajoutez les règles de périodicité à appliquer à cet événement. Chaque règle nécessite une liste de lignes [!UICONTROL RULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] et [!UICONTROL EXDATE] pour un événement récurrent. Notez que les lignes [!UICONTROL DTSTART] et [!UICONTROL DTEND] ne sont pas autorisées dans ce champ ; les heures de début et de fin de l’événement sont spécifiées dans les champs de début et de fin. Ce champ est omis pour les événements uniques ou les instances d’événements récurrents. Pour plus d’informations, voir <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un événement]

Ce module d’action modifie un événement existant.

Vous spécifiez le calendrier et l’identifiant d’événement.

Le module renvoie l’identifiant de l’événement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendrier] </td> 
   <td> <p>Sélectionnez le calendrier que vous souhaitez utiliser.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Saisissez l’identifiant d’événement de la [!DNL Google Calendar] que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
 </tbody> 
</table>

Vous pouvez mettre à jour les informations de l’événement en entrant de nouvelles valeurs dans le champ souhaité. Pour plus d’informations sur les champs individuels, voir [[!UICONTROL Créer un événement]](#create-an-event).

#### [!UICONTROL Suppression d’un événement]

Ce module d’action supprime un événement.

Vous spécifiez le calendrier et l’identifiant d’événement.

Le module renvoie l’identifiant de l’événement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier qui contient l’événement que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID]</td> 
   <td> <p> Saisissez l’identifiant d’événement d’une [!DNL Google Calendar] que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Envoi d’une notification sur la suppression d’événement]</td> 
   <td>Indiquez si vous souhaitez envoyer des notifications sur la suppression d’événement à tous les invités, invités qui n’utilisent pas [!DNL Google Calendar]ou personne.</td> 
  </tr> 
 </tbody> 
</table>

### Calendriers

* [[!UICONTROL Répertorier les calendriers]](#list-calendars)
* [[!UICONTROL Obtention d’un calendrier]](#get-a-calendar)
* [[!UICONTROL Créer un calendrier]](#create-a-calendar)
* [[!UICONTROL Mettre à jour un calendrier]](#update-a-calendar)
* [[!UICONTROL Suppression d’un calendrier]](#delete-a-calendar)
* [[!UICONTROL Effacement d’un calendrier]](#clear-a-calendar)

#### [!UICONTROL Répertorier les calendriers]

Ce module d’action renvoie les calendriers sur la liste des calendriers d’un utilisateur.

Le module renvoie l’identifiant du calendrier et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rôle d’accès minimal]</td> 
   <td> <p>Sélectionnez le rôle d’accès minimal pour l’utilisateur. Le module renvoie des calendriers en fonction de ce rôle d’accès minimal.</p> 
    <ul> 
     <li><strong>[!UICONTROL Reader Occupy gratuit]</strong>: L’utilisateur peut lire des informations libres/occupées. </li> 
     <li><strong>[!UICONTROL Propriétaire]</strong>: L’utilisateur peut lire et modifier des événements et accéder à des listes de contrôle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: L’utilisateur peut lire des événements qui ne sont pas privés. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: L’utilisateur peut lire et modifier des événements.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher les calendriers masqués]</td> 
   <td>Activez cette option pour inclure les calendriers masqués dans la liste que le module renvoie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Définition du nombre maximal de calendriers [!DNL Workfront Fusion] renvoie pendant un cycle d'exécution.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un calendrier]

Ce module d’action récupère un calendrier.

Vous indiquez l’identifiant du calendrier que vous souhaitez récupérer.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier que vous souhaitez récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un calendrier]

Ce module d’action crée un nouveau calendrier.

Vous indiquez un nom pour le calendrier.

Le module renvoie l’identifiant du calendrier et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom du calendrier]</td> 
   <td> <p> Saisissez un nom pour le nouveau calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un calendrier]

Ce module d’action met à jour un calendrier.

Vous indiquez l’identifiant du calendrier que vous souhaitez mettre à jour.

Le module renvoie l’identifiant du calendrier et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nom du calendrier]</td> 
   <td> <p> Saisissez un nouveau nom pour le calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un calendrier]

Ce module d&#39;action supprime un calendrier.

Vous indiquez l’identifiant du calendrier que vous souhaitez supprimer.

Le module renvoie l’identifiant du calendrier et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendrier]</td> 
   <td> <p>Saisissez ou mappez l’identifiant du calendrier que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Effacement d’un calendrier]

Ce module d’action supprime tous les événements du Principal calendrier d’un compte.

Vous spécifiez la connexion au compte qui contient le calendrier que vous souhaitez effacer.

Le module renvoie l’identifiant du calendrier et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Règles de contrôle d&#39;accès

* [[!UICONTROL Règles de contrôle d&#39;accès aux listes]](#list-access-control-rules)
* [[!UICONTROL Obtention d’une règle de contrôle d’accès]](#get-an-access-control-rule)
* [[!UICONTROL Créer une règle de contrôle d’accès]](#create-an-access-control-rule)
* [[!UICONTROL Mettre à jour une règle de contrôle d’accès]](#update-an-access-control-rule)
* [[!UICONTROL Suppression d’une règle de contrôle d’accès]](#delete-an-access-control-rule)

#### [!UICONTROL Règles de contrôle d&#39;accès aux listes]

Ce module d’action renvoie les règles de la liste de contrôle d’accès d’un calendrier.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier qui contient les règles de contrôle d’accès que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Définir le nombre maximal de résultats [!DNL Workfront Fusion] renvoie pendant un cycle d'exécution.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’une règle de contrôle d’accès]

Ce module d’action renvoie les métadonnées d’une règle de contrôle d’accès.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier contenant la règle de contrôle d’accès que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de règle de contrôle d’accès]</td> 
   <td>Sélectionnez la règle de contrôle d’accès que vous souhaitez récupérer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une règle de contrôle d’accès]

Ce module d’action crée une nouvelle règle de contrôle d’accès.

Vous indiquez un nom pour le calendrier.

Le module renvoie l’identifiant de la règle de contrôle d’accès et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier dans lequel vous souhaitez créer une règle de contrôle d'accès.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Sélectionnez le rôle à affecter à la règle d’accès. </p> 
    <ul> 
     <li><strong>[!UICONTROL Reader Occupy gratuit]</strong>: L’utilisateur peut lire des informations libres/occupées. </li> 
     <li><strong>[!UICONTROL Propriétaire]</strong>: L’utilisateur peut lire et modifier des événements et accéder à des listes de contrôle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: L’utilisateur peut lire des événements qui ne sont pas privés. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: L’utilisateur peut lire et modifier des événements.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>Sélectionnez le type de portée. </p> 
    <ul> 
     <li><strong>[!UICONTROL Par Défaut]</strong>: Portée publique. Il s’agit de la valeur par défaut. </li> 
     <li><strong>[!UICONTROL User]</strong>: Limite la portée à un seul utilisateur. </li> 
     <li><strong>[!UICONTROL Group]</strong>: Limite la portée à un groupe. </li> 
     <li><strong>[!UICONTROL Domain]</strong>: Limite la portée à un domaine. </li> 
    </ul> <p>Remarque : Les autorisations accordées au champ [!UICONTROL Par défaut], ou public, s’appliquent à tout utilisateur, authentifié ou non.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td>Entrez l’adresse email d’un utilisateur ou d’un groupe, ou le nom d’un domaine, selon le type de périmètre.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Envoi de notifications]</td> 
   <td> <p>Activez cette option pour envoyer des notifications sur le changement d’accès. </p> <p>Remarque : Aucune notification n’est envoyée lors de la suppression de l’accès. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour une règle de contrôle d’accès]

Ce module d’action met à jour une règle de contrôle d’accès.

Vous indiquez un nom pour le calendrier.

Le module renvoie l’identifiant de la règle de contrôle d’accès et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez le calendrier qui contient la règle de contrôle d’accès que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de règle de contrôle d’accès]</td> 
   <td>Sélectionnez la règle de contrôle d’accès que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Sélectionnez le rôle à affecter à la règle d’accès. </p> 
    <ul> 
     <li><strong>[!UICONTROL Aucun]</strong>: Ce rôle ne fournit aucun accès.</li> 
     <li><strong>[!UICONTROL Reader Occupy gratuit]</strong>: L’utilisateur peut lire des informations libres/occupées. </li> 
     <li><strong>[!UICONTROL Propriétaire]</strong>: L’utilisateur peut lire et modifier des événements et accéder à des listes de contrôle. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: L’utilisateur peut lire des événements qui ne sont pas privés. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: L’utilisateur peut lire et modifier des événements.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Envoi de notifications]</td> 
   <td> <p>Activez cette option pour envoyer des notifications sur le changement d’accès. </p> <p>Remarque : Aucune notification n’est envoyée lors de la suppression de l’accès. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’une règle de contrôle d’accès]

Ce module d’action supprime une règle de contrôle d’accès.

Vous indiquez un nom pour le calendrier.

Le module renvoie l’identifiant de la règle de contrôle d’accès et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de calendrier]</td> 
   <td> <p>Sélectionnez ou mappez l’identifiant du calendrier qui contient la règle de contrôle d’accès que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de règle de contrôle d’accès]</td> 
   <td>Sélectionnez ou mappez l’identifiant de la règle de contrôle d’accès que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

### Itérateurs (obsolète)

Le [!UICONTROL itération des pièces jointes] et [!UICONTROL itérer les participants] Les modules ont été abandonnés. Pour itérer les pièces jointes ou les participants, utilisez le [!UICONTROL Contrôle de flux] > [!UICONTROL Itérateur] module . Pour plus d’informations, voir [Module d’itérateur dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Autre

* [[!UICONTROL Lancer un appel API]](#make-an-api-call)
* [[!UICONTROL Obtenir des informations gratuites/pratiques]](#get-freebusy-information)

#### [!UICONTROL Lancer un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Saisissez un chemin relatif à <code>https://www.googleapis.com/calendar</code>. Exemple: <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode [!UICONTROL]</p> </td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note:   <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir des informations gratuites/pratiques]

Ce module d’action renvoie des informations gratuites et chargées pour un ensemble de calendriers.

Le module renvoie l’identifiant du calendrier et des champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mapper ces informations dans les modules suivants du scénario.

Lors de la configuration de ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la connexion à [!DNL Google Calendar] compte Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d’une connexion à Adobe Workfront Fusion - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minimum time]</td> 
   <td> <p> Saisissez le début de l’intervalle pour lequel vous souhaitez récupérer des informations.</p> <p> Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Durée maximale]</td> 
   <td> <p> Saisissez la fin de l’intervalle pour lequel vous souhaitez récupérer des informations. </p> <p>Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendriers]</td> 
   <td> <p>Pour chaque calendrier duquel vous souhaitez récupérer des informations, cliquez sur <strong>Ajouter</strong> et saisissez ou mappez l’ID de calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Déclenchement d’un scénario avant un événement

Vous pouvez déclencher un scénario à une heure spécifique avant un événement à l’aide de la méthode standard [!DNL Google Calendar] les rappels par e-mail et la variable [!UICONTROL Webhooks] >[!UICONTROL Chaîne de messagerie personnalisée] module .

1. Utilisez la variable [!UICONTROL Calendrier Google] >[!UICONTROL Mettre à jour un événement] pour ajouter un rappel d’email à votre événement :

   ![](assets/trigger-scen-before-event-350x209.png)

1. Créez un scénario commençant par le [!UICONTROL Webhooks] >[!UICONTROL Chaîne de messagerie personnalisée] module .

   1. Copiez l’adresse électronique du point d’extension mailhook.
   1. Enregistrez le scénario et exécutez-le.

1. Dans [!DNL Gmail], redirigez le [!DNL Google Calendar] rappels à l’adresse électronique du mailhook :

   1. Ouvrez votre **[!UICONTROL [!DNL Gmail]paramètres]**.
   1. Ouvrez le **[!UICONTROL Transfert et POP/IMAP]** .
   1. Cliquez sur **[!UICONTROL Ajouter une adresse de transfert].**
   1. Collez l’adresse électronique des emails copiés, puis cliquez sur &#x200B;**[!UICONTROL Suivant]**, confirmez en appuyant sur **[!UICONTROL Continuer]** dans la fenêtre contextuelle, puis cliquez sur **[!UICONTROL OK]**.

   1. Dans [!DNL Workfront Fusion], passez au nouveau scénario qui devrait terminer son exécution en recevant l’email de confirmation.
   1. Cliquez sur la bulle au-dessus du module pour inspecter la sortie du module.
   1. Développez l’objet `Text` et copiez le code de confirmation :

      ![](assets/confirmation-code-350x252.png)

   1. Dans Gmail, collez le code de confirmation dans la zone d’édition, puis cliquez sur &#x200B;**[!UICONTROL Vérifier]**:

      ![](assets/paste-code-350x46.png)

   1. Ouvrez le **[!UICONTROL Filtres et adresses bloquées]** .
   1. Cliquez sur **[!UICONTROL Créer un nouveau filtre]**.
   1. Configurer un filtre pour tous les emails provenant de `     calendar-notification@google.com` et cliquez sur &#x200B;**[!UICONTROL Création d’un filtre]**:
   1. Sélectionner **[!UICONTROL Transférer à]** et sélectionnez l’adresse électronique du mailhooks dans la liste.
   1. Cliquez sur **[!UICONTROL Créer un filtre]** pour créer le filtre.

1. (Facultatif) Dans [!DNL Workfront Fusion], ajoutez le [!UICONTROL Analyseur de texte] > [!UICONTROL Modèle de correspondance] après l’événement [!UICONTROL Webhooks] >[!UICONTROL Chaîne de messagerie personnalisée] pour analyser le code HTML de l’email afin d’obtenir toutes les informations dont vous avez besoin.

   Par exemple, vous pouvez configurer le module comme suit pour obtenir l’identifiant de l’événement :

   *Modèle*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Texte*: Le `HTML content` sortie de l’élément [!UICONTROL Webhooks] >[!UICONTROL Chaîne de messagerie personnalisée] module .
