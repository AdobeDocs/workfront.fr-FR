---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Modifier les informations sur la story
description: Lors de l’affichage d’une mosaïque d’article sur le panorama Kanban, certaines informations peuvent être modifiées en ligne, directement à partir de la mosaïque d’article.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 15%

---

# Modifier les informations sur la story

## Comprendre les informations qui peuvent être affichées et modifiées {#understand-what-information-can-be-viewed-and-edited}

Lors de l’affichage d’une mosaïque d’article sur le panorama [!UICONTROL Kanban], les informations du tableau suivant sont disponibles. Vous pouvez modifier la plupart des informations intégrées, directement à partir de la mosaïque de l’article.

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
   <td> <p>Le nombre de points ou d’heures terminés sur l’article et le nombre de points ou d’heures attribués à l’article<br>Ces chiffres sont utilisés pour calculer et afficher le pourcentage terminé pour chaque article.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Le [!UICONTROL Pourcentage terminé] pour chaque article et numéro.<br>[!UICONTROL Le pourcentage terminé] pour l’itération est calculé d’après le [!UICONTROL Pourcentage terminé] pour chaque article.<br></p> <p>Lors de la mise à jour de [!UICONTROL Pourcentage terminé] pour un article ou un problème, vous pouvez choisir un nombre compris entre 0 et 100.</p> </td> 
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
   <td> <p>Tout champ supplémentaire (y compris les champs personnalisés) qui peut avoir été ajouté à la vue agile en modifiant la vue agile, comme décrit dans "Création et personnalisation d’une vue agile" dans la <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">vue d’ensemble dans [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] forfait*</strong></td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licence*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations des niveau d’accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur [!DNL Workfront] s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la manière dont l’équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Affichage et modification d’informations sur une mosaïque d’article

1. Cliquez sur l’icône *[!UICONTROL *Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Equipes]**.

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Kanban dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Allez sur la carte [!UICONTROL Kanban].
1. Développez la mosaïque de l’article pour afficher tous les champs associés à l’article.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Facultatif) Pour modifier un champ, cliquez dessus, puis apportez toute modification.\
   Vous devez disposer des droits [!UICONTROL Modifier] sur la tâche ou le problème pour pouvoir modifier la mosaïque de l’article.\
   Pour plus d&#39;informations sur chaque champ et sur son édition, voir [Comprendre quelles informations peuvent être affichées et modifiées](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Pour modifier le [!UICONTROL pourcentage terminé], vous devez saisir un nombre compris entre 0 et 100. Le champ n’est pas un curseur que vous pouvez déplacer.
