---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurer le bouton Terminé pour les tâches
description: Le bouton Terminé permet de définir automatiquement l’état d’une tâche ou d’un problème. Par défaut, Adobe Workfront marque une tâche comme terminée lorsqu’un cessionnaire clique sur Terminé sur son élément de travail.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 32%

---

# Configuration du bouton [!UICONTROL Terminé] pour les tâches

Le bouton [!UICONTROL Terminé] peut automatiquement définir l’état d’une tâche ou d’un problème. Par défaut, [!UICONTROL Adobe Workfront] marque une tâche comme [!UICONTROL Terminée] lorsqu’un cessionnaire clique sur Terminé sur Terminé dans son élément de travail.

## Vue d’ensemble

Les utilisateurs disposant de certaines autorisations peuvent configurer le bouton [!UICONTROL Terminé] pour refléter certains états du système. Le bouton [!UICONTROL Terminé] fonctionne de deux manières différentes pour les tâches dans [!UICONTROL Workfront] :

* Si l’utilisateur a une équipe d’accueil affectée, un administrateur [!DNL Workfront] ou un utilisateur disposant d’une licence [!UICONTROL Plan] peut configurer le bouton [!UICONTROL Terminé] afin de refléter certains états pour les membres de l’équipe. Voir [Configuration du bouton [!UICONTROL Terminé] pour une équipe](#configure-the-uicontrol-done-button-for-a-team) dans cet article.
* Si l’utilisateur ne dispose pas d’une [!UICONTROL équipe d’accueil], mais que son profil comporte [!UICONTROL autres équipes], Workfront recherche le paramètre du bouton [!UICONTROL Terminé] sur l’une des équipes associées à l’utilisateur. La sélection est aléatoire et l’état associé à l’une des équipes est utilisé pour la tâche.
* Si l’utilisateur n’a pas d’équipe d’accueil affectée, le bouton [!UICONTROL Terminé] pour les tâches est associé à un état complet. Aucune option de configuration n’est disponible dans ce scénario. Le bouton [!UICONTROL Terminé] propose automatiquement cet état par défaut.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] forfait*</strong></p></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] licence*</strong></p></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour savoir quel plan ou type de licence vous avez, contactez votre administrateur [!DNL Workfront].

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
   >  Par exemple, l’association du bouton [!UICONTROL Terminé] à [!UICONTROL En cours] entraîne l’affichage de l’élément de travail en tant que [!UICONTROL Terminé] pour l’utilisateur qui passe de [!UICONTROL Nouveau] à [!UICONTROL En cours].
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
