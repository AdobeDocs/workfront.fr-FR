---
product-area: home
navigation-topic: use-the-home-area
title: Gérer vos approbations à l’aide du widget Mes approbations
description: Le widget Mes approbations affiche toutes vos approbations en attente, affectées, déléguées et soumises au même endroit. Ici, vous pouvez filtrer et organiser vos approbations, prendre des décisions et déléguer les approbations si nécessaire.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 36%

---

# Gérer vos approbations à l’aide du widget Mes approbations

Le widget Mes approbations affiche toutes vos approbations en attente, affectées, déléguées et soumises au même endroit. Ici, vous pouvez filtrer et organiser vos approbations, prendre des décisions et déléguer les approbations si nécessaire.

Le widget Mes approbations prend en charge les approbations des objets Workfront suivants :

* Tâches
* Problèmes
* Projets
* Documents
* Épreuves
* Requêtes d’enregistrement de planification
* Feuilles de temps

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou version ultérieure</p>
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Afficher ou supérieur aux objets associés à des approbations</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Afficher ou supérieures pour les objets associés aux approbations</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Approuver le travail à partir du widget Mes approbations

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **[!UICONTROL Accueil]**.
1. (Conditionnel) Cliquez sur **Personnaliser** pour ajouter le widget **Mes approbations**.
1. (Conditionnel) Cliquez sur le menu déroulant **Filtre**, puis sélectionnez **Toutes** pour voir les approbations qui vous sont affectées et qui vous sont déléguées.

   >[!NOTE]
   >
   >Les approbations affectées à des fonctions ou à des groupes ne s’affichent pas dans la page d’accueil. Les approbations affectées aux équipes s’affichent dans le widget Mes approbations pour chaque membre de l’équipe.


1. Sélectionnez l’élément pour lequel vous souhaitez prendre une décision d’approbation.

   ![Widget Mes approbations](assets/my-approvals-widget.png)

1. Cliquez sur l’une des options disponibles lorsque vous prenez une décision d’approbation dans le panneau de droite. Les options suivantes s’affichent dans le coin supérieur droit de la page, en fonction du type d’élément que vous approuvez :

   <table>
   <tr>
      <td>
      <p><strong>Accès</strong></p>
      </td>
      <td>
      <p><strong>Éléments de travail</strong></p>
      </td>
      <td>
      <p><strong>Documents</strong></p>
      </td>
      <td>
      <p><strong>Épreuves</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Subvention</li>
      <li>Ignorer</li>
      </ul>
      Vous pouvez ajuster le niveau d’accès dans le menu déroulant <b>Modifier l’accès</b> si vous le souhaitez.
      </td>
      <td>
         <ul>
         <li>Approuver</li>
         <li>Rejeter</li>
         </ul>
      Vous pouvez laisser un commentaire avec votre décision en cliquant sur le menu déroulant dans le bouton de décision.
      </td>
      <td>
   Affecté en tant qu'approbateur
         <ul>
         <li>Approuver</li>
         <li>Approuver avec des modifications</li>
         <li>Travail nécessaire</li>
         </ul>
   Affecté en tant que réviseur/réviseuse
         <ul>
         <li>Terminer mon examen</li>
         </ul>
      Les options de cette colonne s'appliquent uniquement aux approbations unifiées. Les approbations de documents hérités apparaissent comme les approbations d’éléments de travail. 
      </td>
      <td>
         <ul>
         <li>Accéder au BAT</li>
         </ul>
         Vous prenez votre décision dans la visionneuse d’épreuves. Pour plus d’informations sur la révision d’une épreuve, consultez la section <a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Réviser des épreuves dans Adobe Workfront</a>.
      </td>
   </tr>
   </table>

Une fois la décision prise, l’approbation est supprimée du widget Mon approbation .