---
title: Vue d’ensemble de la version du deuxième trimestre 2025
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du deuxième trimestre 2025. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9b78a58e-7ced-4b13-8108-40bd36339667
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1653'
ht-degree: 33%

---

# Vue d’ensemble de la version du deuxième trimestre 2025

Cette page fournit des informations sur les fonctionnalités incluses dans la version du deuxième trimestre 2025. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.

<span class="preview">Les fonctionnalités hors cycle (sorties en production avant la date de la version du deuxième trimestre 2025) sont surlignées en jaune.</span>

## Calendrier des versions

Les versions de Workfront sont numérotées afin de tenir compte des suivis de version mensuels et trimestriels. Le premier chiffre désigne l&#39;année et le second indique le mois de la libération. Exemple : la version d’avril 2025 est numérotée 25.4.

Sauf indication contraire, les versions mensuelles et trimestrielles devraient être disponibles le jeudi de la deuxième semaine complète du mois.

| Version mensuelle | Version trimestrielle |
| ----------------- | ----------------- |
| <ul><li>25.2 (13 Février 2025)</li><li>25.3 (13 mars 2025)</li><li>25.4 (vendredi 10 avril 2025)</li></ul> | <ul><li>25.4 (vendredi 10 avril 2025)</li></ul> |

>[!NOTE]
>
>Pour la version finale de chaque trimestre (25.4 ce trimestre), les utilisateurs disposant du planning de version rapide recevront la version un jour plus tôt que prévu.
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations de la gestion des documents](#document-management-enhancements)
* [Améliorations mobiles](#mobile-enhancements)
* [Améliorations apportées aux projets](#project-enhancements)
* [Amélioration des rapports](#reporting-enhacements)
* [Autres améliorations](#other-enhancements)

### Améliorations apportées aux administrateurs et administratrices

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Améliorations de la logique des formulaires personnalisés</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p>
            <p>Le créateur logique de formulaires personnalisés dispose d’une interface mise à jour afin de vous offrir plus d’espace pour créer des règles logiques. Cette nouvelle conception peut s’adapter plus facilement à d’autres types de logiques qui pourraient être ajoutés à l’avenir.</p><p>Outre les options logiques d’affichage et d’omission actuelles, une logique de validation est également disponible.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version de prévisualisation : vendredi 13 mars 2025</li>
                <li>Version de production pour tous les clients : avec la version 25.4 (avril 2025)</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Expressions ajoutées aux champs calculés personnalisés</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Les expressions suivantes sont désormais disponibles dans les champs personnalisés calculés de Workfront : ARRAY, FORMAT, SWITCH, SORTASCARRAY, SORTDESCARRAY, ARRAYLENGTH, ARRAYELEMENT et ADDHOUR. Les définitions et des exemples de chaque expression sont disponibles dans l’éditeur de calcul et sur Experience League.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : samedi 31 janvier 2025</li>
                <span class="preview"><li>Version de production pour tous les clients : 31 janvier 2025</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Améliorations de la gestion des documents

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
<!--    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            New document approval decision buttons available in proofing viewer</a></p>
            <p>The new document approval decision buttons now appear in the proofing viewer. Now, when you create a simple proof and then add approvers and reviewers from the Document summary, they can make their decision directly inside the proofing viewer.</p>
        </td>
        <td>
            <p><b>Available on these dates:</b></p>
            <ul>
                <li>Preview release: April 9, 2025</li>
                <li>Production release for a limited set of customers: With the 25.4 release (April 2025)</li>
            </ul>
        </td>
    </tr>   -->                     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mise à jour de la visionneuse de relecture de bureau </a></p>[!BADGE In production &#x200B;]{type=Informative}
            <p>Le lecteur de vérification pour bureau a été mis à jour vers la version 2.1.45. Cette mise à jour permet à l’observateur d’utiliser les éléments suivants :
            <ul><li>Electron version 35</li><li>Chromium version 134</li><ul></p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version de prévisualisation : vendredi 20 mars 2025</li>
                <span class="preview"><li>Version de production pour tous les clients : 20 mars 2025</li></span>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Modifier plusieurs documents à la fois dans un rapport de document </a></p>[!BADGE In production &#x200B;]{type=Informative}
            <p>Vous pouvez désormais modifier plusieurs documents à la fois dans un rapport de document. Vous pouvez modifier les descriptions et mettre à jour les formulaires personnalisés.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 6 février 2025</li>
                <span class="preview"><li>Version de production pour tous les clients : 13 mars 2025</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Améliorations mobiles

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Améliorations apportées aux BAT dans l’application mobile (iOS uniquement)</a><p>[!BADGE In production &#x200B;]{type=Informative}</p></p>
            <p>Plusieurs améliorations sont disponibles pour la fonctionnalité BAT dans l’application mobile Adobe Workfront :
            <ul>
            <li>Vous pouvez désormais ouvrir un fichier BAT à partir de votre application de messagerie mobile, à partir d'un lien qui a été partagé avec vous. Auparavant, les liens provenant des e-mails n’étaient pas pris en charge et vous deviez accéder aux épreuves à partir de l’application mobile Workfront.</li>
            <li>Les fichiers d’épreuve multimédia sont désormais pris en charge dans l’application mobile.</li>
            </ul>
            </p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : S/O</li>
                <span class="preview"><li>Version de production pour tous les clients : 12 mars 2025</li> 
            </ul>
            <p><b>Disponible dans les environnements suivants :</b></p>
            <ul>
                <li>Application mobile iOS</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Améliorations apportées aux projets

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Ajoutez un commentaire aux projets lorsque vous les modifiez dans la zone Modifier le projet .</a><p>[!BADGE In production &#x200B;]{type=Informative}</p>
            <p>Vous pouvez maintenant ajouter un commentaire à un projet tel que vous l’avez modifié dans la zone Modifier le projet . Vous pouvez également ajouter un commentaire à plusieurs projets à la fois lors de leur modification en bloc. Avant cette mise à jour, cette fonctionnalité n’existait pas lors de la modification des projets.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 13 février 2025</li>
                <li>Production pour une version rapide : avec la version 25.3 (mars 2025)</li>
                <li>Version de production pour tous les clients : avec la version 25.4 (avril 2025)</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Améliorations des rapports

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Les données d’approbation de document et de décision sont désormais disponibles dans Data Connect</a><p>[!BADGE In production &#x200B;]{type=Informative}</p>
            <p>Vous pouvez désormais accéder aux données pour les approbations de documents et les décisions dans Data Connect. Ce jeu de données associe les approbations de documents aux fonctionnalités de relecture de Workfront et aux approbations Frame.io qui ont lieu sur les documents Workfront. Vous pourrez désormais illustrer la durée du cycle, le nombre de cycles et l’impact sur le calendrier pour les approbations tardives par le biais de vos visualisations BI.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version de prévisualisation : mercredi 25 mars 2025</li>
                <li>Version de production pour tous les clients : 25 mars 2025</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Mises à jour du calendrier Workfront</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p>
            <p>Nous avons mis à jour l’aspect du calendrier Workfront pour le rendre moderne et cohérent avec les autres aspects de Workfront. Il existe de petites différences de fonctionnalité par rapport au calendrier Workfront actuel, notamment :
            <ul>
            <li>Comment ajouter des éléments ad hoc au calendrier</li>
            <li>Comment créer et renommer le calendrier</li>
            <li>Les actions de calendrier ont été déplacées vers un menu Plus en regard du nom du calendrier</li>
            <li>Nouveau panneau latéral pour afficher les informations du calendrier</li>
            <li>Et plus encore</li>
            <ul>        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 27 février 2025</li>
                <li>Cette fonctionnalité sera mise en production dans le cadre d’un déploiement en trois phases : de la version 25.4 (10 avril 2025) au 17 avril 2024</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### Autres améliorations

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Effectuez la mise à niveau vers la nouvelle version d’abonnement aux événements avec les points d’entrée de mise à niveau de version</a></p>
            [!BADGE In production &#x200B;]{type=Informative}
            <p>Workfront dispose désormais de versions d’abonnements aux événements. La nouvelle version ne constitue pas une modification de l’API Workfront, mais plutôt une modification de la fonctionnalité d’abonnement aux événements. Vous pouvez passer vos abonnements aux événements à la nouvelle version sans créer d’écart dans votre abonnement aux événements</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <span class="preview"><li>Version de production pour tous les clients : 6 mars 2025</li></span>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Représenter les modifications utilisateur de Adobe Admin Console sous la forme « Système » dans le flux de mise à jour de Workfront</a></p><p>[!BADGE In production &#x200B;]{type=Informative}</p><p>Désormais, lorsque l’administrateur du Adobe Admin Console apporte une modification aux informations utilisateur d’un utilisateur Workfront, Workfront enregistre cette modification dans l’onglet Activité système de la zone Mises à jour de l’utilisateur comme appartenant au « Système ». Fait référence à l’administrateur Adobe Admin Console.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 23 janvier 2025</li>
                <li>Production pour une version rapide : avec la version 25.2 (13 février 2025)</li>
                <li>Version de production pour tous les clients : avec la version 25.4 (avril 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Mises à jour de l’apparence au cours du deuxième trimestre de 2025</a></p>
            <p>Des mises à jour mineures de l’aspect des différentes zones de l’application Adobe Workfront sont effectuées durant le deuxième trimestre 2025. Consultez les notes de mise à jour individuelles pour connaître les dates de publication spécifiques.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : pendant toute la durée de la version du deuxième trimestre 2025</li>
                <span class="preview"><li>Version de production : passez en revue les notes de mise à jour pour connaître les dates spécifiques.</li></span>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Fonctionnalités bientôt supprimées de Workfront

Les fonctionnalités suivantes seront bientôt supprimées de Workfront :

#### Dépréciation de l’API version 2-15

Alors que nous continuons à améliorer la plateforme Workfront, il est essentiel de maintenir nos API à jour. Cela garantit des performances et une sécurité optimales et prend en charge de nouvelles fonctionnalités. Par conséquent, nous rendons obsolètes les versions 2 à 15 de l’API Workfront.

* **Septembre 2025** : les versions 2 à 14 de l’API, qui ne sont actuellement pas prises en charge, seront obsolètes. Passée cette date, ces versions ne seront plus accessibles.
* **Décembre 2025** : l’API version 15 sera obsolète.

#### Nous supprimons l’ancienne vue Agile dans un projet

La vue Agile héritée dans un projet sera supprimée de Workfront avec la version 25.3 le 13 mars 2025. Vous pourrez toujours afficher vos tâches dans une vue Agile d’un projet en cliquant sur l’icône Panoramas. Les outils Agile hérités existants sont toujours disponibles dans la zone Équipes .

L’image ci-dessous montre l’option Agile héritée qui sera supprimée :
![lien de la vue Agile héritée](assets/project-agile-board-view.png)


#### Obsolescence d’Enhanced Analytics

En raison d’une utilisation faible et en diminution, nous avons pris la décision d’abandonner le produit Enhanced Analytics la semaine du 25 mai 2025.
Nous vous recommandons de considérer notre produit Data Connect comme un remplacement. Data Connect vous permet de créer des visualisations personnalisables similaires à l’aide de vos outils de Business Intelligence préférés.
Pour plus d’informations sur cette obsolescence, consultez le [guide d’obsolescence amélioré d’Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md).

## Annonces

### Modernisation des interfaces

Nous mettons à jour l’interface dans Adobe Workfront afin d’améliorer l’expérience utilisateur et de l’unifier avec d’autres applications Adobe. Ces modifications sont publiées en dehors du planning de publication standard. Pour obtenir la liste de ces modifications, voir [Modernisation des interfaces](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

### Améliorations de Workfront Fusion

>[!IMPORTANT]
>
>La documentation de Workfront Fusion a été déplacée vers un nouvel emplacement. Pour plus d’informations, d’instructions et de versions pour Fusion, consultez la [documentation de Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/home).
>
>Chaque article de documentation Fusion actuel contient un lien vers l’article correspondant dans le nouvel emplacement. Mettez à jour vos signets.
>
>Le jeu de documentation Fusion actuel n’est plus mis à jour et sera supprimé prochainement.

De nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à une cadence en dehors du calendrier de publication standard. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Améliorations apportées à Workfront Planning

De nouvelles fonctionnalités de Workfront Planning sont disponibles en production. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de la version du deuxième trimestre 2025 de la planification Adobe Workfront](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q2.md).

### Améliorations du planificateur de scénarios Workfront

Il n’y a pas de mise à jour du planificateur de scénarios à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de Workfront Proof

Il n’y a pas de mise à jour de Workfront Proof à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des Objectifs Workfront

Il n’y a pas de mise à jour des Objectifs Workfront à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Version 19 de l’API

Pour la version 19 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 19 de l’API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Pour plus d’informations sur les versions d’API actuellement prises en charge, consultez [Contrôle de version et planning de prise en charge des API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version du deuxième trimestre 2025, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/en/docs/workfront-known-issues/releases/current-updates).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/fr/docs/workfront-learn/tutorials-workfront/home).
