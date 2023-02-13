---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Affichage et modification des informations sur l’article dans le panneau Scrum
description: Lors de l’affichage d’une mosaïque d’article sur le panorama Kanban, certaines informations peuvent être modifiées en ligne, directement à partir de la mosaïque d’article.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Affichez et modifiez les informations de l’article dans la [!UICONTROL Scrum] board

## Comprendre les informations qui peuvent être affichées et modifiées

Lors de l’affichage d’une mosaïque d’articles sur le tableau de bord, les informations du tableau suivant sont disponibles. Vous pouvez modifier la plupart des informations intégrées, directement à partir de la mosaïque de l’article.

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
   <td> <p>Nom du projet avec un lien direct vers le projet<br>Ce lien s’affiche uniquement sur les articles (tâches parents, et non sous-tâches) lors de l’utilisation de la vue agile sur une itération ; il n’est pas affiché lors de l’utilisation d’une vue agile sur un projet.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Nombre de points ou d’heures terminés sur l’article et nombre de points ou d’heures attribués à l’article<br>Ces chiffres sont utilisés pour calculer et afficher le [!UICONTROL % terminé] de chaque article.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Le [!UICONTROL Pourcentage terminé] pour chaque article et numéro.<br>Le [!UICONTROL Pourcentage terminé] pour l’itération est calculé d’après le [!UICONTROL Pourcentage terminé] pour chaque article.</p> <p>Lors de la mise à jour de [!UICONTROL Pourcentage terminé] pour un article ou un problème, vous pouvez choisir un nombre compris entre 0 et 100.</p> </td> 
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
   <td> <p>Tout champ supplémentaire (y compris les champs personnalisés) qui peut avoir été ajouté à la vue agile en modifiant la vue agile, comme décrit dans "Création et personnalisation d’une vue [!UICONTROL Agile]" dans <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Présentation des vues dans [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou version ultérieure</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Autorisations d’objet</strong></td> 
   <td> <p>Modifier l’accès à la tâche ou au problème</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Affichage et modification d’informations sur une mosaïque d’article

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. (Facultatif) Cliquez sur le **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]** pour sélectionner une itération spécifique, ou sélectionnez **[!UICONTROL Itération actuelle]**.

1. Accédez au [!UICONTROL Scrum] tableau de bord agile.
1. Développez l’objet [!UICONTROL histoire] pour afficher tous les champs associés à l’article.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Facultatif) Pour modifier un champ, cliquez dessus, puis apportez toute modification.

   Vous devez avoir [!UICONTROL Modifier] droits à la tâche ou au problème pour modifier la mosaïque de l’article.

>[!NOTE]
>
>Pour modifier la variable [!UICONTROL Pourcentage terminé], vous devez saisir un nombre compris entre 0 et 100. Le champ n’est pas un curseur que vous pouvez déplacer.
