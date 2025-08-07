---
title: Prise en main de l’intégration de Workfront Planning and GenStudio for Performance Marketing
description: L’espace de travail GenStudio for Performance Marketing est disponible dans Adobe Workfront Planning lorsque votre société a acheté les deux produits. Découvrez quelques principes de base sur la manière de rationaliser vos workflows à l’aide de cette intégration.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: b366841f3994468624a0c9b07d9de6f2f274cbe0
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 9%

---

# Prise en main de l’intégration de Workfront Planning and GenStudio for Performance Marketing

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
   <li><p> Planification d’Adobe Workfront<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
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
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Autorisations de niveau Contribution ou supérieur à un espace de travail et à un type d’enregistrement  </p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p> </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Exigences d’intégration

* Workfront et GenStudio for Performance Marketing doivent être activés pour la même organisation.
* GenStudio n’est pas disponible dans Workfront Planning lorsque votre société dispose de plusieurs instances Workfront. <!--this will change-->

* L’instance Workfront fait partie de l’expérience unifiée Adobe, y compris l’utilisation du système Identity Management (IMS).

  Pour plus d’informations, voir [Expérience unifiée Adobe pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Les utilisateurs qui utilisent à la fois Planning et GenStudio ne peuvent appartenir qu’à une seule instance Workfront au sein de l’organisation IMS.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->


## Considérations relatives à la gestion d’un espace de travail GenStudio dans Workfront Planning

* Votre entreprise doit acheter Adobe GenStudio for Performance Marketing avant de pouvoir afficher un espace de travail GenStudio dans Workfront Planning.

  Pour plus d’informations sur GenStudio, consultez le [Guide de l’utilisateur d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).

  Pour plus d’informations sur l’intégration de GenStudio à Workfront Planning, consultez la section [Prise en main de l’intégration de Workfront Planning et GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)

* Les utilisateurs de Workfront doivent avoir accès à GenStudio pour pouvoir voir l’espace de travail GenStudio dans Workfront Planning.


* Les sections suivantes décrivent certaines limites de ce que vous pouvez et ne pouvez pas gérer dans un espace de travail GenStudio à partir de Workfront Planning.

### Espace de travail GenStudio dans Workfront Planning

* Si votre organisation dispose de plusieurs instances Workfront, une seule instance de Workfront peut afficher votre espace de travail GenStudio.
* L’espace de travail GenStudio affiche un indicateur visuel qui indique clairement qu’il est importé depuis GenStudio.

### Types d’enregistrements

* Vous ne pouvez pas modifier les types d’enregistrements à partir de GenStudio dans Workfront Planning.
* Vous ne pouvez pas partager des types d’enregistrements de GenStudio avec d’autres utilisateurs. Les administrateurs et administratrices de Workfront peuvent afficher l’espace de travail GenStudio dans leur zone Planning .
* Les types d’enregistrements synchronisés avec GenStudio affichent un indicateur visuel qui indique clairement que les types d’enregistrements sont importés à partir de GenStudio.
* Les utilisateurs qui consultent l’espace de travail GenStudio dans Planning peuvent partager ses types d’enregistrements avec d’autres utilisateurs.

### Enregistrements

* Vous pouvez ajouter ou supprimer des enregistrements dans GenStudio. Ils seront visibles dans Workfront Planning (ou en seront supprimés).
Vous pouvez ajouter ou supprimer des enregistrements dans Workfront Planning. Ils seront visibles dans GenStudio (ou en seront supprimés).
* Vous pouvez ajouter des enregistrements à partir de Workfront Planning des manières suivantes :

   * Manuellement, à partir de zéro
   * En les important au moyen d’un fichier CSV ou Excel

  Pour plus d’informations, voir [Créer des enregistrements](/help/quicksilver/planning/records/create-records.md).
* Vous ne pouvez pas créer ni supprimer des enregistrements d&#39;activation de Workfront Planning.
* Vous pouvez modifier les informations d’enregistrement de tous les enregistrements de l’espace de travail GenStudio dans n’importe quel champ visible de Workfront Planning.

  Pour plus d’informations, voir [Modifier des enregistrements](/help/quicksilver/planning/records/edit-records.md).

### Champs

* Tous les champs d’enregistrement sont importés à partir de GenStudio et les paramètres du champ ne peuvent pas être modifiés.
* Vous ne pouvez créer des champs pour les types d’enregistrements GenStudio dans Workfront Planning que si vous disposez d’un accès d’administrateur système dans GenStudio.
* Vous pouvez créer des champs pour les types d&#39;enregistrements GenStudio dans Planning. Ces champs seront visibles à partir des zones suivantes :
   * Vues Planning
   * Pages de détails des enregistrements de planification
   * Pages de détails des enregistrements GenStudio

  >[!TIP]
  >
  >Les champs créés dans Workfront Planning ne sont pas visibles dans la vue Liste de GenStudio.

* Vous pouvez masquer des champs dans la vue Tableau d&#39;un type d&#39;enregistrement GenStudio dans Planning, mais vous ne pouvez pas supprimer des champs de Workfront Planning.


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### Vues

* Vous pouvez créer des vues pour les types d’enregistrements GenStudio. Vous ne pouvez pas modifier les vues automatiquement importées depuis GenStudio, mais vous pouvez modifier les éléments de vue pour la vue Tableau GenStudio. Par exemple, vous pouvez modifier les filtres, le tri, les regroupements, les couleurs des lignes et la hauteur des lignes en mode Tableau.

  Pour plus d’informations, consultez la section [Gérer les vues d’enregistrement](/help/quicksilver/planning/views/manage-record-views.md).

* Vous pouvez partager la vue d’un type d’enregistrement GenStudio des manières suivantes :

   * Copier le lien d’affichage
   * Exporter la vue vers un fichier (disponible uniquement pour la vue Tableau)

### Connexions

* Dans Planning, vous ne pouvez pas connecter d&#39;autres types d&#39;enregistrements ou d&#39;objets à partir de types d&#39;enregistrements GenStudio.
* Vous pouvez vous connecter à des types d&#39;enregistrements GenStudio à partir d&#39;autres types d&#39;enregistrements dans Planning.
