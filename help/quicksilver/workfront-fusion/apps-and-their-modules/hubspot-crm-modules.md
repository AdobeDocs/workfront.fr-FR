---
title: Modules CRM HubSpot
description: Les modules CRM HubSpot  [!DNL Adobe Workfront Fusion]  vous permettent de surveiller les événements, les enregistrements, les contacts, les engagements et les envois de fichiers et de formulaires, ainsi que de les créer, récupérer, mettre à jour et supprimer dans votre compte  [!DNL HubSpot CRM] .
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: d550ba76a5a6c1d241d1dc73e63e49ef4c22a40d
workflow-type: tm+mt
source-wordcount: '6394'
ht-degree: 41%

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
* [Engagements](#engagements)
* [Événements et notifications](#events-and-notifications)
* [Fichiers](#files)
* [Tâches](#tasks)
* [Utilisateurs](#users)
* [Tickets](#tickets)
* [Formulaires](#forms)
* [Réseaux sociaux (diffusion)](#social-media-broadcast)
* [Publications de blog](#blog-posts)
  <!--* [Workflows]-->
* [Abonnements](#subscriptions)
  <!--* [Associations](#associations)-->
* [Autre](#other)

+++**Objets CRM**

### Objets CRM

* [Recherche d’objets CRM](#search-for-crm-objects)
* [Surveiller les objets CRM](#watch-crm-objects)

#### [!UICONTROL Rechercher des objets CRM]

Ce module de recherche recherche des objets CRM à partir de propriétés personnalisées ou de requêtes. Pour rechercher des produits ou des éléments de ligne, utilisez une connexion spéciale avec une portée personnalisée requise.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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
  </tr> 
   <tr> 
    <td role="rowheader">Début du décalage</td> 
    <td>Saisissez ou mappez l’identifiant du premier élément pour lequel vous souhaitez récupérer les détails. Ce module ne renvoie que 5 000 résultats à la fois. La définition d’un décalage de début vous permet de récupérer des éléments autres que les 5 000 premiers. Si le décalage de début est de 5 000, le module renvoie les éléments 5 000 à 9 999.</td> 
   </tr>
 </tbody> 
</table>

#### Surveiller les objets CRM

Ce module de déclenchement lance un scénario lorsqu’un objet CRM est créé ou mis à jour.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’éléments que le module renverra dans un cycle d’exécution.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’objet à rechercher]</td> 
   <td> <p>Sélectionnez le type d’objet que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Sélectionnez les propriétés que vous souhaitez inclure dans la sortie pour ce module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Créé/Mis à jour]</td> 
   <td>Indiquez si vous souhaitez regarder les objets créés (nouveaux) ou mis à jour (modifiés).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter by]</td> 
   <td>Vous pouvez ajouter un filtre pour vous assurer que le scénario ne commence que lorsque certaines conditions sont remplies.<ul><li><b>Requête</b><p>Saisissez la requête à utiliser pour filtrer.</li><li><b>Propriétés</b><p>Pour chaque propriété que vous souhaitez utiliser pour filtrer les résultats, cliquez sur <b>Ajouter un élément</b> et saisissez le nom, l’opérateur et la valeur de la propriété.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Enregistrements (transactions, contacts et entreprises)**

### Enregistrements (transactions, contacts et entreprises)

* [Créer un enregistrement](#create-a-record)
* [[!UICONTROL Créer un enregistrement (hérité)]](#create-a-record-legacy)
* [[!UICONTROL Supprimer un enregistrement]](#delete-a-record)
* [[!UICONTROL Obtenir un enregistrement]](#get-a-record)
* [[!UICONTROL Obtenir une propriété d’enregistrement]](#get-a-record-property)
* [Lister les enregistrements](#list-records)
* [[!UICONTROL Mettre à jour un enregistrement]](#update-a-record)
* [[!UICONTROL Surveiller les enregistrements]](#watch-records)

#### Créer un enregistrement

Ce module d’action crée un contact, une société ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groupes de propriétés [!UICONTROL]</td> 
   <td>Pour chaque propriété à ajouter lors de la création de l’enregistrement, sélectionnez le groupe dans lequel se trouve la propriété. Le groupe de propriétés s’ouvre. Vous pouvez ensuite remplir la valeur des propriétés. Les groupes de propriétés et les propriétés disponibles dépendent du type d’enregistrement que vous souhaitez créer.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un enregistrement (hérité)]

Ce module d’action crée un contact, une entreprise ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez créer.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### [!UICONTROL Obtenir un enregistrement]

Ce module d’action récupère les détails d’un contact, d’une entreprise ou d’une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### [!UICONTROL Obtenir une propriété d’enregistrement]

Ce module d’action récupère les métadonnées d’une propriété d’enregistrement spécifique par son nom (interne).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### Lister les enregistrements

Ce module de recherche renvoie une liste de contacts, de sociétés ou d’offres. La production est limitée à 5 000 contacts, 12 500 entreprises, soit 12 500 offres.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Sélectionnez le type d’enregistrement que vous souhaitez renvoyer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Sélectionnez les propriétés que vous souhaitez inclure dans la sortie pour ce module.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximum d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### [!UICONTROL Surveiller les enregistrements]

Ce module déclencheur lance un scénario lorsqu’un contact, une entreprise ou une transaction a fait l’objet d’une modification ou d’une création au cours des 30 derniers jours. La sortie est limitée à 10 000 enregistrements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

+++

+++**Contacts**

### Contacts

* [[!UICONTROL Ajouter des contacts à une liste]](#add-contacts-to-a-list)
* [Créer/mettre à jour un contact](#createupdate-a-contact)
* [[!UICONTROL Créer/mettre à jour un contact (hérité)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Créer/mettre à jour un groupe de contacts]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Répertorier les contacts]](#list-contacts)
* [[!UICONTROL Répertorier les contacts d’une entreprise]](#list-contacts-of-a-company)
* [[!UICONTROL Fusionner les contacts]](#merge-contacts)
* [[!UICONTROL Supprimer un contact d’une liste]](#remove-a-contact-from-a-list)
* [[!UICONTROL Rechercher des contacts]](#search-for-contacts)
* [Surveiller les contacts ajoutés à une liste](#watch-contacts-added-to-a-list)

#### [!UICONTROL Ajouter des contacts à une liste]

Ce module ajoute à une liste de contacts les enregistrements de contacts déjà créés dans le système.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### Créer/mettre à jour un contact

Ce module d’action crée un contact s’il n’existe pas dans un portail. Si le contact existe dans le portail, ce module le met à jour avec les valeurs fournies.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groupes de propriétés [!UICONTROL]</td> 
   <td>Pour chaque propriété à ajouter lors de la création du contact, sélectionnez le groupe dans lequel se trouve la propriété. Le groupe de propriétés s’ouvre. Vous pouvez ensuite remplir les valeurs des propriétés.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer/mettre à jour un contact (hérité)]

Crée un contact s’il n’existe pas encore dans un portail ou le met à jour avec les dernières valeurs de propriété s’il existe dans un portail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### [!UICONTROL Répertorier les contacts]

Renvoie tous les contacts qui ont été créés dans le portail. La sortie est limitée à 5 000 contacts. Pour répertorier les contacts précédents ou suivants, vous pouvez utiliser le paramètre [!UICONTROL avancé] pour décaler la liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Nombre maximum de contacts que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Sélectionnez les propriétés à afficher dans la sortie du module. </td> 
  </tr> 
   <tr> 
    <td role="rowheader">ID de contact [décalage de début] </td> 
    <td>Saisissez ou mappez l’identifiant de l’utilisateur que vous souhaitez lancer la liste. Par exemple, la définition de l’ID de contact comme ID du 101e contact permettra au module de répertorier les contacts 101-5100 plutôt que 1-5000. </td> 
   </tr>
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’ID de l’entreprise dont vous souhaitez répertorier les contacts. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Nombre maximum de contacts que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario. </td> 
  </tr> 
   <tr> 
    <td role="rowheader">ID de contact [décalage de début] </td> 
    <td>Saisissez ou mappez l’identifiant de l’utilisateur que vous souhaitez lancer la liste. Par exemple, la définition de l’ID de contact comme ID du 101e contact permettra au module de répertorier les contacts 101-5100 plutôt que 1-5000. </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL Fusionner les contacts]

Ce module d&#39;action fusionne les contacts

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### [!UICONTROL Rechercher des contacts]

Récupère une liste de contacts à l’aide de la requête.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### [!UICONTROL Surveiller les contacts ajoutés à la liste]

Ce module de déclenchement lance un scénario lorsqu’un nouveau contact est ajouté à une liste. Cette option est disponible uniquement pour les utilisateurs et utilisatrices disposant d’un compte Marketing payant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

+++

+++**Offres**

### Transactions

* [[!UICONTROL Obtenir un pipeline CRM pour une transaction]](#get-a-deals-crm-pipeline)
* [[!UICONTROL Répertorier des pipelines de transactions/tickets]](#list-dealticket-pipelines)

#### [!UICONTROL Obtenir un pipeline CRM pour une transaction]

Renvoie le pipeline de la transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### [!UICONTROL Répertorier des pipelines de transactions/tickets]

Renvoie tous les pipelines de transactions et de tickets pour un portail donné.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type] </td> 
   <td>Indiquez si vous souhaitez répertorier les transactions ou les tickets.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Entreprises**

### Entreprises

#### [!UICONTROL Rechercher des entreprises par domaine]

Récupère une liste d’entreprises à partir d’une correspondance exacte avec la propriété de domaine.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

+++

+++**Engagements**

### Engagements

* [Associer un engagement à un objet CRM](#associate-an-engagement-with-a-crm-object)
* [Création d’un engagement](#create-an-engagement)
* [Suppression d’un engagement](#delete-an-engagement)
* [Engagements de contrôle](#watch-engagements)

#### Associer un engagement à un objet CRM

Ce module d’action associe un engagement à un contact, une entreprise ou une transaction.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Sélectionnez le type d'enregistrement CRM auquel vous souhaitez associer un engagement. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID D’Engagement]</td> 
  <td>Saisissez ou mappez l’identifiant de l’engagement que vous souhaitez associer à l’objet.</td> 
   </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record ID]</td> 
  <td>Saisissez ou mappez l’identifiant de l’enregistrement auquel vous souhaitez associer l’engagement.</td> 
   </tr> 
 </tbody> 
</table>

#### Création d’un engagement

Ce module d’action crée un engagement (une note, une tâche ou une activité, par exemple) avec un objet CRM dans HubSpot. Les engagements sont toute interaction avec un contact qui doit être consigné dans le CRM.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Est Actif ?]</td> 
   <td>Activez cette option si le nouvel engagement sera actif lors de sa création. Un engagement doit être actif pour apparaître dans la chronologie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
  <td>Sélectionnez le type d’engagement que vous souhaitez créer.
  <ul>
  <li><b>E-mail</b><p></p>Passez à <a href="#email-metadata" class="MCXref xref" >Métadonnées de courrier électronique</a>.</p></li>
  <li><b>Appeler</b><p>Passez à <a href="#call-metadata" class="MCXref xref" >Appeler les métadonnées</a>.</p></li>
  <li><b>Réunion</b><p>Passez à <a href="#meeting-fields" class="MCXref xref" >Champs de la réunion</a>.</p></li>
  <li><b>Tâche</b><p>Passez à <a href="#task-fields" class="MCXref xref" >Champs de la tâche</a>.</p></li>
  <li><b>Note</b><p>Dans le champ Corps , saisissez le texte de la note.</p></li>
  </ul>
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Horodatage</td> 
   <td>Saisissez ou mappez un horodatage pour l’engagement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID de propriétaire</td> 
   <td>Saisissez ou mappez l’ID de propriétaire de la personne à laquelle l’engagement sera affecté.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">UID</td> 
   <td>Saisissez ou mappez un identifiant pour l’engagement, qui peut être utilisé entre les types d’objets.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Identifiant du portail</td> 
   <td>Saisissez ou mappez l’identifiant du portail. Cela s’avère utile si votre entreprise dispose de plusieurs portails.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contacts associés</td> 
   <td>Pour chaque contact auquel vous souhaitez associer cet engagement, cliquez sur <b>Ajouter un élément</b> et saisissez l’ID de contact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sociétés associées</td> 
   <td>Pour chaque société à laquelle vous souhaitez associer cet engagement, cliquez sur <b>Ajouter un élément</b> et saisissez l’ID de société.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Transactions associées</td> 
   <td>Pour chaque transaction à laquelle vous souhaitez associer cet engagement, cliquez sur <b>Ajouter un élément</b> et saisissez l’ID de transaction.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Billets associés</td> 
   <td>Pour chaque ticket auquel vous souhaitez associer cet engagement, cliquez sur <b>Ajouter un élément</b> et saisissez l’identifiant du ticket.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pièces jointes</td> 
   <td>Pour chaque pièce jointe à laquelle vous souhaitez associer cet engagement, cliquez sur <b>Ajouter un élément</b> et saisissez l’identifiant du fichier à joindre.</td> 
  </tr> 
 </tbody> 
</table>

##### Métadonnées des emails

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL À partir de &gt; Email]</p> </td> 
   <td> <p>Saisissez ou mappez l’adresse électronique à partir de laquelle l’email sera envoyé.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL First Name]</td> 
   <td>Saisissez ou mappez le prénom de la personne à partir de laquelle l'email sera envoyé.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Last Name]</td> 
  <td>Saisissez ou mappez le nom de la personne à partir de laquelle l'email sera envoyé.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">À</td> 
   <td>Pour chaque adresse électronique à laquelle vous souhaitez envoyer l’adresse électronique, cliquez sur <b>Ajouter un élément</b> et saisissez ou mappez l’adresse électronique.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cc</td> 
   <td>Pour chaque adresse électronique à laquelle vous souhaitez envoyer le courrier électronique, cliquez sur <b>Ajouter un élément</b> et saisissez ou mappez l’adresse électronique.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cci</td> 
   <td>Pour chaque adresse électronique à laquelle vous souhaitez envoyer l’email, cliquez sur <b>Ajouter un élément</b> et saisissez ou mappez l’adresse électronique.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objet</td> 
   <td>Saisissez ou mappez le texte de l'objet du courrier électronique.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">HTML</td> 
   <td>Pour envoyer un email au format HTML, saisissez ou mappez le corps de l'email, y compris les balises d'HTML.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Texte</td> 
   <td>Pour envoyer un email au format texte uniquement, saisissez ou mappez le texte du corps de l'email.</td> 
  </tr> 
 </tbody> 
</table>

##### Appeler des métadonnées

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL À Nombre]</p> </td> 
   <td> <p>Saisissez ou mappez le numéro de téléphone vers lequel l'appel sera effectué.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL À Partir Du Numéro]</td> 
   <td>Saisissez ou mappez le numéro de téléphone à partir duquel l'appel sera effectué.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
  <td>Sélectionnez l’état de l’appel.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Corps</td> 
   <td>Saisissez ou mappez les détails ou les notes de l’appel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Identifiant externe</td> 
   <td>Ce champ représente l’identifiant interne d’un appel effectué dans HubSpot. Cela ne nécessite aucune action.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Durée</td> 
   <td>Saisissez ou mappez la longueur de l’appel en millisecondes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Identifiant de compte externe</td> 
   <td>Ce champ représente l’identifiant de compte interne d’un appel effectué dans HubSpot. Cela ne nécessite aucune action.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL d’enregistrement</td> 
   <td>Saisissez ou mappez l’URL du fichier d’enregistrement.</td> 
  </tr> 
 </tbody> 
</table>

##### Champs de réunion

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Title]</p> </td> 
   <td> <p>Saisissez ou mappez le titre ou le sujet de la réunion.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Saisissez ou mappez le texte de la description ou des détails de la réunion.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Heure de début]</td> 
  <td>Saisissez ou mappez l’heure de début de la réunion sous la forme d’un horodatage UNIX.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Heure de fin</td> 
   <td>Saisissez ou mappez l’heure de fin de la réunion sous la forme d’un horodatage UNIX.</td> 
  </tr> 
 </tbody> 
</table>

##### Champs de tâche

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Subject]</p> </td> 
   <td> <p>Saisissez ou mappez le titre ou l’objet de la tâche.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Saisissez ou mappez le texte de la description ou des détails de la tâche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Statut</td> 
   <td>Sélectionnez l’état de la tâche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pour Le Type D’Objet]</td> 
  <td>Saisissez <code>CONTACT</code> ou <code>COMPANY</code>.
  </td> 
   </tr> 
 </tbody> 
</table>

#### Suppression d’un engagement

Ce module d’action supprime un engagement par son identifiant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Saisissez ou mappez l’identifiant de l’engagement que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### Engagements de contrôle

Ce module de déclenchement lance un scénario lorsqu’un nouvel engagement est créé dans un portail. Ce module renvoie uniquement les enregistrements créés au cours des 30 derniers jours, ou les 10 000 enregistrements créés le plus récemment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Nombre maximum d’entreprises que [!DNL Workfront Fusion] doit renvoyer pendant un cycle d’exécution de scénario. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since]</td> 
   <td>Saisissez ou mappez la date la plus ancienne à laquelle vous souhaitez suivre les événements. Utilisez le format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Événements et notifications**

### Événements et notifications

* [Créer/mettre à jour un événement de chronologie](#create--update-a-timeline-event)
* [Liste des types d’événements de journal](#list-timeline-event-types)
* [Événements de calendrier surveillés](#watch-calendar-events)
* [Notifications Watch](#watch-notifications)

#### Créer/mettre à jour un événement de chronologie

Ce module d’action crée ou met à jour un événement de frise chronologique. Ce module ne peut être utilisé qu’avec une connexion de développeur qui inclut votre identifiant utilisateur, votre clé API HubSpot, votre identifiant client et votre secret client.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’application]</td> 
   <td>Saisissez ou mappez l’identifiant de l’application à laquelle cet événement appartient.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td>Saisissez ou mappez un identifiant pour cet événement. Les ID d’événement ne sont pas générés par le système.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Type ID]</td> 
   <td>Saisissez ou mappez l’identifiant du type d’événement de cet événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Saisissez ou mappez l’adresse électronique du contact pour lequel vous créez l’événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object ID]</td> 
   <td>Saisissez ou mappez l’identifiant du contact pour lequel vous créez l’événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp]</td> 
   <td>Saisissez ou mappez l’horodatage de cet événement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Données personnalisées]</td> 
   <td>Pour chaque élément de données personnalisées à ajouter à cet événement, cliquez sur <b>Ajouter un élément</b> et saisissez le nom et la valeur de l’élément.</td> 
  </tr> 
 </tbody> 
</table>

#### Liste des types d’événements de journal

Ce module de recherche renvoie une liste de tous les événements de chronologie d’une application spécifique. Ce module ne peut être utilisé qu’avec une connexion de développeur qui inclut votre identifiant utilisateur, votre clé API HubSpot, votre identifiant client et votre secret client.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’application]</td> 
   <td>Saisissez ou mappez l’identifiant de l’application à laquelle ces événements appartiennent. </td> 
  </tr> 
 </tbody> 
</table>

#### Événements de calendrier surveillés

Ce module de déclenchement lance un scénario lorsqu’un nouvel événement est ajouté à un calendrier. Il comprend jusqu’à 500 tâches dans l’intervalle entre la date de début et la date de fin. Ce module ne peut être utilisé qu’avec une connexion de développeur qui inclut votre identifiant utilisateur, votre clé API HubSpot, votre identifiant client et votre secret client.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Type]</td> 
   <td>Indiquez si vous souhaitez suivre les événements de réseaux sociaux, les événements de contenu ou tous les événements.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de fichiers que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>Saisissez ou mappez la date de début.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>Saisissez ou mappez la date de fin.</td> 
  </tr> 
 </tbody> 
</table>

#### Notifications Watch

Ce module de déclenchement lance un scénario lorsqu’une nouvelle notification de modifications est envoyée.  Il comprend jusqu’à 500 tâches dans l’intervalle entre la date de début et la date de fin. Ce module ne peut être utilisé qu’avec une connexion de développeur qui inclut votre identifiant utilisateur, votre clé API HubSpot, votre identifiant client et votre secret client. Dans HubSpot, vous ne pouvez avoir qu’une seule URL webhook par application de développement.

Pour créer un webhook pour ce module, cliquez sur **Ajouter** en regard du champ webhook et renseignez les champs suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID d’application]</td> 
   <td>Saisissez l’ID de l’application que vous souhaitez utiliser pour ce webhook. Vous pouvez trouver l’identifiant dans votre portail de développement HubSpot.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abonnements]</td> 
   <td> <p>Pour chaque type de notification à regarder, cliquez sur <b>Ajouter un élément</b> et sélectionnez le type d'abonnement.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Forcer à supprimer les anciens abonnements]</td> 
   <td>Activez cette option pour désolidariser ou supprimer les anciens abonnements attachés à ce webhook.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Fichiers**

### Fichiers

* [[!UICONTROL Créer un dossier]](#create-a-folder)
* [Suppression d’un fichier](#delete-a-file)
* [[!UICONTROL Supprimer un dossier]](#delete-a-folder)
* [Fichiers de liste](#list-files)
* [[!UICONTROL Déplacer un fichier]](#move-a-file)
* [Charger un fichier](#upload-a-file)
* [Fichiers de contrôle](#watch-files)

#### [!UICONTROL Créer un dossier]

Ce module crée un dossier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### Suppression d’un fichier

Ce module d’action supprime définitivement un fichier et toutes les données et miniatures associées du gestionnaire de fichiers.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Saisissez ou mappez l’identifiant du fichier que vous souhaitez supprimer.</td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant du dossier que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### Fichiers de liste

Ce module de recherche renvoie une liste de fichiers stockés dans le gestionnaire de fichiers.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de fichiers que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Saisissez ou mappez l’identifiant du dossier contenant les fichiers que vous souhaitez répertorier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Pour inclure uniquement les fichiers contenant des caractères spécifiques dans le nom de fichier, saisissez ou mappez les caractères que vous souhaitez inclure dans le nom de fichier.</td> 
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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

#### Chargement d’un fichier

Ce module d’action charge un fichier dans le gestionnaire de fichiers.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Sélectionnez un fichier source à partir d’un module précédent ou mappez le nom et les données du fichier source.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type d’accès] </td> 
   <td>Indiquez si vous souhaitez que le fichier soit privé, public mais non indexable ou public et indexable. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td>Sélectionnez l’identifiant du dossier dans lequel vous souhaitez charger le fichier. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Activez cette option pour remplacer le fichier s’il existe déjà dans le dossier.</td> 
  </tr> 
 </tbody> 
</table>

### Fichiers de contrôle

Ce module de déclenchement lance un scénario lorsqu’un nouveau fichier est enregistré dans le gestionnaire de fichiers.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de fichiers que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Saisissez ou mappez l’identifiant du dossier contenant les fichiers à regarder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Pour inclure uniquement les fichiers contenant des caractères spécifiques dans le nom de fichier, saisissez ou mappez les caractères que vous souhaitez inclure dans le nom de fichier.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tâches**

### Tâches

* [Créer une tâche de calendrier](#create-a-calendar-task)
* [Suppression d’une tâche de calendrier](#create-a-calendar-task)
* [Événements de tâches de contrôle](#watch-task-events)

#### Création d’une tâche de calendrier

Ce module d’action crée une nouvelle tâche pour un calendrier. La connexion utilisée dans ce module doit utiliser les informations d’identification d’un utilisateur disposant d’un compte Marketing payant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Saisissez ou mappez un nom pour la nouvelle tâche de calendrier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Saisissez ou mappez une description pour la nouvelle tâche de calendrier.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de propriétaire]</td> 
   <td>Saisissez ou mappez l’identifiant du propriétaire de l’utilisateur affecté à cette tâche.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date de l’événement]</td> 
   <td>Saisissez ou mappez la date de cette tâche.<p>Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>Sélectionnez le type d’événement.<ul><li><b>Blog Post</b><p>Saisissez l’identifiant du groupe de contenu. Il s’agit de l’identifiant de la page de blog.</p></li><li><b>E-mail</b><p>Saisissez ou mappez le chemin d’accès au modèle d’email que vous souhaitez utiliser.</li><li><b>Page d’entrée</b><p>Saisissez ou mappez le chemin d’accès au modèle de landing page que vous souhaitez utiliser.</li><li><b>Personnalisé</b></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Indiquez si l’événement se trouve à l’état "À faire" ou "Terminé".</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL GUID Campaign]</td> 
   <td>Saisissez ou mappez l’identifiant HubSpot interne de la campagne dans laquelle cet événement fait partie.</td> 
  </tr> 
 </tbody> 
</table>

#### Suppression d’une tâche de calendrier

Ce module d&#39;action supprime une tâche de calendrier. La connexion utilisée dans ce module doit utiliser les informations d’identification d’un utilisateur disposant d’un compte Marketing payant.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la tâche que vous souhaitez supprimer.</td> 
  </tr> 
 </tbody> 
</table>

#### Événements de tâches de contrôle

Ce module de déclenchement lance un scénario lorsqu’un nouvel événement de tâche se produit dans un calendrier. La connexion utilisée dans ce module doit utiliser les informations d’identification d’un utilisateur disposant d’un compte Marketing payant. Le module renvoie jusqu’à 500 événements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal de fichiers que le module doit renvoyer pour chaque cycle d’exécution de scénario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>Saisissez ou mappez la date la plus ancienne à laquelle vous souhaitez suivre les événements. Utilisez le format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>Saisissez ou mappez la dernière date pour laquelle vous souhaitez regarder les événements. Utilisez le format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Utilisateurs ou utilisatrices**

### Utilisateurs

* [Obtention d’un propriétaire](#get-an-owner)
* [Propriétaires de liste](#list-owners)

#### Obtention d’un propriétaire

Ce module d’action renvoie les détails d’un propriétaire.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de propriétaire]</td> 
   <td> <p>Saisissez ou mappez l’identifiant du propriétaire pour lequel vous souhaitez renvoyer les détails.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Propriétaires de liste

Ce module de recherche renvoie une liste de tous les propriétaires d’un compte HubSpot.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Billets**

### Tickets

<!--* [Create a Ticket]-->
* [Supprimer un ticket](#delete-a-ticket)
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->

<!-- Create a Ticket Need to find a working connection-->

#### [!UICONTROL Supprimer un ticket]

Supprime un ticket existant par son ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez l’ID du ticket que vous souhaitez supprimer. </td> 
  </tr> 
 </tbody> 
</table>

<!-- Get a Ticket  Need to find a working connection-->

<!-- List Tickets  Need to find a working connection-->

&lt;!— Mettre à jour un ticket Besoin de trouver une connexion de travail—>

<!-- Watch Tickets Need to find a working connection-->

+++

+++**Forms**

### Formulaires

* [Obtention d’un fichier téléchargé via le formulaire](#get-a-file-uploaded-via-form)
* [Lister Forms](#list-forms)
  <!--* [Submit Data to a Form]-->
  <!--* [Watch Submissions for a Form]-->

#### Obtention d’un fichier téléchargé via le formulaire

Ce module d’action renvoie un fichier qui a été chargé via un formulaire.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File URL]</td> 
   <td>Saisissez ou mappez l’URL du fichier que vous souhaitez récupérer. Vous pouvez le trouver dans les métadonnées du formulaire.</td> 
  </tr> 
 </tbody> 
</table>

#### List Forms

Ce module d’action renvoie tous les formulaires créés dans le compte associé à la connexion utilisée pour ce module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal de formulaires que le module renverra dans un cycle d’exécution.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Submit Data to a Form Need to find a working connection-->



&lt;!—### Regarder les envois d’un formulaire—Nécessité de trouver une connexion fonctionnelle>—>

+++

+++**Réseaux sociaux (diffusion)**

### Réseaux sociaux (diffusion)

* [Annulation d’un message diffusé](#cancel-a-broadcast-message)
* [Créer un message diffusé](#create-a-broadcast-message)
* [Regarder les messages diffusés](#watch-broadcast-messages)

#### Annulation d’un message diffusé

Ce module d’action annule une diffusion planifiée, telle qu’un tweet ou une publication Facebook.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Broadcast ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la diffusion que vous souhaitez annuler.</td> 
  </tr> 
 </tbody> 
</table>

#### Créer un message diffusé

Ce module d’action crée et publie immédiatement un message sur le canal de médias sociaux spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel ID]</td> 
   <td>Saisissez ou mappez l’identifiant du canal que vous souhaitez utiliser pour cette diffusion.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Saisissez ou mappez un titre pour cette diffusion.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Saisissez ou mappez le texte de la diffusion.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Photo URL]</td> 
   <td>Saisissez ou mappez l’URL d’une photo que vous souhaitez inclure dans la diffusion.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL de miniature]</td> 
   <td>Saisissez ou mappez l’URL d’une miniature que vous souhaitez utiliser pour cette diffusion.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Déclencheur à l’adresse]</td> 
   <td>Saisissez ou mappez la date et l’heure d’envoi de la diffusion. Si ce champ n’est pas renseigné, la diffusion est envoyée immédiatement.<p>Pour obtenir la liste des formats de date et d’heure pris en charge, voir <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Coercition de type dans [!DNL Adobe Workfront Fusion]</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Regarder les messages diffusés

Ce module de déclenchement lance un scénario lorsqu’un message est publié de HubSpot sur le canal de médias sociaux spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’éléments que le module renverra dans un cycle d’exécution.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtrer par état]</td> 
   <td>Pour ne lancer le scénario que lorsque le message est dans un état spécifique, sélectionnez le statut.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtre par canal]</td> 
   <td>Pour lancer le scénario uniquement lorsque le message se trouve sur un canal spécifique, sélectionnez le canal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Broadcast ID]</td> 
   <td>Pour démarrer le scénario uniquement lorsque le message est envoyé à une date spécifique ou après cette date, saisissez ou mappez la date au format <code>MM/DD/YYYY</code>.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Publications de blog**

### Publications de blog

<!--* [Create a Blog Post]-->
* [Supprimer une publication de blog](#delete-a-blog-post)
  <!--* [List Blog Posts]-->
* [Publish/Annuler la publication d’une publication de blog](#publish--unpublish-a-blog-post)
  <!--* [Watch Blog Posts]-->

<!--
#### Create a Blog Post May need connection
-->


#### Suppression d’une publication de blog

Ce module d’action supprime une seule publication de blog.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la publication de blog à supprimer.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### List Blog Posts May need connection

This search module retrieves posts from a HubSpot blog.-->

#### Publish / Annuler la publication d’une publication de blog

Ce module d’action planifie ou annule la publication d’une publication de blog.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Saisissez ou mappez l’identifiant de la publication de blog que vous souhaitez planifier ou annuler.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td>Choisissez si vous souhaitez planifier la publication de blog ou annuler une publication de blog précédemment planifiée.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Watch Blog PostsMay need connection-->

+++

<!--+++**Workflows**>

<!--### Workflows May need connection

#### Add a Contact to a Workflow


#### Remove a Contact from a Workflow

-->

<!--+++-->

+++**Abonnements**

### Abonnements

* [Mettre à jour l’abonnement aux emails](#update-email-subscription)
* [Regarder la chronologie des abonnements pour un portail](#watch-subscriptions-timeline-for-a-portal)

#### Mettre à jour l’abonnement aux emails

Ce module d’action met à jour un abonnement par courrier électronique dans HubSpot.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Saisissez ou mappez l'adresse email de l'abonnement que vous souhaitez mettre à jour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Statuses]</td> 
   <td>Pour chaque état pour lequel vous souhaitez mettre à jour l’abonnement, cliquez sur <b>Ajouter un élément</b> et saisissez l’identifiant du statut, et indiquez si l’adresse électronique sera abonnée à ce statut.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Statut légal de l’abonnement au portail]</td> 
   <td>Pour enregistrer la base légale de cet abonnement pour le RGPD, sélectionnez le statut légal de cet abonnement.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portal Subscription Legal Base Explanation]</td> 
   <td>Pour ajouter une note concernant la base légale de cet abonnement pour le RGPD, saisissez ou mappez le texte de la note.</td> 
  </tr> 
 </tbody> 
</table>

#### Regarder la chronologie des abonnements pour un portail

Ce module de déclenchement lance un scénario lorsqu’un nouvel abonnement à la chronologie des emails est ajouté au portail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Saisissez ou mappez le nombre maximal d’éléments que le module renverra dans un cycle d’exécution.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date et heure de début]</td> 
   <td>Pour renvoyer les résultats à partir d’une date spécifique, saisissez la date au format <code>MM/DD/YYYY.</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Horodatage de fin]</td> 
   <td>Pour renvoyer les résultats à partir d’une date spécifique ou avant, saisissez la date au format <code>MM/DD/YYYY.</code></td> 
  </tr> 
 </tbody> 
</table>

+++

<!--+++**Associations**-->

<!--### Associations-->

<!--#### Associate CRM Objects  May need connection

This action module associates two CRM objects.-->

<!--#### Associate Multiple CRM Objects  May need connection-->



<!--#### Delete an Association May need connection-->



<!--#### Delete Multiple Associations between CRM Objects May need connection-->



<!--#### List Associations for a CRM Object May need connection-->

<!--+++-->

+++**Autre**

### Autre

#### [!UICONTROL Effectuer un appel API]

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
   <td> <p>Pour plus d'informations sur la connexion de votre compte [!DNL HubSpot CRM] à [!DNL Workfront Fusion], voir <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Création d'une connexion à [!DNL Adobe Workfront Fusion] - Instructions de base</a>.</p> </td> 
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

+++

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
