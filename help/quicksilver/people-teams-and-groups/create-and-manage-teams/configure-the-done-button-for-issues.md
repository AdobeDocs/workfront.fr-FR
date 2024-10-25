---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configuration du bouton Terminé pour les problèmes
description: Le bouton Terminé permet de définir automatiquement le statut d’une tâche ou d’un problème. Par défaut, Adobe Workfront marque un problème comme Résolu lorsqu’une personne cessionnaire clique sur Terminé dans son élément de travail.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 97%

---

# Configurer le bouton [!UICONTROL Terminé] pour les problèmes

Le bouton [!UICONTROL Terminer] permet de définir automatiquement le statut d’une tâche ou d’un problème. Par défaut, [!DNL Adobe Workfront] marque un problème comme [!UICONTROL Résolu] lorsqu’une personne cessionnaire clique sur [!UICONTROL Terminé] sur son élément de travail.

>[!NOTE]
>
>Le bouton Terminé s’affiche sous la forme Marquer comme prévu dans toutes les zones de Workfront.

## Vue d’ensemble

Les utilisateurs ou les utilisatrices disposant de certaines autorisations peuvent configurer le bouton [!UICONTROL Terminé] de manière à ce qu’il reflète certains statuts du système. Le bouton [!UICONTROL Terminé] fonctionne de trois manières différentes pour les problèmes relevant de [!DNL Workfront] :

* Si l’utilisateur ou l’utilisatrice dispose d’une [!UICONTROL équipe interne] affectée, un [!DNL Workfront]administrateur ou une administratrice, ou un utilisateur ou une utilisatrice disposant d’une licence [!UICONTROL Plan] peut configurer le bouton [!UICONTROL Terminé] pour refléter certains statuts des personnes membres de l’équipe. Voir [Configurer le bouton [!UICONTROL Terminé] pour une équipe](#configure-the-uicontrol-done-button-for-a-team) dans cet article.
* Si la personne ne dispose pas d’une [!UICONTROL équipe interne], mais qu’elle a [!UICONTROL d’autres équipes] dans son profil, Workfront recherche la configuration du bouton [!UICONTROL Terminé] sur n’importe laquelle des équipes associées à l’utilisateur ou à l’utilisatrice. La sélection est aléatoire et le statut associé à l’une des équipes est utilisé pour le problème.
* Si l’utilisateur ou l’utilisatrice n’a pas d’[!UICONTROL équipe interne] affectée, le bouton [!UICONTROL Terminé] pour les problèmes est lié à un statut [!UICONTROL Résolu] généré par le système et portant le code à trois lettres [!UICONTROL RLV]. Aucune option de configuration n’est disponible dans ce scénario. Le bouton [!UICONTROL Terminé] indique automatiquement ce statut par défaut.
* Si le statut [!UICONTROL Résolu] ([!UICONTROL RLV]) est supprimé et que l’utilisateur ou l’utilisatrice qui marque le problème comme [!UICONTROL Terminé] n’a pas d’[!UICONTROL équipe interne], le statut par défaut de la question est lié à celui défini par défaut pour [!UICONTROL Fermé] pour le groupe affecté au projet auquel le problème appartient. L’équipe d’administration Workfront peut configurer un paramètre par défaut à l’échelle du système pour le groupe. Voir [Configurer le bouton [!UICONTROL Terminé] lorsque le statut [!UICONTROL Résolu] a été supprimé](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) dans cet article.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>L’accès administrateur système est requis pour configurer le bouton Terminé lorsque l’état Résolu est supprimé.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer le bouton [!UICONTROL Terminé] pour une équipe

Vous pouvez modifier le statut appliqué à l’élément de travail avec le bouton [!UICONTROL Terminé]. Vous pouvez également définir plusieurs statuts et permettre à l’utilisateur ou à l’utilisatrice de choisir celui qui lui convient.

{{step1-to-team}}

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]**, puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis cliquez sur **[!UICONTROL Modifier]**.
1. Recherchez la section **[!UICONTROL Bouton Terminé]** au bas de la page **[!UICONTROL Paramètres de l’équipe]**.

1. Sélectionnez un ou plusieurs statuts pour chaque type d’élément de travail.

   >[!NOTE]
   >
   >Tenez compte des éléments suivants lors de la sélection des statuts des tâches ou des problèmes :
   >
   >* Lorsque vous sélectionnez un statut pour chaque type d’élément de travail, le statut de la tâche ou du problème est défini sur ce statut lorsqu’une personne clique sur [!UICONTROL Terminé] sur son élément. Si vous définissez plusieurs statuts pour chaque type d’élément de travail, un menu déroulant est ajouté au bouton [!UICONTROL Terminé] et la personne doit sélectionner un statut pour modifier le statut de l’élément de travail.
   >* Vous pouvez associer uniquement les statuts au niveau du système au bouton [!UICONTROL Terminé]. Il n’est pas possible d’associer des statuts spécifiques à un groupe à des statuts d’élément de travail.
   >* Lorsqu’une personne affectée à l’élément place l’élément dans le statut associé au bouton [!UICONTROL Terminé], l’élément s’affiche comme [!UICONTROL Terminé] pour cette personne, que le statut sélectionné soit [!UICONTROL Terminé] ou [!UICONTROL Fermé] ou qu’il s’agisse d’un statut de travail.
   >   
   >   
   >  Par exemple, l’association du bouton [!UICONTROL Terminé] avec En cours entraîne l’affichage de l’élément de travail comme [!UICONTROL Terminé] pour l’utilisateur ou l’utilisatrice qui modifie le statut de Nouveau à En cours.
   >   
   >* Les types de problèmes sont personnalisables et peuvent avoir des noms différents de ceux énumérés ci-dessous dans votre environnement.\
   >  Les tâches et les types de problèmes par défaut sont décrits ci-dessous :
   >     
   >   * [!UICONTROL Tâches]
   >   * [!UICONTROL Problème]
   >   * [!UICONTROL Demande]
   >   * [!UICONTROL Modifier l&#39;ordre]
   >   * [!UICONTROL Rapport sur les bogues]

   Si la tâche ou le problème est affecté à plusieurs personnes, une option « [!UICONTROL J’ai fait ma part] » s’affiche dans le menu déroulant, en plus des multiples statuts choisis pour votre équipe.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Associer les utilisateurs et utilisatrices à une équipe d’accueil

Pour apporter des modifications à la fonctionnalité du bouton [!UICONTROL Terminé] visible aux utilisateurs et utilisatrices, vous pouvez faire de l’équipe dont vous avez modifié les paramètres l’équipe principale des utilisateurs et utilisatrices.

Pour associer des utilisateurs et des utilisatrices à une équipe d’accueil :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront].

1. Cliquez sur **[!UICONTROL Utilisateurs et utilisatrices]**, puis sélectionnez la ou les personnes que vous souhaitez associer à une équipe principale.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Dans la section **[!UICONTROL Organisation]**, sélectionnez le champ **[!UICONTROL Équipe principale]**. Commencez à taper le nom de l’équipe dont vous souhaitez associer les paramètres aux utilisateurs et utilisatrices. Cliquez sur le nom de l’équipe lorsque vous le voyez dans la liste.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.\
   Les personnes que vous avez sélectionnées sont maintenant associées à une équipe interne.
Tous les paramètres de l’équipe, y compris les statuts associés au bouton [!UICONTROL Terminé], sont désormais visibles pour ces personnes.

## Configurer le bouton [!UICONTROL Terminé] lorsque le statut [!UICONTROL Résolu] a été supprimé

Si une personne ne possède pas d’équipe interne et que la valeur par défaut de [!UICONTROL Résolu] ([!UICONTROL RLV]) à l’échelle du système a été supprimée, un administrateur ou une administratrice [!DNL Workfront] peut configurer le statut [!UICONTROL Fermé] pour le groupe sur le projet. [!DNL Workfront] sélectionne ce statut pour un problème clôturé lorsque l’utilisateur ou l’utilisatrice clique sur le bouton [!DNL Done].

### Trouver le groupe associé au projet

Lorsqu’un utilisateur ou une utilisatrice crée un projet, son groupe interne est automatiquement affecté au projet. Les personnes disposant d’un accès de type [!UICONTROL Gérer] au projet peuvent à tout moment modifier ce groupe dans la section [!UICONTROL Détails du projet]. Pour comprendre le statut que [!DNL Workfront] utilise pour un problème terminé dans ce cas, vous devez connaître le groupe associé au projet sur lequel se trouve le problème et le statut par défaut pour [!UICONTROL Fermé] dont ce groupe dispose pour les problèmes.

Pour trouver le groupe associé au projet :

1. Accédez à un projet.
1. Dans la partie gauche de la page, cliquez sur **[!UICONTROL Détails du projet]**.
1. Localisez la section **[!UICONTROL Association de projets]**, puis trouvez **[!UICONTROL Groupe]**.\
   Il s’agit du nom du groupe que vous devez utiliser pour vérifier le statut dans la zone de configuration. La section suivante explique comment mettre à jour le statut par défaut d’un groupe spécifique.

### Mettre à jour le statut par défaut d’un groupe spécifique

En tant qu’administrateur ou administratrice de [!UICONTROL Workfront], vous pouvez mettre à jour le statut d’un groupe spécifique :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Préférences du projet]**, puis sur **[!UICONTROL Statuts]**.

1. Cliquez sur **[!UICONTROL Problèmes]**, puis saisissez le nom du groupe dans la zone de recherche **[!UICONTROL Statuts du système]** située à droite.

1. Sélectionnez le groupe.
1. Cliquez sur le menu déroulant **[!UICONTROL Définir les statuts par défaut]**, puis choisissez un statut par défaut pour [!UICONTROL Fermé]. [!DNL Workfront] utilise ce statut pour un problème fermé lorsqu’une personne clique sur le bouton [!UICONTROL Terminé].

   >[!IMPORTANT]
   >
   >Ce statut n’est utilisé que lorsque l’utilisateur ou l’utilisatrice n’a pas d’équipe interne affectée et que le statut [!UICONTROL RLV] a été supprimé.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
