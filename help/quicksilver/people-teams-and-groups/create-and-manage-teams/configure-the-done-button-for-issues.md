---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configuration du bouton Terminé pour les problèmes
description: Le bouton Terminé permet de définir automatiquement l’état d’une tâche ou d’un problème. Par défaut, Adobe Workfront marque un problème comme résolu lorsqu’un cessionnaire clique sur Terminé sur son élément de travail.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 1%

---

# Configurez la variable [!UICONTROL Terminé] bouton pour les problèmes

Le [!UICONTROL Terminé] peut définir automatiquement l’état d’une tâche ou d’un problème. Par défaut, [!DNL Adobe Workfront] marque un problème comme [!UICONTROL Résolu] lorsqu’un cessionnaire clique [!UICONTROL Terminé] sur leur élément de travail.

## Vue d’ensemble

Les utilisateurs disposant de certaines autorisations peuvent configurer la variable [!UICONTROL Terminé] pour refléter certains états du système. Il existe 3 manières différentes de [!UICONTROL Terminé] fonctionne pour les problèmes dans [!DNL Workfront]:

* Si l’utilisateur a un [!UICONTROL Équipe Accueil], un [!DNL Workfront] un administrateur ou un utilisateur disposant d’un [!UICONTROL Plan] peut configurer la variable [!UICONTROL Terminé] pour refléter certains états des membres de l’équipe. Voir [Configurez la variable [!UICONTROL Terminé] bouton pour une équipe](#configure-the-uicontrol-done-button-for-a-team) dans cet article.
* Si l’utilisateur n’a pas de [!UICONTROL Équipe Accueil], mais ils ont [!UICONTROL Autres équipes] dans leur profil, Workfront recherche le paramètre de la variable [!UICONTROL Terminé] sur l’une des équipes associées à l’utilisateur. La sélection est aléatoire et l’état associé à l’une des équipes est utilisé pour le problème.
* Si l’utilisateur n’a pas de [!UICONTROL Équipe Accueil] affecté, [!UICONTROL Terminé] est lié à un bouton généré par le système. [!UICONTROL Résolu] état comportant le code à trois lettres [!UICONTROL RLV]. Aucune option de configuration n’est disponible dans ce scénario. Le [!UICONTROL Terminé] par défaut, ce statut est défini.
* Si la variable [!UICONTROL Résolu] ([!UICONTROL RLV]) est supprimé et l’utilisateur marque le problème comme [!UICONTROL Terminé] has no [!UICONTROL Équipe Accueil], l’état du problème par défaut est lié à ce qui est défini comme valeur par défaut pour [!UICONTROL Fermé] pour le groupe affecté au projet, le problème appartient à . L’administrateur Workfront peut configurer un paramètre par défaut à l’échelle du système pour le groupe. Voir [Configurez la variable [!UICONTROL Terminé] lorsque la variable [!UICONTROL Résolu] Le statut a été supprimé](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) dans cet article.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td>L’accès administrateur système est requis pour configurer le bouton [!UICONTROL Terminé] lorsque l’état [!UICONTROL Résolu] est supprimé.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Configurez la variable [!UICONTROL Terminé] bouton pour une équipe

Vous pouvez modifier l’état appliqué à l’élément de travail avec la fonction [!UICONTROL Terminé] bouton . Vous pouvez également définir plusieurs états et permettre à l’utilisateur de choisir l’état approprié.

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Équipes]**.

1. Cliquez sur le bouton **[!UICONTROL Equipe de commutation]** , puis sélectionnez une nouvelle équipe dans le menu déroulant ou recherchez une équipe dans la barre de recherche.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis cliquez sur **[!UICONTROL Modifier]**.
1. Recherchez le **[!UICONTROL Bouton Terminé]** au bas de la section **[!UICONTROL Paramètres de l’équipe]** page.

1. Sélectionnez un état ou plusieurs états pour chaque type d’élément de travail.

   >[!NOTE]
   >
   >Tenez compte des points suivants lorsque vous sélectionnez des états pour des tâches ou des problèmes :
   >
   >* Lorsque vous sélectionnez un état pour chaque type d’élément de travail, l’état de la tâche ou du problème est défini sur cet état lorsqu’un utilisateur clique sur [!UICONTROL Terminé] sur leur élément . Si vous définissez plusieurs états pour chaque type d’élément de travail, un menu déroulant est ajouté au [!UICONTROL Terminé] et l’utilisateur doit sélectionner un état pour modifier l’état de l’élément de travail.
   >* Vous pouvez associer uniquement les états au niveau du système à la variable [!UICONTROL Terminé] bouton . Vous ne pouvez pas associer des états spécifiques à un groupe à des états d’éléments de travail.
   >* Lorsqu’un utilisateur affecté à l’élément le place dans l’état associé à l’événement [!UICONTROL Terminé] , l’élément s’affiche sous la forme [!UICONTROL Terminé] pour cet utilisateur, que l’état sélectionné soit ou non [!UICONTROL Terminé] ou [!UICONTROL Fermé] ou un état de fonctionnement.
   >   
   >   
   >  Par exemple, l’association de la variable [!UICONTROL Terminé] avec le bouton En cours, l’élément de travail s’affiche comme [!UICONTROL Terminé] pour l’utilisateur qui passe de l’état Nouveau à En cours.
   >   
   >* Les types de problème sont personnalisables et peuvent avoir des noms différents de ceux répertoriés ci-dessous dans votre environnement.\
   >  Voici les tâches par défaut et les types de problèmes :
   >     
   >   * [!UICONTROL Tâches]
   >   * [!UICONTROL Problème]
   >   * [!UICONTROL Demande]
   >   * [!UICONTROL Modifier l&#39;ordre]
   >   * [!UICONTROL Rapport sur les bogues]

   Si la tâche ou le problème est assigné à plusieurs utilisateurs, un &quot;[!UICONTROL C&#39;est fait de ma part.]&quot; dans le menu déroulant, en plus des statuts multiples choisis pour votre équipe.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

## Association d’utilisateurs à une équipe d’accueil

Pour apporter des modifications au [!UICONTROL Terminé] pour rendre la fonction de bouton visible aux utilisateurs, vous pouvez rendre visible l’équipe dont vous avez modifié les paramètres l’équipe d’accueil des utilisateurs.

Pour associer des utilisateurs à une équipe d’accueil :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront].

1. Cliquez sur **[!UICONTROL Utilisateurs]**, puis sélectionnez le ou les utilisateurs que vous souhaitez associer à une équipe d’accueil.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Dans le **[!UICONTROL Organisation]** , sélectionnez **[!UICONTROL Équipe Accueil]** champ . Commencez à saisir le nom de l’équipe dont vous souhaitez associer les paramètres aux utilisateurs. Cliquez sur le nom de l’équipe lorsque vous le voyez dans la liste.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.\
   Les utilisateurs que vous avez sélectionnés sont désormais associés à une équipe d’accueil.
Tous les paramètres de l’équipe, y compris les états associés à la variable [!UICONTROL Terminé] sont désormais visibles par ces utilisateurs.

## Configurez la variable [!UICONTROL Terminé] lorsque la variable [!UICONTROL Résolu] Le statut a été supprimé

Si un utilisateur ne dispose pas d’une équipe d’accueil et que la valeur par défaut à l’échelle du système pour [!UICONTROL Résolu] ([!UICONTROL RLV]) a été supprimé, une [!DNL Workfront] l’administrateur peut configurer la variable [!UICONTROL Fermé] statut du groupe sur le projet. [!DNL Workfront] sélectionne cet état pour un problème fermé lorsque l’utilisateur clique sur la variable [!DNL Done] bouton .

### Rechercher le groupe associé au projet

Lorsqu’un utilisateur crée un projet, son groupe d’accueil est automatiquement affecté au projet. Utilisateurs avec [!UICONTROL Gérer] l’accès au projet peut modifier ce groupe dans la variable [!UICONTROL Détails du projet] à tout moment. Comprendre quel état [!DNL Workfront] utilise pour un problème terminé, dans ce cas, vous devez comprendre quel groupe est associé au projet sur lequel le problème se trouve et quel est l’état par défaut pour [!UICONTROL Fermé] ce groupe a des problèmes.

Pour trouver le groupe associé au projet :

1. Accédez à un projet.
1. Sur le côté gauche de la page, cliquez sur **[!UICONTROL Détails du projet]**.
1. Recherchez la variable **[!UICONTROL Association de projets]** , puis recherchez **[!UICONTROL Groupe]**.\
   Il s’agit du nom du groupe que vous devez utiliser pour vérifier l’état dans la zone Configuration . Consultez la section suivante pour savoir comment mettre à jour l’état par défaut d’un groupe spécifique.

### Mettre à jour l’état par défaut d’un groupe spécifique

Comme [!UICONTROL Workfront] administrateur, vous pouvez mettre à jour l’état d’un groupe spécifique :

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).
1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Préférences du projet]**, puis **[!UICONTROL Statuts]**.

1. Cliquez sur **[!UICONTROL Problèmes]**, puis saisissez le nom du groupe dans la variable **[!UICONTROL États du système]** zone de recherche située à droite.

1. Sélectionnez le groupe.
1. Cliquez sur le bouton **[!UICONTROL Définition des états par défaut]** , puis choisissez un état par défaut pour [!UICONTROL Fermé]. [!DNL Workfront] utilise cet état pour un problème fermé lorsqu’un utilisateur clique sur le bouton [!UICONTROL Terminé] bouton .

   >[!IMPORTANT]
   >
   >Cet état est utilisé uniquement lorsque l’utilisateur n’a pas affecté d’équipe d’accueil et que la variable [!UICONTROL RLV] a été supprimé.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
