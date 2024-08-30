---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configuration du bouton Terminé pour les tâches
description: Le bouton Terminé permet de définir automatiquement le statut d’une tâche ou d’un problème. Par défaut, Adobe Workfront marque une tâche comme terminée lorsqu’une personne cessionnaire clique sur Terminé sur son élément de travail.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 99%

---

# Configurer le bouton [!UICONTROL Terminé] pour les tâches

Le bouton [!UICONTROL Terminer] permet de définir automatiquement le statut d’une tâche ou d’un problème. Par défaut, [!UICONTROL Adobe Workfront] marque une tâche comme [!UICONTROL Terminé] lorsqu’une personne cessionnaire clique sur Terminé sur son élément de travail.

## Vue d’ensemble

Les personnes disposant de certaines autorisations peuvent configurer le bouton [!UICONTROL Terminé] pour refléter certains statuts dans le système. Le bouton [!UICONTROL Terminé] fonctionne de deux manières pour les tâches dans [!UICONTROL Workfront] :

* Si l’utilisateur ou l’utilisatrice a une équipe principale d’affectée, un administrateur ou une administratrice [!DNL Workfront] ou un utilisateur ou une utilisatrice disposant d’une licence de [!UICONTROL plan] peut configurer le bouton [!UICONTROL Terminé] pour refléter certains statuts pour les membres de l’équipe. Voir [Configurer le bouton [!UICONTROL Terminé] pour une équipe](#configure-the-uicontrol-done-button-for-a-team) dans cet article.
* Si l’utilisateur ou l’utilisatrice n’a pas d’[!UICONTROL équipe principale], mais dispose d’[!UICONTROL autres équipes] dans leur profil, Workfront recherche le paramètre du bouton [!UICONTROL Terminé] sur l’une des équipes associées à l’utilisateur ou l’utilisatrice. La sélection est aléatoire et le statut associé à l’une des équipes est utilisé pour la tâche.
* Si l’utilisateur ou l’utilisatrice n’a pas d’équipe principale d’affectée, le bouton [!UICONTROL Terminé] pour les tâches est lié à un statut d’achèvement. Aucune option de configuration n’est disponible dans ce scénario. La valeur par défaut du bouton [!UICONTROL Terminé] est automatiquement celle de ce statut.

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
   >* Lorsqu’une personne affectée à l’élément le place dans le statut associé avec le bouton [!UICONTROL Terminé], l’élément s’affiche comme [!UICONTROL Terminé] pour cette personne, que le statut sélectionné soit [!UICONTROL Terminé] ou [!UICONTROL Clos] ou un statut en cours.
   >   
   >   
   >  Par exemple, l’association du bouton [!UICONTROL Terminé] à [!UICONTROL En cours] entraîne l’affichage de l’élément de travail comme [!UICONTROL Terminé] pour la personne qui modifie le statut de [!UICONTROL Nouveau] à [!UICONTROL En cours].
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
Tous les paramètres de l’équipe, y compris les statuts associés au bouton [!UICONTROL Terminé], sont désormais visibles pour ces utilisateurs et utilisatrices.
