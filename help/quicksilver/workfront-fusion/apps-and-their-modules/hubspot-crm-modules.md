---
title: Modules CRM HubSpot
description: Les modules CRM HubSpot  [!DNL Adobe Workfront Fusion]  vous permettent de surveiller les événements, les enregistrements, les contacts, les engagements et les envois de fichiers et de formulaires, ainsi que de les créer, récupérer, mettre à jour et supprimer dans votre compte  [!DNL HubSpot CRM] .
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 1c56cf8aa9da7ec2644955d5533c71f60160d580
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 98%

---

# Modules [!DNL HubSpot CRM]

Les modules [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] vous permettent de surveiller les événements, les enregistrements, les contacts, les engagements, les envois de fichiers et de formulaires, ainsi que de les créer, récupérer, mettre à jour et supprimer dans votre compte [!DNL HubSpot CRM].

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

Pour utiliser les modules [!DNL HubSpot CRM], vous devez disposer d’un compte [!DNL HubSpot CRM].

## Connecter [!DNL Adobe Workfront Fusion] à [!DNL HubSpot CRM]

Pour suivre la procédure de connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez la section [Créer une connexion à  [!DNL Adobe Workfront Fusion]  - Instructions de base](../../workfront-fusion/connections/connect-to-fusion-general.md).

>[!NOTE]
>
>Lors de la configuration d’une connexion, sélectionnez le type de connexion **HubSpot CRM**. Le type HubSpot CRM (obsolète) prend en charge les connexions existantes, mais il est déconseillé de l’utiliser pour créer de nouvelles connexions.

## Modules [!DNL HubSpot CRM] et leurs champs

Lorsque vous configurez les modules [!DNL Hubspot CRM], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces derniers, des champs [!DNL Hubspot CRM] supplémentaires peuvent s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton « Mapper » apparaît au-dessus d’un champ ou d’une fonction, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez la section [Mapper des informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Objets CRM](#crm-objects)
* [Enregistrements (transactions, contacts et entreprises)](#records-deals-contacts-and-companies)
* [Contacts](#contacts)
* [Transactions](#deals)
* [Entreprises](#companies)
* [Fichiers](#files)
* [Tickets](#tickets)
* [Effectuer un appel API](#make-an-api-call)

### Objets CRM

#### [!UICONTROL Rechercher des objets CRM]

Ce module de recherche recherche des objets CRM à partir de propriétés personnalisées ou de requêtes. Pour rechercher des produits ou des éléments de ligne, utilisez une connexion spéciale avec une portée personnalisée requise.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’éléments que le module renverra dans un cycle d’exécution.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type to Search]</td> 
   <td>Sélectionnez le type d’objet CRM Hubspot que vous souhaitez rechercher.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. Les champs disponibles dépendent de l’objet que vous avez sélectionné.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by] </td> 
   <td> <p>Sélectionner le mode de filtrage de la recherche</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Entrer ou mapper la requête</p> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Saisissez les groupes ou filtres de votre recherche.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>Cliquez si vous souhaitez trier les résultats. Si vous choisissez de trier les résultats, les champs suivants s’affichent. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Property name]</strong> </p> <p>Sélectionnez la propriété par laquelle vous souhaitez trier les résultats</p> </li> 
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
* [[!UICONTROL Obtenir un enregistrement]](#get-a-record)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Supprimer un enregistrement]](#delete-a-record)
* [[!UICONTROL Obtenir une propriété d’enregistrement]](#get-a-record-property)
* [[!UICONTROL Surveiller les enregistrements]](#watch-records)

#### [!UICONTROL Créer un enregistrement (hérité)]

Ce module d’action crée un contact, une entreprise ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionner le type d’enregistrement à créer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Renseignez les propriétés à définir pour l’enregistrement. Les champs disponibles dépendent du type d’enregistrement à créer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir un enregistrement]

Ce module d’action récupère les détails d’un contact, d’une entreprise ou d’une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
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
   <td>Si vous recevez un contact, indiquez si vous souhaitez l’identifier par identifiant ou par adresse e-mail.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’identifiant du contact, de l’entreprise ou de la transaction à récupérer. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Saisissez l’adresse e-mail du contact dont vous souhaitez récupérer les informations. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mettre à jour un enregistrement]

Ce module d’action met à jour un contact, une entreprise ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search Type]</td> 
   <td> <p>Si vous recevez un contact, sélectionnez le mode d’identification de l’enregistrement :</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’identifiant du contact, de l’entreprise ou de la transaction que vous souhaitez mettre à jour. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Saisissez l’adresse e-mail du contact dont vous souhaitez mettre à jour les informations. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Renseignez les propriétés à définir pour l’enregistrement. Les champs disponibles dépendent du type d’enregistrement à créer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un enregistrement]

Ce module d’action supprime un contact, une société ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement à supprimer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’identifiant du contact, de l’entreprise ou de la transaction à supprimer. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir une propriété d’enregistrement]

Ce module d’action récupère les métadonnées d’une propriété d’enregistrement spécifique par son nom (interne).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement dont vous souhaitez récupérer les métadonnées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Property Name]</td> 
   <td>Sélectionnez la propriété dont vous souhaitez récupérer les métadonnées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option ID]</td> 
   <td> <p> Certaines propriétés disposent d’un ensemble d’options disponibles qu’un utilisateur ou une utilisatrice peut sélectionner comme valeur de propriété. Saisissez l’identifiant de l’option qui représente la valeur de propriété que vous souhaitez récupérer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les enregistrements]

Ce module déclencheur lance un scénario lorsqu’un contact, une entreprise ou une transaction a fait l’objet d’une modification ou d’une création au cours des 30 derniers jours. La sortie est limitée à 10 000 enregistrements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Sélectionnez le type d’enregistrement comportant la propriété que vous souhaiter surveiller.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Indiquez si vous souhaitez surveiller les enregistrements récemment modifiés ou récemment créés.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Sélectionnez les propriétés à inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Contacts

* [[!UICONTROL Créer/mettre à jour un contact (hérité)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Créer/mettre à jour un groupe de contacts]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Ajouter des contacts à une liste]](#add-contacts-to-a-list)
* [[!UICONTROL Supprimer un contact d’une liste]](#remove-a-contact-from-a-list)
* [[!UICONTROL Fusionner les contacts]](#merge-contacts)
* [[!UICONTROL Rechercher des contacts]](#search-for-contacts)
* [[!UICONTROL Répertorier les contacts]](#list-contacts)
* [[!UICONTROL Répertorier les contacts d’une entreprise]](#list-contacts-of-a-company)

#### [!UICONTROL Créer/mettre à jour un contact (hérité)]

Crée un contact s’il n’existe pas encore dans un portail ou le met à jour avec les dernières valeurs de propriété s’il existe dans un portail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Properties]</td> 
   <td>Renseignez les propriétés que vous souhaitez définir ou mettre à jour pour le contact. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer/mettre à jour un groupe de contacts]

Crée un groupe de contacts ou les met à jour s’ils existent déjà. Les performances sont meilleures lorsque la taille du lot est limitée à 100 contacts ou moins. Les modifications effectuées via ce point d’entrée sont traitées de manière asynchrone. Plusieurs minutes peuvent donc être nécessaires pour que les modifications soient appliquées aux enregistrements de contacts.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Batch of Contacts to Create/Update] </td> 
   <td> <p>Ajoutez le lot de contacts.</p> <p>Cliquez sur <strong>[!UICONTROL Add item]</strong> pour ajouter un nouveau contact. Dans la fenêtre qui s’affiche, saisissez ou mappez les informations suivantes :</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Search Type]</strong> </p> <p>Sélectionnez le mode d’identification du contact :</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Saisissez l’ID du contact que vous souhaitez créer ou mettre à jour. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>Saisissez l’adresse e-mail du contact que vous souhaitez créer ou mettre à jour. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Properties]</strong> </p> <p>Renseignez les propriétés que vous souhaitez définir ou mettre à jour pour le contact.</p> </li> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Sélectionnez l’ID de la liste à laquelle vous souhaitez ajouter le contact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs/Emails] </td> 
   <td> <p>Sélectionnez le mode d’identification des contacts que vous souhaitez ajouter à la liste :</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>Ajoutez les ID des contacts que vous souhaitez ajouter à la liste.</p> </li> 
     <li> <p>[!UICONTROL Emails]</p> <p>Ajoutez les adresses e-mail des contacts que vous souhaitez ajouter à la liste.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un contact d’une liste]

Supprime un contact d’une liste de contacts.

>[!NOTE]
>
>Vous ne pouvez pas supprimer manuellement des contacts d’une liste dynamique.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID] </td> 
   <td>Sélectionnez l’ID de la liste à partir de laquelle vous souhaitez supprimer le contact. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID] </td> 
   <td>Saisissez l’ID du contact que vous souhaitez supprimer de la liste. </td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Saisissez l’ID de l’un des contacts que vous souhaitez fusionner. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Saisissez l’ID de l’autre contact que vous souhaitez fusionner.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rechercher des contacts]

Récupère une liste de contacts à l’aide de la requête.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td>Saisissez la requête.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Entrez ou mappez le nombre maximum de contacts que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Répertorier les contacts]

Renvoie tous les contacts qui ont été créés dans le portail. La sortie est limitée à 5 000 contacts. Pour répertorier les contacts précédents ou suivants, vous pouvez utiliser le paramètre [!UICONTROL avancé] pour décaler la liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Nombre maximum de contacts que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
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

Récupère une liste de contacts de l’entreprise. La sortie est limitée à 5 000 contacts. Pour répertorier les contacts précédents ou suivants, vous pouvez utiliser le paramètre [!UICONTROL avancé] pour décaler la liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’ID de l’entreprise dont vous souhaitez répertorier les contacts. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Nombre maximum de contacts que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les contacts ajoutés à la liste]

Ce module de déclenchement lance un scénario lorsqu’un nouveau contact est ajouté à une liste. Cette option est disponible uniquement pour les utilisateurs et utilisatrices disposant d’un compte Marketing payant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Saisissez ou mappez l’ID de la liste contenant les contacts que vous souhaitez surveiller.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Sélectionnez les propriétés à inclure dans la sortie du module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Transactions

* [[!UICONTROL Répertorier des pipelines de transactions/tickets]](#list-dealticket-pipelines)
* [[!UICONTROL Obtenir un pipeline CRM pour une transaction]](#get-a-deals-crm-pipeline)

#### [!UICONTROL Répertorier des pipelines de transactions/tickets]

Renvoie tous les pipelines de transactions et de tickets pour un portail donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type] </td> 
   <td>Indiquez si vous souhaitez répertorier les transactions ou les tickets.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtenir le pipeline CRM d’une transaction]

Renvoie le pipeline de la transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pipeline ID] </td> 
   <td>Saisissez ou mappez l’ID du pipeline dont vous souhaitez récupérer les détails. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stage ID] </td> 
   <td>Saisissez ou mappez l’ID de l’étape dont vous souhaitez récupérer les détails. </td> 
  </tr> 
 </tbody> 
</table>

### Entreprises

#### [!UICONTROL Rechercher des entreprises par domaine]

Récupère une liste d’entreprises à partir d’une correspondance exacte avec la propriété de domaine.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>Entrez le domaine des entreprises que vous souhaitez rechercher, par exemple <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Nombre maximum d’entreprises que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. </td> 
  </tr> 
 </tbody> 
</table>

### Fichiers

* [[!UICONTROL Créer un dossier]](#create-a-folder)
* [[!UICONTROL Supprimer un dossier]](#delete-a-folder)
* [[!UICONTROL Déplacer un fichier]](#move-a-file)

#### [!UICONTROL Créer un dossier]

Ce module crée un dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir la section <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder Name] </td> 
   <td>Saisissez ou mappez un nom pour le nouveau dossier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID] </td> 
   <td>Sélectionnez l’ID du dossier parent du dossier que vous créez. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Supprimer un dossier]

Marque un dossier comme supprimé.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’ID du dossier que vous souhaitez supprimer.</td> 
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
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID] </td> 
   <td>Saisissez ou mappez l’ID du fichier à déplacer. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td>Sélectionnez l’ID du dossier dans lequel vous souhaitez déplacer le fichier. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Saisissez un nom pour le fichier déplacé.</td> 
  </tr> 
 </tbody> 
</table>

### Tickets

#### [!UICONTROL Supprimer un ticket]

Supprime un ticket existant par son ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour savoir comment connecter votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], consultez <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’ID du ticket que vous souhaitez supprimer. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Lancer un appel API]

Permet d’effectuer un appel API personnalisé.

>[!NOTE]
>
>Les points d’entrée suivants ont été abandonnés dans l’API HubSpot le 31 août 2023 et ne peuvent plus être utilisés dans les modules Fusion.
>
>* Répertorier les événements de contenu
>* Répertorier les événements sociaux
>* Répertorier les événements de tâche du calendrier
>* Répertorier tous les événements du calendrier
>* Créer une tâche de calendrier
>* Obtenir la tâche du calendrier par ID
>* Mettre à jour la tâche du calendrier
>* Supprimer une tâche de calendrier

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Pour les instructions concernant la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Créer une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Saisissez un chemin d’accès relatif à https://api.hubapi.com/. Par exemple, /contacts/v1/lists/all/contacts/all.</p> <p>Pour obtenir la liste des points d’entrée disponibles, voir la documentation de l’API <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Sélectionnez la méthode HTTP à utiliser :</p> <p>[!UICONTROL GET]</p> <p>pour récupérer les informations d’une entrée.</p> <p>[!UICONTROL POST]</p> <p>pour créer une nouvelle entrée.</p> <p>[!UICONTROL PUT]</p> <p>pour mettre à jour/remplacer une entrée existante.</p> <p>[!UICONTROL PATCH]</p> <p>pour effectuer une mise à jour partielle des entrées.</p> <p>[!UICONTROL DELETE]</p> <p>pour supprimer une entrée.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p> Saisissez les en-têtes de requête de votre choix. Vous n’avez pas à ajouter d’en-têtes d’autorisation ; nous l’avons déjà fait pour vous.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Saisissez la chaîne de requête.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Ajoutez le contenu du corps de l’appel API sous la forme d’un objet JSON standard. Lorsque vous utilisez des instructions conditionnelles telles que <code>if</code> dans votre fichier JSON, placez les guillemets en dehors de l’instruction conditionnelle.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemple :** l’appel API suivant renvoie tous les contacts de votre compte [!DNL HubSpot] :
>
>**URL** : `/contacts/v1/lists/all/contacts/all`
>
>**Méthode** : `GET`
>
>![](assets/hubspot-api-config.png)
>
>Les correspondances de la recherche se trouvent dans la sortie du module sous [!UICONTROL Lot] > [!UICONTROL Corps] > [!UICONTROL Contacts].
>
>Dans notre exemple, 3 contacts ont été renvoyés :
>
>![](assets/hubspot-api-output.png)

## Créer une nouvelle application

1. Connectez-vous à votre compte de développement [!DNL HubSpot].
1. Sélectionnez l’option **[!UICONTROL Créer une application]**.
1. Saisissez le nom de l’application, puis cliquez sur [!UICONTROL Enregistrer] dans la boîte de dialogue.
1. Sélectionnez les portées dont vous aurez besoin pour votre webhook.

   Par exemple, ajoutez des portées de contacts pour déclencher le module lorsqu’un nouveau contact est créé ou supprimé.

   La [!UICONTROL portée des contacts] est tout ce dont vous avez besoin pour recevoir des webhooks de contacts, de transactions et d’événements d’entreprise.

   >[!IMPORTANT]
   >
   >Ne remplissez pas le champ [!UICONTROL URL de redirection].
