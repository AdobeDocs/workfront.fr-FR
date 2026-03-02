---
title: Vue d’ensemble de la version du deuxième trimestre 2026
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du deuxième trimestre 2026. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: 8fdc6d1b72967b2a52295c31cb83d43594817d6f
workflow-type: tm+mt
source-wordcount: '1323'
ht-degree: 44%

---

# Vue d’ensemble de la version du deuxième trimestre 2026

Cette page fournit des informations sur les fonctionnalités incluses dans la version du deuxième trimestre 2026 prévue pour avril 2026.

Les améliorations apportées à cette page sont disponibles dans l’environnement de Prévisualisation. Cette page sera mise à jour avec des améliorations supplémentaires à mesure que la version du deuxième trimestre 2026 approche de sa date de sortie en production.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>26.2 (vendredi 12 février 2026)</li><li>26.3 (vendredi 12 mars 2026)</li><li>26.4 (jeudi 15 avril 2026)</li></ul> | <ul><li>26.1 (vendredi 16 avril 2026)</li></ul> |
>
>Notez que pour la version finale de chaque trimestre (26.4 ce trimestre), les utilisateurs disposant du planning de publication rapide recevront la version un jour plus tôt (15 avril 2026).
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations du document](#document-enhancements)
* [Améliorations des projets](#project-enhancements)
* [Amélioration des rapports](#reporting-enhancements)
* [Demande d’améliorations](#requesting-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations apportées aux administrateurs et administratrices

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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Réduire la section de formulaire personnalisé par défaut</a><p>Par défaut, toutes les sections d’un formulaire personnalisé sont développées lorsque le formulaire lui-même est développé. Une nouvelle option du concepteur de formulaire personnalisé vous permet de marquer une section à réduire par défaut lorsqu’un utilisateur ouvre le formulaire. Cette option est appliquée au niveau de la section, et non des champs.</p>
        </td>
        <td><p>jeudi 26 février 2025</p></td>
        <td><p>vendredi 12 mars 2026</p></td>
        <td><p>vendredi 16 avril 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Le type de champ Texte enrichi est désormais disponible sur les formulaires personnalisés</a><p>Le nouveau type de champ <b>Texte enrichi</b> dans les formulaires personnalisés est un puissant éditeur de texte, avec des options de mise en forme telles que l’exposant et l’indice, les en-têtes et les tableaux, en plus des options traditionnelles telles que le gras, l’italique, le soulignement, les puces, la numérotation, les liens hypertexte et les guillemets. La limite de caractères reste de 15 000.</p>
        </td>
        <td><p>vendredi 29 janvier 2026</p></td>
        <td><p>vendredi 12 février 2026</p>
            <p>Cette fonctionnalité a été temporairement supprimée de l’environnement de production le 13 février 2026.</p></td>
        <td><p>À déterminer</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Nouvelles adresses IP pour les notifications par e-mail de Workfront</a><p></p>
            <p>Nous mettons à jour les adresses IP utilisées pour envoyer des notifications par e-mail à partir de Workfront. Si votre entreprise gère une liste autorisée de type e-mail ou pare-feu, vous <b>devez</b> ajouter les nouvelles adresses IP ci-dessous pour assurer la diffusion continue des notifications Workfront.</p><p>Ces mises à jour s’appliquent à tous les e-mails sortants générés par l’application Workfront, y compris les approbations, les rappels, les notifications de BAT et d’autres messages système.</p>
            <ul>
            <li>US :
            <ul>
            <li>206.55.149.212</li>
            <li>206.55.149.214</li>
            <li>206.55.149.215</li>
            <li>206.55.149.213</li>
            <li>206.55.149.211</li>
            </ul>
            </li>
            <li>UE : 
            <ul>
            <li>24.110.76.224</li>
            <li>24.110.76.223</li>
            </ul>
            </li>
            </ul> </p>
        </td>
        <td><p>vendredi 15 janvier 2026</p></td>
        <td><p>vendredi 15 janvier 2026</p></td>
        <td><p>15 janvier 2026</p></td>
    <tr>
            </tbody>
        </table>

<!--

### Document enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Multi‑stage approval workflows available for unified approvals</a><p></p>
            <p>Multi‑stage approval workflows are now available in unified approvals, helping organizations enforce structured, repeatable approval processes that reflect how work is reviewed in the real world. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Set up and use multi-stage approval workflow templates</a><p></p>
            <p>You can now configure and reuse multi-stage approval workflow templates, making it easier to apply consistent governance across repeatable approval workflows. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
             </tbody>
        </table>   

-->

### Améliorations des projets

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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}">Mise à jour de l’expérience lors de la </a> de tâches de modèles d’affectation unique ou en bloc<p>[!BADGE Hors planning]{type=Neutral}</p><p> Nous avons mis à jour la section Affectations de la zone Modifier les tâches de modèles lors de la modification de tâches de modèles uniques ou de leur modification en bloc.  </p>
        </td>
        <td><p>vendredi 5 février 2026</p></td>
        <td><p>À Compter Du 5 Février 2026</p></td>
        <td><p>À Compter Du 5 Février 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Expérience mise à jour lors de l’affectation de tâches en une seule fois ou en bloc </a><p>[!BADGE Hors planning]{type=Neutral}</p><p> Nous avons mis à jour la section Affectations dans la zone Modifier les tâches lors de la modification de tâches uniques ou de leur modification en bloc. </p>
        </td>
        <td><p>mardi 26 janvier 2026</p></td>
        <td><p>À Compter Du 5 Février 2026</p></td>
        <td><p>À Compter Du 5 Février 2026</p></td>
    </tr>
            </tbody>
        </table>

### Amélioration des rapports

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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Libellés de champ personnalisés affichés lors de la création de rapports</a><p></p>
            <p>Le libellé du champ personnalisé s’affiche désormais avant le nom du champ et l’objet dans les outils de création de rapports, ce qui vous permet de localiser plus facilement les champs. Les libellés des champs s’affichent également lors de la définition de filtres, de vues et de regroupements dans des listes.</p>
        </td>
        <td><p>jeudi 26 février 2025</p></td>
        <td><p>vendredi 12 mars 2026</p></td>
        <td><p>vendredi 16 avril 2026</p></td>
    </tr>
   <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Dossiers de rapports partageables</a><p></p>
            <p>Vous pouvez désormais organiser et partager des rapports à l’aide de dossiers de rapports partageables. Cette nouvelle fonctionnalité permet aux équipes qui gèrent d’importants volumes de rapports de conserver un contrôle d’accès évolutif et cohérent.</p>
        </td>
        <td><p>jeudi 26 février 2025</p></td>
        <td><p>vendredi 12 mars 2026</p></td>
        <td><p>vendredi 16 avril 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">Amélioration des libellés de date pour les regroupements de graphiques dans les tableaux de bord Zone de travail</a><p></p>
            <p>Les graphiques qui regroupent les données par date affichent désormais des libellés de date plus clairs et plus lisibles. Grâce à cette mise à jour, les libellés de date s’ajustent de manière dynamique en fonction de l’option Regrouper par sélectionnée (par jour, semaine, mois ou année, par exemple), ce qui facilite la lecture et l’interprétation des graphiques en un coup d’œil.</p><p>Remarque : les tableaux de bord de la zone de travail sont actuellement en version bêta.</p>
        </td>
        <td><p>jeudi 26 février 2025</p></td>
        <td><p>vendredi 12 mars 2026</p></td>
        <td><p>vendredi 16 avril 2026</p></td>
    </tr>
             </tbody>
        </table>

### Demande d’améliorations

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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}">Expérience de partage mise à jour pour les vues améliorées</a><p></p>
            <p>Dans la zone Nouvelles requêtes , lorsque vous partagez une vue améliorée avec un utilisateur et que vous lui donnez des autorisations d’affichage, l’utilisateur peut modifier les éléments d’affichage et ces modifications sont enregistrées dans les préférences personnelles de l’utilisateur. Ils ont désormais la possibilité d’enregistrer une copie de la vue qui comprend leurs modifications ou de réinitialiser la vue partagée à ses paramètres d’origine. Ils peuvent également partager la vue copiée avec d’autres utilisateurs. </p>
        </td>
           <td><p>jeudi 26 février 2025</p></td>
        <td><p>vendredi 12 mars 2026</p></td>
        <td><p>vendredi 16 avril 2026</p></td>
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
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience est désormais disponible pour plus d’organisations Workfront</a>.<p></p>
            <p>Pour permettre aux organisations d’accéder aux avantages d’Adobe Unified Experience, nous avons commencé à la mettre à la disposition des clientes et des clients Workfront existants.</p>
        </td>
        <td><p>vendredi 11 décembre 2025</p></td>
        <td><p>jeudi 11 février 2026</p></td>
        <td><p>jeudi 11 février 2026</p></td>
    </tr>
            </tbody>
        </table>


<!--### Functionality soon to be removed from Workfront-->

<!--

## Interface modernization

We are updating the interface throughout Adobe Workfront to improve the user experience and unify it with other Adobe applications. These changes are released outside the standard release schedule. For a list of these changes, see [Interface Modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

-->

## Notes de mise à jour pour d’autres zones

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production selon un rythme différent du planning de publication standard. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de publication d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Améliorations apportées à Workfront Planning

De nouvelles fonctionnalités Workfront Planning sont disponibles en production. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de la version du deuxième trimestre 2026 pour Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md).

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

## Annonces

### La version d’évaluation de Workfront Planning est désormais disponible.

[!BADGE Horaire de désactivation]{type=Neutral}

>[!NOTE]
>
>* Aperçu et production pour tous : 2 mars 2026
>* Vous devez accepter l&#39;accord d&#39;essai disponible dans votre environnement avant de pouvoir accéder à l&#39;environnement d&#39;essai Planning.
>* Vous n’avez pas besoin de signer le contrat d’agent Adobe AI pour utiliser Planning Designer pendant la période d’évaluation.

La version d’évaluation de Workfront Planning est désormais disponible pour tous les clients Workfront.

L’essai gratuit offre aux clients Workfront un accès de licence Prime de 60 jours à Workfront Planning, à compter du 2 mars 2026. La période d’essai se termine le 1er mai 2026.

La version d’essai gratuite de Workfront Planning offre les avantages suivants :

* Un environnement Planning organisé sur plusieurs espaces de travail
* Exemples de données pour vous donner une idée de l’endroit où commencer
* Formation et conseils intégrés au produit
* Indiquez clairement les jalons de votre configuration qui sont adaptés à des rôles spécifiques.
* Planning Designer : un assistant optimisé par l’IA qui peut vous aider à créer l’environnement souhaité

Pour plus d’informations, voir [Prise en main de la version d’essai gratuite d’Adobe Workfront Planning](/help/quicksilver/planning/general/trial-workfront-planning.md).

### Version 21 de l’API

La version 21 de l’API Workfront a été publiée le 23 octobre 2025. Pour la version 21 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

>[!IMPORTANT]
>
>La modification de cette version de l’API comprend un changement majeur qui peut affecter vos appels API existants. Cela est dû au fait que la version 21 de l’API utilise la version 2 des abonnements aux événements.
>
> Pour les champs à sélection multiple, la version 2 des abonnements aux événements envoie toujours sous la forme d’un tableau. La version 1 envoyait un tableau si plusieurs valeurs étaient sélectionnées. Si une seule valeur était sélectionnée, elle envoyait une chaîne.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 21 de l’API](/help/quicksilver/wf-api/api/new-api-version-21.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions et de la prise en charge de l’API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Autres transitions d’intégration Workfront

Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de l’automatisation et de l’intégration Workfront (Fusion). Dans le cadre de ce processus de transition, les intégrations suivantes ne seront pas disponibles après le **28 février 2026** :

* Workfront pour G Suite
* Workfront pour Jira
* Workfront pour Salesforce.

Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre entreprise à Google Workspace.
Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez la [Vue d’ensemble d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).


### Mises à jour de maintenance pour Workfront

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version du deuxième trimestre 2025, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).
