---
title: Vue d’ensemble de la version 22.4
description: Vue d’ensemble de la version 22.4
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 04b09d8f-71bf-4c5b-b2f3-09c714740969
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '3232'
ht-degree: 99%

---

# Vue d’ensemble de la version 22.4

Cette page fournit des informations sur les fonctionnalités incluses dans la version 22.4.

Ces améliorations ont été apportées à l’environnement de production avec la version 22.4 des 6 et 7 octobre 2022.

## Améliorations apportées à Adobe Workfront

* [Améliorations apportées aux administrateurs et administratrices](#administrator-enhancements)

* [Améliorations apportées aux projets](#project-enhancements)

* [Améliorations de la méthode Agile](#agile-enhancements)

* [Amélioration apportées à la gestion des ressources.](#resource-management-enhancements)

* [Autres améliorations](#other-enhancements)


### Améliorations apportées aux administrateurs et administratrices

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
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
<tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Utiliser des statuts Déverrouillé dans des processus d’approbation
</a></p> <p>Cette fonctionnalité a été supprimée de la version de production 22.3. Cette fonctionnalité devrait être mise en production ultérieurement.</p> 
<p>Pour vous permettre de mieux contrôler les processus et les statuts d’approbation dans votre système, nous avons autorisé la création d’un processus d’approbation basé sur un statut de système déverrouillé. De plus, vous pouvez désormais déverrouiller tout statut déjà utilisé dans un processus d’approbation. Auparavant, un statut système utilisé dans un processus d’approbation devait être verrouillé. Cela le rendait disponible pour tous les groupes, sans possibilité de le supprimer ou de le renommer. Les équipes d’administration de groupe ne pouvaient donc pas rationaliser la liste des statuts de leur groupe en fonction de leurs besoins spécifiques.</p>   
   </td> 
    <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 juin 2022<br></p> </li> 
     <li> <p>Version de production : 15 septembre 2022</p> </li> 
    </ul>  </td>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Migration vers Adobe Unified Experience</a> </p>
                        <p>Si votre organisation a été intégrée à Adobe Admin Console, votre instance Workfront sera migrée vers Adobe Unified Experience avec la version 22.4.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4 <span style="color: #ff0000;">Cette migration a été reportée aux 1er et 2e trimestres 2023.</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">L’icône Plans directeurs du menu principal est désormais contrôlée par le biais de modèles de mise en page</a>.</p>
                        <p>L’équipe d’administration système peut désormais ajouter ou supprimer l’icône Plan directeur dans le menu principal via la configuration du modèle de mise en page. Il est ainsi plus facile de contrôler les personnes qui peuvent parcourir le catalogue de plans directeurs.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 25 août 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Personnalisation de l’en-tête du problème</a></p>
                        <p>En tant qu’administrateur ou administratrice Workfront ou de groupes, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’un problème lorsque vous utilisez un modèle de mise en page. Cette mise à jour comprend plusieurs améliorations, notamment la possibilité de supprimer ou de réorganiser les champs existants de l’en-tête du problème et d’ajouter de nouveaux champs non modifiables pour la vue d’ensemble du problème.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 8 septembre 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Personnalisation de l’en-tête de tâche</a></p>
                        <p>En tant qu’administrateur ou administratrice de Workfront ou de groupes, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’une tâche lorsque vous utilisez un modèle de mise en page. Cette mise à jour comprend plusieurs améliorations, notamment la possibilité de supprimer ou de réorganiser les champs existants dans l’en-tête de tâche et d’ajouter de nouveaux champs non modifiables dans la vue d’ensemble de la tâche.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 25 août 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">Inclusion anticipée des dernières fonctionnalités sur les panoramas</a> </p>
                        <p>Nous sommes ravis d’ouvrir de nouvelles fonctionnalités de panoramas pour l’inclusion préalable des fonctionnalités. Cette option n’est pas disponible pour toutes les organisations.</p>
                        <p>Seulement un administrateur ou une administratrice Workfront peut activer les fonctionnalités anticipées. Lorsque l’administrateur ou l’administratrice active les fonctionnalités anticipées, les personnes appartenant à l’entreprise peuvent en bénéficier et les fonctionnalités supplémentaires sont activées dans votre environnement de production Workfront.</p>
                    </td>
                    <td><b>Disponible à ces dates :</b>
                        <ul>
                            <li>
                                <p>Version préliminaire : 22 juillet 2022 <br /></p>
                            </li>
                            <li>
                                <p>Version de production : 28 juillet 2022</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">L’éditeur de calcul de champ de formulaire personnalisé affiche les informations d’erreur.
</a></p></p> <p>La modification des calculs pour les champs personnalisés est désormais plus facile avec des informations d’erreur utiles indiquées directement dans le calcul. Lorsque vous créez un champ calculé dans un formulaire personnalisé, les erreurs sont surlignées en rose. Lorsque vous pointez sur la partie mise en surbrillance, une info-bulle s’affiche pour décrire le problème.</p>
</td>
    <td><b>Disponible à ces dates :</b>
                        <ul>
                            <li>
                                <p>Version préliminaire : pendant la période de publication de la version 22.3 <br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4
</p>
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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                </tr>
<tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Les détails des tâches antérieures sont désormais disponibles.
</a></p> 
<p>Pour afficher les détails des tâches antérieures d’une tâche, vous pouvez maintenant passer la souris sur le numéro de la tâche antérieure dans la colonne Tâches antérieures. La zone Détails affiche la tâche antérieure et le projet référencés, les dates de début et de fin prévues pour la tâche antérieure et le nombre de tâches antérieures et ultérieures de la tâche antérieure. Vous pouvez développer les détails du projet pour afficher plus d’informations sur le projet. Des informations supplémentaires sont incluses pour les projets transversaux antérieurs.</p>   
   </td> 
    <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 9 septembre 2022 <br></p> </li> 
     <li> <p>Version de production : avec la version 22.4</p> </li> 
     </td>
  </tr>                
<tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Affecter plusieurs équipes à une tâche ou à un problème
</a></p> 
<p>Pour vous offrir une plus grande flexibilité dans la gestion des tâches et des problèmes, nous avons permis d’affecter plusieurs équipes à une tâche ou à un problème. Auparavant, une seule équipe pouvait être affectée à une tâche ou à un problème.

Remarque : cette fonctionnalité n’est pas disponible pour l’instant dans l’équilibreur de charge de travail de la zone Équipes.</p>
</td> 
    <td> <p><b>Disponible à ces dates :</b> </p> 
    <ul> 
     <li> <p>Version préliminaire : 2 septembre 2022<br></p> </li> 
     <li> <p>Version de production : avec la version 22.4</p> </li> 
    </ul> 
    </td>
  </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Sélection intelligente de personnes pour les rôles de projet dans les zones Modifier et Détails</a> </p>
                        <p>Nous avons amélioré la façon dont les utilisateurs et utilisatrices s’affichent lorsque vous les ajoutez aux champs Personne propriétaire du projet, Personne sponsor du projet et Personne gestionnaire des ressources à partir de la zone Modifier et de la section Détails du projet.</p>
                        <p>Désormais, lorsque vous ajoutez une personne à l’un de ces champs dans les zones Modifier ou Détails, son rôle principal et son e-mail s’affichent en plus de son nom et de son avatar. Cela permet de distinguer plusieurs utilisateurs portant des noms similaires ou identiques.</p>
                        <p><b>NOTE :</b> les champs utilisateur supplémentaires pour les projets, les tâches et les problèmes seront mis à jour avec cette fonctionnalité dans les prochaines versions.</p>
                    </td>
                    <td><b>Disponible à ces dates :</b>
                        <ul>
                            <li>
                                <p>Version préliminaire : 25 août 2022</p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Les champs calculés de date sont toujours enregistrés en fonction du temps universel coordonné (UTC).</a> </p>
                        <p>Désormais, vous savez que toutes les fonctions de date dans les champs calculés fonctionnent de manière cohérente et produisent le même résultat pour tout le monde, indépendamment de la manière dont une expression de données personnalisées est mise à jour ou de l’endroit où les personnes collaborent sur l’objet dans le monde entier. </p>
                        <p>Tous les calculs sont désormais calculés et enregistrés selon une norme, le temps universel coordonné (UTC), et non selon les configurations de fuseau horaire définies pour l’instance de votre entreprise et votre profil utilisateur individuel. Cependant, les calculs sont affichés dans un formulaire personnalisé en fonction des fuseaux horaires individuels définis dans le navigateur de chaque personne.</p>
                        <p>Auparavant, les paramètres d’heure dans les calculs étaient source de confusion lorsqu’ils variaient selon les situations suivantes :</p>
                        <ul>
                            <li>
                                <p>Si quelqu’un recalculait une expression de champ calculée à l’aide de « Mettre à jour les calculs précédents » sur le créateur de formulaires, les résultats de la fonction de date étaient déterminés par le fuseau horaire UTC de votre entreprise.</p>
                            </li>
                            <li>
                                <p>Si quelqu’un modifiait l’objet et que l’expression du champ calculé était recalculée, les résultats de la fonction de date étaient déterminés par le fuseau horaire local de la personne. Dans ce scénario, le champ Date calculée entraîne également le calcul en fonction du UTC.</p>
                            </li>
                        </ul>
                        <p>Pour plus d’informations, consultez <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref" xrefformat="{para}">Travailler sur plusieurs fuseaux horaires</a>.</p>
                    </td>
                    <td><b>Disponible à ces dates :</b>
                        <ul>
                            <li>
                                <p>Version préliminaire : 18 août 2022</p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4
</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience de filtrage pour les projets, les tâches et les problèmes (Beta)</a> </p>
                        <p>Le filtrage dans les listes de projets, de tâches et de problèmes a été repensé afin de vous aider à créer et partager rapidement des filtres. Les fonctionnalités incluent :</p>
                        <ul>
                            <li>
                                <p>Une interface intuitive de « création Beta » pour créer un filtre</p>
                            </li>
                            <li>
                                <p>La possibilité de marquer un filtre comme favori</p>
                            </li>
                            <li>
                                <p>Empiler des filtres (appliquer plusieurs filtres enregistrés)</p>
                            </li>
                            <li>
                                <p>Dupliquer des filtres</p>
                            </li>
                            <li>
                                <p>Partager des filtres</p>
                            </li>
                            <li>
                                <p>Supprimer des filtres partagés avec vous</p>
                            </li>
                        </ul>
                        <p>La nouvelle expérience de filtrage est également disponible dans les listes de feuilles de temps et dans le planificateur de scénarios.</p>
                        <p>Le mode Texte reste disponible pour l’édition avancée de filtres, et les administrateurs et administratrices système peuvent toujours attribuer des filtres par défaut à toutes les personnes par le biais des modèles de mise en page.</p>
                    </td>
                    <td><b>Disponible à ces dates :</b>
                        <ul>
                            <li>
                                <p>Version préliminaire : 21 juillet 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : 4 août 2022 </p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations des formulaires personnalisés : Adobe XD et filtre rapide</a>
                        </p>
                        <p>Sur la base de vos commentaires, nous avons introduit les améliorations suivantes afin d’améliorer votre expérience de gestion des formulaires personnalisés :

</p>
<ol>
<li>Ajoutez un fichier Adobe XD pour rendre un formulaire personnalisé plus visuel et informatif. Lorsque le formulaire est joint à un objet, les personnes qui l’utilisent peuvent afficher et interagir avec le fichier XD depuis le formulaire.
</li>
<li>Utilisez le filtre rapide pour localiser facilement des éléments dans la liste de champs et de formulaires personnalisés modernisés. Profitez également d’un aspect amélioré lors de la gestion de vos formulaires et champs.
</li>
</ol>
                    </td>
                    <td>
                        <p><b>Disponible à ces dates :</b>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 4 août 2022 <br /></p>
                            </li>
                            <li>
                                <p>Version de production : 11 août 2022</p>
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
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Colonne de saisie disponible sur les panoramas</a></p>
                        <p>Vous pouvez désormais ajouter une colonne de saisie à un panorama. Cette colonne permet d’ajouter automatiquement des tâches et des problèmes au panorama au fur et à mesure qu’ils sont ajoutés dans Workfront, en fonction des filtres que vous définissez.</p>
                        <p>La colonne de saisie peut servir de colonne de liste d’attente pour une équipe Kanban, d’emplacement de saisie pour une équipe d’assistance afin de voir les problèmes au fur et à mesure qu’ils sont ajoutés à une file d’attente des demandes, ou pour toute autre raison dont vous avez besoin.</p>
                        <p>Une seule colonne de saisie est autorisée sur un panorama.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 8 septembre 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production pour l’opt-in anticipé : 15 septembre 2022</p>
                                <p>Version de production pour tous les clientes et clients : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Mise à jour du panneau Filtre dans les panoramas</a></p>
                        <p>Les icônes de filtre et de recherche sur un panorama ont été déplacées vers la gauche de l’écran. Lorsque vous cliquez sur l’icône de filtre, un panneau s’ouvre sur la gauche pour afficher toutes les options de filtre.</p>
                        <p>Auparavant, les filtres étaient affichés dans une liste déroulante sur le côté droit du panorama.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 8 septembre 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production pour l’opt-in anticipé : 15 septembre 2022</p>
                                <p>Version de production pour tous les clientes et clients : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Utiliser des groupes sur un panorama pour créer des couloirs</a></p>
                        <p>Vous pouvez désormais regrouper les cartes sur un panorama par personne assignée ou par balise. Lorsque vous sélectionnez une option de regroupement, les cartes apparaissent sous la forme d’un couloir. Les cartes non attribuées ou sans balise apparaissent dans leur propre couloir.</p>
                        <p>Vous pouvez également définir ce qui se passe lorsqu’une carte est déplacée d’un groupe à un autre. La personne assignée ou la balise du groupe vers lequel la carte est déplacée peut être ajoutée aux personnes assignées/balises existantes ou remplacer les autres personnes assignées/balises de la carte.</p>
                        <p>Les cartes qui se trouvent dans la colonne de saisie ne sont pas incluses dans un groupe.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 9 septembre 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Amélioration des éléments de la liste de contrôle sur les panoramas</a> </p>
                        <p>L’ouverture d’un élément de la liste de contrôle sur une carte permet désormais d’ajouter des informations plus détaillées sur l’élément, notamment une description, une date d’échéance, des personnes assignées et une estimation. Vous pouvez également copier un élément de la liste de contrôle qui n’était pas disponible auparavant.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 17 août 2022<br /></p>
                            </li>
                            <li>
                                <p>Publication en production pour l’opt-in anticipé : 25 août 2022</p>
                                <p>Version de production pour tous les clientes et clients : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter une équipe à un panorama ou à une carte</a> </p>
                        <p>Vous pouvez désormais ajouter une équipe en tant que membre du panorama. Les membres de l’équipe ne sont plus ajoutés lorsque vous ajoutez une équipe au panorama, bien que l’ensemble des membres de l’équipe ait accès au panorama.</p>
                        <p>Après avoir ajouté l’équipe au panorama, vous pouvez lui attribuer des cartes. Sur les cartes connectées, une seule affectation d’équipe est autorisée. Pour les cartes ad hoc, vous pouvez affecter plusieurs équipes.
                        </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 4 août 2022
<br /></p>
                            </li>
                            <li>
                                <p>Publication en production pour l’opt-in anticipé : 11 août 2022</p>
                                <p>Version de production pour tous les clientes et clients : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">La limite du travail en cours est désormais disponible sur les colonnes des panoramas</a> </p>
                        <p>Vous pouvez désormais fixer une limite de travail en cours (WIP) pour n’importe quelle colonne d’un panorama. Lorsque vous activez une limite WIP, un compteur apparaît dans la colonne avec le nombre actuel de cartes et la limite. Le compteur devient rouge si la colonne contient plus de cartes que la limite. Il s’agit simplement d’un avertissement visuel et il ne vous est pas interdit d’ajouter plus de cartes que la limite.</p>
                    </td>
                    <td><b>Disponible à ces dates :</b>
                        <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 22 juillet 2022 <br /></p>
                            </li>
                            <li>
                                <p>Publication en production pour l’opt-in anticipé : 28 juillet 2022</p>
                                <p>Version de production pour tous les clientes et clients : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajout du champ Estimation aux cartes</a> </p>
                        <p>Un nouveau champ Estimation sur les cartes ad hoc et connectées vous permet de saisir le nombre d’heures estimé pour la réalisation de la carte. Il s’agit d’une saisie manuelle, et non d’une valeur calculée. La valeur ne peut être supérieure à 99. L’estimation s’affiche sur la carte du panorama et dans les détails de la carte.</p>
                    </td>
                    <td>
                        <p><b>Disponible à ces dates :</b>
                        <p>
  </p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 22 juillet 2022 <br /></p>
                            </li>
                            <li>
                                <p>Publication en production pour l’opt-in anticipé : 28 juillet 2022</p>
                                <p>Version de production pour tous les clientes et clients : avec la version 22.4</p>
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
                        <p><span class="bold">Dates de sortie</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Afficher tous les utilisateurs et utilisatrices de l’équilibreur de charge de travail d’un projet</a></p>
                        <p>Pour que vous puissiez avoir une visibilité sur tous les utilisateurs ou utilisatrices du système et sur leur capacité sans quitter l’équilibreur de charge de travail d’un projet, nous avons ajouté une option « Afficher tous les utilisateurs et utilisatrices ». Lorsqu’elle est activée, l’équilibreur de charge de travail du projet affiche tous les utilisateurs et utilisatrices du système dans la zone Travail attribué. Grâce à cette amélioration, vous pouvez facilement identifier qui doit être affecté à un travail répertorié dans la zone Travail non attribué.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 8 septembre 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Afficher toutes les personnes ayant une fonction sélectionnée dans l’équilibreur de charge de travail lors de l’affectation de travail en masse</a></p>
                        <p>Pour faciliter la recherche de la bonne personne lors du remplacement des fonctions par des personnes dans l’équilibreur de charge de travail en bloc, nous avons amélioré la façon dont la liste des utilisateurs ou utilisatrices disponibles est renseignée. Désormais, vous pouvez afficher toutes les personnes du système qui peuvent remplir le rôle sélectionné dans deux zones distinctes de la même liste d’utilisateurs et utilisatrices :</p>
                        <ul>
                            <li>
                                <p>La première zone (Affectations suggérées) affiche les personnes identifiées par la logique Affectations intelligentes.<br /></p>
                            </li>
                            <li>
                                <p>La deuxième zone (Autres affectations) affiche toutes les personnes qui peuvent remplir le rôle sélectionné.</p>
                            </li>
                        </ul>
                        <p>Avant cette amélioration, vous ne pouviez afficher que la liste des personnes pouvant être affectées selon la logique Affectations intelligentes.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 8 septembre 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations apportées à l’équilibreur de charge de travail pour les personnes disposant d’une licence Travail et les paramètres de problème</a></p>
                        <p>Les améliorations suivantes ont été apportées à l’équilibreur de charge de travail, en vue de l’obsolescence des outils de planification :</p>
                        <ul>
                            <li>
                                <p>Les utilisateurs et utilisatrices de licences de travail peuvent désormais ajuster les affectations lors de l’utilisation de l’équilibreur de charge de travail d’un projet.<br /></p>
                            </li>
                            <li>
                                <p>Les problèmes s’affichent dans la zone de travail non assigné lorsque le paramètre « Inclure les heures des problèmes » est activé.</p>
                            </li>
                        </ul>
                        <p>Avant ces améliorations, seuls les utilisateurs et utilisatrices de la licence de plan pouvaient ajuster les affectations d’utilisateur ou utilisatrice et les problèmes s’affichaient uniquement dans la zone Travail attribué.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                     <p>
                        </p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 25 août 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
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
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’aspect pendant la période de publication de la version 22.4</a> </p>
                        <p>Des mises à jour mineures de l’aspect de diverses zones de l’application Adobe Workfront sont effectuées dans le cadre de la chronologie de publication de la version 22.4. Ces améliorations seront disponibles dans l’environnement de production au moins deux semaines après le lancement de la version préliminaire. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : tout au long de la chronologie de la version 22.4<br /></p>
                            </li>
                            <li>
                                <p>Version de production : au minimum deux semaines après la publication en prévisualisation (sauf indication contraire).</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront pour InDesign</a> <span style="color: #ff0000;"> Nouveau en production</span> </p>
                        <p>Ce plug-in peut désormais être installé dans InDesign. Il vous permet d’accéder aux détails des éléments de travail, de collaborer avec les personnes avec qui vous travaillez dans la zone des mises à jour et de soumettre des épreuves pour révision, le tout sans quitter XD. Accédez à la marketplace Adobe Creative Cloud pour télécharger le plug-in dès aujourd’hui. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : S/O<br /></p>
                            </li>
                            <li>
                                <p>Version de production : 6 octobre 2022</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Synchroniser les métadonnées des objets avec l’intégration native d’Experience Manager Assets</a> </p>
                        <p>Désormais, les champs de portfolio, programme, projet, tâche, problème et document Workfront se mettent à jour automatiquement quand le champ est modifié dans Workfront.</p>
                        <p>Pour synchroniser automatiquement les métadonnées d’objets, vous devez activer le bouton (bascule) « Synchroniser les métadonnées d’objets » pour vos intégrations dans Configuration &gt; Intégrations Experience Manager.</p>
                        <p>Auparavant, seuls les champs de projet étaient automatiquement mis à jour.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 6 octobre 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : 26 octobre 2022</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Envois de métadonnées pour les objets parent du programme et du portfolio</a></p>
                        <p>Désormais, lorsqu’une ressource est envoyée pour la première fois à Experience Manager Assets ou Assets Essentials, toutes les métadonnées configurées pour mapper les objets parent des programmes et des portfolios sont également envoyées.</p>
                        <p>Auparavant, seules les données des projet parent étaient envoyées.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 6 octobre 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : 26 octobre 2022</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Campagnes Workfront (Beta)</a> </p>
                        <p>Nous introduisons un nouvel objet dans Adobe Workfront qui a le potentiel de modifier la façon dont vous gérez le travail. </p>
                        <p>Les campagnes Workfront vous permettent d’organiser des projets provenant de différents portfolios et programmes dans un nouveau conteneur de travail.
Les campagnes ont été publiées en juillet 2022 dans la version préliminaire Beta 22.3.</p>
<p>Ce nouveau conteneur évoluera dans les prochaines versions pour relier des objets de travail qui sont actuellement gérés dans des silos séparés.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : tout au long de la chronologie de la version 22.4<br /></p>
                            </li>
                            <li>
                                <p>Version de production : à déterminer</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="../../../product-announcements/product-releases/22.4-release-activity/22-4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Description étendue de l’équipe</a></p>
                        <p>Dans la zone « Équipes », vous pouvez désormais afficher la description complète de l’équipe en cliquant sur la description pour l’afficher dans un pop-up. Les URL figurant dans la description sont cliquables dans le pop-up et vous pouvez cliquer sur le texte de la description pour le modifier (si vous avez accès à la modification des paramètres de l’équipe).</p>
                        <p>Auparavant, la seule manière d’afficher l’intégralité du contenu était de faire défiler la description dans une zone étroite.</p>
<p>Cette amélioration de la description s’applique aux équipes Agile et non Agile.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version préliminaire : 11 août 2022<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 22.4</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

## Annonces

### Mise à niveau de la visionneuse de relecture de bureau vers la version la plus récente

Nous avons lancé une nouvelle version de la visionneuse de relecture de bureau. Cette mise à niveau contient une modification technique qui nécessite une action de la part de tous les utilisateurs et utilisatrices. Les actions nécessaires dépendent du système d’exploitation de chaque personne :

* Les personnes utilisant Mac doivent réinstaller manuellement la visionneuse de relecture de bureau pour la mise à niveau vers la dernière version. Pour obtenir de l’aide, consultez la section Installer la visionneuse de relecture de bureau. Après sa réinstallation, les futures mises à jour de la visionneuse de relecture de bureau seront automatiques.

* Les personnes utilisant Windows verront leur visionneuse de relecture de bureau automatiquement mise à niveau vers la dernière version si elles la lancent avant le 25 juillet. Si les personnes utilisant Windows ne parviennent pas à ouvrir la visionneuse de relecture de bureau avant le 25 juillet, elles devront la réinstaller manuellement pour bénéficier de la mise à niveau.


Avec cette mise à niveau, la visionneuse de relecture de bureau prendra en charge la version 98 de Chrome pour une meilleure compatibilité avec les épreuves interactives.

### Améliorations de Workfront Fusion

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de publication de la version 22.4. Pour plus d’informations sur les dernières fonctionnalités, consultez la section [Activité de version d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Améliorations du planificateur de scénarios Workfront

Il n’y a pas de mise à jour du planificateur de scénarios à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de Workfront Proof

Il n’y a pas de mise à jour de Workfront Proof à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations des Objectifs Workfront

Il n’y a pas de mise à jour des Objectifs Workfront à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Version 14 de l’API

Pour la version 14 de l’API, nous avons modifié certaines ressources et certains points d’entrée. Certains des changements prennent en charge de nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, voir [Nouveautés de la version 14 de l’API](/help/quicksilver/wf-api/api/new-api-version-14.md).

Pour plus d’informations sur les versions de l’API, voir [Calendrier des versions et de la prise en charge de l’API](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors du lancement de la version 22.3, consultez la section [Mises à jour de maintenance pour Workfront](https://experienceleague.adobe.com/en/docs/workfront-known-issues/releases/current-updates).

### Webinaire sur la version 22.4

Le webinaire sur la version 22.4 se tiendra le jeudi 22 septembre 2022 à 9 :00 PDT. Vous pouvez [vous inscrire au webinaire ici](https://event.on24.com/wcc/r/3915365/9E496D02A98ECB8C86B1D2D09DDAA443?partnerref=prodmgt).

### Mise à jour des formations

Découvrez les dernières mises à jour des programmes et parcours de formation, des vidéos et des guides pour chaque version du produit Adobe Workfront. Pour plus d’informations, consultez la [page des mises à jour des versions des formations](https://experienceleague.adobe.com/fr/docs/workfront-learn/tutorials-workfront/home).

### Fonctionnalités supprimées avec la version 22.4

Les fonctionnalités suivantes seront supprimées lors de la mise en production de la version 22.4 :

* Contrôles de liste (à partir de la zone d’interface dans Configuration)

>[!NOTE]
>
>L’obsolescence des contrôles de liste a été reportée après le lancement de la version 22.4. La date d’obsolescence sera annoncée dans de futures communications.


* Planificateur de ressources

>[!NOTE]
>
>L’abandon du planificateur de ressources a été reporté jusqu’à ce que la version 22.4 soit disponible.

L’équilibreur de charge de travail remplace le planificateur de ressources.

* Intégration du zoom

### Fonctionnalité supprimée après la version 22.4

La fonction suivante sera supprimée en novembre 2022 :

* Type d’événement SHARE dans l’API d’abonnement aux événements.

  Ce type d’événement permet aux clientes et clients de surveiller la mise à jour des autorisations sur les objets.

  Pour plus d’informations sur les abonnements aux événements, ainsi que sur d’autres types d’événement qui continueront à être pris en charge, consultez [API d’abonnement aux événements](/help/quicksilver/wf-api/general/event-subs-api.md).
