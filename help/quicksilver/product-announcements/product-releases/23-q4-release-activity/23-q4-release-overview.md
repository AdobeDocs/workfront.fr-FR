---
title: Présentation de la version du quatrième trimestre 2023
description: Présentation de la version du quatrième trimestre 2023
author: Becky
feature: Product Announcements
exl-id: 6c14bd61-60b1-49aa-84bd-d494a226d70e
source-git-commit: 383c87843b3a9a3a7e4e9b78ddd41828013c23c7
workflow-type: tm+mt
source-wordcount: '2665'
ht-degree: 0%

---

# Présentation de la version du quatrième trimestre 2023

Cette page fournit des informations sur les fonctionnalités incluses dans la version du quatrième trimestre 2023. Ces améliorations sont prévues pour être disponibles dans l’environnement de production pour tous les clients de la version 23.10 des 26 et 27 octobre 2023.

<!--
These enhancements will be included in the following releases:

>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>23.8 (August 31, 2023)</li><li>23.9 (September 28, 2023)</li><li>23.10 (October 26, 2023)</li></ul>| <ul><li>23.10 (Week of October 26, 2023)</li></ul>|
-->

Le webinaire de la version 23.10 a eu lieu le 5 octobre 2023. Vous pouvez [Inscrivez-vous au webinaire pour afficher un enregistrement à la demande ici](https://webinars.on24.com/adobe_workfront/whatsnewin2310?partnerref=releasenotes).

<span class="preview">Les fonctionnalités hors cycle (celles qui sont publiées en production avant la date de publication du quatrième trimestre 2023) sont surlignées en jaune.</span>

>[!IMPORTANT]
>
>La version 23.3 incluait l’option permettant de déplacer votre organisation vers les versions mensuelles. Par conséquent, Workfront est en train de modifier le schéma de numérotation des versions afin de prendre en compte à la fois les mises à jour mensuelles et trimestrielles.
>
>* Si vous utilisez la variable **version rapide (mensuelle)** track, la version après 23.3 est **23,8**, le 31 août 2023.
> * Si vous utilisez la variable **trimestriel** suivi de publication, la version après 23.3 est **23,10**, dans la semaine du 26 octobre 2023.
> 
> Les versions trimestrielles comprennent des fonctionnalités issues de trois versions mensuelles. Par exemple, la version trimestrielle 23.10 comprend des fonctionnalités publiées dans les versions mensuelles 23.8, 23.9 et 23.10.
>
>Les mises à jour mensuelles et trimestrielles sont prévues pour le dernier jeudi du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>23.8 (31 août 2023)</li><li>23.9 (28 septembre 2023)</li><li>23.10 (26 octobre 2023)</li></ul> | <ul><li>23.10 (Semaine du 26 octobre 2023)</li></ul> |
>| <ul><li>Aucune version (novembre 2023)</li><li>Aucune publication (décembre 2023)</li><li>24.1 (janvier 2024)</li></ul> | <ul><li>24.1 (janvier 2024)</li></ul> |
>
>Pour plus d’informations sur le processus de publication rapide, voir [Activation ou désactivation du processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs](#administrator-enhancements)
* [Améliorations des panoramas](#boards-enhancements)
* [Améliorations apportées à la gestion financière](#financial-management-enhancements)
* [Améliorations de la page d’accueil](#home-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations des projets](#project-enhancements)
* [Autres améliorations](#other-enhancements)

### Améliorations apportées aux administrateurs

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">BAT et décisions de document disponibles pour les clients de modèles de licence hérités</a></p>
                        <p>Les clients hérités qui n’ont pas encore migré vers le nouveau modèle de licence Adobe Workfront peuvent désormais afficher dans un seul rapport les données avec le nombre de décisions de BAT/document par utilisateur et par mois. Ces données sont disponibles lorsque vous exécutez un rapport Décisions d’utilisateur .</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : 12 octobre 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>            
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Les champs calculés sur les formulaires personnalisés peuvent désormais utiliser le caractère générique $$USER</a></p>
                        <p>Le caractère générique $$USER est désormais disponible dans les champs personnalisés calculés et les champs de recherche externes du nouveau concepteur de formulaire.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 5 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajout d’options de valeur d’une API externe à un formulaire personnalisé</a></p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>un nouveau type de champ, <strong>Recherche externe</strong>, est désormais disponible sur le concepteur de formulaire personnalisé. Lorsque des données sont stockées sur un système externe, ce type de champ vous permet de charger des options à partir d’une API externe et de filtrer selon d’autres valeurs de champ dans le formulaire personnalisé.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 14 septembre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.9</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Sous-tâches désormais disponibles dans les panoramas Adobe Workfront</a><span style="color: #ff0000;"> Nouveau dans Aperçu .</span></p><p>Lorsque vous ajoutez une carte connectée à un panorama pour une tâche Workfront, toutes les sous-tâches existantes sont importées sur la carte. En outre, lorsque vous créez une sous-tâche sur une carte connectée, une sous-tâche est ajoutée à la tâche Workfront.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour un accès anticipé aux panoramas : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations des affectations d’utilisateurs sur les panoramas et les cartes</a></p><p>[!BADGE en production ]{type=Informative}</p><p>Des améliorations sont désormais disponibles, ce qui offre davantage de flexibilité lors de l’ajout d’utilisateurs aux panoramas et aux cartes dans les panoramas Adobe Workfront.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 21 août 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : 24 août 2023</span>
                            </li> 
                       </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajout de documents sur les cartes connectées</a></p><p>Vous pouvez désormais joindre des documents sur les cartes connectées sur les panoramas Adobe Workfront. Tous les documents que vous ajoutez sur la carte sont disponibles dans l’onglet Documents de la tâche ou du problème connecté, et les mêmes types de fichiers sont pris en charge dans les deux zones.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 21 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour un accès anticipé aux panoramas : 24 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Documents disponibles sur les cartes connectées en tant qu’affichage uniquement</a></p><p>Pour les cartes connectées sur les panoramas Adobe Workfront, vous pouvez désormais afficher des documents tels que des images et des PDF. Vous pouvez prévisualiser un document dans le navigateur ou le télécharger sur votre ordinateur. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 3 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour un accès anticipé aux panoramas : 10 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Vue du panorama d’un projet désormais disponible pour les problèmes</a></p><p>Vous pouvez désormais accéder à la vue Panorama d’une liste de problèmes de projet. Le panorama de Kanban peut vous aider à suivre l’état d’avancement des problèmes d’une manière plus visuelle que de les voir dans la liste. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 3 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour un accès anticipé aux panoramas : S.O.</p>
                            </li>
                             <li>
                                <p>Production pour une version rapide : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>    
           </tbody>
        </table>

### Améliorations apportées à la gestion financière

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Date d’entrée en vigueur des coûts et des taux de facturation</a></p>
                        <p>Les taux de coût et de facturation en vigueur à la date sont désormais disponibles sur les objets de rôle d’entreprise, d’utilisateur et de tâche dans Workfront. Lorsque les taux d’efficacité de la date sont appliqués à un projet et que les heures sont consignées dans les tâches du projet, les coûts et les recettes sont calculés à l’aide des taux spécifiés pour chaque période.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 29 juin 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Améliorations de la page d’accueil

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Bouton Déléguer le travail pour les widgets Projet, Tâche et Problème</a> <span style="color: #ff0000;"> Nouveau dans Aperçu .</span></p>
                        <p>Fonctionnalité fréquemment demandée de l’ancienne page d’accueil, nous avons maintenant ajouté un bouton délégué aux widgets Mon travail, Mes tâches et Mes problèmes afin que vous puissiez facilement déléguer du travail lorsque vous êtes absent du bureau.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveau widget Panoramas pour la nouvelle page d’accueil</a> <span style="color: #ff0000;"> Nouveau dans Aperçu .</span></p>
                        <p>En plus des options de gestion du travail disponibles dans la nouvelle page d’accueil, vous pouvez désormais afficher un panorama sur votre page d’accueil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle page d’entrée par défaut du contributeur : Nouvelle page d’accueil</a> <span style="color: #ff0000;"> Nouveau dans Aperçu .</span> </p>
                        <p>La nouvelle page d’accueil est désormais la page d’entrée par défaut des comptes du contributeur/demandeur. Cette nouvelle page d’accueil par défaut comprend un certain nombre de widgets spécifiquement sélectionnés pour permettre aux contributeurs de gérer leur travail immédiatement.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Modifications du suivi de travail dans la nouvelle page d’accueil </a> </p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>En fonction des commentaires des utilisateurs, nous avons supprimé le filtre de période et la barre de résumé à l’échelle de la page qui traitaient les tâches en retard et terminées. Les widgets Projet, Tâche et Problème contiennent chacun des fonctionnalités de filtrage intégrées qui vous permettent de personnaliser leur portée individuellement.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 13 septembre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.9</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveaux boutons d’action rapide pour le widget Mon travail</a> </p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>Afin d’étendre davantage votre capacité à gérer le travail directement à partir de la nouvelle page d’accueil, de nouveaux boutons d’action rapide ont été ajoutés au widget Mon travail.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 13 septembre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.9</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelles options de filtre pour la nouvelle page d’accueil</a> </p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>De nouvelles options de filtre sont désormais disponibles pour le widget Mon travail dans Nouvelle page d’accueil. Les options incluent des filtres pour les types d’objets (tâches, problèmes et requêtes) et les états (non prêts, prêts à démarrer, à travailler et terminés).</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Prise en charge terminologique personnalisée de la nouvelle page d’accueil</a> </p><p>[!BADGE en production ]{type=Informative}</p>
                        <p>Pour mieux répondre aux besoins uniques des organisations, New Home utilise désormais une terminologie personnalisée pour les objets telle que définie dans les modèles de mise en page d’une instance. Par exemple, si des objets "Projet" ont été renommés "Campagnes" dans votre instance Workfront, le widget Mes projets s’affichera comme Mes campagnes dans Nouvelle page d’accueil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : 31 août 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Bouton Essayer une nouvelle page d’accueil supprimé pour les comptes désactivés Nouvelle page d’accueil</a> </p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>Le bouton Essayer une nouvelle page d’accueil n’est plus présent pour les comptes pour lesquels la nouvelle page d’accueil a été désactivée. L’administrateur système doit réactiver la nouvelle page d’accueil pour que les utilisateurs puissent utiliser le bouton pour essayer la nouvelle page d’accueil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Changement du jeu de widgets par défaut Nouvelle page d’accueil</a> </p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>Le widget Tâches, qui nécessite l’autorisation de créer des tâches, n’est désormais présent que dans le widget par défaut défini pour les utilisateurs disposant des types de licence Standard, Plan ou Work. En outre, le widget a été automatiquement supprimé des pages d’accueil des utilisateurs avec tous les autres types de licence.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : 17 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour une publication trimestrielle : 17 août 2023</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations de l’expérience lors de l’envoi de documents à SharePoint (GraphAPI)</a></p><p>[!BADGE en production ]{type=Informative}</p><p>Nous avons apporté quelques modifications afin de faciliter la localisation des dossiers lors de l’envoi de documents à vos dossiers SharePoint (GraphAPI).</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 24 août 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : 31 août 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mises à niveau par glisser-déposer pour les intégrations de documents</a></p><p>Nous avons apporté quelques améliorations afin d’ajouter de la clarté et de supprimer l’erreur utilisateur lors du glisser-déposer d’un fichier dans un dossier lié.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 24 août 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : après la version 23.10</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Améliorations des projets

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelles approbations de documents</a> <span style="color: #ff0000;"> Nouveau dans Aperçu .</span></p>
                        <p>Dans cette version, le processus d’approbation a été simplifié pour la création d’approbations et l’approbation/révision de documents, en plus de la nouvelle fonctionnalité.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 12 octobre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Cette fonctionnalité fait partie d’une version par étapes et est actuellement disponible uniquement pour des clients spécifiques.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mises à jour en temps réel sur la liste des tâches</a> </p>
                        <p>[!BADGE en production]{type=Informative}</p>
                        <p>Les listes de tâches sont désormais mises à jour en temps réel. Les modifications apportées à une tâche sont mises à jour dans la liste des tâches, de sorte qu’un utilisateur qui consulte la liste des tâches puisse voir la modification sans actualiser la page.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : déploiement par phases, terminé le 19 octobre 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mise à jour de la conception lors de l’ajout d’un nouveau problème à un projet</a> </p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>Cette mise à jour a été annoncée avec la version 23.3.</p>
                        <p>Nous avons mis à jour la boîte de dialogue Nouveau problème qui s’affiche lors de l’envoi d’un nouveau problème à un projet. Désormais, l’interface correspond à la zone Nouvelle requête qui s’affiche lors de l’envoi d’une nouvelle requête à une file d’attente de requêtes.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 26 juillet 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Recalcul dynamique des champs calculés sur les formulaires</a></p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>Les champs calculés d’un formulaire joint à un objet sont désormais recalculés dynamiquement en temps réel lorsque les valeurs dépendantes d’un formulaire sur la page sont modifiées. Vous pouvez ainsi afficher les résultats mis à jour sans enregistrer le formulaire.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Définition des heures planifiées sur les tâches récurrentes enfants avec le type Durée simple sans attribution</a></p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>Nous avons modifié la façon dont les heures planifiées sont attribuées aux tâches récurrentes sans affectation et avec un type Durée simple . Désormais, lorsque vous définissez Heures planifiées sur une nouvelle tâche récurrente avec un type de durée simple et aucune affectation, les heures sont également allouées aux récurrences individuelles. Avant cette modification, les heures n’étaient pas enregistrées pour des récurrences individuelles lorsque les tâches parentes n’étaient pas affectées.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Modifications du menu principal du contributeur</a> <span style="color: #ff0000;"> Nouveau dans Aperçu .</span></p>
                        <p>Pour mieux informer les contributeurs/demandeurs des fonctionnalités disponibles avec un type de licence Workfront payant, ils peuvent désormais voir toutes les options disponibles dans le menu principal.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Nouvelles améliorations de la version bêta des commentaires</a> </p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>Des améliorations ont été apportées à la section Mises à jour . Elles sont disponibles dans le délai de publication du quatrième trimestre 2023 pour la version bêta de l’expérience de commentaire. Ces améliorations seront disponibles dans l’environnement de production pour tous les clients de la version du quatrième trimestre 2023 (octobre 2023).</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : pendant tout le délai de publication du quatrième trimestre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : à partir de la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10 (sauf indication contraire)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Nouvelles améliorations bêta des tableaux de bord de canevas</a> </p>
                        <p>[!BADGE en production pour version rapide ]{type=Positif}</p>
                        <p>Des améliorations ont été apportées aux tableaux de bord de la zone de travail dans le cadre de la version bêta en cours du quatrième trimestre 2023. Ces améliorations seront disponibles dans l’environnement de production pour tous les clients de la version du quatrième trimestre 2023 (octobre 2023).</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : pendant tout le délai de publication du quatrième trimestre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : à partir de la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour les versions trimestrielles : avec la version 23.10 (sauf indication contraire)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’apparence au cours du quatrième trimestre 2023</a></p><p>Des mises à jour mineures de l’aspect des différentes zones de l’application Adobe Workfront sont effectuées dans le délai du quatrième trimestre 2023. Consultez les notes de mise à jour individuelles pour connaître les dates de publication spécifiques.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : pendant tout le délai de publication du quatrième trimestre 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : passez en revue les notes de mise à jour pour connaître les dates spécifiques</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

## Annonces

### Améliorations apportées à Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de publication du quatrième trimestre 2023. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Publication de fusion Adobe Workfront](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Améliorations du planificateur de scénario Workfront

Aucune mise à jour du planificateur de scénario n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations du Bon à tirer de Workfront

Aucune mise à jour de BAT Workfront n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des objectifs de Workfront

Aucune mise à jour des objectifs de Workfront n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### API version 17

API version 17 a été publiée le 12 octobre 2023. Pour l’API version 17, nous avons modifié certaines ressources et points de terminaison. Certaines des modifications prennent en charge les nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de l’API version 17](/help/quicksilver/wf-api/api/new-api-version-17.md).

Pour plus d’informations sur les versions d’API, voir [Contrôle de version des API et planification de la prise en charge](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version 22.3, voir [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Mises à jour de formation

Découvrez les dernières mises à jour apportées aux programmes d’apprentissage, aux parcours de formation, aux vidéos et aux guides de chaque version de produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section &quot;Nouveautés&quot; du [Page Tutorials Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### Fonctionnalité bientôt supprimée de Workfront

Les fonctionnalités suivantes seront bientôt supprimées de Workfront :

#### Obsolescence de l’application mobile BAT avec la version 23.10

Avec la version 23.10, nous abandonnerons officiellement l’application mobile BAT. L’application mobile Workfront générale a été améliorée avec de nouvelles fonctionnalités de vérification (voir la note de mise à jour sous Améliorations apportées à Workfront Mobile pour plus d’informations) et il est conseillé aux utilisateurs de commencer à l’utiliser pour le travail de vérification dès que possible.

Notez que l’application mobile Workfront requiert une connexion Workfront. Les utilisateurs externes et les invités peuvent continuer à utiliser l’application BAT pour le travail de vérification ; elle n’est toutefois plus prise en charge et ne sera plus disponible avec la version 23.10.

#### Workflows supprimés pour les comptes qui ne les utilisent pas

Pour les comptes qui n’ont jamais créé de workflow dans les panoramas Adobe Workfront, la zone Flux de travail a été supprimée du tableau de bord des panoramas à compter du 11 octobre 2023. Les comptes qui utilisent des workflows y ont toujours accès. Les prochaines versions aborderont la fonctionnalité de scrum améliorée.

<!-- HTML you might need

New table

### add product area name

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

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>

Badge for available in Fast Release

[!BADGE In production for Fast Release ]{type=Positive}
[!BADGE In production ]{type=Informative}



Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
