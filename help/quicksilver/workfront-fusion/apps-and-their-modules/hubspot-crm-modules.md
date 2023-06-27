---
title: Modules CRM HubSpot
description: Le [!DNL Adobe Workfront Fusion] Les modules CRM HubSpot vous permettent de surveiller les événements, les enregistrements, les contacts, les engagements, les envois de fichiers et de formulaires, ou de créer, récupérer, mettre à jour et supprimer des enregistrements, des contacts, des engagements, des événements ou des fichiers dans vos [!DNL HubSpot CRM] compte .
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2533'
ht-degree: 0%

---

# [!DNL HubSpot CRM] modules

Le [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] Les modules vous permettent de surveiller les événements, les enregistrements, les contacts, les engagements, les envois de fichiers et de formulaires, ou de créer, récupérer, mettre à jour et supprimer des enregistrements, des contacts, des engagements, des événements ou des fichiers dans vos [!DNL HubSpot CRM] compte .

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

Pour utiliser [!DNL HubSpot CRM] modules, vous devez disposer d’un [!DNL HubSpot CRM] compte .

## Connexion [!DNL Adobe Workfront Fusion] to [!DNL HubSpot CRM]

Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir [Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL HubSpot CRM] modules et leurs champs

Lorsque vous configurez [!DNL Hubspot CRM] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!DNL Hubspot CRM] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Objets CRM](#crm-objects)
* [Enregistrements (transactions, contacts et entreprises)](#records-deals-contacts-and-companies)
* [Contacts](#contacts)
* [Offres](#deals)
* [Entreprises](#companies)
* [Fichiers](#files)
* [Billets](#tickets)
* [Lancer un appel API](#make-an-api-call)

### Objets CRM

#### [!UICONTROL Recherche d’objets CRM]

Ce module de recherche recherche des objets CRM par propriétés personnalisées ou par requête. Pour rechercher des produits ou des éléments de ligne, utilisez une connexion spéciale avec une portée personnalisée requise.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Saisissez ou mappez le nombre maximal d’éléments que le module renverra dans un cycle d’exécution.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’objet à rechercher]</td> 
   <td>Sélectionnez le type d’objet CRM Hubspot que vous souhaitez rechercher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriétés de sortie]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. Les champs disponibles dépendent de l’objet sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtrer par] </td> 
   <td> <p>Sélectionner le mode de filtrage de la recherche</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Entrer ou mapper la requête</p> </li> 
     <li> <p><strong>[!UICONTROL Propriétés]</strong> </p> <p>Entrez les groupes ou filtres de votre recherche.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trier par]</td> 
   <td> <p>Cliquez sur si vous souhaitez trier les résultats. Si vous choisissez de trier les résultats, les champs suivants s’affichent. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nom de la propriété]</strong> </p> <p>Sélectionnez la propriété par laquelle vous souhaitez trier les résultats.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Choisissez si vous souhaitez trier les résultats dans une direction ascendante ou descendante.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### Enregistrements (transactions, contacts et entreprises)

* [[!UICONTROL Créer un enregistrement (hérité)]](#create-a-record-legacy)
* [[!UICONTROL Obtention d’un enregistrement]](#get-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Suppression d’un enregistrement]](#delete-a-record)
* [[!UICONTROL Obtention d’une propriété d’enregistrement]](#get-a-record-property)
* [[!UICONTROL Surveillance des enregistrements]](#watch-records)

#### [!UICONTROL Créer un enregistrement (hérité)]

Ce module d’action crée un contact, une société ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriétés]</td> 
   <td>Renseignez les propriétés que vous souhaitez définir pour l’enregistrement. Les champs disponibles dépendent du type d’enregistrement que vous souhaitez créer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un enregistrement]

Ce module d’action récupère les détails d’un contact, d’une société ou d’une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement.</p> 
    <ul> 
     <li>[!UICONTROL Contact]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td>Si vous recevez un contact, indiquez si vous souhaitez l’identifier par identifiant ou par adresse électronique.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l'identifiant du contact, de la société ou de la transaction à récupérer. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Saisissez l'adresse email du contact dont vous souhaitez récupérer les informations. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un contact, une société ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td> <p>Si vous recevez un contact, sélectionnez le mode d'identification de l'enregistrement :</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l'identifiant du contact, de la société ou de l'opération que vous souhaitez mettre à jour. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Saisissez l'adresse email du contact dont vous souhaitez mettre à jour les informations. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriétés]</td> 
   <td>Renseignez les propriétés que vous souhaitez définir pour l’enregistrement. Les champs disponibles dépendent du type d’enregistrement que vous souhaitez créer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un enregistrement]

Ce module d’action supprime un contact, une société ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement à supprimer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’identifiant du contact, de la société ou de la transaction à supprimer. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’une propriété d’enregistrement]

Ce module d’action récupère les métadonnées d’une propriété d’enregistrement spécifique par son nom (interne).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement dont vous souhaitez récupérer les métadonnées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom de la propriété]</td> 
   <td>Sélectionnez la propriété pour laquelle vous souhaitez récupérer les métadonnées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’option]</td> 
   <td> <p> Certaines propriétés disposent d’un ensemble d’options disponibles qu’un utilisateur peut sélectionner comme valeur de propriété. Saisissez l’identifiant de l’option qui représente la valeur de propriété que vous souhaitez récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Surveillance des enregistrements]

Ce module de déclenchement lance un scénario lorsqu’un contact, une société ou une transaction a été modifié ou créé au cours des 30 derniers jours. La sortie est limitée à 10 000 enregistrements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement dont la propriété doit être surveillée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Indiquez si vous souhaitez regarder les enregistrements récemment modifiés ou récemment créés.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Sélectionnez les propriétés à inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Contacts

* [[!UICONTROL Créer/mettre à jour un contact (hérité)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Créer/mettre à jour un groupe de contacts]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Ajouter des contacts à une liste]](#add-contacts-to-a-list)
* [[!UICONTROL Supprimer un contact d’une liste]](#remove-a-contact-from-a-list)
* [[!UICONTROL Fusionner les contacts]](#merge-contacts)
* [[!UICONTROL Recherche de contacts]](#search-for-contacts)
* [[!UICONTROL Répertorier les contacts]](#list-contacts)
* [[!UICONTROL Liste des contacts d’une entreprise]](#list-contacts-of-a-company)

#### [!UICONTROL Créer/mettre à jour un contact (hérité)]

Crée un contact s’il n’existe pas encore dans un portail ou le met à jour avec les dernières valeurs de propriété s’il existe dans un portail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriétés]</td> 
   <td>Renseignez les propriétés que vous souhaitez définir ou mettre à jour pour le contact. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer/mettre à jour un groupe de contacts]

Crée un groupe de contacts ou les met à jour s&#39;ils existent déjà. Les performances sont meilleures lorsque la taille du lot est limitée à 100 contacts ou moins. Les modifications effectuées via ce point de terminaison sont traitées de manière asynchrone. Plusieurs minutes peuvent donc être nécessaires pour que les modifications soient appliquées aux enregistrements de contact.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lot de contacts à créer/mettre à jour] </td> 
   <td> <p>Ajoutez le lot de contacts.</p> <p>Cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong> pour ajouter un nouveau contact. Dans la fenêtre qui s'affiche, saisissez ou mappez les informations suivantes :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Search Type]</strong> </p> <p>Sélectionnez le mode d'identification du contact :</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Saisissez l'identifiant du contact que vous souhaitez créer ou mettre à jour. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>Saisissez l'adresse email du contact que vous souhaitez créer ou mettre à jour. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Propriétés]</strong> </p> <p>Renseignez les propriétés que vous souhaitez définir ou mettre à jour pour le contact.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ajouter des contacts à une liste]

Ce module ajoute à une liste de contacts les enregistrements de contacts déjà créés dans le système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Sélectionnez l'identifiant de la liste à laquelle vous souhaitez ajouter le contact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID/e-mails] </td> 
   <td> <p>Sélectionnez le mode d'identification des contacts que vous souhaitez ajouter à la liste :</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> <p>Ajoutez les identifiants des contacts que vous souhaitez ajouter à la liste.</p> </li> 
     <li> <p>[!UICONTROL Emails]</p> <p>Ajoutez les adresses email des contacts que vous souhaitez ajouter à la liste.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un contact d’une liste]

Supprime un contact d&#39;une liste de contacts.

>[!NOTE]
>
>Vous ne pouvez pas supprimer manuellement des contacts d’une liste dynamique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Sélectionnez l'identifiant de la liste à partir de laquelle vous souhaitez supprimer le contact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de contact] </td> 
   <td>Saisissez l'identifiant du contact à supprimer de la liste. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Fusionner les contacts]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Saisissez l'identifiant de l'un des contacts que vous souhaitez fusionner. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Saisissez l'identifiant de l'autre contact que vous souhaitez fusionner.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Recherche de contacts]

Récupère une liste de contacts à l’aide de la requête de recherche.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Saisissez la requête de recherche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite] </td> 
   <td>Entrer ou mapper le nombre maximum de contacts [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier les contacts]

Renvoie tous les contacts créés dans le portail. La sortie est limitée à 5000 contacts. Pour répertorier les contacts précédents ou suivants, vous pouvez utiliser la variable [!UICONTROL advanced] pour décaler la liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Nombre maximum de contacts [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriétés de sortie]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Liste des contacts d’une entreprise]

Récupère une liste de contacts dans la société. La sortie est limitée à 5000 contacts. Pour répertorier les contacts précédents ou suivants, vous pouvez utiliser la variable [!UICONTROL advanced] pour décaler la liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l'identifiant de la société dont vous souhaitez répertorier les contacts. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Nombre maximum de contacts [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les contacts ajoutés à la liste]

Ce module de déclenchement lance un scénario lorsqu&#39;un nouveau contact est ajouté à une liste. Cette option est disponible uniquement pour les utilisateurs disposant d’un compte Marketing payant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Saisissez ou mappez l'identifiant de la liste contenant les contacts que vous souhaitez voir.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Sélectionnez les propriétés à inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d'enregistrements que le module doit renvoyer pour chaque cycle d'exécution de scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Offres

* [[!UICONTROL Lister des pipelines d’affaires/de tickets]](#list-dealticket-pipelines)
* [[!UICONTROL Obtention d’un pipeline CRM pour une transaction]](#get-a-deals-crm-pipeline)

#### [!UICONTROL Lister des pipelines d’affaires/de tickets]

Renvoie tous les pipelines d’achat et de ticket pour un portail donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’objet] </td> 
   <td>Indiquez si vous souhaitez lister les offres ou les tickets.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un pipeline CRM pour une transaction]

Renvoie un pipeline d’accords spécifique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de pipeline] </td> 
   <td>Saisissez ou mappez l’identifiant du pipeline pour lequel vous souhaitez récupérer les détails. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’évaluation] </td> 
   <td>Saisissez ou mappez l’identifiant de l’étape pour laquelle vous souhaitez récupérer les détails. </td> 
  </tr> 
 </tbody> 
</table>

### Entreprises

#### [!UICONTROL Recherche d’entreprises par domaine]

Récupère une liste d’entreprises en fonction d’une correspondance exacte avec la propriété de domaine.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>Entrez le domaine des sociétés que vous souhaitez rechercher, par exemple <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limite]</td> 
   <td>Nombre maximum d'entreprises [!DNL Workfront Fusion] doit revenir pendant un cycle d'exécution de scénario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Propriétés de sortie]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. </td> 
  </tr> 
 </tbody> 
</table>

### Fichiers

* [[!UICONTROL Création d’un dossier]](#create-a-folder)
* [[!UICONTROL Suppression d’un dossier]](#delete-a-folder)
* [[!UICONTROL Déplacer un fichier]](#move-a-file)

#### [!UICONTROL Création d’un dossier]

Ce module crée un dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder Name] </td> 
   <td>Saisissez ou mappez un nom pour le nouveau dossier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID] </td> 
   <td>Sélectionnez l’identifiant du dossier parent pour le dossier que vous créez. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un dossier]

Marque un dossier comme supprimé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’identifiant du dossier que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un fichier]

Déplace un fichier vers un autre dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID] </td> 
   <td>Saisissez ou mappez l’identifiant du fichier à déplacer. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de dossier] </td> 
   <td>Sélectionnez l’identifiant du dossier dans lequel vous souhaitez déplacer le fichier. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Saisissez le nom du fichier déplacé.</td> 
  </tr> 
 </tbody> 
</table>

### Billets

#### [!UICONTROL Suppression d’un ticket]

Supprime un ticket existant par son identifiant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’identifiant du ticket que vous souhaitez supprimer. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Lancer un appel API]

Permet d’effectuer un appel API personnalisé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour obtenir des instructions sur la connexion à [!DNL HubSpot CRM] compte à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin relatif à https://api.hubapi.com/. Par exemple, /contacts/v1/lists/all/contacts/all</p> <p>Pour obtenir la liste des points de fin disponibles, reportez-vous à la section <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] Documentation API</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Méthode [!UICONTROL]</p> </td> 
   <td> <p>Sélectionnez la méthode HTTP à utiliser :</p> <p>[!UICONTROL GET]</p> <p>pour récupérer les informations d’une entrée.</p> <p>[!UICONTROL POST]</p> <p>pour créer une entrée.</p> <p>[!UICONTROL PUT]</p> <p>pour mettre à jour/remplacer une entrée existante.</p> <p>[!UICONTROL PATCH]</p> <p>pour effectuer une mise à jour partielle des entrées.</p> <p>[!UICONTROL DELETE]</p> <p>pour supprimer une entrée.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> Saisissez les en-têtes de requête souhaités. Vous n’avez pas à ajouter d’en-têtes d’autorisation ; nous l'avons déjà fait pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Saisissez la chaîne de requête de requête de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard. Lors de l’utilisation d’instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** L’appel API suivant renvoie tous les contacts de votre [!DNL HubSpot] compte :
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Méthode**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>Les correspondances de la recherche se trouvent dans la sortie du module sous [!UICONTROL Bundle] > [!UICONTROL Corps] > [!UICONTROL contacts].
>
>Dans notre exemple, 3 contacts ont été renvoyés :
>
>![](assets/hubspot-api-output.png)

## Création d’une application

1. Connectez-vous à [!DNL HubSpot] compte développeur.
1. Sélectionnez la **[!UICONTROL Création d’une application]** .
1. Saisissez le nom de l’application et [!UICONTROL Enregistrer] de la boîte de dialogue.
1. Sélectionnez les portées dont vous aurez besoin pour votre webhook.

   Par exemple, ajoutez des portées de contacts pour déclencher le module lorsqu’un nouveau contact est créé ou supprimé.

   Le [!UICONTROL portée des contacts] est tout ce dont vous avez besoin pour recevoir des contacts, des offres et des webhooks d’événements de société.

   >[!IMPORTANT]
   >
   >Ne remplissez pas le champ [!UICONTROL URL de redirection] champ .
