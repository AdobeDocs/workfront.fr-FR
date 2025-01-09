---
title: Vue d’ensemble de la version du premier trimestre 2025
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du premier trimestre 2025. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: d2e3379e9390f2b419bb2d78b1999c8c2dd7d0d3
workflow-type: tm+mt
source-wordcount: '2527'
ht-degree: 30%

---

# Vue d’ensemble de la version du premier trimestre 2025

Cette page fournit des informations sur les fonctionnalités incluses dans la version du premier trimestre 2025. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.

<span class="preview">Les fonctionnalités hors cycle (celles dont la mise en production est antérieure à la date de diffusion du premier trimestre 2025) sont surlignées en jaune.</span>

>[!IMPORTANT]
>
>La version 23.3 incluait l’option permettant d’opter pour des versions mensuelles dans votre organisation. Par conséquent, Workfront a modifié le schéma de numérotation des versions afin de tenir compte des suivis de versions mensuels et trimestriels. Le premier chiffre désigne l’année, le second le mois de la version. Exemple : la version d’avril 2025 est 25.4.
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>Version 24.11 (14 Novembre 2024)</li><li>Version 24.12 (12 Décembre 2024)</li><li>25.1 (15 janvier 2025)</li></ul> | <ul><li>25.1 (16 janvier 2025)</li></ul> |
>
>Notez que pour la version finale de chaque trimestre (25.1 ce trimestre), les utilisateurs disposant du planning de version rapide recevront la version un jour plus tôt que prévu.
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations des panoramas](#boards-enhancements)
* [Améliorations de la gestion des documents](#document-management-enhancements)
* [Amélioration de l’accueil](#home-enhancements)
* [Améliorations apportées aux projets](#project-enhancements)
* [Améliorations apportées à la relecture](#proofing-enhancements)
* [Améliorations des rapports et des tableaux de bord](#report-and-dashboard-enhancements)
* [Améliorations du flux de mise à jour](#update-stream-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations apportées aux administrateurs et administratrices

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Fonctionnalité</span></p>
        </td>
        <td>
            <p><span class="bold">Dates de publication</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           Comparaison d’objets entre des environnements pour la promotion de l’environnement</a></p>
            <p>Pour faciliter la détermination de l’objet à inclure dans un package de promotion d’environnement, nous avons ajouté la possibilité de comparer des objets entre les environnements. Vous pouvez ensuite ajouter des objets à un package directement à partir de cette comparaison.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : 5 janvier 2023</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Plus d’objets disponibles pour la promotion de l’environnement</a></p>
            <p>Nous avons ajouté d'autres objets pour étendre les fonctionnalités de promotion d'environnement.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : 5 janvier 2023</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (janvier 2025)</li>
            </ul>
        </td>
    </tr>  
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Empêcher le déplacement de tâches en cas d'heures consignées</a></p>
            <p>Comme le déplacement de tâches ou d’événements pour lesquels des heures ont été consignées peut parfois entraîner des problèmes de conformité ou d’audit, nous avons ajouté une préférence dans les Préférences des tâches et des événements de la Configuration qui vous permet d’empêcher les utilisateurs de déplacer des tâches et des événements si des heures y sont consignées.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 19 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Préférence pour l'utilisation des prévisions de projet ou d'utilisateur pour les tâches à affectation unique</a></p>
            [!BADGE In production for Fast Release ]{type=Positive}
            <p>En tant qu’administrateur système ou de groupe, vous disposez désormais d’une nouvelle préférence qui permet d’indiquer si Workfront doit utiliser le planning du projet ou de l’utilisateur pour calculer la chronologie du projet lorsque vous affectez un utilisateur à une tâche et que le projet et l’utilisateur sont tous deux associés à un planning.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 21 novembre 2024</li>
                <li>Production pour une version rapide : avec la version 24.12 (12 décembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Les règles métier prennent désormais en charge les liens hypertexte</a></p>
            [!BADGE In production for Fast Release ]{type=Positive}
            <p>Vous pouvez désormais inclure des liens hypertexte dans le message d’erreur personnalisé d’une règle métier, afin de guider l’utilisateur ou l’utilisatrice sur la manière de modifier son action dans la contrainte de la règle. L’URL statique peut renvoyer vers la documentation ou d’autres pages utiles à l’utilisateur ou à l’utilisatrice.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 21 novembre 2024</li>
                <li>Production pour une version rapide : avec la version 24.12 (12 décembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Le filtrage sur les champs de saisie semi-automatique natifs est désormais disponible</a></p>
            <p>Lorsque vous ajoutez une référence de champ native à un formulaire personnalisé et qu’elle fait référence à un champ de saisie semi-automatique (par exemple, Portfolio, Société ou Propriétaire), une option de filtrage est désormais disponible. Le filtre vous permet de limiter les objets que les utilisateurs peuvent choisir lorsqu’ils utilisent le champ . Ce filtre personnalisé fonctionne de la même manière qu’un filtre sur un champ de saisie semi-automatique personnalisé, en utilisant le mode texte pour définir le filtre.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 21 novembre 2024</li>
                <li>Production pour une version rapide : avec la version 24.12 (12 décembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Icône « Déplacer vers » ajoutée aux champs personnalisés</a></p>
            [!BADGE In production for Fast Release ]{type=Positive}
            <p>Lorsqu’un formulaire personnalisé contient plusieurs sections avec de nombreux champs, il peut être difficile de déplacer un champ d’une section à une autre en effectuant un glisser-déposer. Une icône « Déplacer vers » a été ajoutée à chaque champ, vous permettant de sélectionner la section dans laquelle le champ est placé.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : mercredi 29 octobre 2024</li>
                <li>Production pour une version rapide : avec la version 24.11 (14 novembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Améliorations des panoramas

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Fonctionnalité</span></p>
        </td>
        <td>
            <p><span class="bold">Dates de publication</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Modification du propriétaire d’un panorama</a></p>
            <p>Le créateur d’un panorama en est le propriétaire par défaut. Le propriétaire du panorama est la seule personne qui peut supprimer ce panorama ou mettre à jour ses filtres dans le panneau Configurer.</p>
            <p>Une fonctionnalité a été ajoutée pour permettre aux administrateurs système de Workfront de changer le propriétaire d’un panorama. Le propriétaire actuel d’un panorama peut également changer le propriétaire de ce panorama spécifique. Cette fonctionnalité est disponible sur les tableaux de base, rétrospectifs et kanban, mais pas sur les tableaux dynamiques.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : jeudi 18 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
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
    <tr>
        <td>
            <p><span class="bold">Fonctionnalité</span></p>
        </td>
        <td>
            <p><span class="bold">Dates de publication</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Modifier plusieurs documents à la fois</a></p>
            [!BADGE In production for Fast Release ]{type=Positive}
            <p>Vous pouvez désormais modifier plusieurs documents à la fois. Vous pouvez modifier les descriptions et mettre à jour les formulaires personnalisés.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 21 novembre 2024</li>
                <li>Production pour une version rapide : avec la version 24.12 (12 décembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nouveau statut Retiré disponible pour les approbations de version de document</a></p>
            [!BADGE In production for Fast Release ]{type=Positive}
            <p>Lorsqu'une nouvelle version est ajoutée à un document avec des approbations en attente, l'approbation de la version précédente s'affiche désormais comme « Retirée », ce qui indique que le processus d'approbation préalable est terminé en raison de l'ajout de la nouvelle version.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 7 novembre 2024</li>
                <li>Production pour une version rapide : avec la version 24.11 (14 novembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
            <p><i>Cette fonctionnalité fait partie d’une mise à jour par phases et n’est disponible que pour des clients spécifiques.</i></p>
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
            <p><span class="bold">Fonctionnalité</span></p>
        </td>
        <td>
            <p><span class="bold">Dates de publication</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Utiliser des filtres intelligents pour rechercher votre travail dans les priorités</a></p>
            <p>Utilisez le langage naturel pour filtrer rapidement le travail dans la liste de travail Priorités. Vous pouvez saisir des éléments tels que : </p>
            <ul>
                <li>Afficher les tâches en retard</li>
                <li>Me montrer les tâches dues cette semaine</li>
                <li>Afficher les principales priorités</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 9 janvier 2025</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Rattrapage du travail dans les priorités</a></p>
            <p>Vous pouvez utiliser l'option Rattraper mon retard pour réduire le temps consacré à la recherche d'informations sur les projets actifs.</p>
            <p>Optimisé par l’assistant d’IA de Workfront, Catch me up résume les mises à jour, les documents chargés et d’autres modifications notables concernant vos projets dans les délais suivants : 24 heures, 3 jours ou 7 jours.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : samedi 20 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Affichez les modifications en direct sur la page Détails dans Priorités</a></p>
            <p>Vous pouvez désormais afficher des mises à jour en temps réel sur la page Détails d’une tâche ou d’un événement. Vous pouvez également voir si d’autres personnes consultent la page en même temps que vous avec des indicateurs de présence en temps réel.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 19 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Charger et afficher des documents et des épreuves dans Priorités</a></p>
            <p>Vous pouvez désormais interagir avec des documents et des BAT pour les tâches et les événements dans la liste de travail et le calendrier. Dans le nouvel onglet Documents, vous pouvez :</p>
            <ul>
                <li>charger un document ;</li>
                <li>Créer une épreuve</li>
                <li>Lancer la visionneuse de relecture</li>
                <li>Et plus encore</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 19 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            La vue Calendrier est désormais disponible dans Priorités</a></p>
            <p>Vous pouvez suivre votre travail à l’aide d’un calendrier mensuel visuel clair. Avec le calendrier Priorités, vous pouvez :</p>
            <ul>
                <li>Utiliser des filtres pour trouver votre travail</li>
                <li>Appliquer des champs personnalisés tels que le statut et le niveau de focus pour identifier le travail hautement prioritaire</li>
                <li>Appliquer des couleurs pour une organisation rapide</li>
                <li>Et plus encore</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 19 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mises à jour de la liste de travail des priorités</a></p>
            <p>Nous avons mis à jour la liste de travail des priorités afin d'améliorer les capacités et de nous aligner sur d'autres aspects de l'application.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 12 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Accédez à la page Détails d’un projet à partir des priorités</a></p>
            <p>Vous pouvez désormais accéder directement à un projet dans Workfront à partir de la liste de travail Priorités .</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 5 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mise à jour des options de la colonne Mon focus dans Priorités</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Nous avons mis à jour les options de la colonne Mon focus pour vous aider à hiérarchiser et à trier votre travail de manière plus intuitive. Les nouveaux libellés sont les suivants :</p>
            <ul>
                <li>Urgent</li>
                <li>Élevé</li>
                <li>Normal</li>
                <li>Faible</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 14 novembre 2024</li>
                <li><span class="preview">Version de production pour tous les clients : 14 novembre 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Afficher les détails du projet dans Priorités</a></p>
            [!BADGE In production for Fast Release ]{type=Positive}
            <p>Vous pouvez désormais afficher les détails et les commentaires du projet à partir de la liste de travail dans Priorités.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : jeudi 6 novembre 2024</li>
                <li>Production pour une version rapide : avec la version 24.11 (14 novembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
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
            <p><span class="bold">Fonctionnalité</span></p>
        </td>
        <td>
            <p><span class="bold">Dates de publication</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Affectations plus pertinentes supprimées de la Prévisualisation et de la Production pour les environnements de version rapide</a></p>
            <p>Une fonctionnalité présente dans l’environnement de Prévisualisation depuis décembre 2023 et dans l’environnement de Production à version rapide depuis mars 2024 a été supprimée. Les fonctionnalités ont ajouté des suggestions d’affectations intelligentes plus pertinentes lors de l’affectation de tâches.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 19 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
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
            <p><span class="bold">Fonctionnalité</span></p>
        </td>
        <td>
            <p><span class="bold">Dates de publication</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Nouvelle extension de navigateur pour la révision interactive disponible en version bêta</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Nous introduisons une nouvelle extension de navigateur, l’outil de révision Adobe Workfront, qui remplace l’ancienne extension de navigateur pour la révision du contenu ZIP interactif. Le nouvel outil de révision Adobe Workfront prend en charge la révision du contenu ZIP dans tous les navigateurs courants.</p>
            <p>L’ancienne extension de navigateur sera supprimée le 28 février 2025.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 7 novembre 2024</li>
                <li><span class="preview">Version de production pour tous les clients : 7 novembre 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Améliorations des rapports et des tableaux de bord

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Fonctionnalité</span></p>
        </td>
        <td>
            <p><span class="bold">Dates de publication</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Limite de 25 rapports, pages externes ou calendriers dans les tableaux de bord</a></p>
            <p>Pour maintenir les performances des tableaux de bord, nous avons implémenté une limite au nombre total de rapports, de pages externes ou de calendriers pouvant être placés dans un tableau de bord. Lors de la création d’un tableau de bord, 25 éléments au maximum peuvent être ajoutés.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : mardi 16 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Bouton de création d’un compte de lecteur pour la première fois pour Data Connect</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Les administrateurs qui accèdent pour la première fois à Data Connect ont désormais la possibilité de créer un compte de lecteur de Snowflake en cliquant sur un seul bouton. Le processus prend quelques minutes, mais ne nécessite aucune autre action.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 14 novembre 2024</li>
                <li><span class="preview">Version de production pour tous les clients : 14 novembre 2024</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### Améliorations du flux de mise à jour

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">Fonctionnalité</span></p>
        </td>
        <td>
            <p><span class="bold">Dates de publication</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mise à jour de l’expérience de commentaire dans le widget Mentions sur l’Accueil et dans Mes mises à jour</a></p>
            <p>Nous mettons à jour l’expérience de commentaires dans le widget Mentions de l’Accueil et dans la section Mentions de la zone Mes mises à jour . Désormais, la même expérience dans la zone Mises à jour de la plupart des objets Workfront est également disponible dans le widget Mentions et dans la section Mentions de Mes mises à jour.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 19 décembre 2024</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
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
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Mise à jour sur la gestion des ressources déplacées ou supprimées dans les dossiers liés</a></p>
            [!BADGE In production ]{type=Informative}
            <p>Nous avons modifié la façon dont les ressources déplacées et supprimées sont traitées lors de l’utilisation de l’intégration d’Adobe Workfront à Experience Manager Assets et aux Assets Essentials :</p>
            <ul>
                <li>Ressources supprimées : lorsqu’une ressource est supprimée dans un dossier lié dans Assets ou Assets Essentials, la ressource supprimée est conservée dans la zone des Documents de projet.</li>
                <li>Ressources déplacées : lorsqu’une ressource est déplacée en dehors d’un dossier lié dans Assets ou Assets essentials, la ressource déplacée est conservée dans la zone des Documents de projet.</li>
            </ul>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 21 novembre 2024</li>
                <li><span class="preview">Version de production pour tous les clients : 5 décembre 2024</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Les sections d’un formulaire personnalisé sont désormais réductibles et extensibles</a></p>
            [!BADGE In production for Fast Release ]{type=Positive}
            <p>Lorsqu’un formulaire personnalisé avec plusieurs sections est joint à un objet, vous pouvez désormais réduire et développer toutes les sections, à l’exception de la section par défaut située en haut du formulaire. L’administrateur peut également voir cette fonctionnalité lors de la prévisualisation du formulaire dans le concepteur de formulaire.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : mardi 11 novembre 2024</li>
                <li>Production pour une version rapide : avec la version 24.12 (12 décembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            L’assistant AI peut désormais travailler sur des projets, des tâches et des événements</a></p>
            [!BADGE In production for Fast Release ]{type=Positive}
            <p>Pour faciliter la gestion de vos éléments de travail dans Workfront, nous avons mis à jour l’assistant AI pour qu’il fonctionne avec les projets, les tâches et les événements. Désormais, l’assistant AI peut localiser les projets, les tâches et les événements en fonction des critères que vous spécifiez.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : vendredi 31 octobre 2024</li>
                <li>Production pour une version rapide : avec la version 24.11 (14 novembre 2024)</li>
                <li>Version de production pour tous les clients : avec la version 25.1 (16 janvier 2025)</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            Mises à jour de l’apparence au cours du premier trimestre de 2025</a></p>
            <p>Des mises à jour mineures de l’aspect de diverses zones de l’application Adobe Workfront seront apportées au cours du premier trimestre 2025. Consultez les notes de mise à jour individuelles pour connaître les dates de publication spécifiques.</p>
        </td>
        <td>
            <p><b>Disponible à ces dates :</b></p>
            <ul>
                <li>Version préliminaire : tout au long du premier trimestre de 2025.</li>
                <li><span class="preview">Version de production : passez en revue les notes de mise à jour pour connaître les dates spécifiques.</span></li>
            </ul>
        </td>
    </tr>                            
</tbody>
</table>

<!--
### Functionality soon to be removed from Workfront

The following functionality is soon to be removed from Workfront:
-->

## Annonces

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent de celui du calendrier de la version du premier trimestre 2025. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Améliorations apportées à Workfront Planning

De nouvelles fonctionnalités de Workfront Planning sont disponibles en production. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de la version du premier trimestre 2025 de la planification Adobe Workfront](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md).

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

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version du premier trimestre 2025, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).
