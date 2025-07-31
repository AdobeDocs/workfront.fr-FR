---
title: Vue d’ensemble de la version du quatrième trimestre 2025
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du quatrième trimestre 2025. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 298473d4-7d7d-4401-80bf-899a01f570a6
source-git-commit: eafc56adab1fad3bbc1a4f3dc8f61e599ab21f57
workflow-type: tm+mt
source-wordcount: '1190'
ht-degree: 23%

---

# Vue d’ensemble de la version du quatrième trimestre 2025

Cette page fournit des informations sur les fonctionnalités incluses dans la version du quatrième trimestre 2025 prévue pour octobre 2025.

Les améliorations apportées à cette page sont disponibles dans l’environnement de Prévisualisation. Cette page sera mise à jour avec des améliorations supplémentaires à mesure que la version du quatrième trimestre 2025 approche de sa date de sortie en production.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>25.8 (Août 2025)</li><li>25.9 (Septembre 2025)</li><li>25H10 (Octobre 2025)</li></ul> | <ul><li>25H10 (Octobre 2025)</li></ul> |
>
>Notez que pour la version finale de chaque trimestre (25.10 ce trimestre), les utilisateurs disposant du calendrier de publication rapide recevront la version un jour plus tôt que prévu.
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations des documents et des épreuves](#document-and-proofing-enhancements)
<!--* [Home enhancements](#home-enhancements)
* [Requests enhancements](#requests-enhancements)-->
* [Amélioration apportées à la gestion des ressources.](#resource-management-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations apportées aux administrateurs et administratrices

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Ajouter plusieurs options de valeur d’une API externe à un formulaire personnalisé</a><p></p>
            <p>Un nouveau type de champ, Recherche externe à sélection multiple, est désormais disponible dans le concepteur de formulaire personnalisé. Lorsque des données sont stockées sur un système externe, ce type de champ vous permet de charger des options à partir d’une API externe et de filtrer en fonction d’autres valeurs de champ du formulaire personnalisé. Il s’agit de la même chose qu’une recherche externe à sélection unique.</p>
            <p>Lorsque le formulaire est ajouté à un objet , les valeurs renvoyées par l’API apparaissent dans un champ déroulant et l’utilisateur peut sélectionner plusieurs valeurs.</p>
        </td>
        <td>vendredi 31 juillet 2025</td>
        <td>vendredi 14 août 2025</td>
        <td>vendredi 16 octobre 2025</td>
    </tr>     
  </tbody>
</table>


### Améliorations des documents et des épreuves

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}">Nouvelle intégration de vérification pour Adobe Express</a><p></p>
            <p>Nous sommes ravis d’annoncer une nouvelle intégration entre Adobe Express et Workfront Proof.</p>
            <ul>
            <li>Rationalisez la collaboration entre les équipes créatives, juridiques et de conformité afin de réduire le temps de publication tout en maintenant la surveillance</li>
            <li>Effectuez des révisions approfondies à l’aide des balises de dessin, des annotations et des commentaires avec la visionneuse de relecture Workfront.</li>
            <li>Respectez les normes de conformité d’entreprise avec des signatures électroniques et des journaux d’audit complets</li>
            <li>Demander l'approbation sur tous les fichiers remixés à partir d'un modèle de marque Express</li>
            <li>Mappez un modèle Express à un workflow de révision et d’approbation à plusieurs étapes à l’aide de modèles de BAT avancés</li>
            </ul>
        </td>
        <td>mardi 28 juillet 2025</td>
        <td>mardi 28 juillet 2025</td>
        <td>mardi 28 juillet 2025</td>
    </tr>     
  </tbody>
</table>

<!--### Home enhancements

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-home.md" class="MCXref xref" xrefformat="{para}">Updates to the My Requests widget in Home</a><p></p>
            <p>To create a more seamless experience between Workfront and Workfront Planning, we've redesigned the My Requests widget in Home. The new widget features the following changes:
            <ul>
                <li>Improved layout and organization of request information</li>
                <li>Enhanced filtering and sorting options</li>
                <li>Integration with Workfront Planning for better visibility into resource allocation</li>
            </ul>
            </p>
        </td>
        <td>July 31, 2025</td>
        <td>August 14, 2025</td>
        <td>October 16, 2025</td>
    </tr>     
  </tbody>
</table> 

### Requests enhancements

<table style="table-layout:auto">
  <tbody>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}">Updates to Requesting experience</a><p></p>
            <p>To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:
            <ul>
                <li>View Workfront and Workfront Planning requests in a single list.</li>
                <li>Filter submitted requests based on criteria you specify.</li>
                <li>Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.</li>
                <li>Hide and reorder columns in the submitted requests list.</li>
            </ul>
            </p>
        </td>
        <td>July 31, 2025</td>
        <td>August 14, 2025</td>
        <td>October 16, 2025</td>
    </tr>     
  </tbody>
</table> -->

### Amélioration apportées à la gestion des ressources.

<table style="table-layout:auto">
  <tbody>
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}">L’équilibreur de charge de travail est désormais disponible sur votre profil utilisateur</a><p></p>
            <p>Tous les utilisateurs peuvent désormais afficher leurs propres données de demande et de capacité dans l’équilibreur de charge de travail à partir de leur profil, quel que soit leur niveau d’accès. Lorsque vous accédez à votre profil utilisateur Workfront, l’équilibreur de charge de travail s’affiche dans le panneau de navigation de gauche.</p>
            <p>Les données de l’équilibreur de charge de travail d’un utilisateur sont en lecture seule. Vous ne pouvez pas affecter de travail, annuler l’affectation d’un travail ou ajuster les allocations au niveau de l’utilisateur.</p>
        </td>
        <td>vendredi 31 juillet 2025</td>
        <td>vendredi 14 août 2025</td>
        <td>vendredi 16 octobre 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}">Les affectations de rôles s’affichent dans la </a> de l’équilibreur de charge de travail<p></p>
            <p>Les gestionnaires de ressources peuvent désormais consulter les affectations de fonction dans l’équilibreur de charge de travail. Les affectations s'affichent dans la zone Tâches non affectées, sous les tâches ou événements auxquels les rôles sont affectés. Seules les tâches affectées aux utilisateurs s’affichent dans la zone Tâches affectées . </p>
            <p>Un nouveau paramètre de l’équilibreur de charge de travail, Afficher les affectations de rôles, détermine si les affectations de rôles s’affichent. Le paramètre est activé par défaut.</p>
        </td>
        <td>vendredi 31 juillet 2025</td>
        <td>vendredi 14 août 2025</td>
        <td>vendredi 16 octobre 2025</td>
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
                        <p><span class="bold">Fonctionnalité</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Dates de publication</span>
                        </p>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Mises à jour techniques au cours du quatrième trimestre de 2025</a></p>
                        <p>Des mises à jour mineures de l’aspect de diverses zones de l’application Adobe Workfront sont apportées dans le délai imparti pour la publication de la version du quatrième trimestre 2025. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : tout au long du calendrier de publication du quatrième trimestre de 2025<br /></p>
                            </li>
                            <li>
                                <p>Version de production : au moins 2 semaines après la publication dans l’environnement de prévisualisation (sauf indication contraire)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

<!--
### Functionality soon to be removed from Workfront

* 
-->

## Modernisation des interfaces

Nous mettons à jour l’interface dans Adobe Workfront afin d’améliorer l’expérience utilisateur et de l’unifier avec d’autres applications Adobe. Ces modifications sont publiées en dehors du planning de publication standard. Pour obtenir la liste de ces modifications, voir [Modernisation des interfaces](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Notes de mise à jour pour d’autres zones

### Améliorations de Workfront Fusion

De nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à une cadence en dehors du calendrier de publication standard. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Améliorations apportées à Workfront Planning

De nouvelles fonctionnalités de Workfront Planning sont disponibles en production. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de la version du quatrième trimestre 2025 pour Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q4.md).

Il n’existe aucune mise à jour pour les éléments suivants à ce stade de la version :

* Planificateur de scénarios
* Épreuve
* Objectifs

## Mises à jour du lecteur de vérification pour bureau

### Version 2.1.52

**Version de production pour tous les clients : 31 juillet 2025**

Le lecteur de vérification pour bureau a été mis à jour vers la version 2.1.52, qui corrige les bugs.

La mise à jour 2.1.51 incluait des mises à jour d’outils internes et n’avait aucune incidence sur les fonctionnalités de l’utilisateur final.

Cette mise à jour concerne Mac et Windows.

## Annonces

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

### Version 20 de l’API

L’API Workfront version 20 a été publiée le 4 mai 2025. Pour la version 20 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 20 de l’API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions et de la prise en charge de l’API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version du premier trimestre 2025, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).
