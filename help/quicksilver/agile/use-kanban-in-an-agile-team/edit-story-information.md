---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Modifier les informations de l’article
description: Lors de l’affichage d’une mosaïque d’article sur le panorama Kanban, certaines informations peuvent être modifiées en ligne, directement à partir de la mosaïque d’article.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Modifier les informations de l’article

## Comprendre les informations qui peuvent être affichées et modifiées {#understand-what-information-can-be-viewed-and-edited}

Lors de l’affichage d’une mosaïque d’article sur le [!UICONTROL Kanban] , les informations du tableau suivant sont disponibles. Vous pouvez modifier la plupart des informations intégrées, directement à partir de la mosaïque de l’article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Informations</strong> </th> 
   <th><strong>Visible</strong> </th> 
   <th><strong>Modifiable en ligne</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nom de l’article avec un lien direct vers la tâche ou le problème</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Nom du projet avec un lien direct vers le projet</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Nombre de points ou d’heures terminés sur l’article et nombre de points ou d’heures attribués à l’article<br>Ces chiffres sont utilisés pour calculer et afficher le pourcentage de finalisation pour chaque article.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Le [!UICONTROL Pourcentage terminé] pour chaque article et numéro.<br>[!UICONTROL Le pourcentage terminé] pour l’itération est calculé en fonction du [!UICONTROL % terminé] pour chaque article.<br></p> <p>Lors de la mise à jour de [!UICONTROL Pourcentage terminé] pour un article ou un problème, vous pouvez choisir un nombre compris entre 0 et 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>À qui l’article est affecté</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Couleur ou catégorie de la mosaïque</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Tout champ supplémentaire (y compris les champs personnalisés) qui peut avoir été ajouté à la vue agile en modifiant la vue agile, comme décrit dans "Création et personnalisation d’une vue agile" dans <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Présentation des vues dans [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Affichage et modification d’informations sur une mosaïque d’article

1. Cliquez sur le bouton *[!UICONTROL *Menu principal]** icône ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. (Facultatif) Cliquez sur le **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Kanban dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Accédez au [!UICONTROL Kanban] panorama.
1. Développez la mosaïque de l’article pour afficher tous les champs associés à l’article.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Facultatif) Pour modifier un champ, cliquez dessus, puis apportez toute modification.\
   Vous devez avoir [!UICONTROL Modifier] droits à la tâche ou au problème afin de modifier la mosaïque de l’article.\
   Pour plus d’informations sur chaque champ et sur son édition, voir [Comprendre les informations qui peuvent être affichées et modifiées](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Pour modifier la variable [!UICONTROL Pourcentage terminé], vous devez saisir un nombre compris entre 0 et 100. Le champ n’est pas un curseur que vous pouvez déplacer.
