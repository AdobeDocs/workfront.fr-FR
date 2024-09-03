---
title: Vue d’ensemble de la version du deuxième trimestre 2024
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du deuxième trimestre 2024. L’intégration de ces améliorations dans l’environnement de production s’effectuera tout au long du trimestre.
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bdcfed70-1999-4c40-a38f-12c762c8c1c4
source-git-commit: 21ad93a3438962fd45a6b348960c37402c71a18a
workflow-type: tm+mt
source-wordcount: '2246'
ht-degree: 99%

---

# Vue d’ensemble de la version du deuxième trimestre 2024

Cette page fournit des informations sur les fonctionnalités incluses dans la version du deuxième trimestre 2024. Ces améliorations ont été apportées à l’environnement de production pour l’ensemble des clientes et clients de la version 24.4 des 10 et 11 avril 2024.

<!--The 24.1 release webinar was on January 11, 2024. You can [register for the webinar to view an on-demand recording here](https://webinars.on24.com/adobe_workfront/whatsnewin241?partnerref=releaseoverview).-->
À la place d’un webinaire sur la version, nous vous invitons à vous [inscrire à Adobe Summit](https://summit.adobe.com/na/) pour regarder les sessions Workfront suivantes :

[L’avenir d’Adobe Workfront le 26 mars 2024, pour avoir un aperçu de l’avenir de la planification stratégique et des workflows. ](https://reg.adobe.com/flow/adobe/as24/sessions/page/catalog?search=S302) Découvrez comment l’équipe Workfront prévoit de gérer les fonctionnalités métiers tout au long du cycle de vie marketing, le tout avec une approche centrée sur l’IA qui permet d’automatiser le travail, de simplifier les expériences utilisateurs et d’améliorer la productivité.

[Présentation des calendriers et des outils marketing pour la planification des campagnes de bout en bout](https://reg.adobe.com/flow/adobe/as24/sessions/page/catalog?search=s304) le 28 mars 2024, pour en savoir plus sur les nouvelles fonctionnalités du produit conçues pour vous permettre de gérer et de visualiser les cycles de vie opérationnels de bout en bout.

Vous pouvez également [consulter un fichier PDF](https://acrobat.adobe.com/id/urn:aaid:sc:US:1754831a-dbfe-471d-bca7-386264d90352){target="_blank"} détaillant les nouveautés de la version 24.4.

<span class="preview">Les fonctionnalités hors cycle (sorties en production avant la date de la version du deuxième trimestre 2024) sont surlignées en jaune.</span>

>[!IMPORTANT]
>
>La version 23.3 incluait l’option permettant d’opter pour des versions mensuelles dans votre organisation. Par conséquent, Workfront a modifié le schéma de numérotation des versions afin de tenir compte des suivis de versions mensuels et trimestriels. Le premier chiffre désigne l’année, le second le mois de la version. Exemple : la version d’avril 2024 est 24.4.
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>24.2 (15 février 2024)</li><li>24.3 (14 mars 2024)</li><li>24.4 (11 avril 2024)</li></ul> | <ul><li>24.4 (11 avril 2024)</li></ul> |
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations de la gestion des documents](#document-management-enhancements)
* [Amélioration de l’accueil](#home-enhancements)
* [Améliorations apportées aux projets](#project-enhancements)
* [Améliorations de la gestion des ressources](#resource-management-enhancements)
* [Améliorations du flux de mise à jour et des notifications](#update-stream-and-notification-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">La logique d’affichage et la logique de saut sont désormais disponibles en mode d’aperçu du créateur de formulaire.</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>La version bêta du créateur de formulaire personnalisé vous permet désormais de tester votre logique d’affichage et logique de saut en mode d’aperçu. Auparavant, tous les champs s’affichaient dans l’aperçu même lorsque la logique était appliquée.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 28 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour la clientèle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Les entreprises et les utilisateurs et utilisatrices prennent désormais en charge les champs de formulaire personnalisé avancés.</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les fonctionnalités avancées de formulaire personnalisé telles que les champs de recherche externe et les champs natifs Workfront sont désormais disponibles lorsque vous joignez un formulaire personnalisé à une entreprise ou à un utilisateur ou une utilisatrice.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 14 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour la clientèle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Intégration JumpSeat désormais disponible pour les nouveaux types de packages</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>L’intégration JumpSeat existante est désormais disponible pour les comptes utilisant l’un des nouveaux types de packages (c’est-à-dire Select, Prime ou Ultimate). Vous devez toujours disposer d’un abonnement JumpSeat actif pour activer l’intégration.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : mardi 26 février 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.3 (vendredi 14 mars 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Les champs natifs de Workfront sont disponibles dans la version bêta du créateur de formulaire</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les champs natifs de Workfront sont désormais disponibles pour l’ajout dans vos formulaires personnalisés. Ce nouveau type de champ vous permet d’organiser et de présenter les données à vos utilisateurs et utilisatrices de manière logique, sans avoir à recréer des données existantes dans des champs personnalisés.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 29 février 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.3 (vendredi 14 mars 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Mappage d’attributs désormais disponible pour les organisations qui ont migré vers Adobe IMS</a></p>
                        <p>[!BADGE In production ]{type=Informative}</p><p>Les équipes d’administration système Workfront peuvent désormais configurer le mappage des attributs utilisateur pour les organisations qui ont migré vers Adobe IMS. Cela permet de transmettre les informations des utilisateurs et utilisatrices à Workfront à partir du fournisseur d’authentification unique (SSO) de l’organisation, de sorte qu’il ne soit pas nécessaire de saisir ces données à la fois dans Workfront et dans le fournisseur d’authentification unique.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 22 février 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour l’ensemble des clientes et des clients : 22 février 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Les logiques de saut et d’affichage sont désormais disponibles dans la version bêta du concepteur de formulaires.</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Vous pouvez désormais modifier les logiques d’affichage et de saut existantes et ajouter des nouvelles logiques aux formulaires personnalisés dans la version bêta du concepteur de formulaires. Un générateur de logique convivial permet de définir les champs à afficher ou à ignorer en fonction des sélections dans le formulaire.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 8 février 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.2 (15 février 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter une échéance aux révisions et approbations de documents</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Vous pouvez maintenant spécifier une échéance pour les utilisateurs et utilisatrices ou les équipes affectés à la révision ou à l’approbation d’un document. Les réviseurs et réviseuses et les approbateurs et approbatrices reçoivent des notifications par e-mail 72 heures, puis 24 heures avant l’échéance spécifiée. L’échéance est également répercutée dans le widget Approbations de la nouvelle zone d’accueil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 28 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour la clientèle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Créer et utiliser des modèles d’approbation</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Vous pouvez maintenant créer des modèles d’approbation dans la zone Configuration afin de rationaliser le processus de révision et d’approbation. Les modèles d’approbation vous permettent de rendre le processus de révision et d’approbation plus répétable en
                        <ul>
                            <li>
                                <p>Ajoutant des réviseurs et réviseuses et des approbateurs et approbatrices.</p>
                            </li>
                            <li>
                                <p>Définissant un délai.</p>
                            </li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 28 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour la clientèle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Affichage des informations sur toutes vos approbations en un seul endroit</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Pour vous aider à gérer et analyser vos demandes d’approbation d’un seul coup d’œil, nous avons ajouté les indicateurs clés de performances suivants au widget Toutes les approbations :
                        <ul>
                            <li>
                                <p>Approbations par décision</p>
                            </li>
                            <li>
                                <p>Temps moyen d’approbation</p>
                            </li>
                            <li>
                                <p>Approbations en attente</p>
                            </li>
                            <li>
                                <p>Approbations en retard</p>
                            </li>
                        </ul>
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 28 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour la clientèle : avec la version 24.4 (11 avril 2024)</p>
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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Options de colonne ajoutées aux contrôles d’Administration pour la nouvelle page d’accueil à l’aide des modèles de disposition</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les administrateurs et administratrices peuvent désormais personnaliser les colonnes disponibles pour les utilisateurs et utilisatrices de nouveaux widgets d’accueil spécifiques à l’aide de modèles de disposition. Les options incluent le masquage ou l’affichage des colonnes par défaut et l’ajout de champs existants en tant que nouvelles colonnes.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 2 janvier 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.2 (15 février 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations apportées au workflow de création de dossiers automatisée dans l’intégration Adobe Experience Manager</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Afin de garantir une meilleure adéquation de vos dossiers Adobe Experience Manager avec vos besoins, nous avons apporté quelques mises à jour au workflow des dossiers liés à Adobe Experience Manager.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : mardi 11 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour toute la clientèle : 14 mars 2024</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affectations plus pertinentes ajoutées au workflow Nouvelle tâche</a></p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
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
                                <p>Version de production pour tous les clients : avec la version 24.10 (octobre 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affectations intelligentes plus pertinentes</a></p>
                        <p>[!BADGE In production for Fast Release ]{type=Positive}</p>
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
                                <p>Version de production pour tous les clients : avec la version 24.10 (octobre 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-resource-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Indicateur pour les allocations ajustées manuellement dans l’équilibreur de charge de travail</a></p><p>[!BADGE In production ]{type=Informative}</p><p>Pour plus de clarté sur les ajustements manuels ou les contours dans l’équilibreur de charge de travail, les allocations horaires ajustées manuellement affichent désormais une icône en forme de crayon.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 12 octobre 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.2 (15 février 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Améliorations du flux de mise à jour et des notifications

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelles expériences de commentaires ajoutées aux itérations</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Afin de vous offrir une expérience cohérente dans l’ensemble de l’application, nous avons ajouté la nouvelle expérience de commentaire aux itérations. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 11 avril 2024</p>
                            </li>
                            <li>
                                <p>Production pour toute la clientèle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Suppression de l’accès à la zone de commentaires héritée</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Suppression du bouton (bascule) « Nouveau commentaire » dans la zone Mises à jour pour les projets, les tâches, les problèmes et les documents. Le nouveau commentaire est désormais la seule option par défaut pour ces objets. Grâce à cette modification, vous ne pouvez plus revenir à l’expérience de commentaires héritée. Nous avons également supprimé le paramètre « Afficher le pourcentage d’achèvement pour le statut de la mise à jour » du profil d’une personne.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : mardi 1 avril 2024</p>
                            </li>
                            <li>
                                <p>Production pour toute la clientèle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveau flux de commentaires désormais disponible dans les actions rapides pour les nouveaux widgets de la page d’accueil</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Nous avons maintenant ajouté la nouvelle fonctionnalité de commentaires au bouton d’action rapide « Ajouter une nouvelle mise à jour » dans les widgets Mon travail, Mes projets, Mes tâches et Mes problèmes de la nouvelle page d’accueil.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : samedi 1 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.3 (vendredi 14 mars 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Informations supplémentaires sur les personnes délivrant les commentaires dans la nouvelle expérience de commentaires</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les améliorations suivantes ont été apportées à la nouvelle expérience de commentaire :</p>
                        <ul>
                            <li>
                                <p>Vous pouvez cliquer sur le nom de l’auteur ou de l’autrice du commentaire pour afficher son nom, son rôle et son adresse e-mail dans une zone d’informations. Ces informations peuvent vous aider à identifier la bonne personne si plusieurs utilisateurs ou utilisatrices portent le même nom. Lorsque vous cliquez sur le nom de l’auteur ou de l’autrice du commentaire dans la zone d’informations, son profil d’utilisateur ou d’utilisatrice s’affiche.</p>
                            </li>
                            <li>
                                <p>Votre nom d’utilisateur ou d’utilisatrice est mis en surbrillance dans les commentaires sur lesquels vous êtes tagué lorsque vous êtes mentionné dans le texte du commentaire.</p>
                            </li>
                        </ul>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 29 février 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.3 (vendredi 14 mars 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>  
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">L’onglet Activité du système sur la nouvelle expérience de commentaire prend en charge les commentaires en lecture seule.</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Les commentaires apportés aux enregistrements d’activité du système dans l’expérience de commentaire héritée sont désormais renseignés dans l’onglet Activité du système de la nouvelle expérience de commentaire en lecture seule. Vous ne pouvez pas répondre aux enregistrements d’activité du système dans la nouvelle expérience de commentaire.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 22 février 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.3 (vendredi 14 mars 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr> 
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvel onglet de flux de mise à jour pour capturer les commentaires et les entrées d’activité du système</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Pour vous donner une vue chronologique cohérente des commentaires et des journaux d’activité du système, nous vous proposons un troisième onglet dans la zone Mises à jour de tous les objets. L’onglet « Tous » capture les commentaires des utilisateurs et utilisatrices et les commentaires sur l’activité du système dans un flux cohérent.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 22 février 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.3 (vendredi 14 mars 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouveau flux de commentaires maintenant disponible dans le panneau Résumé</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Nous avons ajouté la nouvelle fonctionnalité de commentaires au panneau Résumé des listes de tâches et de problèmes.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 22 février 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.3 (vendredi 14 mars 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.4 (11 avril 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’apparence pendant le deuxième trimestre 2024</a></p><p>[!BADGE In production ]{type=Informative}</p>
                        <p>Des mises à jour mineures de l’aspect des différentes zones de l’application Adobe Workfront sont effectuées durant le deuxième trimestre 2024. Consultez les notes de mise à jour individuelles pour connaître les dates de publication spécifiques.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : pendant toute la durée de la version du deuxième trimestre 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : passez en revue les notes de mise à jour pour connaître les dates spécifiques.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>   
           </tbody>
        </table>

## Annonces

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent de celui du calendrier de la version du deuxième trimestre 2024. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Améliorations du planificateur de scénarios Workfront

Il n’y a pas de mise à jour du planificateur de scénarios à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de Workfront Proof

Il n’y a pas de mise à jour de Workfront Proof à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des Objectifs Workfront

Il n’y a pas de mise à jour des Objectifs Workfront à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### API version 18

Pour l’API version 18, nous avons modifié certaines ressources et points d’entrée. Certaines des modifications participent à la prise en charge des nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, consultez les [Nouveautés de l’API version 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions et de la prise en charge de l’API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version du deuxième trimestre 2024, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).

