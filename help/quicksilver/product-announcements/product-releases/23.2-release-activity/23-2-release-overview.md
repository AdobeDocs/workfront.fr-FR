---
title: Vue d’ensemble de la version 23.2
description: Vue d’ensemble de la version 23.2
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b0e2ce08-d9f7-4fb5-b35c-ba979ab9d03e
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '2770'
ht-degree: 99%

---

# Vue d’ensemble de la version 23.2

Cette page fournit des informations sur les fonctionnalités incluses dans la version 23.1. Ces améliorations ont été mises à disposition dans l’environnement de production avec la version 23.2 les 6 et 7 avril 2023.

Pour obtenir des conseils sur la préparation de la prochaine version, consultez la section [Se préparer aux versions trimestrielles d’Adobe Workfront](/help/quicksilver/product-announcements/product-releases/release-readiness.md).

## Webinaire sur la version

En lieu et place d’un webinaire sur la version, nous vous invitons à vous inscrire à Adobe Summit pour assister aux sessions Workfront suivantes :

[Expériences marquantes : de la création de contenu à la personnalisation](https://reg.adobe.com/flow/adobe/as23/sessions/page/catalog/session/1661982243928001D5Z9) le 21 mars 2023, pour apprendre de nouvelles façons de créer, de gérer et de personnaliser le contenu et d’offrir des expériences marquantes avec une plus grande efficacité. Cette session sera retransmise en direct pour les audiences virtuelles.

[L’avenir d’Adobe Workfront](https://reg.adobe.com/flow/adobe/as23/sessions/page/catalog/session/1661982239896001DoHU) le 23 mars 2023, pour découvrir la vision de Workfront et sa place dans l’écosystème Adobe et avoir un aperçu de la future feuille de route. Cette session sera enregistrée et disponible ultérieurement sous forme de contenu à la demande.

<span class="preview">Les fonctionnalités hors cycle (celles qui ont été mises en production avant la date de sortie de la version 23.2) sont surlignées en jaune.</span>

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations de la méthode Agile](#agile-enhancements)
* [Amélioration apportées à la gestion de projets](#project-management-enhancements)
* [Amélioration apportées à la gestion des ressources.](#resource-management-enhancements)
* [Amélioration apportées aux rapports et tableaux de bord](#reports-and-dashboards-enhancements)
* [Améliorations mobiles](#mobile-enhancements)
* [Autres améliorations](#other-enhancements)

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Mapper les valeurs des champs Workfront aux balises dans Experience Manager Assets</a>
                        <p>Vous pouvez désormais classer et rechercher rapidement des ressources en fonction des données de Workfront.  Vous pouvez mapper ces données dans le cadre de votre configuration de métadonnées dans l’intégration Workfront pour Experience Manager Assets.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                 <p>Version de production : 30 mars 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Créer des formulaires personnalisés avec le nouveau concepteur de formulaires Beta</a>
                        <p>Le nouveau concepteur de formulaires dispose d’un nouvel espace de travail de style zone de travail qui vous permet d’afficher simultanément les champs, la zone de travail et les paramètres des champs.</p>
                        <p>Avec le nouveau concepteur de formulaires, nous avons ajouté la possibilité de : 
                        <ul>
                        <li><strong>Copier un champ</strong> : vous pouvez maintenant copier des champs existants en cliquant sur l’icône « Copier » sur les champs directement à partir de la zone de travail.</li>
                        <li><strong>Utiliser une section par défaut</strong> : lorsque le créateur ou la créatrice du formulaire n’a pas inséré de section en haut du formulaire, une section par défaut apparaît maintenant dans la zone de travail pour que les utilisateurs et les utilisatrices puissent accorder des autorisations aux champs sans section personnalisée affectée. </li>
                        <li><strong>Modifier la taille des champs de texte descriptif</strong> : vous pouvez désormais attribuer une taille petite, moyenne ou grande aux champs de texte descriptif. Vous pouvez également les utiliser sur la même ligne que d’autres champs. <span style="color: #ff0000;">Modifier la taille du texte descriptif a été temporairement retardé, mais sera bientôt disponible.</span></li> 
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 9 mars 2023</p>
                            </li>
                            <li>
                                 <p>Version de production : avec la version 23.2<br />
                                 <span style="color: #ff0000;">La nouvelle version Beta du créateur de formulaire a été temporairement désactivée dans les versions de prévisualisation et de production du 24 mai au 21 juillet 2023.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Renommer les épingles dans le modèle de mise en page</span></a>
                        <p>Dans un modèle de mise en page, vous pouvez désormais renommer les épingles pour les rendre plus significatives pour vos utilisateurs ou vos utilisatrices, au lieu d’utiliser le nom par défaut de la page épinglée. Les épingles créées par l’équipe d’administration sont visibles pour l’ensemble des utilisateurs et des utilisatrices du modèle de mise en page et ne peuvent pas être renommées par ces utilisateurs et ces utilisatrices.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 9 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Améliorations de la méthode Agile

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des tâches et des problèmes à un panorama ou à un flux de travail Workfront à partir des détails d’un objet</a></p>
                        <p>Vous pouvez désormais ajouter des tâches ou des problèmes existants à un panorama Workfront ou à une liste de cartes de flux de travail directement à partir des détails de l’objet. Tous les éléments que vous ajoutez à un panorama deviendront des cartes connectées et tous les éléments ajoutés à un flux de travail seront ajoutés à la liste des cartes en tant que cartes non planifiées.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 23 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Fonctionnalité d’itération disponible dans les panoramas Adobe Workfront</a></p>
                        <p>Plusieurs nouvelles fonctionnalités disponibles dans les tableaux Workfront permettent d’utiliser la fonctionnalité Agile Scrum. Ces fonctionnalités sont les suivantes :
                        <ul>
                        <li>Flux de travail pour regrouper des panoramas liés à la même équipe et collaborer sur le travail</li>
                        <li>Liste de cartes, ou liste d’attente du travail, avec la possibilité d’utiliser des sources pour connecter les cartes aux tâches et problèmes Workfront</li>
                        <li>Panoramas de processus et de planification d’itération</li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des tâches et des problèmes provenant de listes et de rapports à une liste de cartes de flux de travail</a></p>
                        <p>Vous pouvez désormais ajouter des tâches et des problèmes existants à un flux de travail dans les panoramas Workfront directement à partir d’une vue liste ou rapport. Tous les éléments que vous ajoutez au flux de travail sont ajoutés à la liste des cartes en tant que cartes non planifiées.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des champs personnalisés aux cartes d’un panorama</a></p>
                        <p>Vous pouvez désormais inclure des champs personnalisés dans les panoramas Adobe Workfront. Le champ doit déjà être créé dans Workfront. Vous ne pouvez pas concevoir et créer de nouveaux champs personnalisés dans un panorama.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des tâches et des problèmes à un panorama Workfront à partir de listes et de rapports</a></p>
                        <p>Vous pouvez désormais ajouter des tâches et des problèmes existants à un panorama Workfront directement à partir d’une vue liste ou rapport. Tous les éléments que vous ajoutez au panorama seront des cartes connectées.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 2 mars 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Consigner les heures sur les cartes connectées à un panorama</a></p>
                        <p>Vous pouvez désormais consigner des heures sur les cartes connectées, comme vous le feriez pour une tâche ou un problème. Pour consigner des heures, vous devez disposer des autorisations appropriées pour la tâche ou le problème.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 23 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Version de production pour opt-in anticipé : 2 mars 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement par le biais de l’opt-in anticipé pour les panoramas Workfront.</span></p>
                                <p>Version de production pour l’ensemble de la clientèle : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
              <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Personnaliser l’affichage des champs sur une carte</a></p>
                        <p>La personnalisation est désormais disponible pour configurer les champs qui s’affichent sur une carte, à la fois en vue complète lorsque la carte est ouverte et en vue condensée de la carte sur le panorama. Lorsque vous désactivez un champ, il ne s’affiche dans aucune des deux vues. Vous pouvez également activer un champ dans la vue complète et le masquer dans la vue condensée.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Version de production pour l’opt-in anticipé : 23 février 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement par le biais de l’opt-in anticipé pour les panoramas Workfront.</span></p>
                                <p>Version de production pour l’ensemble de la clientèle : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Définir un statut par défaut pour les cartes déplacées dans une colonne du panorama</a></p>
                        <p>Vous pouvez désormais définir un statut par défaut à appliquer aux cartes déplacées dans une colonne spécifique, en sélectionnant un statut personnalisé et un statut système dans les politiques de colonne. Lorsque vous déplacez une carte dans la colonne, Workfront tente d’abord d’appliquer le statut personnalisé (par exemple, Commentaires en attente). Si le statut personnalisé n’est pas disponible pour cette carte, Workfront applique le statut du système (par exemple, En attente). En outre, si le statut de la tâche connectée ou du problème connecté est modifié dans le statut personnalisé ou système défini dans la politique de colonne, la carte est automatiquement déplacée dans la colonne.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Version de production pour l’opt-in anticipé : 23 février 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement par le biais de l’opt-in anticipé pour les panoramas Workfront.</span></p>
                                <p>Version de production pour l’ensemble de la clientèle : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Les collections sont désormais disponibles dans les panoramas Adobe Workfront.</a></p>
                        <p>Vous pouvez désormais créer des collections dans le tableau de bord des panoramas. Une collection est un groupe de panoramas pour travailler en collaboration. Une fois que vous avez nommé la collection, vous pouvez y ajouter des panoramas à l’aide d’un ensemble de modèles offrant des paramètres prédéfinis tels que les noms de colonne.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p>Version de production pour l’opt-in anticipé : 23 février 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement par le biais de l’opt-in anticipé pour les panoramas Workfront.</span></p>
                                <p>Version de production pour l’ensemble de la clientèle : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Le champ d’estimation sur les cartes connectées correspond au champ des points de l’histoire sur les objets Workfront.</a></p>
                        <p>Le champ Estimation des cartes connectées dans les panoramas Workfront est désormais associé au champ Points de l’histoire pour l’objet Workfront associé. </p>
                        <p>Le nouveau champ Points de l’histoire est un champ à structure libre modifiable que vous pouvez ajouter à une vue dans une liste ou un rapport de tâches ou de problèmes. Il n’est pas lié au nombre d’heures prévues ou aux affectations d’équipe.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 26 janvier 2023<br /></p>
                            </li>
                            <li>
                                 <p>Version de production pour l’opt-in anticipé : cette fonctionnalité a été retardée et sera disponible le 9 février. <span style="color: #ff0000;">Cette fonctionnalité n’est disponible en production qu’à partir de cette date, par le biais d’un opt-in anticipé pour les panoramas Workfront.</span></p>
                                <p>Version de production pour l’ensemble de la clientèle : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Prévisualiser la carte dans la colonne de saisie</a></p>
                        <p>Vous pouvez maintenant cliquer sur une carte connectée dans la colonne de saisie pour afficher une version en lecture seule de son contenu. Vous ne pouvez pas modifier le contenu de la carte tant que celle-ci n’a pas été déplacée de la colonne de saisie vers une autre colonne du panorama.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 26 janvier 2023<br /></p>
                            </li>
                            <li>
                                 <p>Version de production pour l’opt-in anticipé : 2 février 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement par le biais de l’opt-in anticipé pour les panoramas Workfront.</span></p>
                                <p>Version de production pour l’ensemble de la clientèle : avec la version 23.2</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Amélioration apportées à la gestion de projets

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience lors de la modification de projets en bloc</a>
                        <p>Dans le cadre de la mise à jour de l’aspect de l’expérience Workfront, nous avons repensé la zone Modifier les projets, lors de la modification simultanée de plusieurs projets, en masse. Vous pouvez accéder à la nouvelle zone Modifier les projets lorsque vous sélectionnez simultanément plusieurs projets dans une liste des projets.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 9 mars 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : à partir du 23 mars, la mise en production se fera par étapes et s’achèvera après le 11 mai 2023.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Amélioration de l’expérience de filtrage disponible de façon générale dans Adobe Workfront</a>
                        <p>L’expérience améliorée de filtrage sera disponible et deviendra le créateur de filtres standard dans l’environnement de prévisualisation le 2 mars 2023. Un déploiement par étapes dans l’environnement de production commencera également le 2 mars, avec une disponibilité pour l’ensemble des clientes et clients dans la version 23.2.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 2 mars 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : avec la version 23.2</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Copier les heures budgétées lors de la copie d’un projet</a>
                        <p>Vous avez désormais la possibilité de copier les heures budgétées dans la zone Établissement du budget de ressources du Business Case ou du Planificateur de ressources lorsque vous copiez un projet. Avant cette amélioration, les heures budgétées du projet n’étaient pas transférées vers le projet copié.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : 2 mars 2023 (hors cycle)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### Amélioration apportées à la gestion des ressources.

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Introduction du champ Temps de travail pour calculer avec précision la capacité des utilisateurs et utilisatrices</a>
                        <p>Pour permettre aux gestionnaires de ressources de calculer précisément la disponibilité de leurs utilisateurs et utilisatrices et de tenir compte du temps que ceux-ci consacrent à des tâches réelles liées au projet, nous proposons le concept de temps de travail dans Adobe Workfront.</p>
                        <p>Vous pouvez définir la valeur du champ Temps de travail pour chaque utilisateur ou utilisatrice lorsque vous créez ou modifiez son profil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 16 février 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : 2 mars 2023 (hors cycle)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>


### Amélioration apportées aux rapports et tableaux de bord


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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-reports-dashboards.md" class="MCXref xref" xrefformat="{para}">Tableaux de bord de zones de travail</a></p>
                        <p>Les tableaux de bord de zones de travail ont été ajoutés en tant que fonctionnalité en cours de développement pour les tableaux de bord, qui peut être activée dans les modèles de mise en page. La fonctionnalité de tableaux de bord de zones de travail permettra de combiner les visualisations de la zone de travail de reporting avec les rapports existants, en plus des nouvelles options de disposition. Actuellement, seuls les rapports sous forme de liste sont pris en charge, mais d’autres options seront ajoutées au fur et à mesure du développement.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S.O.<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : avec la version 23.2</span></p>
                            </li>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">Connexion biométrique et panoramas dans l’application mobile</span></a>
                        <p>La connexion biométrique est désormais une option pour une connexion plus rapide à l’application mobile. Une fois la vérification biométrique mise en place après une première connexion, les utilisateurs et utilisatrices pourront utiliser les empreintes digitales ou la reconnaissance faciale pour se reconnecter rapidement à l’application, avec seulement une revérification occasionnelle du mot de passe. En outre, une mise à jour ultérieure apportera un certain nombre d’améliorations de l’aspect à l’expérience de connexion générale.</p>
                        <p>Les collections de panoramas sont désormais également prises en charge dans l’application mobile, ce qui permet aux utilisateurs et utilisatrices mobiles d’afficher toutes les collections auxquelles ils ont accès dans la version pour bureau à partir de leur liste de panoramas mobiles.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                 <p>Version de production : disponible sur l’Apple App Store et le Google Play Store le 13 mars 2023.</p>
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
                        <p><span class="bold">Dates de publication</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveautés dans les plug-ins Workfront pour Creative Cloud</a>
                        <p>Nous avons ajouté les modifications suivantes aux plug-ins Workfront pour Creative Cloud :
                        <ul>
                        <li>Le plug-in vous avertit désormais lorsqu’une tâche possède une tâche antérieure.</li>
                        <li>Le coréen est désormais une langue prise en charge.</li>
                        </ul> </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : 23 mars 2023 </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience de commentaires pour les problèmes (Beta)</a>
                        <p>Une mise à jour de l’expérience de commentaires dans Adobe Workfront est actuellement en cours de développement. Cette mise à jour inclut une nouvelle interface, de nouvelles fonctionnalités et une amélioration des performances dans la section Mises à jour de certains objets. </p>
                        <p>Cette nouvelle expérience finira par unifier les commentaires dans Adobe Workfront et au-delà, dans Adobe Experience Cloud. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : 20 mars 2023<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : avec la version 23.2 </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle clientèle Net à intégrer à Adobe Unified Experience</a></p>
                        <p>Adobe Unified Experience comprend :
                        <ul>
                        <li>Une seule connexion pour toutes les applications Adobe via Adobe Experience Cloud.</li>
                        <li>Un sélecteur d’organisation à déplacer entre les organisations et les environnements Workfront.</li>
                        <li>Une navigation avec options pour les pages Workfront, les préférences Adobe Experience Cloud et votre profil Workfront.</li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                <p>Version de production : mi-mars à fin mars 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">La visionneuse de relecture s’ouvre dans un nouvel onglet pour les utilisateurs et les utilisatrices d’Unified Experience.</a></p>
                        <p>La visionneuse de relecture s’ouvre désormais dans un nouvel onglet pour les utilisateurs et les utilisatrices d’Unified Experience.
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                <p>Version de production : mi-mars à fin mars 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Exporter les plans de travail sous forme de fichiers PDF uniques ou multiples dans Adobe Workfront pour XD</span></a>
                        <p>Dans le plug-in Adobe Workfront pour XD, vous pouvez désormais choisir d’exporter vos tableaux de bord sous la forme d’un seul fichier PDF ou de plusieurs fichiers PDF.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                 <p>Version de production : 6 février 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-look-and-feel.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’aspect pendant toute la durée de la version 23.2</a></p>
                        <p>Des mises à jour mineures de l’aspect de diverses parties de l’application Adobe Workfront sont effectuées dans le cadre de la version 23.2. Ces améliorations seront disponibles dans l’environnement de production au moins deux semaines après le lancement de la version préliminaire. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : pendant toute la période de de la version 23.2<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : au moins 2 semaines après la publication dans l’environnement de prévisualisation (sauf indication contraire)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

## Annonces

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de la version 23.2. Pour plus d’informations sur les dernières fonctionnalités, consultez [Activité Version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Améliorations du planificateur de scénarios Workfront

Il n’y a pas de mise à jour du planificateur de scénarios à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de Workfront Proof

Il n’y a pas de mise à jour de Workfront Proof à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des Objectifs Workfront

De nouvelles fonctionnalités seront ajoutées à la version 23.2 d’Objectifs Workfront. Pour plus d’informations sur ces nouvelles fonctionnalités disponibles en version de prévisualisation, consultez [Objectifs Adobe Workfront avec la version 23.2](/help/quicksilver/product-announcements/product-releases/goals-release-activity/goals-23-2-release/goals-23-2-release.md).

### API version 16

La version 16 de l’API sera publiée avec la version 22.3. Pour l’API version 16, nous avons modifié certaines ressources et points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, consultez les [Nouveautés de l’API version 16](/help/quicksilver/wf-api/api/new-api-version-16.md).

Pour plus d’informations sur les versions d’API, consultez [Contrôle de version des API et planning de la prise en charge](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées dans le cadre de la version 23.2, consultez [Mises à jour de maintenance pour Workfront](https://experienceleague.adobe.com/fr/docs/workfront-known-issues/releases/current-updates).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, voir la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/fr/docs/workfront-learn/tutorials-workfront/home).

### Fonctionnalités bientôt supprimées de Workfront

Les fonctionnalités suivantes seront bientôt supprimées de Workfront :

#### **Les pages externes du tableau de bord ne prennent plus en charge les URL du tableau de bord**.

Afin d’améliorer la stabilité des tableaux de bord et les temps de chargement, les pages externes des tableaux de bord ne pourront plus faire référence aux URL de tableaux de bord. L’équipe d’administration système des comptes qui contiennent des pages externes faisant référence à des tableaux de bord recevront une notification in-app pour les avertir de ce changement. Pour plus d’informations, voir [Incorporer une page externe dans un tableau de bord](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

#### **Modifications de l’API par défaut de Workfront**

Pour s’assurer que les appels API puissent bénéficier des fonctionnalités les plus récentes de l’API Workfront, nous mettons à jour l’API par défaut. Lorsqu’un appel API ne spécifie pas de version de l’API, l’appel est effectué à l’API par défaut.

Désormais, l’API par défaut reflétera la version la plus récente de l’API. À l’avenir, nous mettrons à jour l’API par défaut chaque fois qu’une nouvelle version de l’API sera publiée, de sorte que les appels API par défaut utiliseront toujours la version la plus récente de l’API.

Auparavant, l’API par défaut utilisait la version 2.0 de l’API Workfront, qui a été supprimée.

Si votre organisation utilise actuellement l’API par défaut, votre administrateur ou administratrice Workfront a reçu un message du centre des annonces contenant des instructions supplémentaires concernant l’API par défaut.

Pour plus d’informations, voir [Mettre à jour les intégrations qui utilisent le contrôle de version par défaut de l’API](/help/quicksilver/wf-api/api/update-default-api-versioning.md).


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
