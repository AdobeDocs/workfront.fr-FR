---
title: Vue d’ensemble de la version 23.3
description: Vue d’ensemble de la version 23.3
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 441d84d6-6c40-4a03-967e-836cf78c8fc1
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '2798'
ht-degree: 18%

---

# Vue d’ensemble de la version 23.3

Cette page fournit des informations sur les fonctionnalités incluses dans la version 23.3. Ces améliorations ont été apportées à l’environnement de production avec la version 23.3 des 20 et 21 juillet 2023.

Le webinaire de la version 23.3 date du 29 juin 2023. Vous pouvez [vous inscrire au webinaire pour afficher un enregistrement à la demande ici](https://webinars.on24.com/adobe_workfront/whatsnewin233?partnerref=exlreleaseoverview).

<span class="preview">Les fonctionnalités hors cycle (celles qui sont publiées en production avant la date de publication de la version 23.3) sont surlignées en jaune.</span>

>[!IMPORTANT]
>
>La version 23.3 comprend la possibilité de déplacer votre entreprise vers les versions mensuelles. Par conséquent, Workfront est en train de modifier le schéma de numérotation des versions afin de prendre en compte à la fois les mises à jour mensuelles et trimestrielles.
>
>* Si vous utilisez la piste **version rapide (mensuelle)**, la version après la version 23.3 sera **23.8**, le 31 août 2023.
> * Si vous utilisez la version **trimestrielle**, la version qui suivra la version 23.3 sera **23.10**, dans la semaine du 26 octobre 2023.
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
>Pour plus d’informations sur le processus de version rapide, consultez [Activer ou désactiver le processus de version rapide](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Améliorations Adobe Workfront

* [Améliorations d’administration](#administrator-enhancements)
* [Améliorations rapides](#agile-enhancements)
* [Améliorations apportées à la gestion financière](#financial-management-enhancements)
* [Améliorations de l’intégration](#integration-enhancements)
* [Améliorations des projets](#project-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Activer des cycles de publication Workfront plus rapides</a></p>
                        <p>Pour vous permettre de recevoir plus rapidement les nouvelles fonctionnalités et mises à jour du produit Workfront, nous avons ajouté la possibilité d’activer des cycles de publication plus rapides. Désormais, vous pouvez demander à votre entreprise de recevoir les versions de Workfront plus fréquemment qu’une fois par trimestre. Le cycle de publication trimestriel sera toujours disponible pour les organisations qui préfèrent les versions moins fréquentes.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 22 juin 2023</p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Contrôle au niveau du groupe disponible pour "Où les utilisateurs peuvent consigner l’heure", la feuille de temps et la préférence d’heure</a></p>
                        <p>L’administrateur système peut désormais verrouiller et déverrouiller les préférences "Où les utilisateurs peuvent consigner l’heure" et "Heure". Lorsque cette préférence est déverrouillée, les administrateurs de groupe peuvent configurer les paramètres "Où les utilisateurs peuvent consigner l’heure" séparément pour chaque groupe.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 4 mai 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : vendredi 18 mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Afficher la logique et ignorer les indicateurs de logique et les règles affichés dans la version bêta du concepteur de formulaire</a></p>
                        <p>La version bêta publique du concepteur de formulaire a été réactivée dans Aperçu et production le 21 juillet 2023. En outre, vous pouvez désormais afficher les règles logiques existantes créées dans des formulaires personnalisés hérités dans le concepteur de formulaires.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : samedi 21 juillet 2023</p>
                            </li>
                            <li>
                                <p>Version de production : samedi 21 juillet 2023</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">La vue agile d’un projet affiche un panorama kanban</a></p>
                        <p>La vue agile d’un projet inclut désormais des fonctionnalités supplémentaires pour filtrer, regrouper et trier le travail dans un panorama kanban. La nouvelle conception flexible de la vue comprend une fonction de recherche robuste et la possibilité d’ajouter de nouvelles tâches au projet directement à partir du panorama.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 29 juin 2023</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Tri par colonnes de panorama</a></p>
                        <p>Nous avons ajouté la possibilité de trier les cartes dans les colonnes d’un panorama. Lorsque vous sélectionnez une option de tri, toutes les colonnes sont triées. Vous ne pouvez pas trier une seule colonne, et la colonne de journal ou d’entrée n’est pas triée.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 22 juin 2023</p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>                             
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Le mode sombre est désormais disponible sur les panoramas Adobe Workfront</a></p>
                        <p>Vous pouvez désormais afficher tous vos panoramas et flux de travail en mode sombre. Le nouveau paramètre est disponible via les préférences du tableau de bord Panoramas.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 22 juin 2023<span style="color: #ff0000;"> Cette fonctionnalité a été supprimée de la version d’aperçu et ne sera pas publiée avec la version 23.3.</span></p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : S.O.</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Objectifs disponibles sur les itérations de workflows dans les panoramas Adobe Workfront</a></p>
                        <p>Nous avons ajouté la possibilité d’ajouter des objectifs à une itération, sans avoir à les répertorier sur une carte. Les objectifs sont ajoutés au format liste de contrôle et peuvent être marqués comme étant terminés. La zone des mesures située en haut à droite de l’itération indique le nombre d’objectifs existants et le nombre d’objectifs terminés.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 22 juin 2023<span style="color: #ff0000;"> Cette fonctionnalité a été supprimée de la version d’aperçu et ne sera pas publiée avec la version 23.3.</span></p>
                            </li>
                            <li>
                                <p>Version de production pour tous les clients : S.O.</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajouter des commentaires aux cartes sur les panoramas</a></p>
                        <p>Vous pouvez maintenant ajouter des commentaires aux cartes ad hoc et connectées sur les panoramas et marquer d’autres utilisateurs sur les commentaires. Les commentaires sont disponibles dans les détails de la carte. La fonction de commentaire des panoramas utilise la nouvelle expérience de commentaire d’Adobe Workfront.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 15 juin 2023</p>
                            </li>
                            <li>
                                 <p>Version de production pour la pré-inscription : 22 juin 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via la pré-inscription de la fonctionnalité pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Améliorations apportées au gestionnaire de balises des panoramas</a></p>
                        <p>L’interface du gestionnaire de balises a été améliorée, ce qui vous permet de créer de nouvelles balises rapidement et de les appliquer aux cartes. Vous pouvez également créer des balises pour les flux de travail.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : samedi 19 mai 2023</p>
                            </li>
                            <li>
                                 <p><span class="preview">Version de production : samedi 19 mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Filtres simples disponibles sur les colonnes d’entrée de panorama</a></p>
                        <p>Des filtres simplifiés ont été ajoutés à la configuration de la colonne d’entrée afin que vous puissiez définir la colonne d’entrée plus rapidement. Les filtres disponibles sont des projets Workfront et des affectations par équipe ou utilisateur. Vous pouvez passer aux filtres avancés si vous le souhaitez.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : jeudi 10 mai 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : 10 mai 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Filtres simples ajoutés au modèle de carte dynamique</a></p>
                        <p>Les filtres sur le modèle de panorama dynamique ont été simplifiés afin que vous puissiez créer un panorama plus rapidement.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 27 avril 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : 28 avril 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Modèle de panorama dynamique</a></p>
                        <p>Un nouveau modèle, la carte dynamique, est désormais disponible pour les panoramas autonomes. Ce modèle n’est pas disponible pour les panoramas à l’intérieur d’un workflow.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 20 avril 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : 28 avril 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</span></p>
                                <p>Version de production pour tous les clients : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Migrer les cartes Kanban de l’équipe agile vers les panoramas</a></p>
                        <p>Un nouveau bouton <b>Ajouter aux panoramas</b> sur les panoramas Kanban de l’équipe agile vous permet d’ajouter toutes les cartes du panorama Kanban à un panorama Workfront. Vous pouvez choisir de créer un panorama Workfront ou d’ajouter les cartes à un panorama existant.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 20 avril 2023<br /></p>
                            </li>
                            <li>
                                 <s><p>Mise à jour de la production pour l’inclusion anticipée : 28 avril 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</span></p></s>
                                 </li>
                                 <li>
                                <p><span class="preview">Version de production pour toute la clientèle : vendredi 18 mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Navigation de gauche ajoutée aux détails de carte sur les panoramas</a></p>
                        <p>À mesure que d’autres options de champ sont ajoutées aux cartes sur les panoramas Workfront, les détails des cartes sont devenus plus longs. Un nouveau panneau de navigation situé à gauche des détails de la carte vous permet de sélectionner une section et de passer automatiquement à ce groupe de champs.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 20 avril 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production pour toute la clientèle : vendredi 27 avril 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-agile-enhancements.md" class="MCXref xref" xrefformat="{para}">Forums de notification électronique et préférences</a></p>
                        <p>Les notifications électroniques sont désormais disponibles pour les panoramas Adobe Workfront. Les notifications sont activées par défaut et vous pouvez sélectionner dans vos préférences les emails que vous souhaitez recevoir. Vous recevrez un e-mail lorsque vous serez ajouté à un panorama et lorsqu’une carte vous sera attribuée.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 13 avril 2023<br /></p>
                            </li>
                            <li>
                                 <p>Mise à jour de la production pour l’inclusion anticipée : 13 avril 2023 <span style="color: #ff0000;"> Cette fonctionnalité est disponible en production à cette date uniquement via l’inclusion anticipée des fonctionnalités pour les panoramas Workfront.</p>
                                <p>Version de production pour tous les clients : avec la version 23.3</p>
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
                        <p><span class="bold">Dates de version</span>
                        </p>
                    </td>
                 </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-finance-enhancements.md" class="MCXref xref" xrefformat="{para}">Date d’entrée en vigueur des taux de coût et de facturation</a></p>
                        <p>Les taux de coût et de facturation en vigueur à la date sont désormais disponibles sur les objets de rôle d’entreprise, d’utilisateur et de tâche dans Workfront. Lorsque les taux d’efficacité de la date sont appliqués à un projet et que les heures sont consignées dans les tâches du projet, les coûts et les recettes sont calculés à l’aide des taux spécifiés pour chaque période.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 29 juin 2023</p>
                            </li>
                            <li>
                                <p>Version de production pour les clients de la version rapide : à annoncer, après la version de production 23.3</p>
                                <p>Mise à jour de production pour tous les clients : à annoncer<br>
                                La fonction de remplacement du taux d’affectation a été temporairement désactivée dans Aperçu du 30 juin au 13 juillet 2023.</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle intégration de Google Workspace désormais disponible</a></p> 
                        <p>Une nouvelle intégration Google Workspace est désormais disponible dans Google Marketplace. La nouvelle intégration s’authentifie à l’aide d’OAuth2 et remplace l’intégration précédente.</p><p>L’intégration précédente de Google Workspace est désormais obsolète et sera automatiquement désinstallée.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : mercredi 27 juin 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Les intégrations Adobe Creative Cloud prennent désormais en charge plusieurs utilisateurs affectés</a></p> 
                        <p>L’intégration de Adobe Creative Cloud prend désormais en charge la possibilité de choisir entre "Terminé avec ma part" et "Terminé" (ou "Résolu") lorsqu’une tâche ou un problème comporte plusieurs utilisateurs affectés.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : vendredi 22 juin 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Affichage et gestion des notifications Workfront à partir de Workfront pour les modules externes de Creative Cloud</a></p> 
                        <p>Afin de vous permettre de recevoir plus facilement les notifications dont vous avez besoin, nous avons rendu possible l’affichage et la gestion des notifications Workfront sans quitter Adobe Creative Cloud. Vous pouvez désormais afficher des notifications, ainsi que accéder aux tâches et aux commentaires associés à ces notifications, directement depuis la fenêtre du module externe Workfront dans l’application du Creative Cloud.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : vendredi 22 juin 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
 <!--               <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Improved experience when moving a document to a linked folder with drag and drop</a></p> 
                        <p>We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder. </p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release: June 7, 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: June 15, 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>-->
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}"> Créer automatiquement des dossiers liés à Adobe Experience Manager Assets lors de la création d’un projet </a></p>
                        <p>Avec le nouveau workflow Créer un dossier lié pour l’intégration de Adobe Experience Manager, vous pouvez configurer l’intégration avec un chemin d’accès à un dossier Adobe Experience Manager Assets. Lorsque l’intégration est ajoutée à un modèle de projet, tout projet créé à partir du modèle crée automatiquement un sous-dossier lié dans Experience Manager Assets dans le dossier spécifié. </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 11 mai 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : jeudi 24 mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mappage des valeurs de champ Workfront aux balises dans Experience Manager Assets</a></p>
                        <p>Vous pouvez désormais classer et rechercher rapidement des ressources en fonction des données de Workfront. Vous pouvez mapper ces données dans le cadre de votre configuration de métadonnées dans l’intégration de Workfront for Experience Manager Assets.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : jeudi 10 mai 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : jeudi 10 mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Mappage des champs Workfront aux champs de métadonnées Experience Manager Assets personnalisés</a></p>
                        <p>Avec l’intégration native, vous pouvez désormais mapper les champs Workfront natifs et intégrés aux champs de schéma de métadonnées personnalisés as a Cloud Service Experience Manager Assets.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : jeudi 10 mai 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : jeudi 10 mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Ajuster les paramètres du modèle de workflow de BAT automatisé à l’aide d’Adobe Workfront pour Creative Cloud</a></p>
                        <p>Vous pouvez désormais ajuster les paramètres de modèle de workflow automatisé existants directement dans le Creative Cloud.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 27 avril 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : vendredi 27 avril 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelles validations de document</a> </p>
                        <p>L’approbation des documents est en cours de reconception dans un déploiement échelonné qui sera mis à la disposition d’un plus grand nombre d’utilisateurs avec chaque version.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 31 mai 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : jeudi 14 juin 2023</span></p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Cette fonctionnalité fait partie d’une version par étapes et est actuellement disponible uniquement pour des clients spécifiques.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Bouton Nouveau partage</a> </p>
                        <p>L’option Partager a été supprimée du menu Plus pour les projets, les tâches et les problèmes afin de rendre le partage plus intuitif.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : vendredi 22 juin 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.3</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle fonctionnalité de BAT dans l’application mobile Workfront</a> </p>
                        <p>Avec l’abandon de l’application Workfront Proof autonome dans la version 23.10 (octobre 2023), des fonctionnalités de vérification ont été ajoutées à l’application mobile principale de Workfront pour permettre la poursuite de la vérification sur mobile.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : S.O.</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : disponible dans Apple App Store et Google Play Store le 21 juin 2023</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience d’accueil</a></p>
                        <p>Pour permettre aux utilisateurs de tous types d’utiliser Workfront en fonction de leurs besoins spécifiques, Home a reçu une mise à jour majeure. L’expérience Nouvelle page d’accueil offre une personnalisation visuelle et de contenu pour votre page d’accueil, ce qui vous permet d’afficher uniquement les informations les plus pertinentes pour votre travail.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : samedi 23 juin 2023</p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                 </tr>                                 
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience de commentaire pour des objets supplémentaires</a> </p>
                        <p>La nouvelle expérience de commentaires sera disponible pour les objets suivants, peu après la mise en production de la version 23.3 : tâches de modèle, modèles, feuilles de temps, équipes, utilisateurs ou utilisatrices, programmes, portfolios.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : à annoncer, après la version de production 23.3</p>
                            </li>
                            <li>
                                <p>Version de production pour les clients de la version rapide : à annoncer, après la version de production 23.3 </p>
                                <p>Version de production pour tous les clients : avec la version 23.10 (octobre 2023)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>                
            <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Nouvelle expérience de commentaires Beta pour les projets, les tâches et les documents</a> </p>
                        <p>La nouvelle expérience de commentaires en version bêta est désormais disponible pour les projets, les tâches et les documents. Avant cette mise à jour, l’expérience de commentaires en version bêta n’était disponible que pour les problèmes et les objectifs.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 1er juin 2023<br /></p>
                            </li>
                            <li>
                                <p>Version de production : avec la version 23.3</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> Les profils sans avatars affichent désormais les initiales de l’utilisateur </a></p>
                        <p>Pour faciliter la recherche d’utilisateurs spécifiques dans des listes volumineuses, les profils sans avatars personnalisés affichent désormais leurs initiales sur un arrière-plan coloré dans des listes et des rapports hérités. Il s’agit d’un changement cosmétique mineur qui ne s’applique pas si une photo d’avatar est déjà utilisée ou si l’utilisateur est désactivé.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : 20 avril 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : vendredi 4 mai 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Nouvelles améliorations de l’expérience bêta de commentaires</a></p>
                        <p>Des améliorations ont été apportées à la section Mises à jour . Elles sont disponibles dans le délai de publication de la version 23.3 pour la nouvelle expérience bêta de commentaires. Ces améliorations seront disponibles dans l’environnement de production avec la version 23.3, sauf indication contraire.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : pendant toute la période de la version 23.3<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : avec la version 23.3 (sauf indication contraire)</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Nouvelles améliorations de l’expérience du tableau de bord du canevas</a></p>
                        <p>Des améliorations ont été apportées au tableau de bord de la zone de travail pendant la période de publication de la version 23.3. Ces améliorations seront disponibles dans l’environnement de production avec la version 23.3, sauf indication contraire. 
 </p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Version d’aperçu : mardi 5 juin 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : mardi 5 juin 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Mises à jour de l’apparence pendant la période de publication de la version 23.3</a></p>
                        <p>Des mises à jour mineures de l’aspect des différentes zones de l’application Adobe Workfront sont effectuées dans le délai de publication de la version 23.3. Ces améliorations seront rendues disponibles dans l’environnement de production au moins 2 semaines après la publication de la version de prévisualisation.</p>
                    </td>
                    <td><p><b>Disponible à ces dates :</b></p>
                        <ul>
                            <li>
                                <p>Aperçu de la version : pendant toute la période de la version 23.3</p>
                            </li>
                            <li>
                                <p><span class="preview">Version de production : au moins 2 semaines après la publication dans Aperçu (sauf indication contraire)</span></p>
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

Les nouvelles fonctionnalités de Workfront Fusion sont disponibles en production à un rythme différent du calendrier de version 23.3. Pour plus d’informations sur les dernières fonctionnalités, voir [Activité Version d’Adobe Workfront Fusion](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Améliorations du planificateur de scénarios Workfront

Aucune mise à jour du planificateur de scénario n’est disponible à ce stade de la version. Cette zone sera mise à jour lorsque des mises à jour seront disponibles.

### Améliorations de l’épreuve Workfront

Nouvelles fonctionnalités de la version Workfront Proof au cours de la période de publication 23.3. Pour plus d’informations sur ces nouvelles fonctionnalités désormais disponibles dans l’aperçu, voir [BAT Adobe Workfront avec la version 23.3](/help/quicksilver/product-announcements/product-releases/workfront-proof-release-activity/proof-23-3-release/proof-23-3-overview.md).

### Améliorations des Objectifs Workfront

Nouvelles fonctionnalités de la version 23.3 des objectifs de Workfront. Pour plus d’informations sur ces nouvelles fonctionnalités désormais disponibles dans l’aperçu, voir [Objectifs d’Adobe Workfront avec la version 23.3](/help/quicksilver/product-announcements/product-releases/goals-release-activity/goals-23-3-release/goals-23-3-release.md).

### API version 16

Pour l’API version 16, nous avons modifié certaines ressources et points d’entrée. Certaines des modifications participent à la prise en charge des nouvelles fonctionnalités, tandis que d’autres facilitent l’utilisation des informations disponibles via l’API.

Pour plus d’informations sur les nouveautés et les mises à jour, consultez les [Nouveautés de l’API version 16](/help/quicksilver/wf-api/api/new-api-version-16.md).

Pour plus d’informations sur les versions d’API, consultez [Contrôle de version des API et planification de la prise en charge](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Mises à jour de maintenance pour Workfront 

Pour plus d’informations sur les mises à jour de maintenance effectuées lors de la version 22.3, consultez [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr).

### Mises à jour de formation

Découvrez les dernières mises à jour apportées aux programmes de formation, aux parcours de formation, aux vidéos et aux guides de chaque version de produit Adobe Workfront. Pour plus d’informations, reportez-vous à la section « Nouveautés » de la [page Tutoriels Workfront](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr).

### Fonctionnalité bientôt supprimée de Workfront

Les fonctionnalités suivantes seront bientôt supprimées de Workfront :

#### Obsolescence de l’application mobile BAT avec la version 23.10 (octobre 2023)

L’application mobile BAT sera officiellement abandonnée avec la version 23.10 (octobre 2023). L’application mobile Workfront générale a été améliorée avec de nouvelles fonctionnalités de vérification (voir la note de mise à jour sous Améliorations apportées à Workfront Mobile pour plus d’informations) et il est conseillé aux utilisateurs de commencer à l’utiliser pour le travail de vérification dès que possible.

Notez que l’application mobile Workfront requiert une connexion Workfront. Les utilisateurs externes et les invités peuvent continuer à utiliser l’application Bon à tirer pour le travail de vérification. Toutefois, elle n’est plus prise en charge et ne sera plus disponible avec la version 23.10 (octobre 2023).


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


Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
