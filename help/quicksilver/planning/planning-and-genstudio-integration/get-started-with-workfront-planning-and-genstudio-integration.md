---
title: Prise en main de l’intégration de Workfront Planning and GenStudio for Performance Marketing
description: L’espace de travail GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits. Découvrez quelques principes de base sur la manière de rationaliser vos workflows à l’aide de cette intégration.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 5%

---

# Prise en main de l’intégration d’Adobe Workfront Planning et d’Adobe GenStudio for Performance Marketing

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->

Les organisations qui utilisent à la fois Adobe Workfront Planning et Adobe GenStudio for Performance Marketing définissent souvent des concepts marketing tels que des campagnes, des produits et des rôles de manière plus détaillée que ce que GenStudio prend en charge par défaut.

Il existe une intégration native entre GenStudio for Performance Marketing et Workfront Planning. Cette intégration permet aux utilisateurs de Workfront Planning de gérer les campagnes, produits, rôles, activations, canaux et régions utilisés dans GenStudio. Il leur permet également de configurer GenStudio pour référencer les types d’enregistrements existants à partir de Workfront Planning, ce qui crée un workflow marketing plus connecté et plus cohérent.

Cette intégration vous permet d’éviter la saisie de données en double, de maintenir l’alignement des efforts de planification et d’activation et de prendre en charge votre système d’enregistrement marketing.

L’espace de travail GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits.

Grâce à l’intégration entre Workfront Planning et GenStudio for Performance Marketing, vous pouvez :

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Affichez l’espace de travail GenStudio dans Workfront Planning.
* Modifiez vos campagnes dans GenStudio et disposez des mises à jour en temps réel des mêmes informations dans Workfront Planning.
* Modifiez vos campagnes dans Workfront Planning et disposez des mises à jour en temps réel des mêmes informations dans GenStudio.

## Exigences d’intégration

* Workfront et GenStudio for Performance Marketing doivent être activés pour la même organisation.

  Pour plus d’informations sur GenStudio, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).

* GenStudio n’est pas disponible dans Workfront Planning lorsque votre société dispose de plusieurs instances Workfront. <!--this will change-->

* L’instance Workfront fait partie de l’expérience unifiée Adobe, y compris l’utilisation du système Identity Management (IMS).

  Pour plus d’informations, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Les utilisateurs qui utilisent à la fois Planning et GenStudio ne peuvent appartenir qu’à une seule instance Workfront au sein de l’organisation IMS.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Conditions d’accès

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe GenStudio for Performance Marketing</p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tout package de workflow Workfront</p>  
<p>Tout package Workfront Planning</p>
   </td> </tr>

<tr> 
   <td role="rowheader"><p>Package Adobe GenStudio</p></td> 
   <td> 
<p>???</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p> 
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p> Administrateur ou administratrice système</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe GenStudio</p></td> 
   <td><p> ???</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>  
   <p>Configuration pour GenStudio : ???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  
   <p>Dans Workfront Planning : </p>
   <ul>
   <li><p>Autorisations de niveau Contribution ou supérieur à un espace de travail et à un type d’enregistrement  </p> </li> 
   <li><p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p></li>
   </ul>
   <p>Dans Adobe GenStudio for Performance Marketing : <p>
   <ul>
   <li><p> Toutes les autorisations dans Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Création d’autorisations dans Adobe GenStudio for Performance Marketing pour créer des éléments</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Pour plus d’informations sur Adobe GenStudio for Performance Marketing, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).


## Présentation de l’intégration de Workfront Planning et GenStudio

Les sections suivantes décrivent ce qui suit :

* Fonctionnalités de mise à jour des informations de planification Workfront depuis GenStudio
* Fonctionnalités de mise à jour des informations GenStudio à partir de Workfront Planning
* Limites de ce que vous pouvez et ne pouvez pas gérer dans un espace de travail GenStudio à partir de Workfront Planning.

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Espace de travail GenStudio dans Workfront Planning

* Si votre organisation dispose de plusieurs instances Workfront, l’espace de travail GenStudio n’est visible depuis aucune de vos instances Workfront. <!-- this might change-->
* L’espace de travail GenStudio affiche un indicateur visuel qui indique clairement qu’il est importé depuis GenStudio. Pour plus d’informations, voir [Gérer l’espace de travail GenStudio dans Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Tous les utilisateurs ayant accès à GenStudio et à Workfront Planning peuvent également voir l’espace de travail GenStudio dans Workfront Planning.
* Les utilisateurs de Workfront Planning doivent être gérés par le biais du système Adobe Identity Management System (IMS) pour pouvoir afficher et utiliser l’espace de travail GenStudio depuis Workfront.

  Les utilisateurs Workfront uniquement ne peuvent pas voir l’espace de travail GenStudio, même s’il est disponible dans Workfront.

  Pour plus d’informations, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


### Types d’enregistrements

* Vous pouvez modifier les informations sur les types d’enregistrements (par exemple, leur apparence) à partir de GenStudio dans Workfront Planning.
* Vous pouvez partager des types d&#39;enregistrements GenStudio avec d&#39;autres utilisateurs dans Planning.
* Vous pouvez créer des types d’enregistrements à partir de Planning dans l’espace de travail GenStudio. Ces types d&#39;enregistrements restent uniquement dans Planning. Elles ne s’affichent pas dans GenStudio.
* Les types d’enregistrements synchronisés avec GenStudio affichent un indicateur visuel dans Workfront Planning qui indique clairement que les types d’enregistrements sont importés à partir de GenStudio.

### Enregistrements

* Vous pouvez ajouter ou supprimer des enregistrements dans GenStudio. Ils seront visibles dans Workfront Planning (ou en seront supprimés).
* Vous pouvez ajouter ou supprimer des enregistrements dans Workfront Planning. Ils seront visibles dans GenStudio (ou en seront supprimés).
* Lorsque vous supprimez des enregistrements de Workfront Planning ou de GenStudio, ils sont placés pendant 30 jours dans la classe Récemment supprimés . GenStudio ne comporte pas de classe Récemment supprimé.
* La restauration d’un enregistrement à partir de la classe Récemment supprimé les replace dans Workfront Planning and GenStudio.
* Vous pouvez ajouter des enregistrements à partir de Workfront Planning des manières suivantes :

   * Manuellement, à partir de zéro, depuis n’importe quel affichage à l’aide du bouton Nouvel enregistrement .
   * En les important au moyen d’un fichier CSV ou Excel
   * Manuellement, en ligne, en mode Tableau
   * Manuellement, directement en mode Chronologie

  Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* Vous ne pouvez pas créer ni supprimer des enregistrements d&#39;activation de Workfront Planning.
* Vous pouvez modifier les informations d’enregistrement de tous les enregistrements de l’espace de travail GenStudio dans Planning, dans n’importe quel champ visible de Workfront Planning.

  Pour plus d’informations, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Champs

* Les champs d’enregistrement sont importés depuis GenStudio. Vous pouvez modifier les paramètres de champ dans Workfront Planning.
* Vous pouvez créer des champs pour les types d’enregistrements GenStudio dans Workfront Planning si vous disposez d’un accès de niveau Gérer dans Gen Studio.
* Lorsque vous créez des champs pour des types d&#39;enregistrements GenStudio dans Planning, ils sont visibles à partir des zones suivantes :
   * Vues Planning
   * Pages de détails des enregistrements de planification
   * Pages de détails des enregistrements GenStudio

  >[!TIP]
  >
  >Les champs créés dans Workfront Planning ne sont pas visibles dans la vue Liste de GenStudio.

* Vous pouvez masquer des champs dans la vue Tableau d&#39;un type d&#39;enregistrement GenStudio dans Planning.
* Vous ne pouvez pas supprimer des champs importés de GenStudio à partir de Workfront Planning.
* Vous pouvez supprimer des champs créés dans Workfront Planning pour les types d’enregistrements GenStudio à partir de Workfront Planning.


### Les champs Créé par et Approuvé par

* Vous pouvez ajouter les champs Créé par et Approuvé par pour les types d’enregistrements GenStudio dans Workfront Planning à partir de Workfront Planning.
* Les enregistrements qui s&#39;affichent dans les types d&#39;enregistrements Canal et Région afficheront « Système » comme le Créé par l&#39;utilisateur. Ces enregistrements sont créés automatiquement lors de la création de l’espace de travail GenStudio dans Workfront Planning.
* Les enregistrements créés dans GenStudio après la mise à disposition de l&#39;espace de travail dans Workfront Planning affichent le nom de l&#39;utilisateur IMS qui a créé l&#39;enregistrement dans le champ Créé par , même si l&#39;utilisateur a créé les enregistrements dans GenStudio et n&#39;est pas un utilisateur Workfront.
* Le champ Approuvé par affiche le nom de l&#39;approbateur lorsqu&#39;un formulaire de demande est envoyé pour créer un enregistrement.

### Vues

* Vous pouvez créer des vues pour les types d’enregistrements GenStudio.

  Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

* Vous pouvez partager la vue d&#39;un type d&#39;enregistrement GenStudio comme vous le feriez pour un type d&#39;enregistrement Planning.
* Vous ne pouvez pas créer plusieurs vues dans GenStudio.

### Connexions

* Dans Workfront Planning, vous pouvez établir les connexions suivantes entre les types d&#39;enregistrements GenStudio et d&#39;autres types d&#39;enregistrements ou d&#39;objets :

   * Deux types d’enregistrements GenStudio
   * Un type d’enregistrement GenStudio et un type d’enregistrement Planning du même espace de travail
   * Un type d’enregistrement GenStudio et un type d’enregistrement Planning d’un autre espace de travail, si les types d’enregistrement sont configurés pour se connecter à partir d’un autre espace de travail.
   * Un type d’enregistrement GenStudio et un type d’objet Workfront (projets, portfolios, programmes, sociétés, groupes)
   * Un type d’enregistrement GenStudio et un type d’objet AEM Assets.

### Formulaires de demande et automatisations

* Vous pouvez ajouter des formulaires de demande et des automatisations à un type d’enregistrement GenStudio dans Workfront Planning.

### Environnement de prévisualisation

* L’espace de travail GenStudio accessible à partir de votre environnement de production s’affiche également dans votre environnement de prévisualisation.
* Vous pouvez effectuer toutes les activités décrites dans cet article sur l’espace de travail GenStudio dans la planification Workfront dans votre environnement de prévisualisation, mais ces modifications ne seront pas transférées vers GenStudio.
Seules les modifications apportées aux éléments de l’environnement de production synchronisent Workfront Planning et GenStudio.
GenStudio ne dispose pas d’un environnement de prévisualisation.

