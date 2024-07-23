---
title: Vue d’ensemble de la version du troisième trimestre 2024
description: Cette page fournit des informations sur les fonctionnalités incluses dans la version du troisième trimestre 2024. Ces améliorations sont prévues pour être disponibles dans l’environnement de production tout au long du trimestre.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 76b44f3d5ff7d7747da801a051a457157e08ea4a
workflow-type: tm+mt
source-wordcount: '1849'
ht-degree: 44%

---

# Vue d’ensemble de la version du troisième trimestre 2024

Cette page fournit des informations sur les fonctionnalités incluses dans la version du troisième trimestre 2024. Ces améliorations sont prévues pour être disponibles dans l’environnement de production tout au long du trimestre.

Le webinaire de la version 24.7 en direct a été annulé, mais vous pouvez toujours [regarder une démonstration vidéo des fonctionnalités 24.7 ici](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">Les fonctionnalités hors cycle (celles qui sont publiées en production avant la date de version du troisième trimestre 2024) sont surlignées en jaune.</span>

>[!IMPORTANT]
>
>La version 23.3 incluait l’option permettant de faire passer votre organisation aux versions mensuelles. Par conséquent, Workfront a modifié le schéma de numérotation des versions afin de tenir compte des suivis des versions mensuelles et trimestrielles. Le premier chiffre désigne l’année, le second le mois de la version. Exemple : la version d’avril 2024 est 24.4.
>
>Sauf indication contraire, les versions mensuelles et trimestrielles sont prévues pour être disponibles le jeudi de la deuxième semaine complète du mois.
>
>| Version mensuelle | Version trimestrielle |
>|----|----|
>| <ul><li>24.5 (16 mai 2024)</li><li>24.6 (13 juin 2024)</li><li>24.7 (18 juillet 2024)</li></ul> | <ul><li>24.7 (18 juillet 2024)</li></ul> |
>
>Pour plus d’informations sur le processus de version rapide, consultez [Activer ou désactiver le processus de version rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations Adobe Workfront

* [Améliorations d’administration](#administrator-enhancements)
* [Améliorations de la gestion financière](#financial-management-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations des projets](#project-enhancements)
* [Améliorations de la vérification](#proofing-enhancements)
* [Améliorations de la gestion des ressources](#resource-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> Des règles métier sont désormais disponibles</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Les administrateurs peuvent désormais ajouter des règles de fonctionnement dans la zone Configuration de Workfront.</p>
                        <p>Une règle de fonctionnement vous permet d’appliquer la validation aux objets Workfront et d’empêcher les utilisateurs de créer, modifier ou supprimer un objet lorsque certaines conditions sont remplies. Les règles sont créées à l’aide d’une formule similaire aux champs calculés dans les formulaires personnalisés.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 4 juillet 2024</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Concepteur de formulaire personnalisé généralement disponible dans Adobe Workfront</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Avec la version 24.7, le concepteur de formulaires sera disponible en général et deviendra l’expérience par défaut pour la création et la modification de formulaires personnalisés dans Adobe Workfront. Lorsque vous créez un formulaire personnalisé ou ouvrez un formulaire existant, l’espace de travail du concepteur de formulaire dans le style de zone de travail s’affiche.</p>
                        <p>Après cette version, vous n’aurez plus la possibilité de revenir à l’ancien créateur de formulaires.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : jeudi 19 juin 2024</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> Déplacer des objets entre les environnements Workfront avec promotion d’environnement</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>La promotion d’environnement vous permet de déplacer des objets d’un environnement Workfront vers un autre, par exemple d’un environnement de test vers un environnement de production. Vous pouvez configurer et tester des objets sans aucun risque pour les données et les enregistrements de votre entreprise. Vous pouvez ensuite déplacer ces objets en production sans avoir à les reconfigurer, ce qui vous permet de gagner du temps et vous évite d'avoir à les reconfigurer.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.6 (13 juin 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Partager des formulaires et des champs personnalisés dans le concepteur de formulaire personnalisé</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Vous pouvez désormais partager des formulaires personnalisés et des champs personnalisés dans le nouveau concepteur de formulaires. Cela permet une plus grande collaboration entre les utilisateurs sur les formulaires personnalisés.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 6 juin 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour tous les clients : 13 juin</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> Ajoutez un nouveau champ personnalisé à partir de la zone Champs</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Vous pouvez désormais ajouter un nouveau champ ou widget personnalisé directement à partir de la zone Champs de Workfront, sans ouvrir de formulaire personnalisé pour créer le champ. Vous pouvez ainsi créer rapidement des champs personnalisés réutilisables.</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Type de champ déroulant à sélection multiple disponible sur le concepteur de formulaire</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Pour vous aider à définir plus facilement des champs de liste déroulante, nous avons ajouté le champ Liste déroulante à sélection multiple au concepteur de formulaire personnalisé. Ce type de champ permet aux utilisateurs de choisir plusieurs options dans une liste déroulante.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : mercredi 4 juin 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : 4 juin 2024</span></p>
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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Champs de dépenses facturables et non facturables disponibles pour les projets et les tâches</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Pour vous aider à visualiser plus facilement les types de dépenses, les dépenses ont été séparées en dépenses facturables et non facturables sur les projets et les tâches. Vous pouvez ajouter les champs suivants aux vues et aux rapports :</p>
                        <ul>
                            <li><p>Coût prévu des dépenses facturables</p></li>
                            <li><p>Coût des dépenses non facturables planifié</p></li>
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
                                <p><span class="preview">Production pour tous les clients : 10 mai 2024</span></p>
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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations de Workfront pour Experience Manager Assets et les Assets Essentials</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Nous avons apporté les améliorations suivantes aux intégrations Workfront pour Experience Manager Assets et Assets Essentials :</p>
                        <ul>
                            <li><p>L’intégration prend désormais en charge GCP en tant que fournisseur de services cloud. AWS et Azure étaient auparavant pris en charge.</p></li>
                            <li><p>La taille limite des fichiers envoyés à Experience Manager par le biais de l’intégration a été augmentée à 30 Go. Auparavant, la limite était de 5 Go.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 27 juin 2024</p>
                            </li>
                            <li>
                                <p>Production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Modifiez la tâche et publiez la Date et la condition de validation de la tâche à partir de l’en-tête ou de la section Détails</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Pour faciliter la mise à jour des tâches et des problèmes, nous avons maintenant ajouté les champs Date de validation et Condition en tant qu’options à ajouter à la section En-têtes de tâche et de problème et Détails dans un modèle de mise en page. Les utilisateurs peuvent désormais mettre à jour ces champs à partir de l’en-tête ou de la section Détails d’une page lorsqu’ils sont affectés au modèle de mise en page modifié.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 30 mai 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.6 (13 juin 2024)</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                        <p><span class="preview">Cette fonctionnalité a été temporairement supprimée de la production pour les clients qui ne sont pas sur le calendrier de publication rapide.</span></p>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affectations plus pertinentes ajoutées au workflow Nouvelle tâche</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Nous avons ajouté la même fonctionnalité pour des affectations intelligentes plus pertinentes au champ Affectations dans la zone Nouvelle tâche lors de l’ajout d’une tâche à un projet et dans une liste de tâches de projet.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 13 février 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.5 (16 mai 2024)</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                        <p><span class="preview">Cette fonctionnalité a été temporairement supprimée de la production pour les clients qui ne sont pas dans le calendrier de publication rapide.</span>&lt;/
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affectations intelligentes plus pertinentes</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Nous avons modifié l’algorithme utilisé par Workfront pour calculer et suggérer des affectations intelligentes pour les tâches. Le nouvel algorithme s’applique aux zones suivantes de Workfront où vous affectez une tâche : listes de tâches, zone Affectations dans l’en-tête de la tâche, Accueil et panneau Résumé.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 21 décembre 2023</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.5 (16 mai 2024)</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Améliorations de la vérification

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}"> Mises à jour de sécurité pour la visionneuse de vérification de l’appli de bureau </a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>La mise à jour de sécurité de Workfront Proof Desktop Proofing Viewer 2.1.35 fournit des correctifs de bogues de sécurité pour les vulnérabilités identifiées dans les versions précédentes.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 4 juillet 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Production pour tous les clients : 4 juillet 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">Le temps de pause se reflète désormais dans l’équilibreur de charge de travail</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Pour régler facilement le travail lorsque le responsable principal d’une tâche a programmé un congé, l’équilibreur de charge de travail réalloue désormais les heures aux utilisateurs principaux et secondaires lorsque la chronologie du projet est recalculée.</p>
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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Modification du serveur principal vers les guides internes au produit</a></p>
                        <p>Au cours des prochaines semaines, nous allons mettre en oeuvre un changement technologique pour nos guides intégrés au produit. Bien que nous ayons essayé de minimiser l’impact de cette transition, certains utilisateurs peuvent rencontrer des guides qu’ils ont précédemment vus.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Production pour tous les clients : par incréments jusqu’à la mi-août 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience désormais disponible pour plus d’organisations Workfront</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Pour permettre aux entreprises d’accéder aux avantages de l’expérience unifiée Adobe, nous avons commencé à la mettre à la disposition des clients Workfront existants. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 20 juin 2024</p>
                            </li>
                            <li>
                                <p>Production pour des clients spécifiés : avec la version 24.7 (18 juillet 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">L'Adobe Unified Shell est rendu disponible dans un déploiement par étapes. D’autres organisations seront intégrées à l’Adobe Unified Shell avec les versions 24.10 et 25.1. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Bouton d’aide supprimé de la barre de navigation principale</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Pour unifier l’expérience pour les utilisateurs qui ne sont pas sur un Shell unifié, le bouton Aide de la barre de navigation principale a été supprimé. Ce bouton, qui n’est pas présent pour les utilisateurs de Shell unifié, est lié à la documentation de Workfront et a été redondant avec un bouton d’aide similaire disponible pour tous les utilisateurs dans le menu principal.</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Amélioration de l’expérience de l’interface utilisateur pour les utilisateurs disposant d’un accès limité aux objets</a></p>
                        [!BADGE In production ]{type=Informative}
                        <p>Lorsqu’un utilisateur n’a pas accès à un objet, il voit "Aucun accès" partout où ce nom s’affiche dans Workfront. Cette expérience améliorée s’applique également à l’API Workfront.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : jeudi 27 mars 2024</p>
                            </li>
                            <li>
                                <p>Production pour une version rapide : avec la version 24.5 (16 mai 2024)</p>
                            </li>
                            <li>
                                <p>Production pour une version trimestrielle : avec la version 24.7 (vendredi 18 juillet 2024)</p>
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

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent de celui du calendrier de la version du troisième trimestre 2024. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité de version d’Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Améliorations du planificateur de scénarios Workfront

Aucune mise à jour du planificateur de scénario n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de l’épreuve Workfront

Aucune mise à jour de l’épreuve Workfront n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des Objectifs Workfront

Aucune mise à jour des Objectifs Workfront n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### API version 18

Pour l’API version 18, nous avons modifié certaines ressources et points d’entrée. Certaines des modifications participent à la prise en charge des nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, consultez les [Nouveautés de l’API version 18](/help/quicksilver/wf-api/api/new-api-version-18.md).

Pour plus d’informations sur les versions d’API, consultez [Contrôle de version des API et planification de la prise en charge](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées au cours de la version du troisième trimestre 2024, voir [Mises à jour de maintenance de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr).

### Mises à jour de formation

Découvrez les dernières mises à jour apportées aux programmes de formation, aux parcours de formation, aux vidéos et aux guides de chaque version de produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).
