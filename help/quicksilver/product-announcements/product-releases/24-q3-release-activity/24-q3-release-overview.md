---
title: Vue d’ensemble de la version du troisième trimestre 2024
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du troisième trimestre 2024. Ces améliorations sont prévues pour être disponibles dans l’environnement de production tout au long du trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 77%

---

# Vue d’ensemble de la version du troisième trimestre 2024

Cette page fournit des informations sur les fonctionnalités incluses dans la version du troisième trimestre 2024. Ces améliorations sont prévues pour être disponibles dans l’environnement de production tout au long du trimestre.

Le webinaire en direct sur la version 24.7 a été annulé, mais vous pouvez toujours [regarder une démonstration vidéo des fonctionnalités 24.7 ici](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Les fonctionnalités hors cycle (celles qui sont publiées en production avant la date de version du troisième trimestre 2024) sont surlignées en jaune.</span>

>[!IMPORTANT]
>
>La version 23.3 incluait l’option permettant de faire passer votre organisation aux versions mensuelles. Par conséquent, Workfront a modifié le schéma de numérotation des versions afin de tenir compte des suivis de versions mensuels et trimestriels. Le premier chiffre désigne l’année, le second le mois de la version. Exemple : la version d’avril 2024 est 24.4.
>
>Sauf indication contraire, la sortie des versions mensuelles et trimestrielles est prévue le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>24.5 (16 mai 2024)</li><li>24.6 (13 juin 2024)</li><li>24.7 (18 Juillet 2024)</li></ul> | <ul><li>24.7 (18 Juillet 2024)</li></ul> |
>
>Pour plus d’informations sur le processus de publication rapide, voir la section [Activer ou désactiver le processus de publication rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)
* [Améliorations de la gestion financière](#financial-management-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations apportées aux projets](#project-enhancements)
* [Améliorations apportées à la relecture](#proofing-enhancements)
* [Amélioration apportées à la gestion des ressources.](#resource-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Les règles métier sont désormais disponibles</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Les administrateurs peuvent désormais ajouter des règles métier dans la zone Configuration de Workfront.</p>
                        <p>Une règle métier vous permet d’appliquer une validation aux objets Workfront et d’empêcher les utilisateurs de créer, modifier ou supprimer un objet lorsque certaines conditions sont remplies. Les règles sont créées à l’aide d’une formule similaire aux champs calculés dans les formulaires personnalisés.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : vendredi 4 juillet 2024</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                        <p><i>Disponible uniquement pour les organisations dans le cadre du nouveau plan Ultimate.</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Le créateur de formulaire personnalisé est généralement disponible dans Adobe Workfront</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Avec la version 24.7, le créateur de formulaire sera disponible pour tous et deviendra l’expérience par défaut pour la création et la modification de formulaires personnalisés dans Adobe Workfront. Lorsque vous créez un formulaire personnalisé ou ouvrez un formulaire existant, l’espace de travail de style zone de travail du concepteur du formulaire s’affiche.</p>
                        <p>Après cette version, vous n’aurez plus la possibilité de revenir au créateur de formulaires hérité.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : jeudi 19 juin 2024</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Déplacer des objets entre les environnements Workfront avec la promotion d’environnement</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>La promotion d’environnement vous permet de déplacer des objets d’un environnement Workfront vers un autre, par exemple d’un environnement de sandbox vers un environnement de production. Vous pouvez configurer et tester des objets sans aucun risque pour les données et pour les enregistrements de votre organisation. Vous pouvez ensuite déplacer ces objets en production sans avoir à les reconfigurer, ce qui vous permet de gagner du temps et d’économiser des efforts.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de production pour l’ensemble des clientes et clients : avec la version 24.6 (13 juin 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Partager des formulaires personnalisés et des champs personnalisés dans le concepteur de formulaires personnalisés</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Vous pouvez désormais partager des formulaires personnalisés et des champs personnalisés dans le nouveau concepteur de formulaires. Cela permet une meilleure collaboration entre les utilisateurs et les utilisatrices concernant les formulaires personnalisés.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 6 juin 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour l’ensemble des clientes et clients : 13 juin</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Ajouter un nouveau champ personnalisé à partir de la zone Champs</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Vous pouvez désormais ajouter un nouveau champ personnalisé ou un widget directement à partir de la zone Champs dans Workfront, sans avoir à ouvrir de formulaire personnalisé pour créer le champ. Cela vous permet de créer rapidement des champs personnalisés réutilisables.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 6 juin 2024</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Type de champ de liste déroulante à sélection multiple disponible dans le concepteur de formulaires</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Pour vous aider à définir plus facilement les champs de liste déroulante, nous avons ajouté le champ de liste déroulante à sélection multiple au concepteur de formulaires personnalisés. Ce type de champ permet aux utilisateurs et aux utilisatrices de choisir plusieurs options dans une liste déroulante.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : mercredi 4 juin 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour l’ensemble des clientes et des clients : 4 juin 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Champs de dépenses facturables et non facturables disponibles pour les projets et les tâches</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Pour vous aider à visualiser plus facilement les types de dépenses, les dépenses ont été séparées en dépenses facturables et non facturables dans les projets et les tâches. Vous pouvez ajouter les champs suivants aux vues et aux rapports :</p>
                        <ul>
                            <li><p>Coût prévu des dépenses facturables</p></li>
                            <li><p>Coût prévu des dépenses non facturables</p></li>
                            <li><p>Coût réel des dépenses non facturables</p></li>
                            <li><p>Coût réel des dépenses non facturables</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : samedi 10 mai 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour l’ensemble des clientes et des clients : 10 mai 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations de Workfront pour Experience Manager Assets et Assets Essentials</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Nous avons apporté les améliorations suivantes aux intégrations de Workfront pour Experience Manager Assets et Assets Essentials :</p>
                        <ul>
                            <li><p>L’intégration prend désormais en charge GCP en tant que fournisseur de services cloud. AWS et Azure étaient auparavant pris en charge.</p></li>
                            <li><p>La taille maximale des fichiers envoyés à Experience Manager par le biais de l’intégration est passée à 30 Go. Auparavant, la limite était de 5 Go.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : vendredi 27 juin 2024</p>
                            </li>
                            <li>
                                <p>Production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Modifier la date d’engagement et la condition d’une tâche et d’un problème à partir de l’en-tête ou de la section Détails</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Pour faciliter la mise à jour des tâches et des problèmes, nous avons désormais ajouté les champs Date d’engagement et Condition en tant qu’options à ajouter aux en-têtes de tâches et de problèmes et à la section Détails dans un modèle de mise en page. Les utilisateurs et les utilisatrices peuvent désormais mettre à jour ces champs à partir de l’en-tête ou de la section Détails d’une page lorsqu’ils sont affectés au modèle de mise en page modifié.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 30 mai 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.6 (13 juin 2024)</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affectations plus pertinentes ajoutées au workflow Nouvelle tâche</a></p>
                        [!BADGE In production for Fast Release &#x200B;]{type=Positive}
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
                        </ul>
                    <p><i>Cette fonctionnalité a été supprimée de la prévisualisation et de la production en version rapide.</i></p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affectations intelligentes plus pertinentes</a></p>
                        [!BADGE In production for Fast Release &#x200B;]{type=Positive}
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
                        </ul>
                    <p><i>Cette fonctionnalité a été supprimée de la prévisualisation et de la production en version rapide.</i></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">Mises à jour de sécurité pour le lecteur de vérification pour bureau</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>La mise à jour de sécurité du lecteur de vérification pour bureau Workfront Proof version 2.1.35 fournit des correctifs de sécurité pour les vulnérabilités qui ont été identifiées dans les versions précédentes.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de prévisualisation : vendredi 4 juillet 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : 4 juillet 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Les congés sont désormais reflétés dans l’équilibreur de charge de travail</a>.</p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Pour ajuster facilement le travail lorsque la personne cessionnaire principale d’une tâche a programmé un congé, l’équilibreur de charge de travail réalloue désormais les heures aux personnes principales et secondaires lorsque la chronologie du projet est recalculée.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 6 juin 2024</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Modification du serveur principal dans les guides intégrés au produit</a></p>
                        <p>Nous apporterons un changement technologique à nos guides intégrés au produit au cours des prochaines semaines. Bien que nous ayons essayé de minimiser l’impact de cette transition, certains utilisateurs peuvent rencontrer des guides qu’ils ont déjà vus.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Production pour tous les clients : de manière progressive jusqu’à la mi-août 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience est désormais disponible pour plus d’organisations Workfront</a>.</p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Pour permettre aux organisations d’accéder aux avantages d’Adobe Unified Experience, nous avons commencé à la mettre à la disposition des clientes et des clients Workfront existants. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : vendredi 20 juin 2024</p>
                            </li>
                            <li>
                                <p>Production pour les clients spécifiés : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">Adobe Unified Shell est mis à disposition selon un déploiement échelonné. Des organisations supplémentaires seront intégrées à Adobe Unified Shell avec les versions 24.10 et 25.1. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Bouton Aide supprimé de la barre de navigation principale</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Pour unifier l’expérience pour les utilisateurs et les utilisatrices qui ne sont pas sur Unified Shell, le bouton Aide de la barre de navigation principale a été supprimé. Ce bouton, qui n’est pas présent pour les utilisateurs et utilisatrices de Unified Shell, redirigeait vers la documentation de Workfront et était redondant avec le bouton d’aide similaire disponible pour toutes les personnes dans le menu principal.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 6 juin 2024</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Amélioration de l’expérience d’utilisation pour les utilisateurs et les utilisatrices disposant d’un accès limité aux objets</a></p>
                        [!BADGE In production &#x200B;]{type=Informative}
                        <p>Lorsqu’une personne n’a pas accès à un objet, le message « Pas d’accès » s’affiche partout où le nom de l’objet s’affiche dans Workfront. Cette expérience améliorée s’applique également à l’API Workfront.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : jeudi 27 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.5 (16 mai 2024)</p>
                            </li>
                            <li>
                                <p>Production pour la version trimestrielle : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’aspect pendant le troisième trimestre 2024</a></p>
                        <p>Des mises à jour mineures de l’aspect des différentes zones de l’application Adobe Workfront sont effectuées durant le troisième trimestre 2024. Consultez les notes de mise à jour individuelles pour connaître les dates de publication spécifiques.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : pendant toute la durée de la version du troisième trimestre 2024</p>
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

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent de celui du calendrier de la version du troisième trimestre 2024. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

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

Pour plus d’informations sur les mises à jour de maintenance effectuées au cours de la version du troisième trimestre 2024, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/fr/docs/workfront-known-issues/releases/current-updates).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/fr/docs/workfront-learn/tutorials-workfront/home).
