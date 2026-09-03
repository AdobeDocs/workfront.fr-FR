---
title: Gérer les connexions dépendantes
description: En tant que gestionnaire d'espace de travail, vous pouvez définir des connexions dépendantes lors de la création de champs de connexion entre les types d'enregistrements dans Adobe Workfront Planning. Lors de l’ajout de champs connectés, vous pouvez activer un paramètre qui indique que les valeurs du type d’enregistrement connecté dépendent des valeurs du type d’enregistrement source (celui où vous ajoutez la connexion), chaque fois que les deux champs apparaissent ensemble sur un troisième type d’enregistrement.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 4%

---


# Gestion des connexions dépendantes

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Une fois la version à prévisualiser, les mêmes fonctionnalités sont également disponibles tous les mois dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

En tant que gestionnaire d&#39;espace de travail, vous pouvez définir des connexions dépendantes lors de la création de champs de connexion entre les types d&#39;enregistrements dans Adobe Workfront Planning.

Lors de l’ajout de champs connectés, vous pouvez activer un paramètre qui indique que les valeurs du type d’enregistrement connecté dépendent des valeurs du type d’enregistrement source (celui où vous ajoutez la connexion), chaque fois que les deux champs apparaissent ensemble sur un troisième type d’enregistrement.

Par exemple, vous pouvez vous assurer qu’un champ Région affiche uniquement les valeurs liées à la zone géographique sélectionnée. Cette configuration s’effectue directement dans la configuration du champ de connexion : lors de l’ajout d’une connexion d’un type d’enregistrement Géographique à un type d’enregistrement dépendant (comme Région), un nouveau paramètre permet aux gestionnaires de l’espace de travail de la marquer comme dépendante du type d’enregistrement Géographique, en utilisant les relations déjà établies entre ces types d’enregistrement.

Une fois configuré, tout type d’enregistrement qui fait référence aux deux champs (une campagne, par exemple) voit immédiatement l’effet : la sélection d’une valeur Géo limite le sélecteur de Région aux régions réellement liées à cette zone géographique. Cela permet d’appliquer automatiquement la structure des enregistrements, d’éliminer les combinaisons incohérentes et de réduire le nettoyage manuel.

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Pour connecter des types d’enregistrements à partir du même espace de travail : </p>
<ul> 
<li><p>Tout package Workfront ou Workflow avec tout package Planning</p></li>
<p>Ou</p>
<li><p>Tout package Planning lorsqu’il est acheté en tant que produit autonome</p></li>
</ul>

<p>Pour connecter des types d’enregistrements à partir de différents espaces de travail :</p>

<ul>

<li><p>Tout workflow et un package Planning Prime ou Ultimate</p></li>
<p>Ou</p>
<li><p>Tout package Planning Prime ou Ultimate lorsqu’il est acheté en tant que produit autonome</p></li>
</ul>
   </td> 
<tr> 
<td> 
   <p> Produits supplémentaires</p> </td> 
   <td> 
   <p> En plus d’Adobe Workfront, vous devez disposer des éléments suivants si vous souhaitez connecter des types d’enregistrements à des objets des applications suivantes :</p>
   <ul><li><p>Une licence Adobe Experience Manager Assets et une intégration entre AEM Assets et Workfront pour connecter les ressources AEM aux types d’enregistrements Planning.</p>
   <p>Pour plus d’informations, voir <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront pour Experience Manager Assets et Assets Essentials : index d’article</a>. </p></li>
   <li><p> Une licence Adobe GenStudio for Performance Marketing permettant de connecter des types d’enregistrements aux objets GenStudio et aux marques</p>
   <p>Pour plus d’informations, voir <a href="https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/get-started">Prise en main d’Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Norme de workflow</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Planning</p></td> 
   <td><p>Norme de planification</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Vous devez ajouter un workflow et un type de licence Planning au niveau d'accès lorsque vous disposez à la fois d'un workflow et d'un package Planning</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations d’un espace de travail</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Sent a slack message to Norayr, Predator, Snowstorm, Armine for info for this section: 
-->

## Considérations relatives aux champs connectés dépendants


* Les champs connectés dépendants ne peuvent être configurés qu’entre des types d’enregistrements ayant une relation de champ de connexion établie. Vous ne pouvez pas définir de logique de dépendance entre des types d’enregistrements non liés.

* Vous pouvez avoir un champ connecté dépendant entre les types d’enregistrements dans des espaces de travail distincts.

* Vous ne pouvez pas avoir de champ connecté dépendant entre les types d&#39;enregistrements Planning et les types d&#39;objets Workfront ou AEM.

* Le paramètre de dépendance est configuré une connexion à la fois, dans la configuration du champ de connexion elle-même, plutôt que comme une règle globale.

* Le comportement de filtrage entre les deux enregistrements connectés ne s’active que lorsque les champs source et dépendants sont tous deux présents sur un troisième type d’enregistrement. La dépendance n’a aucun effet si un seul des deux champs s’affiche sur un type d’enregistrement.

* Le sélecteur du champ dépendant est limité aux valeurs déjà liées à la valeur source sélectionnée au niveau de l’enregistrement ; il ne peut pas afficher ni suggérer de valeurs non liées.

* Si la valeur du champ source change, le champ dépendant est automatiquement effacé plutôt que laissé dans un état non valide, ce qui empêche la persistance de combinaisons incohérentes.

  Vous recevez un message intégré ou toast expliquant pourquoi le champ dépendant a été effacé.

* Chaque champ dépendant peut avoir jusqu’à 3 champs de contrôle direct.

* Les niveaux de dépendance sont limités à 6 connexions. Cela signifie que jusqu’à 7 types d’enregistrements peuvent être connectés.

* Pour que la chaîne de dépendance fonctionne, tous les champs dépendants doivent exister simultanément sur le même type d’enregistrement.

## Créer une connexion dépendante

1. En tant que gestionnaire d’espace de travail, accédez à un type d’enregistrement dans Workfront Planning et ouvrez-le en mode Tableau.
1. Cliquez sur l’icône **+** dans le coin supérieur droit de la vue Tableau pour ajouter un nouveau champ.
1. Cliquez sur **Nouvelle connexion**, puis commencez à ajouter une nouvelle connexion pour un deuxième type d’enregistrement.

   >[!TIP]
   >
   >Vous ne pouvez créer une connexion dépendante qu&#39;entre deux types d&#39;enregistrements Planning. Vous ne pouvez pas créer de connexions dépendantes entre les types d’enregistrements et les objets à partir de Workfront ou AEM.
1. Dans la section **Paramètres de connexion**, activez l’option **Rendre cette connexion dépendante**.

   >[!TIP]
   >
   >Activer le paramètre **Rendre cette connexion dépendante** active automatiquement le **Créer un champ correspondant sur le type d’enregistrement lié**. La limite est de 500 champs par type d’enregistrement.

   ![Nouvel onglet de connexion avec la connexion dépendante activée](assets/dependent-connection-enabled-setting.png)

1. Continuez à configurer la connexion, comme décrit dans l’article [Connecter des types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).
1. Cliquer sur **Enregistrer**.

   Les événements suivants se produisent :

   * La connexion entre les deux types d’enregistrement est créée et leurs valeurs dépendent l’une de l’autre lorsqu’elles s’affichent ensemble sur le même type d’enregistrement.
   * Un champ correspondant affichant le premier type d’enregistrement est créé pour le second type d’enregistrement.
   * Lorsque les deux types d’enregistrement sont connectés à un troisième type d’enregistrement, les valeurs affichées sous forme de choix pour le deuxième champ d’enregistrement connecté sont celles qui sont connectées au premier enregistrement. Les valeurs affichées comme choix pour le premier type d’enregistrement sont celles connectées au second type d’enregistrement.

     Pour plus d’informations, consultez la section [Exemple de types d’enregistrements connectés dépendants](#example-of-dependent-connected-record-types) dans cet article.
   * L’en-tête de colonne des champs d’enregistrement connectés indique que le champ est dans une relation de connexion dépendante.

     ![Info-bulle de l’icône Dépendante dans l’en-tête de colonne](assets/dependent-icon-tooltip-in-column-header.png)
1. (Facultatif) Cliquez sur **Règles de filtrage des enregistrements** et sélectionnez des champs à partir du type d’enregistrement auquel vous vous connectez pour limiter les options pour les valeurs de ce champ, puis cliquez sur **Terminé**.

   Lorsque les deux champs sont présents sur un troisième type d’enregistrement, les options pour le type d’enregistrement de champ connecté sont limitées par le filtre que vous sélectionnez ici.
1. (Facultatif et recommandé) Accédez à un troisième type d’enregistrement et ajoutez les premier et deuxième types d’enregistrement en tant que champs d’enregistrement connectés.

   ![Indicateur de champ connecté dépendant sur un troisième type d’enregistrement](assets/dependent-connected-field-indicator-on-a-third-record-type.png)

## Exemple de types d’enregistrements dépendants connectés

Cette section fournit un exemple simple de la manière dont vous pouvez configurer des types d’enregistrements dépendants et dont ils fonctionnent pour un troisième type d’enregistrement.

1. Dans un espace de travail que vous pouvez gérer, créez les types d’enregistrements suivants :

   * Campaign
   * Pays
   * Continents

1. Dans le type d&#39;enregistrement **Pays**, ajoutez les enregistrements suivants :

   * France
   * États-Unis
   * Japon
1. Dans le type d&#39;enregistrement **Continents**, ajoutez les enregistrements suivants :

   * Europe
   * Amérique
   * Asie

1. Dans le type d’enregistrement **Pays**, créez un champ dépendant connecté pour **Continents**.

   Cela ajoute les champs d’enregistrement connectés suivants :

   * Le champ d’enregistrement connecté **Pays** pour le type d’enregistrement **Continents**.
   * Le champ d’enregistrement connecté **Continents** pour le type d’enregistrement **Pays**.

1. Utilisez l’une des méthodes suivantes :

   * Dans la vue de tableau **Pays** type d&#39;enregistrement, ajoutez les valeurs suivantes pour le champ d&#39;enregistrement connecté Continents :

     * L’Europe pour la France
     * L’Amérique pour les États-Unis
     * Asie pour le Japon
   * Dans la vue du tableau **Continents** type d&#39;enregistrement , ajoutez les valeurs suivantes pour le champ d&#39;enregistrement connecté **Pays** :

     * La France pour l&#39;Europe
     * États-Unis pour l’Amérique
     * Le Japon pour l&#39;Asie
1. Ajoutez les champs connectés **Pays** et **Continents** à la vue de table de type enregistrement **Campaign**.
1. Sélectionnez **Japon** pour le champ **Pays** sur le type d’enregistrement **Campagne**. Notez que la seule valeur disponible pour le champ connecté **Continents** sur la campagne est **Asie**.

   Ou

   Sélectionnez **Europe** pour le champ **Continents** dans le type d’enregistrement Campagne .

   Notez que la seule valeur disponible pour le champ connecté **Pays** sur la campagne est **France**.



