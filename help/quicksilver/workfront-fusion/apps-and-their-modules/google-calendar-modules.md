---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Modules du calendrier Google
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent le calendrier Google et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3837'
ht-degree: 98%

---

# Modules [!DNL Google Calendar]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent le [!UICONTROL calendrier Google] et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, consultez [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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
   <p>Exigences actuelles du produit : si vous avez le plan [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Google Calendar], vous devez disposer d’un compte [!DNL Google].

## Informations sur l’API du calendrier Google

Le connecteur du calendrier Google utilise les éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL de base</td> 
   <td> https://www.googleapis.com/calendar/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Version de l’API</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Balise API</td> 
   <td>v5.4.5</td> 
  </tr>
 </tbody> 
 </table>

## Modules [!DNL Google Calendar] et leurs champs

Lorsque vous configurez les modules [!DNL Google Calendar], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Google Calendar] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Événements](#events)
* [Calendriers](#calendars)
* [Règles de contrôle d’accès](#access-control-rules)
* [Itérateurs (obsolète)](#iterators-deprecated)
* [Autre](#other)

### Événements

* [[!UICONTROL Surveiller les événements]](#watch-events)
* [[!UICONTROL Rechercher des événements]](#search-events)
* [[!UICONTROL Obtenir un événement]](#get-an-event)
* [[!UICONTROL Créer un événement]](#create-an-event)
* [[!UICONTROL Mettre à jour un événement]](#update-an-event)
* [[!UICONTROL Supprimer un événement]](#delete-an-event)


#### [!UICONTROL Surveiller les événements]

Ce module de déclenchement exécute un scénario lorsqu’un nouvel événement est ajouté, mis à jour, supprimé, démarré ou se termine dans le calendrier que vous indiquez. Le module renvoie tous les champs standard associés à l’enregistrement ou aux enregistrements, ainsi que les champs et valeurs personnalisés auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>Sélectionnez le calendrier avec lequel vous souhaitez que le module fonctionne.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch Events]</td> 
   <td> <p>Indiquez si vous souhaitez surveiller les événements par date de création, date de mise à jour, date de début ou date de fin.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show deleted events]</td> 
   <td> <p>Activez cette option pour inclure les événements qui ont été supprimés.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] </td> 
   <td> <p>Saisissez le texte à rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Définissez le nombre maximal d’événements avec lesquels [!DNL Workfront Fusion] fonctionne pendant un cycle (nombre de répétitions par exécution de scénario). Si la valeur est définie sur une valeur trop élevée, la connexion peut être interrompue du côté du service tiers donné (délai d’expiration). [!DNL Workfront Fusion] n’a aucune influence sur cela. Nous vous recommandons de définir une valeur inférieure et de définir une valeur supérieure pour le nombre maximal de cycles ou d’exécuter le scénario plus fréquemment.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des événements]

Ce module d’action recherche un événement dans le calendrier sélectionné.

Vous indiquez le calendrier et les paramètres de la recherche.

Le module renvoie l’identifiant de l’événement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe Workfront Fusion - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez le calendrier que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start date]</td> 
   <td> <p> Entrez ou mappez la date de début de l’événement. Ce module récupère également les événements qui commencent avant cette date et qui se produisent toujours à la date de début saisie. </p> <p>Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End date]</td> 
   <td> <p> Saisissez ou mappez la date de fin de l’événement. </p> <p> Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Single events]</td> 
   <td> <p> Activez cette option pour traiter les événements récurrents comme des instances uniques. Par exemple, si vous disposez d’une réunion hebdomadaire et que cette option est activée, le module renvoie la réunion de chaque semaine sous la forme d’un événement distinct.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Saisissez ou mappez le terme de recherche souhaité. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td> <p>Sélectionnez l’ordre des événements renvoyés dans le résultat.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Time]</strong> : triez par date et heure de début (croissant). Cette option n’est disponible que lors de l’interrogation d’événements uniques.</li> 
     <li><strong>[!UICONTROL Updated Time]</strong> : triez par heure de dernière modification (croissant).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Définissez le nombre maximal d’événements que [!DNL Workfront Fusion] renvoie pendant un cycle d’exécution.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un événement]

Ce module d’action renvoie les métadonnées d’un événement unique dans le calendrier indiqué.

Vous indiquez le calendrier et l’événement.

Le module renvoie l’identifiant de l’événement et tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant du calendrier qui contient l’événement que vous souhaitez obtenir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Saisissez l’identifiant d’événement de l’événement [!DNL Google Calendar] existant que vous souhaitez obtenir.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un événement]

Ce module d’action crée un événement.

Vous spécifiez le calendrier et les paramètres de l’événement.

Le module renvoie l’identifiant de l’événement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Pour savoir comment connecter votre compte [!DNL Google Calendar] à Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe Workfront Fusion - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create an Event]</td> 
   <td> <p>Sélectionnez le mode de création de l’événement.</p> 
    <ul> 
     <li><b>[!UICONTROL In Detail]</b><p>Cette option vous permet de fournir plus de détails sur l’événement.<br></p></li> 
     <li><b>[!UICONTROL Quickly]</b><p>Il vous suffit de sélectionner le calendrier et de saisir un nom pour l’événement. Vous pouvez inclure des informations sur l’heure et l’endroit dans le nom, et [!DNL Google Calendar] planifiera l’événement pour cet endroit et cette heure.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Choisissez le calendrier dans lequel vous souhaitez que l’événement apparaisse.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color]</td> 
   <td>Sélectionnez la couleur que l’événement doit afficher dans le calendrier.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event name]</td> 
   <td> <p> Saisissez ou mappez un nom pour l’événement. </p> <p>Note : si vous avez sélectionné [!UICONTROL Quick add] dans le champ [!UICONTROL Create an event], vous pouvez inclure la date et l’heure de l’événement, et [!DNL Workfront Fusion] crée alors l’événement pour cette date et cette heure. Exemple : <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Si vous avez sélectionné [!UICONTROL Quick add] sans inclure de date et d’heure dans le nom de l’événement, l’événement est créé à partir de l’heure actuelle et dure une heure.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL All day event]</td> 
   <td>Activez cette option si l’événement est un événement qui dure toute la journée (il n’a alors pas besoin d’heure de début ni de fin).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start date]</td> 
   <td> <p>S’il s’agit d’un événement qui dure toute la journée, saisissez la date de début de l’événement. </p> <p>Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End date]</td> 
   <td> <p> S’il s’agit d’un événement qui dure toute la journée, saisissez la date de fin de l’événement. </p> <p>Pour obtenir la liste des formats de date pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description pour l’événement. Ce champ prend en charge le format HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Location]</td> 
   <td>Saisissez l’emplacement de l’événement dans le formulaire texte.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Use the default reminder settings for this event]</td> 
   <td>Activez cette option pour utiliser les paramètres de rappel par défaut. Si vous définissez un rappel personnalisé dans le champ [!UICONTROL Reminder], cette valeur est définie sur Non.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reminder] </td> 
   <td> <p>Ajoutez un rappel pour l’événement. Pour chaque rappel, sélectionnez la méthode que vous souhaitez utiliser pour le rappel et définissez la durée (en minutes) qui précède l’événement pour lequel vous souhaitez obtenir ce rappel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attendees]</td> 
   <td>Ajoutez les personnes participant à l’événement. Pour chaque personne participant, saisissez ou mappez son nom et son adresse e-mail.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show me as]</td> 
   <td>Définissez votre statut sur « Occupé » ou « Disponible » à afficher pour les personnes qui ont accès à votre calendrier lors de cet événement.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibility] </td> 
   <td> <p>Sélectionnez la visibilité de cet événement. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Default]</b></p> <p>La visibilité de l’événement est définie dans les paramètres du calendrier.</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>Toutes les personnes avec qui le calendrier est partagé peuvent voir cet événement.</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>Seules les personnes inscrites peuvent voir cet événement.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notification about the event creation]</td> 
   <td> <p>Choisissez d’envoyer des notifications sur la création d’un nouvel événement à toutes les personnes invitées, à celles qui ne sont pas invitées dans [!DNL Google Calendar], ou à personne.</p> <p>Conseil : nous vous recommandons d’utiliser l’option [!UICONTROL None] uniquement pour les cas de migration.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Guests can modify the event]</td> 
   <td> <p>Activez cette option si vous souhaitez que les personnes invitées puissent modifier cet événement.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurrence]</td> 
   <td>Ajoutez des règles de périodicité à cet événement. Chaque règle nécessite une liste de lignes [!UICONTROL RRULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] et [!UICONTROL EXDATE] pour un événement récurrent. Notez que les lignes [!UICONTROL DTSTART] et [!UICONTROL DTEND] ne sont pas autorisées dans ce champ ; les heures de début et de fin de l’événement sont spécifiées dans les champs de début et de fin. Ce champ est omis pour les événements uniques ou les instances d’événements récurrents. Pour plus d’informations, consultez la section <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un événement]

Ce module d’action modifie un événement existant.

Spécifiez le calendrier et l’identifiant d’événement.

Le module renvoie l’identifiant de l’événement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>Sélectionnez le calendrier que vous souhaitez utiliser.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Saisissez l’identifiant d’événement de l’événement [!DNL Google Calendar] précédemment créé que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour actualiser les informations relatives à l’événement, il suffit de saisir de nouvelles valeurs dans le champ souhaité. Pour plus d’informations sur les champs individuels, consultez la section [[!UICONTROL Créer un événement]](#create-an-event).

#### [!UICONTROL Supprimer un événement]

Ce module d’action supprime un événement.

Spécifiez le calendrier et l’identifiant d’événement.

Le module renvoie l’identifiant de l’événement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez le calendrier qui contient l’événement que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID]</td> 
   <td> <p> Saisissez l’identifiant d’événement de l’événement [!DNL Google Calendar] précédemment créé que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notification about the event deletion]</td> 
   <td>Indiquez si vous souhaitez envoyer des notifications sur la suppression d’événement à toutes les personnes invitées, aux personnes invitées qui n’utilisent pas [!DNL Google Calendar] ou à personne.</td> 
  </tr> 
 </tbody> 
</table>

### Calendriers

* [[!UICONTROL Répertorier les calendriers]](#list-calendars)
* [[!UICONTROL Obtenir un calendrier]](#get-a-calendar)
* [[!UICONTROL Créer un calendrier]](#create-a-calendar)
* [[!UICONTROL Mettre un calendrier à jour]](#update-a-calendar)
* [[!UICONTROL Supprimer un calendrier]](#delete-a-calendar)
* [[!UICONTROL Effacer un calendrier]](#clear-a-calendar)

#### [!UICONTROL Répertorier les calendriers]

Ce module d’action renvoie les calendriers sur la liste des calendriers d’une personne.

Le module renvoie l’identifiant du calendrier et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Minimum access role]</td> 
   <td> <p>Sélectionnez le rôle d’accès minimal pour la personne. Le module renvoie des calendriers en fonction de ce rôle d’accès minimal.</p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong> : la personne peut lire des informations de disponibilité. </li> 
     <li><strong>[!UICONTROL Owner]</strong> : la personne peut lire et modifier des événements et accéder à des listes de contrôle. </li> 
     <li><strong>[!UICONTROL Reader]</strong> : la personne peut lire les événements qui ne sont pas privés. </li> 
     <li><strong>[!UICONTROL Writer]</strong> : la personne peut lire et modifier des événements.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show hidden calendars]</td> 
   <td>Activez cette option pour inclure les calendriers masqués dans la liste que le module renvoie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Définissez le nombre maximal de calendriers que [!DNL Workfront Fusion] renvoie pendant un cycle d’exécution.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un calendrier]

Ce module d’action permet de récupérer un calendrier.

Vous indiquez l’identifiant du calendrier que vous souhaitez récupérer.

Le module renvoie l’identifiant de l’enregistrement et de tous les champs associés, ainsi que les champs personnalisés et les valeurs auxquels la connexion a accès. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez le calendrier que vous souhaitez récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un calendrier]

Ce module d’action crée un calendrier.

Spécifiez un nom pour le calendrier.

Le module renvoie l’identifiant du calendrier et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar name]</td> 
   <td> <p> Saisissez un nom pour le nouveau calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre un calendrier à jour]

Ce module d’action met à jour un calendrier.

Vous indiquez l’identifiant du calendrier que vous souhaitez mettre à jour.

Le module renvoie l’identifiant du calendrier et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez le calendrier à mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar name]</td> 
   <td> <p> Saisissez un nouveau nom pour le calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un calendrier]

Ce module d’action supprime un calendrier.

Indiquez l’identifiant du calendrier que vous souhaitez supprimer.

Le module renvoie l’identifiant du calendrier et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant du calendrier que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un calendrier]

Ce module d’action supprime tous les événements du calendrier principal d’un compte.

Vous indiquez la connexion au compte qui contient le calendrier à effacer.

Le module renvoie l’identifiant du calendrier et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Règles de contrôle d’accès

* [[!UICONTROL Répertorier les règles de contrôle d’accès]](#list-access-control-rules)
* [[!UICONTROL Obtenir une règle de contrôle d’accès]](#get-an-access-control-rule)
* [[!UICONTROL Créer une règle de contrôle d’accès]](#create-an-access-control-rule)
* [[!UICONTROL Mettre à jour une règle de contrôle d’accès]](#update-an-access-control-rule)
* [[!UICONTROL Supprimer une règle de contrôle d’accès]](#delete-an-access-control-rule)

#### [!UICONTROL Répertorier les règles de contrôle d’accès]

Ce module d’action renvoie les règles de la liste de contrôle d’accès sur un calendrier.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez le calendrier qui contient les règles de contrôle d’accès que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Définissez le nombre maximum de résultats que [!DNL Workfront Fusion] renvoie au cours d’un cycle d’exécution.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une règle de contrôle d’accès]

Ce module d’action renvoie les métadonnées d’une règle de contrôle d’accès.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez le calendrier qui contient la règle de contrôle d’accès que vous souhaitez récupérer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Access control rule ID]</td> 
   <td>Sélectionnez la règle de contrôle d’accès que vous souhaitez récupérer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer une règle de contrôle d’accès]

Ce module d’action crée une nouvelle règle de contrôle d’accès.

Spécifiez un nom pour le calendrier.

Le module renvoie l’identifiant de la règle de contrôle d’accès et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez le calendrier dans lequel vous souhaitez créer une règle de contrôle d’accès.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Sélectionnez le rôle à affecter à la règle d’accès. </p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong> : la personne peut lire des informations de disponibilité. </li> 
     <li><strong>[!UICONTROL Owner]</strong> : la personne peut lire et modifier des événements et accéder à des listes de contrôle. </li> 
     <li><strong>[!UICONTROL Reader]</strong> : la personne peut lire les événements qui ne sont pas privés. </li> 
     <li><strong>[!UICONTROL Writer]</strong> : la personne peut lire et modifier les événements.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>Sélectionnez le type de portée. </p> 
    <ul> 
     <li><strong>[!UICONTROL Default]</strong> : portée publique. Il s’agit de la valeur par défaut. </li> 
     <li><strong>[!UICONTROL User]</strong> : limite la portée à une seule personne. </li> 
     <li><strong>[!UICONTROL Group]</strong> : limite la portée à un groupe. </li> 
     <li><strong>[!UICONTROL Domain]</strong> : limite la portée à un domaine. </li> 
    </ul> <p>Note : les permissions accordées à la portée [!UICONTROL Default], ou publique, s’appliquent à toute personne, authentifiée ou non.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td>Saisissez l’adresse e-mail d’un utilisateur ou d’une utilisatrice ou d’un groupe, ou le nom d’un domaine, en fonction du type de portée.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notifications]</td> 
   <td> <p>Activez cette option pour envoyer des notifications sur le changement d’accès. </p> <p>Note : il n’y a pas de notification pour la suppression d’accès. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour une règle de contrôle d’accès]

Ce module d’action met à jour une règle de contrôle d’accès.

Spécifiez un nom pour le calendrier.

Le module renvoie l’identifiant de la règle de contrôle d’accès et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez le calendrier qui contient la règle de contrôle d’accès que vous souhaitez mettre à jour.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>Sélectionnez la règle de contrôle d’accès que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Sélectionnez le rôle à affecter à la règle d’accès. </p> 
    <ul> 
     <li><strong>[!UICONTROL None]</strong> : ce rôle ne fournit aucun accès.</li> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong> : la personne peut lire des informations de disponibilité. </li> 
     <li><strong>[!UICONTROL Owner]</strong> : la personne peut lire et modifier des événements et accéder à des listes de contrôle. </li> 
     <li><strong>[!UICONTROL Reader]</strong> : la personne peut lire les événements qui ne sont pas privés. </li> 
     <li><strong>[!UICONTROL Writer]</strong> : la personne peut lire et modifier des événements.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notifications]</td> 
   <td> <p>Activez cette option pour envoyer des notifications sur le changement d’accès. </p> <p>Note : il n’y a pas de notification pour la suppression d’accès. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer une règle de contrôle d’accès]

Ce module d’action supprime une règle de contrôle d’accès.

Spécifiez un nom pour le calendrier.

Le module renvoie l’identifiant de la règle de contrôle d’accès et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Sélectionnez ou mappez l’identifiant du calendrier qui contient la règle de contrôle d’accès que vous souhaitez supprimer.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>Sélectionnez ou mappez l’identifiant de la règle de contrôle d’accès que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

### Itérateurs (obsolète)

Les modules [!UICONTROL itérer les pièces jointes] et [!UICONTROL itérer les personnes participantes] sont obsolètes. Pour itérer les pièces jointes ou les personnes participantes, utilisez le module [!UICONTROL Contrôle de flux] > [!UICONTROL Itérateur]. Pour plus d’informations, voir [Module itérateur dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

### Autre

* [[!UICONTROL Effectuer un appel API]](#make-an-api-call)
* [[!UICONTROL Obtenir des informations de disponibilité]](#get-freebusy-information)

#### [!UICONTROL Lancer un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Google Calendar] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Saisissez un chemin relatif à <code>https://www.googleapis.com/calendar</code>. Exemple : <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :   <p>Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre JSON, saisissez les guillemets à l’extérieur de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir des informations de disponibilité]

Ce module d’action renvoie les informations relatives aux informations de disponibilité concernant les statuts libre et occupé d’un ensemble de calendriers.

Le module renvoie l’identifiant du calendrier et tous les champs associés, ainsi que tous les champs et valeurs personnalisés auxquels la connexion accède. Vous pouvez mettre en correspondance ces informations dans les modules suivants du scénario.

Lorsque vous configurez ce module, les champs suivants s’affichent.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Pour obtenir des instructions sur la procédure de connexion de votre compte [!DNL Google Calendar] à Workfront Fusion, voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion vers Adobe Workfront Fusion - Instructions de base</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minimum time]</td> 
   <td> <p> Saisissez le début de l’intervalle pour lequel vous souhaitez obtenir des informations.</p> <p> Pour une liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum time]</td> 
   <td> <p> Saisissez la fin de l’intervalle de temps pour lequel vous souhaitez récupérer les informations. </p> <p>Pour une liste des formats de date et de temps pris en charge, consultez la section <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendars]</td> 
   <td> <p>Pour chaque calendrier dont vous souhaitez récupérer les informations, cliquez sur <strong>Ajouter</strong> et saisissez ou mappez l’identifiant du calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Déclencher un scénario avant un événement

Pour déclencher un scénario à un moment précis avant un événement, utilisez les rappels par e-mails standard de [!DNL Google Calendar] et du module [!UICONTROL Webhooks] > [!UICONTROL Mailhook personnalisé].

1. Utilisez le module [!UICONTROL Calendrier Google] > [!UICONTROL Mettre à jour un événement] pour ajouter un rappel par e-mail à votre événement :

   ![](assets/trigger-scen-before-event-350x209.png)

1. Créez un scénario à partir du module [!UICONTROL Webhooks] >[!UICONTROL Mailhook personnalisé].

   1. Copiez l’adresse e-mail du mailhook.
   1. Enregistrez le scénario et exécutez-le.

1. Dans [!DNL Gmail], redirigez les rappels par e-mail de [!DNL Google Calendar] vers l’adresse e-mail du mailhook :

   1. Ouvrez vos paramètres **[!UICONTROL [!DNL Gmail]]**.
   1. Ouvrez l’onglet **[!UICONTROL Transfert et POP/IMAP]**.
   1. Cliquez sur **[!UICONTROL Ajouter une adresse de transfert].**
   1. Collez l’adresse e-mail copiée du mailhook, cliquez sur **[!UICONTROL Suivant]**, confirmez en appuyant sur **[!UICONTROL Continuer]** dans la fenêtre contextuelle, puis cliquez sur **[!UICONTROL OK]**.

   1. Dans [!DNL Workfront Fusion], passez au nouveau scénario qui devrait terminer son exécution après avoir reçu l’e-mail de confirmation.
   1. Cliquez sur la bulle au-dessus du module pour inspecter la sortie du module.
   1. Développez l’élément `Text` et copiez le code de confirmation :

      ![](assets/confirmation-code-350x252.png)

   1. Dans Gmail, collez le code de confirmation dans la boîte de dialogue de modification et cliquez sur **[!UICONTROL Vérifier]** :

      ![](assets/paste-code-350x46.png)

   1. Ouvrez l’onglet **[!UICONTROL Filtres et adresses bloqués]**.
   1. Cliquez sur **[!UICONTROL Créer un filtre]**.
   1. Configurez un filtre pour tous les e-mails provenant de `     calendar-notification@google.com` et cliquez sur **[!UICONTROL Créer un filtre]** :
   1. Sélectionnez **[!UICONTROL Transférer à]** et choisissez l’adresse e-mail du mailhook dans la liste.
   1. Cliquez sur **[!UICONTROL Créer un filtre]** pour créer le filtre.

1. (Facultatif) Dans [!DNL Workfront Fusion], ajoutez le module [!UICONTROL Analyseur de texte] > [!UICONTROL Filtrage par motif] après le module [!UICONTROL Webhooks] > [!UICONTROL Mailhook personnalisé] pour analyser le code HTML de l’e-mail afin d’obtenir toutes les informations dont vous avez besoin.

   Par exemple, vous pouvez configurer le module comme suit pour obtenir l’identifiant de l’événement :

   *Motif* : `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Texte* : l’élément `HTML content` produit par le module [!UICONTROL Webhooks] > [!UICONTROL Mailhook personnalisé].
