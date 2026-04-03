---
title: Vue d’ensemble des publications du premier trimestre 2026
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du premier trimestre 2026. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed348f44-eae1-4478-8425-6114f2b310ad
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '2885'
ht-degree: 100%

---

# Vue d’ensemble des publications du premier trimestre 2026

Cette page fournit des informations sur les fonctionnalités incluses dans la version du premier trimestre 2026, prévue pour janvier 2026.

Les améliorations apportées à cette page sont disponibles dans l’environnement de Prévisualisation. Cette page sera mise à jour avec des améliorations supplémentaires à mesure que la version du premier trimestre 2026 approche de sa date de sortie en production.


<!--
 Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>.
-->

>[!IMPORTANT]
>
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>25.11 (13 novembre 2025)</li><li>25.12 (11 décembre 2025)</li><li>26.1 (14 janvier 2026)</li></ul> | <ul><li>26.1 (15 janvier 2026)</li></ul> |
>
>Notez que pour la version finale de chaque trimestre (26.1 ce trimestre), les personnes disposant du planning de publication rapide recevront la version un jour plus tôt (14 janvier 2026).
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations des documents et des approbations](#documents-and-approvals-enhancements)
* [Amélioration de l’accueil](#home-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations des projets](#project-enhancements)
* [Amélioration des rapports](#reporting-enhancements)
* [Améliorations des demandes](#requests-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations apportées aux administrateurs et administratrices

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Fonctionnalité</strong>
        </td>
        <td><strong>Aperçu</strong></td>
        <td><strong>Version rapide</strong></td>
        <td><strong>Tous les trimestres</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Gérer les priorités dans le modèle de mise en page</a>
            <p><span class="preview">Temporairement indisponible dans l’environnement de prévisualisation</span></p>
            <p>Vous pouvez désormais activer ou désactiver les priorités pour des utilisateurs et utilisatrices spécifiques dans le modèle de mise en page. Si les priorités étaient auparavant désactivées pour votre organisation, elles le resteront dans le modèle de mise en page avec cette modification.</p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2025</td>
        <td>15 janvier 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Rechercher les conflits de formulaires multiples pour les champs personnalisés calculés</a>
            <p>Pour déterminer les objets susceptibles d’être affectés lors de la modification d’une expression dans des champs personnalisés, nous avons ajouté une option permettant de vérifier les conflits. Cette boîte de dialogue affiche tous les objets qui pourraient être affectés par la modification de la formule, regroupés par type d’objet. Vous pouvez accéder aux détails de chaque objet et consulter les champs pour décider si le champ doit être supprimé de l’un des formulaires ou si l’expression doit rester inchangée.</p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2025</td>
        <td>15 janvier 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Date de saisie et ID Saisi par stockés dans des objets personnalisés</a><p>[!BADGE Hors planning]{type=Neutral}</p>
            <p>La date de saisie et l’ID Saisi par sont désormais stockés dans des formulaires, champs et sections personnalisés. Vous pouvez utiliser ces options de données dans les rapports sous la forme de filtres, de vues ou de regroupements. Pour les afficher dans la liste des formulaires, champs ou sections personnalisés de la configuration, ajoutez Date de saisie et Saisi par : nom sous forme de colonnes dans une vue nouvelle ou existante.</p>
        </td>
        <td>13 novembre 2025</td>
        <td>13 novembre 2025</td>
        <td>13 novembre 2025</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Met à jour les noms de bouton lors de la modification d’un modèle de mise en page</a>
            <p>Pour plus de cohérence avec d’autres zones de la configuration, telles que le concepteur de formulaire personnalisé, les boutons affichés lors de la modification d’un modèle de mise en page ont été modifiés en Appliquer, Enregistrer et fermer et Annuler. La nouvelle option Appliquer permet d’enregistrer les modifications apportées au modèle de mise en page et de continuer la modification. Auparavant, les options disponibles étaient Enregistrer et Annuler. </p>
        </td>
        <td>30 octobre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 janvier 2026</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Amélioration de la gestion des champs avec l’indicateur Actif sur les champs personnalisés</a>
            <p>Lorsque le système comporte un grand nombre de champs personnalisés, la gestion de ces champs dans les formulaires et les rapports personnalisés peut s’avérer difficile. Vous pouvez désormais marquer les champs personnalisés comme inactifs avec le nouvel indicateur <b>Actif</b>. Cet indicateur est disponible lors de l’utilisation d’un champ dans un formulaire personnalisé ou lors de l’ajout ou de la modification d’un champ de la liste Champs. </p>
        </td>
        <td>30 octobre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 janvier 2026</td>
    </tr>   
  </tbody>
</table>

### Améliorations des documents et des approbations

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Fonctionnalité</strong>
        </td>
        <td><strong>Aperçu</strong></td>
        <td><strong>Version rapide</strong></td>
        <td><strong>Tous les trimestres</strong></td>
        </tr>
       <!--
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Set up brands for the AI reviewer in Workfront<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>You can now set up brands for the AI reviewer in the Workfront Setup area. This allows you to customize the AI review process based on your organization's branding guidelines.</p>
            <p>The AI reviewer is currently in beta.</p>
        </td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
    </tr>
    -->
    </tr>
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Choisir un projet Workfront lors de l’envoi d’une révision dans Adobe Express<p>[!BADGE Hors planning]{type=Neutral}</p> </a>
            <p>Vous pouvez choisir un projet Workfront pour y envoyer une épreuve. Cela permet de conserver toutes les ressources et épreuves associées au sein d’un même projet.</p>
        </td>
        <td>15 décembre 2025</td>
        <td>15 décembre 2025</td>
        <td>15 décembre 2025</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Prise en charge inter-organisations d’Adobe Express avec Workfront Proof<p>[!BADGE Hors planning]{type=Neutral}</p> </a>
            <p>Nous introduisons la prise en charge inter-organisations d’Adobe Express avec Workfront Proof. Cette amélioration permet aux clients et clientes qui travaillent dans plusieurs organisations IMS d’utiliser et de gérer facilement les workflows d’épreuves.</p>
        </td>
        <td>13 novembre 2025</td>
        <td>13 novembre 2025</td>
        <td>13 novembre 2025</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager désormais disponible avec l’intégration Frame.io <p>[!BADGE Hors planning]{type=Neutral}</p> </a>
            <p>Vous pouvez désormais utiliser Experience Manager Assets pour gérer et stocker vos ressources numériques qui ont passé le cycle de révision et d’approbation. Cette intégration permet d’exploiter les fonctionnalités d’Adobe Experience Manager, Frame.io et Workfront afin de rationaliser vos processus de gestion de contenu et de collaboration. </p>
        </td>
        <td>30 octobre 2025</td>
        <td>30 octobre 2025</td>
        <td>30 octobre 2025</td>
    </tr>   
  </tbody>
</table>



### Amélioration de l’accueil

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Fonctionnalité</strong>
        </td>
        <td><strong>Aperçu</strong></td>
        <td><strong>Version rapide</strong></td>
        <td><strong>Tous les trimestres</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-home.md" class="MCXref xref" xrefformat="{para}">Mise à jour du widget Mentions sur la page d’accueil</a>
            <p>Nous avons apporté les améliorations suivantes au widget Mentions sur la page d’accueil : <ul><li>La même expérience dans la zone Mises à jour de la plupart des objets Workfront est désormais également disponible dans le widget Mentions de la page d’accueil. </li><li>Le widget Mentions contient maintenant les commentaires que l’utilisateur ou l’utilisatrice a faits ou dans lesquels il a été identifié au cours des deux dernières semaines.</li><ul></p>
        </td>
        <td>17 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>   
  </tbody>
</table>

### Améliorations de l’intégration

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Fonctionnalité</strong>
        </td>
        <td><strong>Aperçu</strong></td>
        <td><strong>Version rapide</strong></td>
        <td><strong>Tous les trimestres</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Sélection d’un projet Workfront lors de l’envoi d’une révision dans Creative Cloud Express</a><p>[!BADGE Hors planning]{type=Neutral}</p>
            <p>Vous pouvez choisir un projet Workfront pour y envoyer une épreuve. Cela permet de conserver toutes les ressources et épreuves associées au sein d’un même projet. </p>
        </td>
        <td>15 décembre 2025</td>
        <td>15 décembre 2025</td>
        <td>15 décembre 2025</td>
    </tr>   
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Mise à jour du sélecteur de ressources pour l’intégration native Adobe Workfront pour Experience Manager Assets</a>
            <p>Nous avons mis à niveau le sélecteur de ressources dans l’intégration Adobe Workfront pour Experience Manager Assets. Grâce à cette mise à niveau, vous pouvez désormais sélectionner et extraire des collections AEM directement dans Workfront. </p>
        </td>
        <td>20 novembre 2025</td>
        <td>11 décembre 2025</td>
        <td>15 janvier 2026</td>
    </tr>   
    <!--
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">New version of Salesforce integration now available </a>
            <p>To stay up-to-date with recent changes to the Workfront API, we've created a new Salesforce integration. The new integration features the same functionality as the previous version, and was updated to avoid losing functionality deprecated in the API.</p><p>NOTE: The Workfront for Salesforce integration, including the new version, will not be available after **February 28, 2026**. </p>
        </td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
    </tr>
    -->
  </tbody>
</table>

### Améliorations des projets

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Fonctionnalité</strong>
        </td>
        <td><strong>Aperçu</strong></td>
        <td><strong>Version rapide</strong></td>
        <td><strong>Tous les trimestres</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">Les utilisateurs et utilisatrices de la licence Light peuvent enregistrer le temps passé sur les projets</a>
            <p>Les utilisateurs et utilisatrices de la licence Light peuvent désormais consigner le temps directement dans les projets. Auparavant, seuls les utilisateurs et utilisatrices de la licence standard pouvaient enregistrer des heures sur les projets.</p>
        </td>
        <td>11 décembre 2025</td>
        <td>15 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>   
  </tbody>
</table>

### Amélioration des rapports

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Fonctionnalité</strong>
        </td>
        <td><strong>Aperçu</strong></td>
        <td><strong>Version rapide</strong></td>
        <td><strong>Tous les trimestres</strong></td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Mises à jour des devises dans les tableaux de bord de la zone de travail</a>
            <p>Nous avons effectué les mises à jour suivantes pour les champs de devise :<ul><li>Lorsque plusieurs devises sont définies dans Workfront, vous pouvez désormais choisir une devise par défaut pour le tableau de bord lors de la création. </li><li>Lors de la création d’un rapport, vous pouvez verrouiller un champ de devise. Cela permet de s’assurer que la préférence de devise au niveau du tableau de bord n’affecte pas l’affichage de ces valeurs.</li><li>Lors de l’affichage d’un tableau de bord, les utilisateurs et utilisatrices peuvent basculer entre les devises définies dans Workfront. Ces modifications s’appliquent à l’ensemble du tableau de bord, à l’exception des champs de devise verrouillés.</li></ul></p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}"> Résultats du tableau de recherche rapide dans les tableaux de bord de la zone de travail</a>
            <p>Nous avons ajouté une recherche rapide dans les rapports Tableau. Cette recherche fonctionne sur toutes les pages. Vous pouvez donc trouver des données même si elles ne sont pas actuellement visibles.</p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nouvelle option Afficher le total pour les graphiques en secteurs</a>
            <p>Nous avons introduit une nouvelle option Afficher le total qui convertit les graphiques en secteurs en graphiques en anneau. Cette fonctionnalité permet aux utilisateurs et utilisatrices d’afficher une valeur centrale qui représente le total de tous les segments du graphique.</p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nouvelles options de configuration pour les graphiques en secteurs dans les tableaux de bord de la zone de travail</a>
            <p>Nous avons introduit deux nouvelles options de configuration pour les graphiques en secteurs : <ul><li>Masquer les libellés de segment : vous pouvez désormais choisir de masquer les libellés de segment dans un graphique en secteurs s’ils sont trop longs et ont un impact sur la lisibilité du graphique.</li><li>Masquer et repositionner la légende du graphique : vous pouvez désormais choisir de masquer une légende de graphique en secteurs. Vous pouvez également définir la position de la légende à droite (par défaut), à gauche, en haut ou en bas du graphique. </li></ul></p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Améliorations du nombre de regroupements de tableaux de bord de la zone de travail</a>
            <p>Nous avons mis à jour la barre de regroupement dans les tableaux de bord de la zone de travail afin d’afficher le nombre d’enregistrements pour la page active et le nombre total d’enregistrements pour le regroupement sur toutes les pages. </p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nouvelle fonctionnalité Ligne de référence dans les rapports des tableaux de bord de la zone de travail</a>
            <p>Vous pouvez désormais définir une ligne de référence dans les graphiques à barres, en colonnes et linéaires pour définir une cible ou un seuil pour vos rapports basés sur des séries. </p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Personnaliser les libellés d’axe dans les rapports sur les graphiques des tableaux de bord de la zone de travail</a>
            <p>Vous pouvez désormais personnaliser les libellés des axes sur les rapports de graphique. Cette nouvelle fonctionnalité vous permet de saisir un libellé d’axe de remplacement à afficher au lieu de l’objet et du chemin d’accès au champ par défaut. De plus, vous pouvez choisir de masquer entièrement les libellés de l’axe.</p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Dupliquer un rapport dans un tableau de bord de la zone de travail</a><p>[!BADGE Hors planning]{type=Neutral}</p>
            <p>Vous pouvez désormais dupliquer un rapport de KPI, de tableau ou de graphique dans un tableau de bord de la zone de travail après sa création. Une fois dupliqué, vous pouvez modifier le rapport selon vos besoins avant de l’enregistrer.</p>
        </td>
        <td>23 octobre 2025</td>
        <td>23 octobre 2025</td>
        <td>23 octobre 2025</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Suppression des options de champ des filtres de rapport</a>
            <p>Nous avons supprimé les options de champ suivantes qui étaient auparavant disponibles lors de l’application d’un filtre à un rapport :
            <ul>
            <li>ID d’autres groupes</li>
            <li>ID d’autres fonctions</li>
            <li>ID d’autres équipes</li>
            </ul>
            </p>
        </td>
        <td>6 novembre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 janvier 2026</td>
    </tr>    
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nouveaux mécanismes de sécurisation pour améliorer les temps de chargement dans les tableaux de bord de la zone de travail</a>
            <p>Pour éviter les retards de chargement et améliorer les performances globales dans les tableaux de bord de la zone de travail, nous avons appliqué des limites au nombre de composants de tableau de bord pouvant être ajoutés à un tableau de bord :
            <ul>
            <li>Rapports par tableau de bord : limite de 25</li>
            <li>Regroupements sur les vues du tableau : limite de 5</li>
            <li>Distance par rapport à l’objet de base du rapport : limite de 10</li>
            <li>Colonnes dans une vue de tableau : limite de 25</li>
            <li>Prompts de filtre au niveau du tableau de bord : limite de 10</li>
            </ul></p>
        </td>
       <td>6 novembre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 janvier 2026</td>
    </tr>   
  </tbody>
</table>

### Améliorations des demandes

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>Fonctionnalité</strong>
        </td>
        <td><strong>Aperçu</strong></td>
        <td><strong>Version rapide</strong></td>
        <td><strong>Tous les trimestres</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Les liens d’objet créés sont désormais disponibles dans la zone Requêtes et dans le widget Mes requêtes</a>
            <p>Pour accéder plus facilement à l’objet créé par une requête spécifique, nous avons ajouté des liens vers la colonne Objet créé. Vous pouvez maintenant cliquer sur le lien de cette colonne pour accéder directement à la page de l’objet créé.</p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr> 
    <!--
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Create groupings in the Requests list and My Requests widget</a>
            <p>To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr>
    -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Ajout de champs personnalisés à la liste Requêtes et au widget Mes requêtes</a>
            <p>Pour accéder plus facilement aux informations dont vous avez besoin, vous avez désormais la possibilité d’ajouter des champs personnalisés sous forme de colonnes dans la liste Requêtes et le widget Mes requêtes sur la page d’accueil. Vous pouvez désormais ajouter des champs de formulaires personnalisés sous forme de colonnes, et les requêtes qui contiennent des informations dans ce champ afficheront ces informations dans la liste ou le widget.</p><p>Cette fonctionnalité n’est disponible que pour la nouvelle expérience des requêtes.</p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Le caractère générique pour l’utilisateur actuel est désormais disponible dans le filtre Requêtes</a>
            <p>Pour faciliter le filtrage des requêtes qui vous concernent, nous avons créé un caractère générique pour l’utilisateur actuel. Désormais, lors du filtrage, vous pouvez sélectionner « Moi (utilisateur connecté) ». Le filtre s’applique alors à l’utilisateur ou l’utilisatrice qui consulte la liste des requêtes.   </p>
        </td>
        <td>18 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Le remplissage de formulaire optimisé par l’IA est désormais disponible pour les requêtes</a>
            <p>Pour faciliter la création de requêtes, nous avons créé un remplissage de formulaire optimisé par l’IA. Désormais, vous pouvez coller un prompt ou charger un document dans un formulaire de requête, et l’IA extrait les informations pertinentes pour remplir le formulaire.  </p>
        </td>
        <td>11 décembre 2025</td>
        <td>11 décembre 2025</td>
        <td>11 décembre 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Partage de vues dans la zone des Requêtes et le widget Mes requêtes</a>
            <p>Pour accéder facilement aux informations dont vous avez besoin, nous avons ajouté la possibilité de partager des vues à la nouvelle expérience de création de requêtes. Vous pouvez désormais partager des vues avec d’autres utilisateurs et utilisatrices, équipes ou groupes. </p>
        </td>
        <td>4 décembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Enregistrement des brouillons des requêtes dans la nouvelle expérience de création de requêtes</a>
            <p>Pour faciliter la création et l’envoi de requêtes, nous avons ajouté la possibilité d’enregistrer des brouillons dans la nouvelle expérience de création de requêtes. Désormais, lorsque vous commencez à remplir une requête en cours et que vous la fermez, la requête est enregistrée au statut Brouillon et figure sur le formulaire de requête utilisé pour créer le brouillon. Vous pouvez ensuite rouvrir, mettre à jour et envoyer le brouillon à votre convenance. </p>
        </td>
        <td>20 novembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Suppresion des requêtes envoyées dans la nouvelle expérience de création de requêtes</a>
            <p>Pour que vos requêtes soient plus faciles à organiser et à gérer, nous avons ajouté la possibilité de supprimer des requêtes à la nouvelle expérience de création de requêtes. Désormais, vous pouvez supprimer les requêtes que vous avez envoyées. Les administrateurs et administratrices des espaces de travail Workfront et Workfront Planning peuvent également supprimer des requêtes.</p>
        </td>
        <td>20 novembre 2025</td>
        <td>14 janvier 2026</td>
        <td>15 janvier 2026</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Création de requêtes en copiant les requêtes précédemment envoyées dans la nouvelle expérience de création de requêtes</a>
            <p>Pour faciliter l’envoi de requêtes, nous avons ajouté la possibilité de copier des requêtes dans la nouvelle expérience de création de requêtes. Vous pouvez désormais copier une requête, modifier n’importe quel champ et l’envoyer en tant que nouvelle requête. </p>
        </td>
        <td>20 novembre 2025</td>
        <td>11 décembre 2025</td>
        <td>15 janvier 2026</td>
    </tr>    
  </tbody>
</table>

### Autres améliorations

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Fonctionnalité</strong>
        </td>
        <td><strong>Aperçu</strong></td>
        <td><strong>Version rapide</strong></td>
        <td><strong>Tous les trimestres</strong></td>
    </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’apparence au cours des versions publiées au premier trimestre 2026</a>
                        <p>Des mises à jour mineures de l’aspect de diverses zones de l’application Adobe Workfront sont effectuées pendant la période du premier trimestre 2026. </p>
                    </td>
                    <td><p>Tout au long de la période de publication du premier trimestre 2026<br /></p>
                    <td colspan="2"><p>Version rapide : au moins 1 semaine après la publication dans l’environnement de prévisualisation (sauf indication contraire)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}"> Limites de sélection sur les champs à sélection multiple</a>
              <p>Les champs qui autorisent plusieurs sélections, tels que les cases à cocher et les listes déroulantes à sélection multiple, sont désormais limités à 5 000 sélections lors du remplissage d’un formulaire.</p>
             </td>
        <td>30 octobre 2025</td>
        <td>13 novembre 2025</td>
        <td>15 janvier 2026</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience est désormais disponible pour plus d’organisations Workfront</a>.<p></p>
            <p>Pour permettre aux organisations d’accéder aux avantages d’Adobe Unified Experience, nous avons commencé à la mettre à la disposition des clientes et des clients Workfront existants.</p>
        </td>
        <td><p>vendredi 11 décembre 2025</p></td>
        <td><p>jeudi 11 février 2026</p></td>
        <td><p>jeudi 11 février 2026</p></td>
    <tr>
            </tbody>
        </table>


### Fonctionnalités bientôt supprimées de Workfront

#### Abandon de la devise de remplacement pour les fonctions dans la version 25.11

Dans le cadre de la simplification du modèle financier, nous allons rendre obsolète la devise de remplacement sur les fonctions dans la prévisualisation le 30 octobre et dans la production pour l’ensemble de la clientèle avec la version 25.11. Cette modification affecte la façon dont les devises et les taux sont configurés sur les fonctions dans la zone Configuration.

* Les champs **Devise de remplacement** d’une fonction ne seront plus disponibles.
* Chaque fonction dispose d’une devise unique avec son coût et son taux de facturation associés.
* Toutes les devises de remplacement existantes et leurs valeurs de taux seront automatiquement migrées pour devenir la devise et les taux uniques de cette fonction.

## Modernisation de l’interface

Nous mettons à jour l’interface d’Adobe Workfront afin d’améliorer l’expérience client et de l’harmoniser avec les autres applications Adobe. Ces modifications sont publiées selon un rythme différent du planning de publication standard. Pour obtenir la liste de ces modifications, voir [Modernisation de l’interface](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Notes de mise à jour pour d’autres zones

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production selon un rythme différent du planning de publication standard. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de publication d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Améliorations apportées à Workfront Planning

De nouvelles fonctionnalités Workfront Planning sont disponibles en production. Pour plus d’informations sur les dernières fonctionnalités, voir [Premier trimestre 2026 - Activité de publication d’Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md).

Les éléments suivants n’ont pas été modifiés à ce stade de la publication :

* Planificateur de scénarios
* Épreuve
* Objectifs

## Mises à jour de la visionneuse de relecture de bureau

### Version 2.1.54

**Version de production pour tous les clients et clientes : 11 décembre 2025**

La visionneuses de relecture de bureau a été mise à jour et passe de la version 2.1.52 à la version 2.1.54. Cette mise à jour inclut des mises à jour d’outils internes et n’a aucune incidence sur les fonctionnalités accessibles par les utilisatrices et utilisateurs finaux.

La version 2.1.53 incluait également des modifications des outils internes.

Cette mise à jour concerne Mac et Windows.

### Version 2.1.52

**Version de production pour tous les clients et clientes : 31 juillet 2025**

La visionneuse de relecture de bureau a été mise à jour vers la version 2.1.52, qui inclut des correctifs.

La mise à jour 2.1.51 incluait des mises à jour des outils internes et n’avait aucune incidence sur les fonctionnalités accessibles par les utilisatrices et utilisateurs finaux.

Cette mise à jour concerne Mac et Windows.

## Annonces

### Version 21 de l’API

La version 21 de l’API Workfront a été publiée le 23 octobre 2025. Pour la version 21 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

>[!IMPORTANT]
>
>La modification de cette version de l’API comprend un changement majeur qui peut affecter vos appels API existants. Cela est dû au fait que la version 21 de l’API utilise la version 2 des abonnements aux événements.
>
> Pour les champs à sélection multiple, la version 2 des abonnements aux événements envoie toujours un tableau. La version 1 envoyait un tableau si plusieurs valeurs étaient sélectionnées. Si une seule valeur était sélectionnée, elle envoyait une chaîne.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 21 de l’API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions et de la prise en charge de l’API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Nouvelle version de Workfront pour Microsoft Teams

Comme [Microsoft passe au nouveau client Teams](https://learn.microsoft.com/fr-fr/microsoftteams/teams-classic-client-end-of-availability), le client Teams classique ne sera plus disponible après le 1er juillet 2025. Pour continuer à utiliser Microsoft Teams et les applications intégrées telles que Workfront, les clients et clientes devront passer au nouveau client Teams avant cette date.

L’intégration Workfront mise à jour est désormais disponible et entièrement compatible avec la nouvelle expérience Teams. Dans la plupart des cas, Workfront s’affiche automatiquement une fois la transition effectuée. Si ce n’est pas le cas, l’intégration peut être installée manuellement à partir de l’App Store Microsoft Teams. Pour installer ou vérifier l’intégration de Workfront dans le nouveau client Teams, voir [Installer  [!DNL Adobe Workfront]  pour Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront pour Microsoft Outlook

[Microsoft désactive progressivement la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/fr-fr/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le module complémentaire Workfront Outlook pour l’authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et les clientes, et continuera à être déployée par phases jusqu’en octobre 2025.

* **Une fois que Microsoft aura complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionnera plus.**

Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière de réactiver les jetons. À partir du **30 juin 2025**, les équipes d’administration ne pourront plus réactiver les jetons elles-mêmes. Seul le support Microsoft pourra accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Aucune exception ne sera accordée.**

### Autres transitions d’intégration Workfront

Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de l’automatisation et de l’intégration Workfront (Fusion). Dans le cadre de ce processus de transition, les intégrations suivantes ne seront pas disponibles après le **28 février 2026** :

* Workfront pour G Suite
* Workfront pour Jira
* Workfront pour Salesforce.

Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre entreprise à Google Workspace.
Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez la [Vue d’ensemble d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Mises à jour de maintenance pour Workfront

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version du premier trimestre 2025, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).
