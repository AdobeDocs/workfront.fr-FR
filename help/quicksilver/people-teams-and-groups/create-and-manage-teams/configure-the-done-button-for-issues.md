---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurer le bouton Terminé pour les problèmes
description: Le bouton Terminé permet de définir automatiquement l’état d’une tâche ou d’un problème. Par défaut, Adobe Workfront marque un problème comme résolu lorsqu’un cessionnaire clique sur Terminé sur son élément de travail.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 23%

---

# Configuration du bouton [!UICONTROL Terminé] pour les problèmes

Le bouton [!UICONTROL Terminé] peut automatiquement définir l’état d’une tâche ou d’un problème. Par défaut, [!DNL Adobe Workfront] marque un problème comme [!UICONTROL Résolu] lorsqu’un cessionnaire clique sur [!UICONTROL Terminé] sur son élément de travail.

## Vue d’ensemble

Les utilisateurs disposant de certaines autorisations peuvent configurer le bouton [!UICONTROL Terminé] pour refléter certains états du système. Le bouton [!UICONTROL Terminé] fonctionne de trois manières différentes pour résoudre des problèmes dans [!DNL Workfront] :

* Si l’utilisateur a une [!UICONTROL équipe d’accueil] affectée, un administrateur [!DNL Workfront] ou un utilisateur disposant d’une licence [!UICONTROL Plan] peut configurer le bouton [!UICONTROL Terminé] pour refléter certains statuts des membres de l’équipe. Voir [Configuration du bouton [!UICONTROL Terminé] pour une équipe](#configure-the-uicontrol-done-button-for-a-team) dans cet article.
* Si l’utilisateur ne dispose pas d’une [!UICONTROL équipe d’accueil], mais que son profil comporte [!UICONTROL autres équipes], Workfront recherche le paramètre du bouton [!UICONTROL Terminé] sur l’une des équipes associées à l’utilisateur. La sélection est aléatoire et l’état associé à l’une des équipes est utilisé pour le problème.
* Si l’utilisateur ne dispose pas d’une [!UICONTROL équipe d’accueil] affectée, le bouton [!UICONTROL Terminé] pour les problèmes est lié à un état [!UICONTROL Résolu] généré par le système et comportant le code à trois lettres [!UICONTROL RLV]. Aucune option de configuration n’est disponible dans ce scénario. Le bouton [!UICONTROL Terminé] propose automatiquement cet état par défaut.
* Si l’état [!UICONTROL Résolu] ([!UICONTROL RLV]) est supprimé et que l’utilisateur qui marque le problème comme [!UICONTROL Terminé] n’a pas [!UICONTROL Home Team], l’état du problème par défaut est lié à ce qui est défini comme valeur par défaut pour [!UICONTROL Fermé] pour le groupe affecté au projet auquel le problème appartient. L’administrateur Workfront peut configurer un paramètre par défaut à l’échelle du système pour le groupe. Voir [Configurer le bouton [!UICONTROL Terminé] lorsque l’état [!UICONTROL Résolu] a été supprimé](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) dans cet article.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td>L’accès administrateur système est requis pour configurer le bouton [!UICONTROL Terminé] lorsque l’état [!UICONTROL Résolu] est supprimé.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Configuration du bouton [!UICONTROL Terminé] pour une équipe

Vous pouvez modifier l’état appliqué à l’élément de travail à l’aide du bouton [!UICONTROL Terminé] . Vous pouvez également définir plusieurs statuts et autoriser l’utilisateur ou l’utilisatrice à choisir le statut approprié.

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Equipes]**.

1. Cliquez sur l’icône **[!UICONTROL Changer d’équipe]**, puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sur **[!UICONTROL Modifier]**.
1. Vous trouverez le bouton **[!UICONTROL Terminé]** au bas de la page **[!UICONTROL Paramètres de l’équipe]**.

1. Sélectionnez un statut ou plusieurs statuts pour chaque type d’élément de travail.

   >[!NOTE]
   >
   >Tenez compte des points suivants lorsque vous sélectionnez des statuts pour des tâches ou des problèmes :
   >
   >* Lorsque vous sélectionnez un état pour chaque type d’élément de travail, l’état de la tâche ou du problème est défini sur cet état lorsqu’un utilisateur clique sur [!UICONTROL Terminé] sur son élément. Si vous définissez plusieurs états pour chaque type d’élément de travail, un menu déroulant est ajouté au bouton [!UICONTROL Terminé] et l’utilisateur doit sélectionner un état pour modifier l’état de l’élément de travail.
   >* Vous pouvez associer uniquement les états au niveau du système au bouton [!UICONTROL Terminé] . Vous ne pouvez pas associer des statuts spécifiques à un groupe à des statuts d’élément de travail.
   >* Lorsqu’un utilisateur affecté à l’élément place l’élément dans l’état associé au bouton [!UICONTROL Terminé], l’élément s’affiche sous la forme [!UICONTROL Terminé] pour cet utilisateur, que l’état sélectionné soit [!UICONTROL Terminé] ou [!UICONTROL Fermé] ou un état de travail.
   >   
   >   
   >  Par exemple, l’association du bouton [!UICONTROL Terminé] à En cours entraîne l’affichage de l’élément de travail comme [!UICONTROL Terminé] pour l’utilisateur qui passe de l’état Nouveau à En cours.
   >   
   >* Les types de problèmes sont personnalisables et peuvent avoir des noms différents de ceux répertoriés ci-dessous dans votre environnement.\
   >  Les types de tâches et de problèmes par défaut sont les suivants :
   >     
   >   * [!UICONTROL Tâches]
   >   * [!UICONTROL Problème]
   >   * [!UICONTROL Demande]
   >   * [!UICONTROL Modifier l&#39;ordre]
   >   * [!UICONTROL Rapport sur les bogues]

   Si la tâche ou le problème est assigné à plusieurs utilisateurs, l’option &quot;[!UICONTROL Terminé avec ma partie]&quot; s’affiche dans le menu déroulant, en plus des statuts multiples choisis pour votre équipe.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Associer des utilisateurs et utilisatrices à une équipe d’accueil

Pour que les modifications apportées à la fonctionnalité de bouton [!UICONTROL Terminé] soient visibles par les utilisateurs, vous pouvez rendre visible l’équipe dont vous avez modifié les paramètres à l’équipe d’accueil des utilisateurs.

Pour associer des utilisateurs et des utilisatrices à une équipe d’accueil :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront].

1. Cliquez sur **[!UICONTROL Utilisateurs et utilisatrices]**, puis sélectionnez la ou les personnes que vous souhaitez associer à une équipe d’accueil.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Dans la section **[!UICONTROL Organisation]**, sélectionnez le champ **[!UICONTROL Équipe d’accueil]**. Commencez à saisir le nom de l’équipe dont vous souhaitez associer les paramètres aux utilisateurs et utilisatrices. Cliquez sur le nom de l’équipe lorsque vous le voyez dans la liste.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.\
   Les utilisateurs et utilisatrices que vous avez sélectionnés sont maintenant associés à une équipe d’accueil.
Tous les paramètres de l’équipe, y compris les états associés au bouton [!UICONTROL Terminé], sont désormais visibles par ces utilisateurs.

## Configurez le bouton [!UICONTROL Terminé] lorsque l’état [!UICONTROL Résolu] a été supprimé.

Si un utilisateur ne dispose pas d’une équipe d’accueil et que la valeur par défaut à l’échelle du système pour [!UICONTROL Resolved] ([!UICONTROL RLV]) a été supprimée, un administrateur [!DNL Workfront] peut configurer l’état [!UICONTROL Closed] pour le groupe sur le projet. [!DNL Workfront] sélectionne cet état pour un problème fermé lorsque l’utilisateur clique sur le bouton [!DNL Done].

### Rechercher le groupe associé au projet

Lorsqu’un utilisateur crée un projet, son groupe d’accueil est automatiquement affecté au projet. Les utilisateurs disposant de l’accès [!UICONTROL Gérer] au projet peuvent modifier ce groupe dans la section [!UICONTROL Détails du projet] à tout moment. Pour comprendre l’état utilisé par [!DNL Workfront] pour un problème terminé dans ce cas, vous devez comprendre le groupe associé au projet sur lequel le problème se trouve et l’état par défaut de [!UICONTROL Fermé] de ce groupe pour les problèmes.

Pour trouver le groupe associé au projet :

1. Accédez à un projet.
1. Sur le côté gauche de la page, cliquez sur **[!UICONTROL Détails du projet]**.
1. Recherchez la section **[!UICONTROL Association de projet]** , puis recherchez **[!UICONTROL Groupe]**.\
   Il s’agit du nom du groupe que vous devez utiliser pour vérifier l’état dans la zone Configuration . Consultez la section suivante pour savoir comment mettre à jour l’état par défaut d’un groupe spécifique.

### Mettre à jour l’état par défaut d’un groupe spécifique

En tant qu&#39;administrateur [!UICONTROL Workfront], vous pouvez mettre à jour l&#39;état d&#39;un groupe spécifique :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **[!UICONTROL Configurer]** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Préférences du projet]**, puis sur **[!UICONTROL Statuts]**.

1. Cliquez sur **[!UICONTROL Problèmes]**, puis saisissez le nom du groupe dans la zone de recherche **[!UICONTROL États du système]** située à droite.

1. Sélectionnez le groupe.
1. Cliquez sur le menu déroulant **[!UICONTROL Définir les états par défaut]** , puis sélectionnez un état par défaut pour [!UICONTROL Fermé]. [!DNL Workfront] utilise cet état pour un problème fermé lorsqu’un utilisateur clique sur le bouton [!UICONTROL Terminé] .

   >[!IMPORTANT]
   >
   >Cet état est utilisé uniquement lorsque l’utilisateur n’a pas affecté d’équipe d’accueil et que l’état [!UICONTROL RLV] a été supprimé.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
