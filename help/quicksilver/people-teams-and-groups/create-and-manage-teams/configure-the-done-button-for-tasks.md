---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configuration du bouton Terminé pour les tâches
description: Le bouton Terminé permet de définir automatiquement l’état d’une tâche ou d’un problème. Par défaut, Adobe Workfront marque une tâche comme terminée lorsqu’un cessionnaire clique sur Terminé sur son élément de travail.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# Configurez la variable [!UICONTROL Terminé] bouton pour les tâches

Le [!UICONTROL Terminé] peut définir automatiquement l’état d’une tâche ou d’un problème. Par défaut, [!UICONTROL Adobe Workfront] marque une tâche comme [!UICONTROL Terminé] lorsqu’une personne désignée clique sur Terminé sur son élément de travail.

## Vue d’ensemble

Les utilisateurs disposant de certaines autorisations peuvent configurer la variable [!UICONTROL Terminé] pour refléter certains états du système. Il existe deux manières différentes de [!UICONTROL Terminé] fonctionne pour les tâches dans [!UICONTROL Workfront]:

* Si l’utilisateur a une équipe d’accueil affectée, une [!DNL Workfront] un administrateur ou un utilisateur disposant d’un [!UICONTROL Plan] peut configurer la variable [!UICONTROL Terminé] pour refléter certains états des membres de l’équipe. Voir [Configurez la variable [!UICONTROL Terminé] bouton pour une équipe](#configure-the-uicontrol-done-button-for-a-team) dans cet article.
* Si l’utilisateur n’a pas de [!UICONTROL Équipe Accueil], mais ils ont [!UICONTROL Autres équipes] dans leur profil, Workfront recherche le paramètre de la variable [!UICONTROL Terminé] sur l’une des équipes associées à l’utilisateur. La sélection est aléatoire et l’état associé à l’une des équipes est utilisé pour la tâche.
* Si l’utilisateur ne dispose pas d’une équipe d’accueil affectée, la variable [!UICONTROL Terminé] pour les tâches est lié à un état complet. Aucune option de configuration n’est disponible dans ce scénario. Le [!UICONTROL Terminé] par défaut, ce statut est défini.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] plan*</strong></p></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] license*</strong></p></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan ou le type de licence dont vous disposez, contactez votre [!DNL Workfront] administrateur.

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
   >  Par exemple, l’association de la variable [!UICONTROL Terminé] bouton avec [!UICONTROL En cours] entraîne l’affichage de l’élément de travail en tant que [!UICONTROL Terminé] pour l’utilisateur qui modifie l’état à partir de [!UICONTROL Nouveau] to [!UICONTROL En cours].
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
