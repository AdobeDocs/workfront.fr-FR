---
title: Vue d’ensemble de la version du quatrième trimestre 2023
description: Vue d’ensemble de la version du quatrième trimestre 2023
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6c14bd61-60b1-49aa-84bd-d494a226d70e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '2773'
ht-degree: 99%

---

# Vue d’ensemble de la version du quatrième trimestre 2023

Cette page fournit des informations sur les fonctionnalités incluses dans la version du quatrième trimestre 2023. Ces améliorations devraient être disponibles dans l’environnement de production pour toute la clientèle avec la version 23.10 les 26 et 27 octobre 2023.

<!--
These enhancements will be included in the following releases:

>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>23.8 (August 31, 2023)</li><li>23.9 (September 28, 2023)</li><li>23.10 (October 26, 2023)</li></ul>| <ul><li>23.10 (Week of October 26, 2023)</li></ul>|
-->

Le webinaire sur la version 23.10 a eu lieu le 5 octobre 2023. Vous pouvez [vous inscrire ici au webinaire pour regarder un enregistrement à la demande](https://webinars.on24.com/adobe_workfront/whatsnewin2310?partnerref=releasenotes).

<span class="preview">Les fonctionnalités hors cycle (celles qui sont publiées en production avant la date de publication du quatrième trimestre 2023) sont surlignées en jaune.</span>

>[!IMPORTANT]
>
>La version 23.3 incluait l’option permettant d’opter pour des versions mensuelles dans votre organisation. Par conséquent, Workfront modifie le schéma de numérotation des versions afin de tenir compte des suivis des versions mensuelles et trimestrielles.
>
>* Si vous être sur le suivi de **version rapide (mensuel)**, la version suivant la version 23.3 est la version **23.8**, publiée le 31 août 2023.
> * Si vous êtes sur le suivi **trimestriel** des versions, la version suivant la version 23.3 est la version **23.10**, publiée la semaine du 26 octobre 2023.
> 
> Les versions trimestrielles incluront les fonctionnalités de trois versions mensuelles. Par exemple, la version trimestrielle 23.10 comprendra les fonctionnalités publiées dans les versions mensuelles 23.8, 23.9 et 23.10.
>
>Les versions mensuelles et trimestrielles devraient être disponibles le dernier jeudi du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>23.8 (31 août 2023)</li><li>23.9 (28 septembre 2023)</li><li>23.10 (26 octobre 2023)</li></ul> | <ul><li>23.10 (Semaine du 26 octobre 2023)</li></ul> |
>| <ul><li>Pas de version (novembre 2023)</li><li>Pas de version (décembre 2023)</li><li>24.1 (janvier 2024)</li></ul> | <ul><li>24.1 (janvier 2024)</li></ul> |
>
>Pour plus d’informations sur le processus de version rapide, consultez l’article [Activer ou désactiver le processus de version rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations des panoramas](#boards-enhancements)
* [Améliorations de la gestion financière](#financial-management-enhancements)
* [Amélioration de l’accueil](#home-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations apportées aux projets](#project-enhancements)
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
                        <p><span class="bold">Dates de sortie</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Les décisions relatives aux épreuves et documents sont disponibles pour les clientes et les clients des anciens modèles de licence.</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>La clientèle héritée qui n’a pas encore migré vers le nouveau modèle de licence Adobe Workfront peut désormais afficher les données relatives au nombre de décisions en matière d’épreuves/documents par personne et par mois, dans un rapport unique. Ces données sont disponibles lorsque vous exécutez un rapport Décisions des utilisateurs et utilisatrices.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour toute la clientèle : 12 octobre 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>            
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Les champs calculés des formulaires personnalisés peuvent désormais utiliser le caractère générique $$USER.</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Le caractère générique $$USER est maintenant disponible dans les champs personnalisés calculés et les champs de recherche externes du nouveau créateur de formulaire.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 5 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter à un formulaire personnalisé des options de valeur provenant d’une API externe</a></p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Un nouveau type de champ, <strong>Recherche externe</strong>, est désormais disponible dans le créateur de formulaire personnalisé. Lorsque des données sont stockées sur un système externe, ce type de champ vous permet de charger des options à partir d’une API externe et de filtrer selon d’autres valeurs de champ dans le formulaire personnalisé.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 14 septembre 2023</p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.9</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Les sous-tâches sont désormais disponibles sur les panoramas Adobe Workfront.</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Lorsque vous ajoutez une carte connectée à un panorama pour une tâche Workfront, toutes les sous-tâches existantes sont importées sur la carte. De plus, lorsque vous créez une sous-tâche sur une carte connectée, une sous-tâche est ajoutée à la tâche Workfront.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour accès anticipé aux panoramas : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations de l’affectation des utilisateurs et des utilisatrices aux panoramas et aux cartes</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Des améliorations ont été apportées pour accroître la flexibilité lors de l’ajout d’utilisateurs et d’utilisatrices aux panoramas et aux cartes dans les panoramas Adobe Workfront.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 21 août 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour toute la clientèle : 24 août 2023</span>
                            </li> 
                       </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des documents sur les cartes connectées</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Vous pouvez désormais joindre des documents sur des cartes connectées dans les panoramas Adobe Workfront. Tous les documents que vous ajoutez sur la carte sont accessibles dans l’onglet des documents de la tâche ou du problème connecté(e), et les mêmes types de fichiers sont pris en charge dans les deux zones.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 21 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour accès anticipé aux panoramas : 24 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Documents disponibles sur les cartes connectées en lecture seule</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Désormais, sur les panoramas Adobe Workfront, les cartes connectées permettent la visualisation de documents tels que des images et des PDF. Vous pouvez soit prévisualiser un document dans le navigateur, soit le télécharger sur votre ordinateur. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 3 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour accès anticipé aux panoramas : 10 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Maintenant, la vue en panorama d’un projet est disponible également pour les problèmes.</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Vous pouvez désormais accéder à une vue en panorama de la liste des problèmes d’un projet. Le tableau Kanban offre une manière plus visuelle de suivre la progression des problèmes, par rapport à une simple visualisation sous forme de liste. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 3 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour accès anticipé aux panoramas : S.O.</p>
                            </li>
                             <li>
                                <p>Production pour la version rapide : S.O.</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>    
           </tbody>
        </table>

### Améliorations de la gestion financière

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Fonctionnalités</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Dates de publication</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Date d’entrée en vigueur des taux de facturation et de coût</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>La date d’entrée en vigueur des coûts et des taux de facturation est désormais disponible sur les objets « Entreprise », « Utilisateur ou utilisatrice » et « Fonction » dans Workfront. Lorsque les taux de date d’entrée en vigueur sont appliqués à un projet et que les heures sont consignées dans les tâches du projet, les coûts et les revenus sont calculés à l’aide des taux spécifiés pour chaque période.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 29 juin 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Bouton de délégation du travail pour les widgets de projets, de tâches et de problèmes</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Conformément à vos demandes, un bouton « Déléguer » a été ajouté aux widgets « Mon travail », « Mes tâches » et « Mes problèmes » pour faciliter la délégation en cas d’absence du bureau. Notez que la délégation de travail doit être activée dans votre environnement Workfront pour que le bouton apparaisse.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveau widget de panoramas pour une nouvelle page d’accueil</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les options de gestion du travail disponibles dans la nouvelle page d’accueil s’enrichissent d’une nouveauté majeure : vous pouvez désormais afficher un panorama dans votre page d’accueil.
</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle page de destination par défaut du contributeur ou de la contributrice : la nouvelle page d’accueil</a>  </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>La nouvelle page d’accueil est désormais la page de destination par défaut pour les comptes des personnes qui contribuent ou émettent des requêtes. Cette nouvelle page d’accueil par défaut comprend un certain nombre de widgets spécialement sélectionnés pour permettre aux contributeurs et aux contributrices de gérer leur travail immédiatement.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Changements dans le suivi du travail dans la nouvelle page d’accueil</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Pour répondre aux commentaires des utilisateurs et des utilisatrices,le filtre de période à l’échelle de la page et la barre de résumé des tâches dues et terminées ont été supprimés. Les widgets Projet, Tâche et Problème sont tous dotés de fonctions de filtrage intégrées qui vous permettent de personnaliser leur portée au cas par cas.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 13 septembre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.9</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveaux boutons d’action rapide pour le widget « Mon travail »</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>De nouveaux boutons d’action rapide ont été ajoutés au widget « Mon travail », vous permettant de gérer vos tâches directement depuis la nouvelle page d’accueil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 13 septembre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.9</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelles options de filtrage pour la nouvelle page d’accueil</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>De nouvelles options de filtrage sont désormais disponibles pour le widget « Mon travail » dans la nouvelle page d’accueil. Les options comprennent des filtres pour les types d’objets (tâches, problèmes et requêtes) et les statuts (non prêt, prêt à démarrer, en train de travailler sur et terminé).</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Prise en charge de la terminologie personnalisée pour la nouvelle page d’accueil</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Pour répondre plus efficacement aux besoins spécifiques des organisations, la nouvelle page d’accueil utilise désormais une terminologie personnalisée conforme aux définitions des objets dans les modèles de mise en page d’une instance. Par exemple, si les objets « Projet » ont été renommés « Campagnes » dans votre instance Workfront, le widget « Mes projets » s’affichera à la place de « Mes campagnes » dans la nouvelle page d’accueil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour toute la clientèle : 31 août 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Le bouton « Essayer la nouvelle page d’accueil » a été supprimé pour les comptes qui ont désactivé la nouvelle page d’accueil.</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Le bouton « Essayer la nouvelle page d’accueil » n’est plus présent pour les comptes qui ont désactivé la nouvelle page d’accueil. Pour utiliser le bouton permettant d’essayer la nouvelle page d’accueil, les utilisateurs et les utilisatrices doivent d’abord la réactiver via l’administration système.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Passer au jeu de widgets par défaut de la nouvelle page d’accueil</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Le widget « À faire », qui nécessite une autorisation pour créer des tâches, est désormais inclus dans le jeu de widgets par défaut uniquement pour les utilisateurs et les utilisatrices disposant des types de licence Standard, Plan ou Travail. De plus, ce widget a été automatiquement supprimé des pages d’accueil des utilisateurs et des utilisatrices disposant de tous les autres types de licence.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : 17 août 2023</p>
                            </li>
                            <li>
                                <p>Production pour la version trimestrielle : 17 août 2023</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations de l’expérience lors de l’envoi de documents à SharePoint (GraphAPI)</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Nous avons simplifié la localisation des dossiers lors de l’envoi de documents vers vos dossiers SharePoint (GraphAPI).</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 24 août 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour toute la clientèle : 31 août 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations de la fonction « glisser-déposer » pour les intégrations de documents</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Nous avons apporté des améliorations pour créer de la clarté et éviter les erreurs d’utilisation lors du glisser-déposer d’un fichier dans un dossier lié.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 24 août 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour toute la clientèle : après la version 23.10</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveau processus d’approbation de documents</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Dans cette version, le processus d’approbation a été simplifié pour la création et la gestion des approbations de documents, en plus de l’intégration de nouvelles fonctionnalités.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 12 octobre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Cette fonctionnalité fait partie d’une version déployée de manière progressive et n’est actuellement disponible que pour certaines personnes.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Mise à jour en temps réel de la liste des tâches</a> </p>
                        <p>[!BADGE In production]{type=Informative}</p>
                        <p>Les listes de tâches sont désormais mises à jour en temps réel. Les modifications apportées à une tâche sont mises à jour dans la liste de tâches, de sorte qu’un utilisateur ou une utilisatrice qui consulte la liste de tâches puisse voir la modification sans actualiser la page.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour toute la clientèle : déploiement progressif, achevé le 19 octobre 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">La conception a été mise à jour pour l’ajout d’un nouveau problème à un projet.</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Cette mise à jour a été annoncée avec la version 23.3.</p>
                        <p>Nous avons mis à jour la zone Nouveau problème qui s’affiche lors de la soumission d’un nouveau problème à un projet. Désormais, l’interface correspond à la zone Nouvelle demande qui s’affiche lors de la soumission d’une nouvelle demande à une file d’attente des demandes.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 26 juillet 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Les champs calculés dans les formulaires sont désormais recalculés de manière dynamique.</a></p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les champs calculés d’un formulaire joint à un objet sont désormais recalculés dynamiquement en temps réel lorsque les valeurs dépendantes d’un formulaire sur la page sont modifiées. Vous pouvez ainsi afficher les résultats mis à jour sans enregistrer le formulaire.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Définir le nombre d’heures prévues sur les tâches enfants récurrentes avec un type de durée simple sans affectations</a></p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Nous avons modifié le mode d’affectation du nombre d’heures prévues aux tâches récurrentes sans affectations et avec un type de durée simple. Désormais, lorsque vous définissez un nombre d’heures prévues sur une nouvelle tâche récurrente avec un type de durée simple et sans affectations, les heures sont également affectées aux récurrences individuelles. Avant cette modification, les heures n’étaient pas enregistrées pour les récurrences individuelles lorsque les tâches parent n’étaient pas affectées.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 août 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Modifications dans le menu principal des contributeurs et contributrices</a> </p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Afin de mieux informer les personnes contributrices et demandeuses à propos des fonctionnalités disponibles avec un type de licence Workfront payant, elles peuvent désormais voir toutes les options disponibles dans le menu principal.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 12 octobre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 23.10</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 23.10</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Améliorations de la version bêta de la nouvelle expérience de commentaires</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les améliorations de la section « Mises à jour » seront disponibles dans la version bêta de l’expérience de commentaires au cours du quatrième trimestre 2023. Ces améliorations seront disponibles dans l’environnement de production pour toute la clientèle avec la version du quatrième trimestre 2023 (octobre 2023).</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : tout au long de la période de publication du quatrième trimestre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour la version trimestrielle : avec la version 23.10 (sauf indication contraire)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Nouvelles améliorations de la version bêta des tableaux de bord de zones de travail</a> </p>
                        <p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les améliorations des tableaux de bord des zones de travail seront disponibles dans le cadre de la version bêta en cours pendant le quatrième trimestre 2023. Ces améliorations seront disponibles dans l’environnement de production pour toute la clientèle avec la version du quatrième trimestre 2023 (octobre 2023).</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : tout au long de la période de publication du quatrième trimestre 2023<br /></p>
                            </li>
                            <li>
                                <p>Production pour la version rapide : avec la version 23.8</p>
                            </li>
                            <li>
                                <p>Production pour la version trimestrielle : avec la version 23.10 (sauf indication contraire)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Mise à jour de l’apparence et de la convivialité au cours du quatrième trimestre 2023</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Des mises à jour mineures de l’aspect et de la convivialité de différentes parties de l’application Adobe Workfront seront réalisées au cours du quatrième trimestre 2023. Consultez les notes de mise à jour individuelles pour connaître les dates de publication spécifiques.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : tout au long de la période de publication du quatrième trimestre 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : passez en revue les notes de mise à jour pour connaître les dates spécifiques.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

## Annonces

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à une cadence autre que le calendrier des versions du quatrième trimestre 2023. Pour plus d’informations sur les dernières fonctionnalités, consultez la section [Activité Version Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Améliorations du planificateur de scénarios Workfront

Il n’y a pas de mise à jour du planificateur de scénarios à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de Workfront Proof

Il n’y a pas de mise à jour de Workfront Proof à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des Objectifs Workfront

Il n’y a pas de mise à jour des Objectifs Workfront à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Version 17 de l’API

La version 17 de l’API a été publiée le 12 octobre 2023. Pour la version 17 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 17 de l’API](/help/quicksilver/wf-api/api/new-api-version-17.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions de l’API et de la prise en charge](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version 22.3, consultez [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/en/docs/workfront-known-issues/releases/current-updates).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, voir la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home).

### Fonctionnalités bientôt supprimées de Workfront

Les fonctionnalités suivantes seront bientôt supprimées de Workfront :

#### Obsolescence de l’application mobile Workfront Proof avec la version 23.10

L’application mobile Workfront Proof sera officiellement supprimée avec la version 23.10. L’application mobile générale de Workfront a été améliorée avec une nouvelle fonctionnalité de relecture (voir la note de version sous « Améliorations apportées à Workfront Mobile » pour plus d’informations). Il est recommandé aux utilisateurs et aux utilisatrices de commencer à l’utiliser pour le travail de relecture dès que possible.

Notez que l’application mobile Workfront nécessite une connexion Workfront. Les utilisateurs et les utilisatrices externes, personnes invitées incluses, peuvent toujours utiliser l’application Workfront Proof pour les travaux de relecture. Cependant, elle n’est plus prise en charge et deviendra indisponible avec la version 23.10.

#### Flux de travail supprimés pour les comptes qui ne les utilisent pas.

Pour les comptes n’ayant jamais créé de flux de travail dans les panoramas Adobe Workfront, la zone de flux de travail a été supprimée du tableau de bord des panoramas au 11 octobre 2023. Les comptes qui utilisent des flux de travail y ont toujours accès. L’amélioration de la fonctionnalité scrum sera abordée dans les prochaines versions.

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
