---
title: Vue d’ensemble de la version 23.2
description: Vue d’ensemble de la version 23.2
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b0e2ce08-d9f7-4fb5-b35c-ba979ab9d03e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '2769'
ht-degree: 36%

---

# Vue d’ensemble de la version 23.2

Cette page fournit des informations sur les fonctionnalités incluses dans la version 23.1. Ces améliorations ont été apportées à l’environnement de production avec la version 23.2 des 6 et 7 avril 2023.

Pour obtenir des conseils sur la préparation de la prochaine version, reportez-vous à la section [Préparation d’une version trimestrielle d’Adobe Workfront](/help/quicksilver/product-announcements/product-releases/release-readiness.md).

## Webinaire sur la version

Au lieu d&#39;un webinaire sur la publication de ce rapport, nous vous invitons à vous inscrire pour assister aux sessions Workfront suivantes :

[Expériences affectées : de la création de contenu à Personalization](https://reg.adobe.com/flow/adobe/as23/sessions/page/catalog/session/1661982243928001D5Z9) le 21 mars 2023, pour découvrir de nouvelles façons de créer, gérer et personnaliser du contenu et offrir des expériences percutantes avec une plus grande efficacité. Cette session sera diffusée en continu pour les audiences virtuelles.

[The Future of Adobe Workfront](https://reg.adobe.com/flow/adobe/as23/sessions/page/catalog/session/1661982239896001DoHU) le 23 mars 2023, pour découvrir la vision de Workfront et sa place dans l’écosystème de l’Adobe et obtenir un aperçu de la feuille de route future. Cette session sera enregistrée et disponible ultérieurement sous forme de contenu à la demande.

<span class="preview">Les fonctionnalités hors cycle (celles qui sont publiées en production avant la date de publication de la version 23.2) sont surlignées en jaune.</span>

## Améliorations Adobe Workfront

* [Améliorations d’administration](#administrator-enhancements)
* [Améliorations rapides](#agile-enhancements)
* [Améliorations de la gestion de projet](#project-management-enhancements)
* [Améliorations de la gestion des ressources](#resource-management-enhancements)
* [Améliorations des rapports et tableaux de bord](#reports-and-dashboards-enhancements)
* [Améliorations apportées aux mobiles](#mobile-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations d’administration

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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Mappage des valeurs de champ Workfront aux balises dans Experience Manager Assets</a>
                        <p>Vous pouvez désormais classer et rechercher rapidement des ressources en fonction des données de Workfront.  Vous pouvez mapper ces données dans le cadre de votre configuration de métadonnées dans l’intégration de Workfront for Experience Manager Assets.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.<br /></p>
                            </li>
                            <li>
                                 <p>Version de production : vendredi 30 mars 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Créer des formulaires personnalisés avec la nouvelle version bêta du concepteur de formulaires</a>
                        <p>Le nouveau concepteur de formulaire dispose d’un nouvel espace de travail de style zone de travail qui vous permet d’afficher simultanément les paramètres des champs, de la zone de travail et des champs.</p>
                        <p>Avec le nouveau concepteur de formulaires, nous avons ajouté la possibilité d’utiliser 
                        <ul>
                        <li><strong>Copier un champ</strong> : vous pouvez désormais copier des champs existants en cliquant sur l’icône Copier dans les champs directement depuis la zone de travail.</li>
                        <li><strong>Utiliser une section par défaut</strong> : si la personne à l’origine du formulaire n’a pas ajouté de section en haut du formulaire, une section Par défaut est désormais visible dans la zone de travail, de sorte que les utilisateurs et utilisatrices puissent ajuster les autorisations pour les champs auxquels aucune section personnalisée n’est affectée. </li>
                        <li><strong>Modifier la taille du texte descriptif</strong> : vous pouvez désormais choisir des petites, moyennes ou grandes tailles pour les champs de texte descriptif. Vous pouvez également les utiliser sur la même ligne avec d’autres champs. <span style="color: #ff0000;"> La modification de la taille du texte descriptif a été temporairement retardée, mais sera bientôt disponible.</span></li> 
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 9 mars 2023</p>
                            </li>
                            <li>
                                 <p>Version de production : avec la version 23.2<br />
                                 <span style="color: #ff0000;">La version bêta du concepteur de formulaire a été temporairement désactivée dans l’aperçu et la production du 24 mai au 21 juillet 2023.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}"> Renommer les pin's dans le modèle de mise en page</span></a>
                        <p>Vous pouvez désormais renommer les pin’s dans un modèle de mise en page afin qu’ils aient plus de sens pour vos utilisateurs, au lieu d’utiliser le nom par défaut de la page épinglée. Les broches créées par les administrateurs s’affichent pour tous les utilisateurs affectés au modèle de mise en page, et les utilisateurs ne peuvent pas renommer ces broches.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 9 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Améliorations rapides

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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajout de tâches et de problèmes à partir des détails de l’objet sur un panorama ou un workflow Workfront</a></p>
                        <p>Vous pouvez désormais ajouter des tâches ou des problèmes existants à un panorama ou à une liste de cartes de flux de travail Workfront directement à partir des détails de l’objet. Tous les éléments que vous ajoutez à un panorama deviennent des cartes connectées et tous les éléments ajoutés à un flux de travail seront ajoutés à la liste des cartes en tant que cartes non prévues.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 23 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Fonctionnalité d’itération disponible dans les panoramas Adobe Workfront</a></p>
                        <p>Plusieurs nouvelles fonctionnalités disponibles dans les panoramas Workfront permettent d’utiliser la fonctionnalité Scrum d’Agile. Ces fonctionnalités sont les suivantes :
                        <ul>
                        <li>Flux de travail pour regrouper des panoramas liés à la même équipe et collaborer sur le travail</li>
                        <li>Liste de cartes, ou liste d’attente des travaux, avec la possibilité d’utiliser des sources pour connecter les cartes aux tâches et problèmes Workfront</li>
                        <li>Panneaux de processus de planification et d’itération</li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : samedi 17 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des tâches et des problèmes à partir de listes et de rapports à une liste de cartes de workflows</a></p>
                        <p>Vous pouvez désormais ajouter des tâches ou des problèmes existants à un flux de travail dans les panoramas Workfront directement à partir d’une vue de liste ou de rapport. Tous les éléments que vous ajoutez au flux de travail sont ajoutés à la liste des cartes en tant que cartes non prévues.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : samedi 17 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des champs personnalisés aux cartes sur un panorama</a></p>
                        <p>Vous pouvez désormais inclure des champs personnalisés dans les panoramas Adobe Workfront. Le champ doit déjà être créé dans Workfront. Vous ne pouvez pas concevoir et créer de nouveaux champs personnalisés dans un panorama.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : samedi 17 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajout de tâches et de problèmes à partir de listes et de rapports sur un panorama Workfront</a></p>
                        <p>Vous pouvez désormais ajouter des tâches ou des problèmes existants à un panorama Workfront directement à partir d’une vue de liste ou de rapport. Tous les éléments que vous ajoutez au panorama seront des cartes connectées.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 2 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}"> Afficher les heures sur les cartes connectées sur un panorama</a></p>
                        <p>Vous pouvez désormais consigner les heures pour les cartes connectées, comme vous le feriez pour une tâche ou un problème. Vous devez disposer des autorisations appropriées concernant la tâche ou le problème pour consigner des heures.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 23 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : 2 mars 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
              <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Personnalisation de l’affichage des champs sur une carte</a></p>
                        <p>La personnalisation est désormais disponible pour configurer les champs qui s’affichent sur une carte, à la fois dans la vue complète lorsque la carte est ouverte, et dans la vue de carte condensée du panorama. Lorsque vous désactivez un champ, il n’est affiché dans aucune des deux vues. Vous pouvez également activer un champ dans la vue complète et le masquer dans la vue condensée.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : 23 février 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Définir un état par défaut pour les cartes déplacées dans une colonne de panorama</a></p>
                        <p>Vous pouvez désormais définir un statut par défaut à appliquer aux cartes déplacées dans une colonne spécifique, en sélectionnant un statut personnalisé et un statut système dans les politiques de colonne. Lorsque vous déplacez une carte dans la colonne, Workfront tente d’abord d’appliquer le statut personnalisé (par exemple, Réaction en attente). Si le statut personnalisé n’est pas disponible pour cette carte, Workfront applique plutôt le statut système (par exemple, En attente). En outre, si le statut de la tâche ou du problème connecté passe au statut personnalisé ou système défini dans la politique de colonne, la carte est automatiquement déplacée dans la colonne.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : 23 février 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Collections désormais disponibles dans les panoramas Adobe Workfront</a></p>
                        <p>Vous pouvez désormais créer des collections dans le tableau de bord des panoramas. Une collection est un groupe de panoramas permettat de collaborer à un travail. Une fois que vous avez nommé la collection, vous pouvez ajouter des panoramas à la collection à l’aide d’un ensemble de modèles offrant des paramètres prédéfinis tels que les noms de colonne.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : 23 février 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Champ d’estimation sur les cartes connectées correspond au champ Points d’article sur les objets Workfront</a></p>
                        <p>Le champ Estimation des cartes connectées dans les panoramas Workfront est désormais associé au champ Points de l’histoire pour l’objet Workfront associé. </p>
                        <p>Le nouveau champ Points de l’histoire est un champ de forme libre modifiable que vous pouvez ajouter à une vue dans une liste ou un rapport pour des tâches ou des problèmes. Il n’est pas lié au nombre d’heures prévues ou aux affectations d’équipe.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 26 janvier 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : cette fonctionnalité a été retardée et est publiée le 9 février. <span style="color: #ff0000;">Cette fonctionnalité est disponible en production à cette date uniquement par le biais de l’accord préalable de la fonctionnalité pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Carte d’aperçu dans la colonne d’entrée</a></p>
                        <p>Vous pouvez maintenant cliquer sur une carte connectée dans la colonne d’entrée pour afficher une version en lecture seule de son contenu. Vous ne pouvez pas modifier le contenu de la carte tant que celle-ci n’a pas été déplacée de la colonne d’entrée vers une autre colonne du panorama.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 26 janvier 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de production pour la pré-inscription : 2 février 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via la pré-inscription de la fonctionnalité pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Améliorations de la gestion de projet

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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de l’édition de projets en bloc</a>
                        <p>Dans le cadre de la mise à jour de l’aspect de l’expérience Workfront, nous avons repensé la boîte de dialogue Modifier les projets, lors de la modification simultanée de plusieurs projets, en bloc. Vous pouvez accéder à la nouvelle boîte de dialogue Modifier les projets lorsque vous sélectionnez simultanément plusieurs projets dans une liste de projets.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 9 mars 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : à compter du 23 mars, cette version sera mise en production dans un déploiement par étapes qui prendra fin après le 11 mai 2023.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> Expérience de filtrage améliorée généralement disponible dans Adobe Workfront</a>
                        <p>L’expérience améliorée de filtrage sera disponible dans l’ensemble et deviendra le créateur de filtres standard dans Aperçu le 2 mars 2023. Un déploiement par étapes dans Production commencera également le 2 mars, avec la disponibilité de tous les clients dans la version 23.2.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 2 mars 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : avec la version 23.2</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Copier les heures budgétaires lors de la copie d’un projet</a>
                        <p>Vous avez désormais la possibilité de copier les heures budgétées dans la zone Ressource/Budget de l’Analyse de cas ou du Planificateur de ressources lorsque vous copiez un projet. Avant cette amélioration, les heures budgétées du projet n’étaient pas transférées vers le projet copié.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : 2 mars 2023 (hors cycle)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Améliorations de la gestion des ressources

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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Présentation du champ Durée du travail pour calculer précisément la capacité de l’utilisateur</a>
                        <p>Pour permettre aux gestionnaires de ressources de calculer précisément la disponibilité de leurs utilisateurs et de tenir compte du temps que les utilisateurs consacrent à des tâches réelles liées au projet, nous proposons le concept de temps de travail à Adobe Workfront.</p>
                        <p>Vous pouvez définir la valeur du champ Durée du travail pour chaque utilisateur, lorsque vous créez ou modifiez son profil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : 2 mars 2023 (hors cycle)</span></p>
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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-reports-dashboards.md" class="MCXref xref" xrefformat="{para}">Tableaux de bord de canevas</a></p>
                        <p>Ajout de tableaux de bord de canevas en tant que fonctionnalité de travail en cours pour les tableaux de bord qui peuvent être activés dans les modèles de mise en page - Les tableaux de bord du canevas de rapports permettent de combiner les visualisations du canevas de rapports avec les rapports existants, en plus des nouvelles options de mise en page. Actuellement, seuls les rapports de liste sont pris en charge, mais d’autres options seront ajoutées au fur et à mesure du développement.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : avec la version 23.2</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Améliorations apportées aux mobiles

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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}"> Connexion biométrique et collections de panoramas dans l'application mobile </span></a>
                        <p>La connexion biométrique est désormais une option permettant une connexion plus rapide à l’application mobile ! Une fois la vérification biométrique configurée après une connexion initiale, les utilisateurs pourront utiliser l’empreinte digitale ou la reconnaissance faciale pour se reconnecter rapidement à l’application avec une réauthentification occasionnelle du mot de passe. En outre, plusieurs améliorations de l’apparence de l’expérience générale de connexion arriveront lors d’une mise à jour ultérieure.</p>
                        <p>Les collections de panoramas sont désormais prises en charge dans l’application mobile, ce qui permet aux utilisateurs mobiles d’afficher toutes les collections auxquelles ils ont accès dans la version de bureau à partir de leur liste de panoramas mobiles.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.<br /></p>
                            </li>
                            <li>
                                 <p>Version de production : disponible dans Apple App Store et Google Play Store 13 mars 2023</p>
                            </li>
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
                        <p><span class="bold">Fonctionnalité</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveau dans Workfront pour les modules externes de Creative Cloud</a>
                        <p>Nous avons ajouté les modifications suivantes aux modules externes Workfront for Creative Cloud :
                        <ul>
                        <li>Le module externe vous avertit désormais lorsqu’une tâche possède un prédécesseur</li>
                        <li>Le coréen est désormais une langue prise en charge</li>
                        </ul> </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : vendredi 23 mars 2023 </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience de commentaires pour les problèmes Beta</a>
                        <p>Une mise à jour de l’expérience de commentaires dans Adobe Workfront est actuellement en cours de développement. Cette mise à jour inclut une nouvelle interface, de nouvelles fonctionnalités et une amélioration des performances dans la section Mises à jour de certains objets. </p>
                        <p>Cette nouvelle expérience finira par unifier les commentaires dans Adobe Workfront et au-delà, dans Adobe Experience Cloud. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : mardi 20 mars 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : avec la version 23.2 </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> Nouveaux clients réseau à intégrer pour Adobe d’une expérience unifiée </a></p>
                        <p>L’expérience unifiée Adobe comprend :
                        <ul>
                        <li>Une seule connexion pour toutes les applications Adobe via Adobe Experience Cloud</li>
                        <li>Sélecteur d’organisation à déplacer entre les organisations et les environnements Workfront</li>
                        <li>Navigation avec options pour les pages Workfront, les préférences Adobe Experience Cloud et votre profil Workfront</li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.<br /></p>
                            </li>
                            <li>
                                <p>Version de production : de mi-à-fin mars 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> La visionneuse de vérification s’ouvre dans un nouvel onglet pour les utilisateurs de l’expérience unifiée </a></p>
                        <p>La visionneuse de vérification visuelle s’ouvre désormais dans un nouvel onglet pour les utilisateurs de l’expérience unifiée.
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.<br /></p>
                            </li>
                            <li>
                                <p>Version de production : de mi-à-fin mars 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Exporter des artefacts en tant que fichiers de PDF unique ou de PDF multiples dans Adobe Workfront pour XD</span></a>
                        <p>Dans le module externe Adobe Workfront for XD, vous pouvez désormais choisir d’exporter vos tableaux de bord sous la forme d’un seul fichier de PDF ou de plusieurs fichiers de PDF.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.<br /></p>
                            </li>
                            <li>
                                 <p>Version de production : mardi 6 février 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-look-and-feel.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’apparence pendant la période de publication de la version 23.2</a></p>
                        <p>Des mises à jour mineures de l’aspect des différentes zones de l’application Adobe Workfront sont effectuées dans le délai de publication de la version 23.2. Ces améliorations seront rendues disponibles dans l’environnement de production au moins 2 semaines après la publication de la version de prévisualisation. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : pendant toute la période de la version 23.2<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : au moins 2 semaines après la publication dans Aperçu (sauf indication contraire)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

## Annonces

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de version 23.2. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Améliorations du planificateur de scénarios Workfront

Aucune mise à jour du planificateur de scénario n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de l’épreuve Workfront

Aucune mise à jour de l’épreuve Workfront n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des Objectifs Workfront

Nouvelles fonctionnalités de la version 23.2 des objectifs de Workfront . Pour plus d’informations sur ces nouvelles fonctionnalités désormais disponibles dans l’aperçu, voir [Objectifs d’Adobe Workfront avec la version 23.2](/help/quicksilver/product-announcements/product-releases/goals-release-activity/goals-23-2-release/goals-23-2-release.md).

### API version 16

La version 16 de l’API sera publiée avec la version 22.3. Pour l’API version 16, nous avons modifié certaines ressources et points d’entrée. Certaines des modifications participent à la prise en charge des nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, consultez les [Nouveautés de l’API version 16](/help/quicksilver/wf-api/api/new-api-version-16.md).

Pour plus d’informations sur les versions d’API, consultez [Contrôle de version des API et planification de la prise en charge](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version 23.2, consultez [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr).

### Mises à jour de formation

Découvrez les dernières mises à jour apportées aux programmes de formation, aux parcours de formation, aux vidéos et aux guides de chaque version de produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).

### Fonctionnalité bientôt supprimée de Workfront

Les fonctionnalités suivantes seront bientôt supprimées de Workfront :

#### **Les pages externes du tableau de bord ne prennent plus en charge les URL du tableau de bord**

Pour améliorer la stabilité et les temps de chargement des tableaux de bord, les pages externes des tableaux de bord ne pourront plus référencer les URL des tableaux de bord. Les administrateurs système pour les comptes qui contiennent des pages externes référençant des tableaux de bord recevront une notification in-app les informant de cette modification. Pour plus d’informations, voir [Incorporation d’une page externe dans un tableau de bord](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

#### **Modifications de l’API Workfront par défaut**

Afin que les appels API puissent tirer parti des fonctionnalités d’API Workfront les plus récentes, nous mettons actuellement à jour l’API par défaut. Lorsqu’un appel API ne spécifie pas de version de l’API, l’appel est effectué à l’API par défaut.

Désormais, l’API par défaut reflète la version la plus récente de l’API. Dorénavant, nous mettrons à jour l’API par défaut chaque fois qu’une nouvelle version d’API est publiée, de sorte que les appels à l’API par défaut utiliseront toujours la version la plus récente de l’API.

Auparavant, l’API par défaut utilisait l’API Workfront version 2.0, qui était obsolète.

Si votre entreprise utilise actuellement l’API par défaut obsolète, votre administrateur Workfront a reçu un message du centre d’annonces contenant des instructions supplémentaires sur l’API par défaut.

Pour plus d’informations, voir [Mise à jour des intégrations qui utilisent le contrôle de version d’API par défaut](/help/quicksilver/wf-api/api/update-default-api-versioning.md).


<!--
<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>  

        -->
