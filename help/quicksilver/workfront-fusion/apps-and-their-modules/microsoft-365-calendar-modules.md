---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connecteur
navigation-topic: apps-and-their-modules
title: Calendrier Microsoft Office 365
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent le calendrier Microsoft Office 365, et les connecter à plusieurs applications et services tiers.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1999'
ht-degree: 100%

---

# [!DNL Microsoft Office 365 Calendar]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL Microsoft Office 365 Calendar] et le connecter à plusieurs applications et services tiers.

Pour utiliser [!DNL Office 365 Calendar] avec [!DNL Adobe Workfront Fusion], vous devez disposer d’un compte [!DNL Office 365 Excel]. Vous pouvez en créer un à l’adresse [www.office.com](https://www.office.com/).

Pour obtenir des instructions sur la connexion de votre compte Office 365 à [!DNL Workfront Fusion], voir [Créer une connexion à Adobe  [!DNL Workfront Fusion]  - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md).

Une fois le consentement accordé, le système vous redirige vers la page d’administration de [!UICONTROL Workfront Fusion] où vous pouvez continuer à créer votre scénario.

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
   <p>Conditions requises du produit actuel : si vous disposez de la formule [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans la formule [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences liées aux produits hérités : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi qu’[!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], voir Licences [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser les modules [!DNL Microsoft Office 365 Calendar], vous devez disposer d’un compte [!DNL Microsoft Office 365 Calendar].

## Connexion du service [!DNL Office 365 Calendar] à [!DNL Workfront Fusion].

Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365 Calendar] à [!UICONTROL Workfront Fusion], voir [Créer une connexion à [!UICONTROL Adobe Workfront Fusion] : instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Certaines applications Microsoft utilisent la même connexion, qui est liée à des autorisations d’utilisateur ou d’utilisatrice. Ainsi, lors de la création d’une connexion, l’écran de consentement aux autorisations affiche les autorisations précédemment accordées à la connexion de cet utilisateur ou de cette utilisatrice, en plus des nouvelles autorisations nécessaires à l’application actuelle.
>
>Par exemple, si un utilisateur ou une utilisatrice dispose d’autorisations « Lire le tableau » accordées via le connecteur Excel, puis crée une connexion dans le connecteur Outlook pour lire les e-mails, l’écran de consentement aux autorisations affiche à la fois l’autorisation « Lire le tableau » déjà accordée et l’autorisation « Écrire des e-mails » nouvellement requise.

## Modules [!DNL Microsoft Office 365 Calendar] et leurs champs

Lorsque vous configurez les modules [!DNL Microsoft Office 365 Calendar], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Microsoft Office 365 Calendar] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Événement](#event)
* [Calendrier](#calendar)
* [Autre](#other)

### Événement

* [[!UICONTROL Surveiller des événements]](#watch-events)
* [[!UICONTROL Rechercher des événements]](#search-events)
* [[!UICONTROL Obtenir un événement]](#get-an-event)
* [[!UICONTROL Créer un événement]](#create-an-event)
* [[!UICONTROL Mettre à jour un événement]](#update-an-event)
* [[!UICONTROL Supprimer un événement]](#delete-an-event)

#### [!UICONTROL Surveiller des événements]

Ce module de déclenchement récupère les détails d’un événement lorsque celui-ci est créé, mis à jour, supprimé, démarré ou se termine dans le calendrier sélectionné.

>[!NOTE]
>
>Pour rechercher les occurrences supprimées d’une série d’événements, sélectionnez [!UICONTROL Par heure de mise à jour] dans le champ [!UICONTROL Surveiller les événements]. Ce module ne recherche pas les événements uniques supprimés ni les séries d’événements supprimées.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch events]</td> 
   <td> <p>Sélectionnez le mode de surveillance des événements.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By Created Time]</strong> </p> <p>Surveillez les nouveaux événements.</p> </li> 
     <li> <p><strong>[!UICONTROL By Updated Time]</strong> </p> <p>Surveillez les événements mis à jour.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Sélectionnez le [!UICONTROL calendar group] qui contient le calendrier dans lequel vous souhaitez surveiller les événements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>Sélectionnez le calendrier spécifique à surveiller.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Définissez les conditions de filtrage pour filtrer les résultats par objet, identifiant d’événement ou corps.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez le nombre maximum de messages que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des événements]

Ce module de recherche récupère les détails d’un événement lorsque celui-ci est créé, mis à jour, supprimé, démarré ou se termine dans le calendrier sélectionné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Sélectionnez le [!UICONTROL calendar group] qui contient le calendrier dans lequel vous souhaitez surveiller les événements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>Sélectionnez le calendrier spécifique à surveiller.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Définissez les conditions de filtrage pour filtrer les résultats. Vous pouvez filtrer selon les propriétés suivantes :</p> 
    <ul> 
     <li>[!UICONTROL Subject]</li> 
     <li>[!UICONTROL Event ID]</li> 
     <li>[!UICONTROL Created Date Time]</li> 
     <li>[!UICONTROL Last Modified Date Time]</li> 
     <li>[!UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>Sélectionnez le mode de classement des résultats.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, croissant ou décroissant</li> 
     <li><strong>[!UICONTROL Created Date Time]</strong>, croissant ou décroissant</li> 
     <li><strong>[!UICONTROL Last Modified Date Time]</strong>, croissant ou décroissant</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez le nombre maximal d’événements que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un événement]

Ce module d’action récupère les détails de l’événement spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Saisissez ou mappez l’ID de l’événement dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un événement]

Ce module d’action crée un nouvel événement.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Saisissez ou mappez un titre pour l’événement créé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start date]</td> 
   <td> Saisissez le moment où l’événement commence, en indiquant une date et une heure. Utilisez le format <code>({date}T{time}</code> ; par exemple, <code>2017-08-29T04:00:00.0000000</code>. Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End date]</td> 
   <td> Saisissez le moment où l’événement se termine, en indiquant une date et une heure. Utilisez le format <code>{date}T{time}</code> ; par exemple, <code>2017-08-29T04:00:00.0000000</code>. Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</td> 
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
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Sélectionnez la sensibilité de cet événement.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>La personne destinataire voit un message « [!UICONTROL Please treat this as Personal] ».</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>La personne destinataire voit un message « [!UICONTROL Please treat this as Private] ». Cet événement n'est pas transféré ou redirigé par les règles de la boîte de réception de la personne destinataire.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>La personne destinataire voit un message « [!UICONTROL Please treat this as Confidential] ». </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content type]</td> 
   <td>Indiquez si le contenu du corps est en texte brut ou en HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td>Saisissez ou mappez le corps du message associé à l’événement. Il peut être au format HTML ou texte (comme spécifié dans le champ [!UICONTROL Body Content Type] ci-dessus).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Saisissez les détails de l’emplacement de l’événement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Response requested]</td> 
   <td>Sélectionnez <strong>[!UICONTROL Yes]</strong> pour demander à la personne invitée d’envoyer une réponse à l’invitation de l’événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show as]</td> 
   <td> <p>Sélectionnez le mode d’affichage de l’événement pour les personnes qui consultent votre calendrier.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL Busy]</li> 
     <li>[!UICONTROL Out of office]</li> 
     <li>[!UICONTROL Working elsewhere]</li> 
     <li>[!UICONTROL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attendees]</p> </td> 
   <td> <p>Ajoutez des personnes participant à l’événement.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom de la personne participante.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Saisissez l’adresse e-mail de la personne participante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>Saisissez ou mappez les catégories que vous souhaitez que l’événement affiche comme sur le calendrier.</td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Start date]</td> 
   <td> Saisissez le moment où l’événement commence, en indiquant une date et une heure. Utilisez le format <code>{date}T{time}</code> ; par exemple, <code>2017-08-29T04:00:00.0000000</code>. Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End date]</td> 
   <td> Saisissez le moment où l’événement se termine, en indiquant une date et une heure. Utilisez le format <code>({date}T{time}</code> ; par exemple, <code>2017-08-29T04:00:00.0000000</code>. Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</td> 
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
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Sélectionnez la sensibilité de cet événement.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>La personne destinataire voit un message « [!UICONTROL Please treat this as Personal] ».</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>La personne destinataire voit un message « [!UICONTROL Please treat this as Private] ». Cet événement n'est pas transféré ou redirigé par les règles de la boîte de réception de la personne destinataire.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>La personne destinataire voit un message « [!UICONTROL Please treat this as Confidential] ». </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content type]</td> 
   <td>Indiquez si le contenu du corps du message associé à l’événement est en texte brut ou en HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td>Saisissez ou mappez le corps du message associé à l’événement. Il peut être au format HTML ou texte (comme spécifié dans le champ [!UICONTROL Body Content Type] ci-dessus).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Saisissez les détails de l’emplacement de l’événement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Response requested]</td> 
   <td>Sélectionnez <strong>[!UICONTROL Yes]</strong> pour demander à la personne invitée d’envoyer une réponse à l’invitation de l’événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show as]</td> 
   <td> <p>Sélectionnez le mode d’affichage de l’événement pour les personnes qui consultent votre calendrier.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL Busy]</li> 
     <li>[!UICONTROL Out of office]</li> 
     <li>[!UICONTROL Working elsewhere]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attendees]</p> </td> 
   <td> <p>Ajoutez des personnes participant à l’événement.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Saisissez le nom de la personne participante.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Saisissez l’adresse e-mail de la personne participante.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>Saisissez ou mappez les catégories que vous souhaitez que l’événement affiche comme sur le calendrier.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un événement]

Ce module d’action supprime un événement existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Saisissez ou mappez l’ID de l’événement que vous souhaitez supprimer.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Calendrier

* [[!UICONTROL Répertorier les calendriers]](#list-calendars)
* [[!UICONTROL Obtenir un calendrier]](#get-a-calendar)
* [[!UICONTROL Créer un calendrier]](#create-a-calendar)
* [[!UICONTROL Mettre à jour un calendrier]](#update-a-calendar)
* [[!UICONTROL Supprimer un calendrier]](#delete-a-calendar)

#### [!UICONTROL Répertorier les calendriers]

Ce module de recherche récupère une liste de tous les calendriers de la personne authentifiée.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Sélectionnez le [!UICONTROL calendar group] qui contient les calendriers que vous souhaitez répertorier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez le nombre maximal de calendriers que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un calendrier]

Ce module d’action récupère les détails d’un seul calendrier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Saisissez ou mappez l’ID du calendrier dont vous souhaitez récupérer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un calendrier]

Ce module d’action crée un nouveau calendrier dans votre compte Google.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar name]</td> 
   <td> <p>Saisissez un nom pour le nouveau calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un calendrier]

Ce module d’action modifie un calendrier existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td>Saisissez l’[!UICONTROL Calendar ID] pour le calendrier que vous souhaitez mettre à jour. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New Calendar name]</td> 
   <td> <p>Saisissez un nom pour le nouveau calendrier.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un calendrier]

Ce module d&#39;action supprime un calendrier existant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL Office 365] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td>Saisissez l’[!UICONTROL Calendar] du calendrier que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

### Autre

#### [!UICONTROL Réaliser un appel API]

Ce module vous permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Pour les instructions concernant la connexion de votre compte [!DNL Office 365] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td> <p>Ajoutez les en-têtes de la requête sous la forme d’un objet JSON standard. Par exemple : <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] ajoute les en-têtes d’autorisation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Ajoutez la requête pour l’appel API sous la forme d’un objet JSON standard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard.</p> <p>Note :   <p>Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
