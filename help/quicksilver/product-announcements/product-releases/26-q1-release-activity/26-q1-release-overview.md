---
title: Vue d’ensemble de la version du premier trimestre 2026
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du premier trimestre 2026. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 8f126e75845e15ff5d4e0b327abcfafb1dbffd99
workflow-type: tm+mt
source-wordcount: '2152'
ht-degree: 16%

---

# Vue d’ensemble de la version du premier trimestre 2026

Cette page fournit des informations sur les fonctionnalités incluses dans la version du premier trimestre 2026 prévue pour janvier 2026.

Les améliorations apportées à cette page sont disponibles dans l’environnement de Prévisualisation. Cette page sera mise à jour avec des améliorations supplémentaires à mesure que la version du premier trimestre 2026 approche de sa date de sortie en production.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>Version 25.11 (13 Novembre 2025)</li><li>Version 25.12 (11 Décembre 2025)</li><li>26.1 (14 janvier 2026)</li></ul> | <ul><li>26.1 (15 janvier 2026)</li></ul> |
>
>Notez que pour la version finale de chaque trimestre (26.1 ce trimestre), les utilisateurs disposant du planning de publication rapide recevront la version un jour plus tôt (14 janvier 2026).
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations des documents et des approbations](#documents-and-approvals-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations apportées aux projets](#project-enhancements)
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Date de saisie et ID Entré par stocké dans des objets personnalisés</a><p>[!BADGE Off schedule]{type=Neutral}</p>
            <p>La date de saisie et l’ID saisi par sont désormais stockés dans des formulaires, champs et sections personnalisés. Vous pouvez utiliser ces options de données dans les rapports sous la forme de filtres, de vues ou de regroupements. Pour les afficher dans la liste des formulaires, champs ou sections personnalisés de la configuration, ajoutez Date de saisie et Nom saisi comme colonnes dans une vue nouvelle ou existante.</p>
        </td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 13 novembre 2025</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Met à jour les noms de bouton lors de la modification d’un modèle de mise en page</a>
            <p>Pour plus de cohérence avec d’autres zones de la configuration, telles que le concepteur de formulaire personnalisé, les boutons affichés lors de la modification d’un modèle de mise en page ont été modifiés en Appliquer, Enregistrer et fermer et Annuler. La nouvelle option Appliquer permet d’enregistrer les modifications apportées au modèle de mise en page et de continuer la modification. Auparavant, les options disponibles étaient Enregistrer et Annuler. </p>
        </td>
        <td>vendredi 30 octobre 2025</td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Amélioration de la gestion des champs avec l’indicateur Actif sur les champs personnalisés </a>
            <p>Lorsque le système comporte un grand nombre de champs personnalisés, la gestion de ces champs dans les formulaires et les rapports personnalisés peut s’avérer difficile. Vous pouvez désormais marquer les champs personnalisés comme inactifs avec le nouvel indicateur <b>Actif</b>. Cet indicateur est disponible lors de l’utilisation d’un champ dans un formulaire personnalisé ou lors de l’ajout ou de la modification d’un champ de la liste Champs . </p>
        </td>
        <td>vendredi 30 octobre 2025</td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
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
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Choisir un projet Workfront lors de l’envoi d’une révision dans Creative Cloud Express<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Vous pouvez choisir un projet Workfront auquel envoyer un BAT. Cela permet de conserver toutes les ressources et épreuves associées organisées au sein d’un même projet.</p>
        </td>
        <td>mardi 15 décembre 2025</td>
        <td>mardi 15 décembre 2025</td>
        <td>mardi 15 décembre 2025</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Prise en charge inter-organisations d’Adobe Express avec la relecture Workfront<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Nous introduisons la prise en charge inter-organisations d’Adobe Express avec la relecture Workfront. Cette amélioration permet aux clients qui travaillent dans plusieurs organisations IMS d’utiliser et de gérer facilement les workflows de relecture.</p>
        </td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 13 novembre 2025</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager désormais disponible avec l'intégration Frame.io <p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>Vous pouvez désormais utiliser Experience Manager Assets​ pour gérer et stocker vos ressources numériques qui ont passé le cycle de révision et d’approbation. Cette intégration vous permet d’exploiter les fonctionnalités de Adobe Experience Manager, Frame.io et Workfront afin de rationaliser vos processus de gestion de contenu et de collaboration. </p>
        </td>
        <td>vendredi 30 octobre 2025</td>
        <td>vendredi 30 octobre 2025</td>
        <td>vendredi 30 octobre 2025</td>
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Mise à jour du sélecteur de ressources pour le </a> d’intégration natif d’Adobe Workfront for Experience Manager Assets
            <p>Nous avons mis à niveau le sélecteur de ressources dans l’intégration Adobe Workfront for Experience Manager Assets. Grâce à cette mise à niveau, vous pouvez désormais sélectionner et extraire des collections AEM directement dans Workfront. </p>
        </td>
        <td>vendredi 20 novembre 2025</td>
        <td>vendredi 11 décembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">Nouvelle version de l’intégration Salesforce désormais disponible </a>
            <p>Pour rester à jour avec les récentes modifications apportées à l’API Workfront, nous avons créé une nouvelle intégration Salesforce. La nouvelle intégration propose la même fonctionnalité que la version précédente et a été mise à jour afin d’éviter de perdre une fonctionnalité obsolète dans l’API.</p><p>REMARQUE : l’intégration de Workfront for Salesforce, y compris la nouvelle version, ne sera plus disponible après le **28 février 2026**. </p>
        </td>
        <td>vendredi 30 octobre 2025</td>
        <td>vendredi 30 octobre 2025</td>
        <td>vendredi 30 octobre 2025</td>
    </tr>   
  </tbody>
</table>

### Améliorations apportées aux projets

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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">Les utilisateurs légers peuvent enregistrer le temps passé sur les projets</a>
            <p>Les utilisateurs de Light peuvent désormais consigner le temps directement dans les projets. Auparavant, seuls les utilisateurs de licence standard pouvaient enregistrer des heures sur les projets.</p>
        </td>
        <td>vendredi 11 décembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
        <td>vendredi 15 janvier 2026</td>
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Duplication d’un rapport dans un tableau de bord Zone de travail</a><p>![!BADGE Off schedule]{type=Neutral}</p>
            <p>Vous pouvez désormais dupliquer un rapport d’indicateur de performance clé, de tableau ou de graphique dans un tableau de bord de zone de travail après sa création. Une fois dupliqué, vous pouvez modifier le rapport selon vos besoins avant d’enregistrer.</p>
        </td>
        <td>vendredi 23 octobre 2025</td>
        <td>vendredi 23 octobre 2025</td>
        <td>vendredi 23 octobre 2025</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Suppression des options de champ des filtres de rapport</a>
            <p>Nous avons supprimé les options de champ suivantes qui étaient auparavant disponibles lors de l’application d’un filtre à un rapport :
            <ul>
            <li>Autres ID de groupe</li>
            <li>ID d'autres rôles</li>
            <li>Autres ID d'équipe</li>
            </ul>
            </p>
        </td>
        <td>vendredi 6 novembre 2025</td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Affichage amélioré du nombre de regroupements dans les tableaux de bord de la zone de travail</a>
            <p>Lorsqu’un rapport tabulaire comporte plusieurs pages de résultats et que le tableau est configuré avec des regroupements, le tableau affiche désormais à la fois la quantité d’enregistrements de la page active et le nombre total d’enregistrements de toutes les pages. Par exemple, si votre rapport de tableau comporte 7 regroupements et que la première page affiche 3, le tableau affiche 3 de 7.</p>
        </td>
       <td>vendredi 6 novembre 2025</td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">Nouveaux mécanismes de sécurisation pour améliorer les temps de chargement dans les tableaux de bord de la zone de travail</a>
            <p>Pour éviter les retards de chargement et améliorer les performances globales dans les tableaux de bord de la zone de travail, nous avons appliqué des limites au nombre de composants de tableau de bord pouvant être ajoutés à un tableau de bord :
            <ul>
            <li>Rapports par tableau de bord : limite de 25</li>
            <li>Regroupements sur les vues de la table : 5 limite</li>
            <li>Distance par rapport à l'objet de base du rapport : limite de 10</li>
            <li>Colonnes dans une vue Tableau : limite de 25</li>
            <li>Invites de filtre au niveau du tableau de bord : limite de 10</li>
            </ul></p>
        </td>
       <td>vendredi 6 novembre 2025</td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Le remplissage de formulaire optimisé par l’IA est désormais disponible pour les requêtes</a>
            <p>Pour faciliter la création de requêtes, nous avons créé un remplissage de formulaire optimisé par l’IA. Désormais, vous pouvez coller une invite ou charger un document dans un formulaire de demande, et AI extraira les informations pertinentes et remplira le formulaire.  </p>
        </td>
        <td>vendredi 11 décembre 2025</td>
        <td>vendredi 11 décembre 2025</td>
        <td>vendredi 11 décembre 2025</td>
    </tr> 
    <tr>
        <!--<td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Share views in the Requests area and the My Requests widget</a>
            <p>To make it easier to ensure to see the information you need, we've added the ability to share views to the new reporting experience. Now, you can share views with other users, teams, or groups. </p>
        </td>
        <td>December 4, 2025</td>
        <td>December 11, 2025</td>
        <td>January 15, 2026</td>
    </tr> -->
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Enregistrer les brouillons des demandes dans la nouvelle expérience de demande</a>
            <p>Pour faciliter la création et l’envoi de demandes, nous avons ajouté la possibilité d’enregistrer des brouillons dans la nouvelle expérience de demande. Désormais, lorsque vous commencez à remplir une demande et que vous la fermez, la demande est enregistrée au statut Brouillon et figure sur le formulaire de demande utilisé pour créer le brouillon. Vous pouvez ensuite rouvrir, mettre à jour et envoyer le brouillon à votre convenance. </p>
        </td>
        <td>vendredi 20 novembre 2025</td>
        <td>jeudi 14 janvier 2026</td>
        <td>vendredi 15 janvier 2026</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Supprimer les demandes envoyées dans la nouvelle expérience de demande</a>
            <p>Pour que vos requêtes restent plus faciles à organiser et à gérer, nous avons ajouté la possibilité de supprimer des requêtes à la nouvelle expérience de requête. Désormais, vous pouvez supprimer les requêtes que vous avez envoyées. Les administrateurs de Workfront et les administrateurs de Workfront Planning Workspace peuvent également supprimer des requêtes.</p>
        </td>
        <td>vendredi 20 novembre 2025</td>
        <td>jeudi 14 janvier 2026</td>
        <td>vendredi 15 janvier 2026</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Créez de nouvelles demandes en copiant les demandes précédemment envoyées dans la nouvelle expérience de demande</a>
            <p>Pour faciliter l’envoi de demandes, nous avons ajouté la possibilité de copier des demandes dans la nouvelle expérience de demande. Vous pouvez désormais copier une demande, modifier n’importe quel champ et l’envoyer en tant que nouvelle demande. </p>
        </td>
        <td>vendredi 20 novembre 2025</td>
        <td>vendredi 11 décembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Mises à jour en fonction de l’apparence au cours du premier trimestre de 2026</a>
                        <p>Des mises à jour mineures de l’aspect de diverses zones de l’application Adobe Workfront sont apportées dans le cadre de la publication de la version du premier trimestre 2026. </p>
                    </td>
                    <td><p>Tout au long de la période de publication du premier trimestre 2026<br /></p>
                    <td colspan="2"><p>Version rapide : au moins 1 semaine après la publication dans l’aperçu (sauf indication contraire).</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                Limites de <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}"> Selection sur les champs à sélection multiple</a>
              <p>Les champs qui autorisent plusieurs sélections, tels que les cases à cocher et les listes déroulantes à sélection multiple, sont désormais limités à 5 000 sélections lorsqu’un utilisateur remplit le formulaire.</p>
             </td>
        <td>vendredi 30 octobre 2025</td>
        <td>vendredi 13 novembre 2025</td>
        <td>vendredi 15 janvier 2026</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience est désormais disponible pour plus d’organisations Workfront</a>.<p></p>
            <p>Pour permettre aux entreprises d’accéder aux avantages de l’expérience unifiée Adobe, nous continuons à la rendre disponible pour les clients Workfront existants.</p>
        </td>
        <td><p>vendredi 11 décembre 2025</p></td>
        <td><p>vendredi 15 janvier 2026</p></td>
        <td><p>vendredi 15 janvier 2026</p></td>
    <tr>
            </tbody>
        </table>


### Fonctionnalités bientôt supprimées de Workfront

#### Abandon de la devise de remplacement pour les fonctions dans la version 25.11

Dans le cadre de la simplification du modèle financier, nous allons rendre obsolète la devise de remplacement sur les fonctions dans l’aperçu le 30 octobre et dans la production pour tous les clients avec la version 25.11. Cette modification affecte la façon dont les devises et les taux sont configurés sur les fonctions dans la zone Configuration.

* Les champs **Devise de remplacement** d’une fonction ne seront plus disponibles.
* Chaque fonction dispose d’une devise unique avec son coût et son taux de facturation associés.
* Toutes les devises de remplacement existantes et leurs valeurs de taux seront automatiquement migrées pour devenir la devise et les taux uniques de cette fonction.

## Modernisation des interfaces

Nous mettons à jour l’interface dans Adobe Workfront afin d’améliorer l’expérience utilisateur et de l’unifier avec d’autres applications Adobe. Ces modifications sont publiées en dehors du planning de publication standard. Pour obtenir la liste de ces modifications, voir [Modernisation des interfaces](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Notes de mise à jour pour d’autres zones

### Améliorations de Workfront Fusion

De nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à une cadence en dehors du calendrier de publication standard. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Améliorations apportées à Workfront Planning

De nouvelles fonctionnalités de Workfront Planning sont disponibles en production. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de la version du premier trimestre 2026 pour Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md).

Il n’existe aucune mise à jour pour les éléments suivants à ce stade de la version :

* Planificateur de scénarios
* Épreuve
* Objectifs

## Mises à jour du lecteur de vérification pour bureau

### Version 2.1.54

**Version de production pour tous les clients : 11 décembre 2025**

Le lecteur de vérification pour bureau a été mis à jour et passe de la version 2.1.52 à la version 2.1.54. Cette mise à jour incluait des mises à jour d’outils internes et n’avait aucune incidence sur les fonctionnalités des utilisateurs finaux.

La version 2.1.53 incluait également des modifications d’outils internes.

Cette mise à jour concerne Mac et Windows.

### Version 2.1.52

**Version de production pour tous les clients : 31 juillet 2025**

Le lecteur de vérification pour bureau a été mis à jour vers la version 2.1.52, qui corrige les bugs.

La mise à jour 2.1.51 incluait des mises à jour d’outils internes et n’avait aucune incidence sur les fonctionnalités de l’utilisateur final.

Cette mise à jour concerne Mac et Windows.

## Annonces

### Version 21 de l’API

L’API Workfront version 21 a été publiée le 23 octobre 2025. Pour la version 21 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

>[!IMPORTANT]
>
>Cette modification de version de l’API comprend une modification avec rupture qui peut affecter vos appels API existants. Cela est dû au fait que l’API version 21 utilise la version 2 des abonnements aux événements.
>
> Pour les champs à sélection multiple, la version 2 des abonnements aux événements envoie toujours sous la forme d’un tableau. La version 1 a envoyé un tableau si plusieurs valeurs ont été sélectionnées. Si une seule valeur a été sélectionnée, une chaîne a été envoyée.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 21 de l’API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions et de la prise en charge de l’API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Nouvelle version de Workfront pour Microsoft Teams

Comme [Microsoft passe au client Nouvelles équipes](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability), le client Équipes classiques ne sera plus disponible après le 1er juillet 2025. Pour continuer à utiliser Microsoft Teams et les applications intégrées telles que Workfront, les clients doivent passer au client New Teams avant cette date.

L’intégration Workfront mise à jour est désormais disponible et entièrement compatible avec la nouvelle expérience Équipes . Dans la plupart des cas, Workfront s’affiche automatiquement une fois la transition effectuée. Si ce n’est pas le cas, l’intégration peut être installée manuellement à partir de Microsoft Teams App Store. Pour installer ou vérifier l’intégration de Workfront dans le client New Teams, voir [Installer [!DNL Adobe Workfront] pour Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront pour Microsoft Outlook

[Microsoft est en train de désactiver la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le complément Workfront Outlook pour l&#39;authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et continuera à être déployée par phases jusqu’en octobre 2025.

* **Une fois que Microsoft a complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionne plus.**

Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière dont les jetons sont réactivés. Après le **30 juin 2025**, les administrateurs ne pourront plus réactiver les jetons eux-mêmes. Seule la prise en charge de Microsoft peut accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Les exceptions ne seront pas accordées.**

### Autres transitions d’intégration Workfront

Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, les intégrations suivantes ne seront pas disponibles après le **28 février 2026** :

* Workfront pour G Suite
* Workfront pour Jira
* Workfront pour Salesforce.

Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre entreprise avec Google Workspace.
Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version du premier trimestre 2025, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).
