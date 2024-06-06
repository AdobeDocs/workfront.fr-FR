---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: Connecteur
navigation-topic: apps-and-their-modules
title: Calendrier Microsoft Office 365
description: Dans un [!DNL Adobe Workfront Fusion] vous pouvez automatiser les workflows qui utilisent le calendrier Microsoft Office 365, et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1999'
ht-degree: 16%

---

# [!DNL Microsoft Office 365 Calendar]

Dans un [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft Office 365 Calendar], ainsi que de la connecter à plusieurs applications et services tiers.

Pour utiliser [!DNL Office 365 Calendar] avec [!DNL Adobe Workfront Fusion], une [!DNL Office 365 Excel] compte . Vous pouvez en créer un à l’adresse [www.office.com](https://www.office.com/).

Pour obtenir des instructions sur la connexion de votre compte Office 365 à [!DNL Workfront Fusion], voir [Créer une connexion à Adobe [!DNL Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

Une fois le consentement accordé, vous êtes redirigé vers le [!UICONTROL Workfront Fusion] page d’administration où vous pouvez continuer à créer votre scénario.

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
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
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

Pour utiliser [!DNL Microsoft Office 365 Calendar] modules, vous devez disposer d’un [!DNL Microsoft Office 365 Calendar] compte .

## Connexion de la variable [!DNL Office 365 Calendar] service à [!DNL Workfront Fusion]

Pour obtenir des instructions sur la connexion à [!DNL Office 365 Calendar] compte à [!UICONTROL Workfront Fusion], voir [Créer une connexion à [!UICONTROL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations utilisateur individuelles. Par conséquent, lors de la création d’une connexion, l’écran de consentement des autorisations affiche les autorisations qui ont été accordées à la connexion de cet utilisateur, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur dispose d’autorisations &quot;Lecture de tableau&quot; accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les emails, l’écran de consentement des autorisations affiche à la fois l’autorisation &quot;Lecture de tableau&quot; déjà accordée et l’autorisation &quot;Ecriture d’email&quot; nouvellement requise.

## Modules [!DNL Microsoft Office 365 Calendar] et leurs champs

Lorsque vous configurez des modules [!DNL Microsoft Office 365 Calendar], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL Microsoft Office 365 Calendar] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Événement](#event)
* [Calendrier](#calendar)
* [Autre](#other)

### Événement

* [[!UICONTROL Événements de contrôle]](#watch-events)
* [[!UICONTROL Événements de recherche]](#search-events)
* [[!UICONTROL Obtention d’un événement]](#get-an-event)
* [[!UICONTROL Créer un événement]](#create-an-event)
* [[!UICONTROL Mettre à jour un événement]](#update-an-event)
* [[!UICONTROL Suppression d’un événement]](#delete-an-event)

#### [!UICONTROL Événements de contrôle]

Ce module de déclenchement récupère les détails d’un événement lorsque celui-ci est créé, mis à jour, supprimé, démarré ou se termine dans le calendrier sélectionné.

>[!NOTE]
>
>Pour rechercher les occurrences supprimées d’une série d’événements, sélectionnez [!UICONTROL Par heure de mise à jour] dans le [!UICONTROL Surveiller les événements] champ . Ce module ne recherche pas les événements uniques supprimés ni les séries d’événements supprimées.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Événements de contrôle]</td> 
   <td> <p>Sélectionnez le mode de surveillance des événements.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Par Heure De Création]</strong> </p> <p>Attention aux nouveaux événements.</p> </li> 
     <li> <p><strong>[!UICONTROL Par Heure De Mise À Jour]</strong> </p> <p>Recherchez les événements mis à jour.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de groupe de calendrier]</td> 
   <td>Sélectionnez le [!UICONTROL Groupe de calendrier] qui contient le calendrier dans lequel vous souhaitez regarder les événements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendrier]</td> 
   <td> <p>Sélectionnez le calendrier spécifique à afficher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Définissez les conditions de filtrage pour filtrer les résultats par objet, identifiant d’événement ou corps.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Entrer le nombre maximum de messages [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Événements de recherche]

Ce module de recherche récupère les détails d’un événement lorsque celui-ci est créé, mis à jour, supprimé, démarré ou se termine dans le calendrier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de groupe de calendrier]</td> 
   <td>Sélectionnez le [!UICONTROL Groupe de calendrier] qui contient le calendrier dans lequel vous souhaitez regarder les événements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendrier]</td> 
   <td> <p>Sélectionnez le calendrier spécifique à afficher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Définissez les conditions de filtrage pour filtrer les résultats. Vous pouvez filtrer selon les propriétés suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Subject]</li> 
     <li>[!UICONTROL Event ID]</li> 
     <li>[!UICONTROL Heure de la date de création]</li> 
     <li>[!UICONTROL Last Modified Date Time]</li> 
     <li>[!UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordre par]</td> 
   <td> <p>Sélectionnez le mode de tri des résultats.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, croissant ou décroissant</li> 
     <li><strong>[!UICONTROL Heure de la date de création]</strong>, croissant ou décroissant</li> 
     <li><strong>[!UICONTROL Last Modified Date Time]</strong>, croissant ou décroissant</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Entrer le nombre maximal d’événements [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un événement]

Ce module d’action récupère les détails de l’événement spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’événement dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un événement]

Ce module d’action crée un événement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez ou mappez un titre pour l’événement créé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date de début]</td> 
   <td> Saisissez une seule heure lorsque l’événement commence dans une représentation de date et d’heure combinée. Utiliser le format <code>({date}T{time}</code>; par exemple, <code>2017-08-29T04:00:00.0000000</code>. Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date de fin]</td> 
   <td> Saisissez une seule heure lorsque l’événement se termine par une représentation de date et d’heure combinée. Utiliser le format <code>{date}T{time}</code>; par exemple, <code>2017-08-29T04:00:00.0000000</code>. Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder on]</td> 
   <td>Indiquez si vous souhaitez activer un rappel pour cet événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Saisissez ou mappez le nombre de minutes avant le début de l’événement lorsque le rappel doit se déclencher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionnez l’importance de cet événement.</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Support]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensibilité] </td> 
   <td> <p>Sélectionnez la sensibilité de cet événement.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>Le destinataire voit un message "[!UICONTROL Veuillez le traiter comme personnel]".</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>Le destinataire voit un message "[!UICONTROL Veuillez le traiter comme privé]". Cet événement n'est pas transféré ou redirigé par les règles de la boîte de réception du destinataire.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>Le destinataire voit un message "[!UICONTROL Veuillez le traiter comme confidentiel]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de contenu du corps]</td> 
   <td>Indiquez si le contenu du corps est en texte brut ou en HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu du corps]</td> 
   <td>Saisissez ou mappez le corps du message associé à l’événement. Il peut être au format HTML ou texte (comme spécifié dans le champ [!UICONTROL Body Content Type] ci-dessus).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Emplacement]</td> 
   <td> <p>Saisissez les détails de l’emplacement de l’événement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Réponse demandée]</td> 
   <td>Sélectionner <strong>[!UICONTROL Oui]</strong> pour demander à l’invité d’envoyer une réponse à l’invitation de l’événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher sous]</td> 
   <td> <p>Sélectionnez le mode d’affichage de l’événement pour les personnes qui visualisent votre calendrier.</p> 
    <ul> 
     <li>[!UICONTROL Libre]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL Occupé]</li> 
     <li>[!UICONTROL Absence du bureau]</li> 
     <li>[!UICONTROL Travail ailleurs]</li> 
     <li>[!UICONTROL Inconnu]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Participants]</p> </td> 
   <td> <p>Ajoutez des participants à l’événement.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du participant.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Saisissez l’adresse électronique du participant.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Catégorie]</td> 
   <td>Entrez ou mappez les catégories que vous souhaitez que l’événement s’affiche comme sur le calendrier.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un événement]

Ce module d’action met à jour un événement existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td>Saisissez, mappez ou sélectionnez l’identifiant de l’événement que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez ou mappez un titre pour l’événement créé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date de début]</td> 
   <td> Saisissez une seule heure lorsque l’événement commence dans une représentation de date et d’heure combinée. Utiliser le format <code>{date}T{time}</code>; par exemple, <code>2017-08-29T04:00:00.0000000</code>. Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date de fin]</td> 
   <td> Saisissez une seule heure lorsque l’événement se termine par une représentation de date et d’heure combinée. Utiliser le format <code>({date}T{time}</code>; par exemple, <code>2017-08-29T04:00:00.0000000</code>. Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Type de contrainte dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder on]</td> 
   <td>Indiquez si vous souhaitez activer un rappel pour cet événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Saisissez ou mappez le nombre de minutes avant le début de l’événement lorsque le rappel doit se déclencher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Sélectionnez l’importance de cet événement.</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Support]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensibilité] </td> 
   <td> <p>Sélectionnez la sensibilité de cet événement.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>Le destinataire voit un message "[!UICONTROL Veuillez le traiter comme personnel]".</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>Le destinataire voit un message "[!UICONTROL Veuillez le traiter comme privé]". Cet événement n'est pas transféré ou redirigé par les règles de la boîte de réception du destinataire.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>Le destinataire voit un message "[!UICONTROL Veuillez le traiter comme confidentiel]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type de contenu du corps]</td> 
   <td>Indiquez si le contenu du corps du message associé à l’événement est en texte brut ou en HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenu du corps]</td> 
   <td>Saisissez ou mappez le corps du message associé à l’événement. Il peut être au format HTML ou texte (comme spécifié dans le champ [!UICONTROL Body Content Type] ci-dessus).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Emplacement]</td> 
   <td> <p>Saisissez les détails de l’emplacement de l’événement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Réponse demandée]</td> 
   <td>Sélectionner <strong>[!UICONTROL Oui]</strong> pour demander à l’invité d’envoyer une réponse à l’invitation de l’événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Afficher sous]</td> 
   <td> <p>Sélectionnez le mode d’affichage de l’événement pour les personnes qui visualisent votre calendrier.</p> 
    <ul> 
     <li>[!UICONTROL Libre]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL Occupé]</li> 
     <li>[!UICONTROL Absence du bureau]</li> 
     <li>[!UICONTROL Travail ailleurs]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Participants]</p> </td> 
   <td> <p>Ajoutez des participants à l’événement.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom du participant.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Saisissez l’adresse électronique du participant.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Catégorie]</td> 
   <td>Entrez ou mappez les catégories que vous souhaitez que l’événement s’affiche comme sur le calendrier.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un événement]

Ce module d’action supprime un événement existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Saisissez ou mappez l’identifiant de l’événement que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendrier

* [[!UICONTROL Liste des calendriers]](#list-calendars)
* [[!UICONTROL Obtention d’un calendrier]](#get-a-calendar)
* [[!UICONTROL Création d’un calendrier]](#create-a-calendar)
* [[!UICONTROL Mise à jour d’un calendrier]](#update-a-calendar)
* [[!UICONTROL Suppression d’un calendrier]](#delete-a-calendar)

#### [!UICONTROL Liste des calendriers]

Ce module de recherche récupère une liste de tous les calendriers de l’utilisateur authentifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de groupe de calendrier]</td> 
   <td>Sélectionnez le [!UICONTROL Groupe de calendrier] qui contient les calendriers que vous souhaitez répertorier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Entrer le nombre maximal de calendriers [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un calendrier]

Ce module d’action récupère les détails d’un seul calendrier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendrier]</td> 
   <td> <p>Saisissez ou mappez l’identifiant du calendrier dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Création d’un calendrier]

Ce module d’action crée un nouveau calendrier dans votre compte Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom du calendrier]</td> 
   <td> <p>Saisissez un nom pour le nouveau calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mise à jour d’un calendrier]

Ce module d’action édite un calendrier existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendrier]</td> 
   <td>Saisissez l’[!UICONTROL ID du calendrier pour le calendrier que vous souhaitez mettre à jour. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nouveau nom du calendrier]</td> 
   <td> <p>Saisissez un nom pour le nouveau calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un calendrier]

Ce module d&#39;action supprime un calendrier existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de calendrier]</td> 
   <td>Saisissez l’ID [!UICONTROL Calendrier] du calendrier que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

### Autre

#### [!UICONTROL Lancer un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL Office 365] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à <code>https://graph.microsoft.com</code>. Exemple :<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Sélectionnez la méthode de requête HTTP dont vous avez besoin pour configurer l’appel API. Pour plus d’informations, voir <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Méthodes de requête HTTP dans [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Remarque :   <p>lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
