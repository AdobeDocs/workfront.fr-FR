---
title: Vue d’ensemble de la version du quatrième trimestre 2024
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du quatrième trimestre 2024. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '2187'
ht-degree: 39%

---

# Vue d’ensemble de la version du quatrième trimestre 2024

Cette page fournit des informations sur les fonctionnalités incluses dans la version du quatrième trimestre 2024. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.

<span class="preview">Les fonctionnalités hors cycle (celles qui sont publiées en production avant la date de publication du quatrième trimestre 2024) sont surlignées en jaune.</span>

>[!IMPORTANT]
>
>La version 23.3 incluait l’option permettant d’opter pour des versions mensuelles dans votre organisation. Par conséquent, Workfront a modifié le schéma de numérotation des versions afin de tenir compte des suivis de versions mensuels et trimestriels. Le premier chiffre désigne l’année, le second le mois de la version. Exemple : la version d’avril 2024 est 24.4.
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>24.8 (15 août 2024)</li><li>24.9 (12 septembre 2024)</li><li>24.10 (17 octobre 2024)</li></ul> | <ul><li>24.10 (17 octobre 2024)</li></ul> |
>
>Notez que pour la version finale de chaque trimestre (24.10 ce trimestre), les utilisateurs de la version rapide recevront la version un jour plus tôt.
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations de la gestion des documents](#document-management-enhancements)
* [Amélioration de l’accueil](#home-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations apportées aux projets](#project-enhancements)
* [Améliorations apportées à la relecture](#proofing-enhancements)
* [Améliorations des rapports et tableaux de bord](#report-and-dashboard-enhancements)
* [Autres améliorations](#other-enhancements)
* [Fonctionnalités bientôt supprimées de Workfront](#functionality-soon-to-be-removed-from-workfront)

### Améliorations apportées aux administrateurs et administratrices

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Niveau d’accès désormais disponible dans la promotion de l’environnement</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Pour étendre les fonctionnalités de promotion de l’environnement, nous avons ajouté la possibilité d’inclure des niveaux d’accès. Vous pouvez maintenant configurer un niveau d’accès dans un environnement Sandbox, puis le promouvoir dans votre environnement de production.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version préliminaire : vendredi 17 octobre 2024</p>
                        </li>
                        <li>
                            <p>Version de production pour tous les clients : avec la version 24.10 (17 octobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Un compteur sur les formulaires personnalisés affiche le nombre de champs</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Les formulaires personnalisés sont limités à 500 champs. Sur un formulaire long, il peut être difficile de connaître le nombre de champs du formulaire et de savoir si vous approchez de la limite. Un compteur a été ajouté aux formulaires personnalisés en bas à gauche. Le compteur affiche le nombre de champs utilisés dans le formulaire et il est toujours visible lorsque vous faites défiler le concepteur de formulaires.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version préliminaire : mercredi 1 octobre 2024</p>
                        </li>
                        <li>
                            <p>Version de production pour tous les clients : avec la version 24.10 (17 octobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}"> Une option "Tout sélectionner" est désormais disponible dans les modèles de mise en page</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Pour afficher et masquer plus facilement des champs avec des modèles de mise en page, une case à cocher "Tout sélectionner" a été ajoutée aux zones Aperçu et Finance de la vue Détails dans un modèle de mise en page. Cette option est disponible lorsque vous avez sélectionné Projet, Tâche, Problème, Portfolio ou Programme sous "Personnaliser ce que voient les utilisateurs".</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version d’aperçu : 29 août 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Version de production pour tous les clients : 29 août 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Restauration des packages de promotion d’environnement</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Pour rendre la promotion de l’environnement plus flexible et plus facile à utiliser, nous avons activé la fonctionnalité de restauration. Vous pouvez désormais restaurer les packages en moins de 24 heures, ce qui vous permet de restaurer plus facilement les configurations précédentes qui ont été affectées par un package de promotion d’environnement.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version d’aperçu : 29 août 2024</p>
                        </li>
                        <li>
                            <p>Production pour une version rapide : avec la version 24.9 (12 septembre 2024)</p>
                        </li>
                        <li>
                            <p>Version de production pour tous les clients : avec la version 24.10 (17 octobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Le bouton Disposition sur le concepteur de formulaire personnalisé accepte deux ou trois colonnes</a></p>
                    <p>Un bouton "Disposition" sur le concepteur de formulaire personnalisé vous permet de choisir parmi une zone de travail de deux ou trois colonnes. Le concepteur de formulaire d’origine utilise trois colonnes et les paramètres de champ s’affichent dans la colonne à l’extrême droite. Si vous sélectionnez deux colonnes, les paramètres du champ s’affichent en regard de la bibliothèque de champs dans la colonne située à l’extrême gauche.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p><s>Version d’aperçu : 12 août 2024</s></p>
                        </li>
                        <li>
                            <p>Production pour la version rapide : S.O.</p>
                        </li>
                        <li>
                            <p>Version de production pour tous les clients et toutes les clientes : S/O</p>
                        </li>
                    </ul>
                    <p><i>Cette fonctionnalité a été supprimée de l’aperçu et ne sera pas publiée avec les prochaines versions.</i></p>
                </td>
            </tr>
        </tbody>
</table>

### Améliorations de la gestion des documents

>[!IMPORTANT]
>
>Les fonctionnalités répertoriées dans **Améliorations de la gestion des documents** font partie d’une version par étapes et ne sont disponibles que pour des clientes et clients spécifiques.

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md">Afficher l’état de décision du document directement dans la liste de documents</a></p>
                    <p>Vous pouvez désormais afficher l’état de décision d’un document directement dans la liste des documents.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p><s>Version préliminaire : vendredi 3 octobre 2024</s></p>
                        </li>
                        <li>
                            <p>Version de production pour tous les clients : avec la version 24.10 (17 octobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-document-mgmt-enhancements.md"> Ajoutez rapidement les réviseurs et les approbateurs précédents aux nouvelles versions de document </a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Vous pouvez désormais ajouter rapidement des réviseurs et des approbateurs à partir des versions précédentes du document.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version préliminaire : vendredi 3 octobre 2024</p>
                        </li>
                        <li>
                            <p>Version de production pour tous les clients : avec la version 24.10 (17 octobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Amélioration de l’accueil

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Mises à jour du widget J’attends mon approbation dans la nouvelle page d’accueil</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Nous avons apporté les modifications suivantes au widget En attente de mon approbation :</p>
                        <ul>
                            <li>Le widget a été renommé : le nom de ce widget est désormais Mes approbations.</li>
                            <li>Ajout de l’option de filtrage Validations que j’ai envoyées : vous pouvez désormais afficher les validations que vous avez soumises dans le nouveau Accueil avec ce widget.</li>
                            <li>Date limite : vous pouvez maintenant voir la date limite du BAT si elle a été définie. Si aucun délai n’est défini, la date limite est définie par défaut sur la date de création.</li>
                        </ul>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version préliminaire : vendredi 10 octobre 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Version de production pour tous les clients : 10 octobre 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-home-enhancements.md">Présentation des priorités : expérience Workfront simple, simple et intuitive pour les propriétaires de tâches</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Les priorités améliorent la concentration et la productivité afin d’aider les clients à accomplir plus en moins de temps.</p>
                    <p>Grâce aux priorités, vous pouvez profiter des avantages suivants :</p>
                        <ul>
                            <li>Gérer et classer par priorité les tâches quotidiennes : organisez votre journée ou votre semaine avec une navigation consolidée pour une meilleure clarté.</li>
                            <li>Plus grande productivité : accédez au contexte du projet et effectuez les tâches plus rapidement avec moins de clics.</li>
                            <li>Fonctionnalités personnalisées : profitez de fonctionnalités conçues de manière unique pour les propriétaires de tâches.</li>
                        </ul>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version préliminaire : vendredi 3 octobre 2024</p>
                        </li>
                        <li>
                            <p>Version de production pour tous les clients : avec la version 24.10 (17 octobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Améliorations de l’intégration

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations de l’expérience de connexion à l’intégration Outlook</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>L’expérience de connexion à l’intégration d’Outlook a été rationalisée afin que tous les clients voient le même bouton pour se connecter à Workfront qu’ils soient activés ou non sur IMS. Les étapes de connexion suivantes restent différentes pour les instances IMS et non IMS, mais la page initiale est la même pour tous les utilisateurs.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version d’aperçu : 6 août 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Version de production pour tous les clients : 6 août 2024</span></p>
                        </li>
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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affectations plus pertinentes ajoutées au workflow Nouvelle tâche</a></p>
                    [!BADGE In production for Fast Release ]{type=Positive}
                    <p>Nous avons ajouté la même fonctionnalité pour des affectations intelligentes plus pertinentes au champ Affectations dans la zone Nouvelle tâche lors de l’ajout d’une tâche à un projet et dans une liste de tâches de projet.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version d’aperçu : 13 février 2024</p>
                        </li>
                        <li>
                            <p>Production pour une version rapide : avec la version 24.5 (16 mai 2024)</p>
                        </li>
                        <li>
                            <p>Mise à jour de production pour tous les clients : à annoncer</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affectations intelligentes plus pertinentes</a></p>
                    [!BADGE In production for Fast Release ]{type=Positive}
                    <p>Nous avons modifié l’algorithme utilisé par Workfront pour calculer et suggérer des affectations intelligentes pour les tâches. Le nouvel algorithme s’applique aux zones suivantes de Workfront où vous affectez une tâche : listes de tâches, zone Affectations dans l’en-tête de la tâche, Accueil et panneau Résumé.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version de prévisualisation : 21 décembre 2023</p>
                        </li>
                        <li>
                            <p>Production pour une version rapide : avec la version 24.5 (16 mai 2024)</p>
                        </li>
                        <li>
                            <p>Mise à jour de production pour tous les clients : à annoncer</p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Améliorations apportées à la relecture

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Correctif du problème de copier/coller pour la visionneuse de vérification de l’appli de bureau</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Correction d’un problème en raison duquel le contenu se collait incorrectement dans la section Mises à jour de la visionneuse de vérification de l’appli de bureau.</p>
                    <p>Nouvelle version : 2.1.39</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version préliminaire : jeudi 2 octobre 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Version de production pour tous les clients : 2 octobre 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Correctif vierge pour les utilisateurs Windows de la visionneuse de vérification de l’appli de bureau</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Correction d’un problème lié à la nouvelle version 2.1.36 de la visionneuse de vérification de l’appli de bureau, en raison duquel certains utilisateurs de Windows voyaient un écran vide après l’ouverture de la visionneuse. </p>
                    <p>Nouvelle version pour les utilisateurs de Windows : 2.1.37</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version d’aperçu : 30 août 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Version de production pour tous les clients : 30 août 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Mise à jour Chromium pour la visionneuse de vérification de l’appli de bureau</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Nous mettons à niveau la visionneuse de vérification de l’appli de bureau afin qu’elle prenne en charge Chromium 126.0.6478.127, ce qui résoudra les problèmes liés aux éléments de l’interface utilisateur dans les bons à tirer interactifs.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version d’aperçu : 29 août 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Version de production pour tous les clients : 29 août 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

### Améliorations des rapports et tableaux de bord

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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Data Connect disponible pour les nouveaux plans</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Workfront Data Connect sera disponible pour les organisations qui ont souscrit à l’un des nouveaux plans Workfront. Data Connect permet aux entreprises d’accéder à leurs données sous la forme d’un lac de données sécurisé et évolutif, qui peut être analysé et visualisé à l’aide d’outils de Business Intelligence ou stocké en externe. En outre, les entreprises peuvent utiliser Data Connect pour afficher les analyses de données qui n’étaient pas disponibles auparavant, telles que l’analyse des tendances temporelles, le mappage des variables et l’analyse des données système externes en combinaison avec les données Workfront.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version de production pour tous les clients : avec la version 24.10 (17 octobre 2024)</p>
                        </li>
                    </ul>
                    <p><i>Disponible uniquement pour les organisations sur l’un des nouveaux plans Adobe Workfront. Data Connect fait partie du plan Ultimate et sera disponible à l’achat en tant que complément des plans Prime et Select au cours du premier semestre 2025.</i></p>
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
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Résumer les projets ou les mises à jour en un seul clic</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Afin de faciliter l’affichage rapide des mises en surbrillance d’un projet ou d’un flux de mise à jour, nous avons ajouté des boutons Résumer à ces zones de Workfront. Vous pouvez maintenant cliquer sur le bouton pour générer un résumé dans l’assistant d’IA.</p><p>Auparavant, les utilisateurs pouvaient ouvrir l’assistant d’IA et saisir une invite pour créer un résumé du projet ou mettre à jour le flux.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version préliminaire : vendredi 3 octobre 2024</p>
                        </li>
                        <li>
                            <p>Version de production pour tous les clients : avec la version 24.10 (17 octobre 2024)</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md" class="MCXref xref" xrefformat="{para}"> Disponibilité générale de la planification Adobe Workfront </a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Workfront Planning est disponible pour tous les clients qui ont acheté une licence Workfront Planning, en plus de leur licence Workfront. Pour plus d’informations sur la planification Workfront, contactez le représentant du compte.</p>
                    <p>Pour obtenir les dernières informations sur la version de Workfront Planning chaque trimestre, reportez-vous à la section <a href="#workfront-planning-enhancements">Améliorations de la planification Workfront</a> ci-dessous.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p><span class="preview">Version de production pour tous les clients : 28 août 2024</span></p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Assistant d’Adobe d’IA disponible dans Workfront</a></p>
                    [!BADGE In production ]{type=Informative}
                    <p>Afin de vous faciliter la tâche, nous avons ajouté l’assistant AI d’Adobe à Workfront. L’assistant IA peut vous aider en procédant comme suit :</p>
                    <ul>
                        <li>Résumer les éléments de travail et les documents, ce qui vous permet d’acquérir rapidement une compréhension générale des tâches, des projets et des ressources.</li>
                        <li>Fournissant des informations à partir de la documentation Experience League, en apportant des instructions et du matériel de référence dans Workfront, tout en liant à une documentation plus détaillée.</li>
                        <li>Créer et affiner des formules pour des champs de formulaire personnalisés calculés, générer des formules à partir d’invites de texte ou rechercher des erreurs dans des formules existantes.</li>
                        </ul>
                        <p>Votre administrateur Workfront peut activer ou désactiver l’assistant d’IA pour votre entreprise. L’assistant d’IA est disponible pour les instances avec des plans Select, Prime et Ultimate.</p>
                    </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version d’aperçu : 28 août 2024</p>
                        </li>
                        <li>
                            <p class="preview">Version de production : 28 août 2024</p>
                        </li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>
                    <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Mise à jour de l’apparence et de la convivialité au cours du quatrième trimestre 2024</a></p>
                    <p>Des mises à jour mineures de l’aspect et de la convivialité de différentes parties de l’application Adobe Workfront seront réalisées au cours du quatrième trimestre 2024. Consultez les notes de mise à jour individuelles pour connaître les dates de publication spécifiques.</p>
                </td>
                <td><p><b>Disponible à ces dates :</b></p>
                    <ul>
                        <li>
                            <p>Version préliminaire : tout au long de la période de publication du quatrième trimestre 2024</p>
                        </li>
                        <li>
                            <p><span class="preview">Version de production : passez en revue les notes de mise à jour pour connaître les dates spécifiques.</span></p>
                        </li>
                    </ul>
                </td>
            </tr>                            
        </tbody>
</table>

### Fonctionnalités bientôt supprimées de Workfront

Les fonctionnalités suivantes seront bientôt supprimées de Workfront :

#### Obsolescence de l’expérience d’accueil héritée avec la version 24.10

Nous abandonnerons officiellement l’expérience héritée d’accueil avec la version 24.10. Nous vous recommandons de commencer à utiliser la nouvelle page d’accueil, qui continuera à être enrichie de fonctionnalités supplémentaires avant l’obsolescence.

## Annonces

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à une cadence autre que le calendrier des versions du quatrième trimestre 2024. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Améliorations de la planification Workfront

De nouvelles fonctionnalités de la planification Workfront sont disponibles dans la production. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de mise à jour du quatrième trimestre 2024 d’Adobe Workfront Planning](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-24-q4.md).

### Améliorations du planificateur de scénarios Workfront

Il n’y a pas de mise à jour du planificateur de scénarios à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de Workfront Proof

Il n’y a pas de mise à jour de Workfront Proof à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des Objectifs Workfront

Il n’y a pas de mise à jour des Objectifs Workfront à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Version 19 de l’API

Pour la version 19 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 19 de l’API](/help/quicksilver/wf-api/api/new-api-version-19.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions et de la prise en charge de l’API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version du quatrième trimestre 2024, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).
