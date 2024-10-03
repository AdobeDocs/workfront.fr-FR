---
title: Personnalisation de l’accueil et du résumé à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Vous pouvez utiliser un modèle de disposition pour configurer ce que voient les personnes lorsqu’elles cliquent sur une tâche ou un problème dans Accueil et dans le résumé. Chaque configuration que vous effectuez en suivant les étapes ci-dessous affecte de la même manière la zone Accueil et le panneau Résumé. Ces personnalisations ne s’appliquent pas au panneau Résumé du document.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 115757a829b92c13cb684369120e26602b9a1782
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 90%

---

# Personnaliser l’Accueil et le Résumé à l’aide d’un modèle de disposition

<span class="preview">Cet article sera renommé &quot;Personnaliser le panneau de résumé à l’aide d’un modèle de mise en page&quot; lorsque la page d’accueil héritée sera supprimée de Workfront avec la version du 4e trimestre le 17 octobre. 2024.</span>

Vous pouvez utiliser un modèle de disposition pour configurer ce que voient les personnes lorsqu’elles cliquent sur une tâche ou un problème dans Accueil et dans le résumé. Chaque configuration que vous effectuez en suivant les étapes ci-dessous affecte de la même manière la zone Accueil et le panneau Résumé. Ces personnalisations ne s’appliquent pas au panneau Résumé du document.

Vous pouvez configurer les éléments suivants :

* Les champs qui s’affichent pour une tâche ou un problème dans la zone Détails et dans quel ordre.
* Si les mises à jour, le temps consigné, les documents joints et les horodatages s’affichent pour une tâche ou un problème sélectionné.

Vous pouvez également personnaliser les champs affichés par les personnes dans la zone Accueil lorsque les personnes cliquent sur l’approbation d’un projet, l’approbation de document ou l’approbation de version du document qui leur est affectée.

Pour plus d’informations sur la zone Accueil, voir [Utiliser la zone Accueil](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). Pour plus d’informations sur le panneau Résumé, voir [Vue d’ensemble du résumé](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Pour plus d’informations sur la création de modèles de disposition, voir [Créer et gérer des modèles de disposition](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de disposition aux utilisateurs et utilisatrices, voir [Affecter des utilisateurs et utilisatrices à un modèle de disposition](../use-layout-templates/assign-users-to-layout-template.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouveau : Standard</p>
  <p> Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.
Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser l’Accueil et le Résumé à l’aide d’un modèle de disposition

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow.png) sous **Personnaliser des éléments affichés par les utilisateurs et utilisatrices**, puis cliquez sur **Accueil et résumé**.

1. Dans la liste de gauche, cliquez sur le type d’objet (**Tâches**, **Problèmes**, **Projets**, **Documents** ou **Document Versions**) que vous souhaitez personnaliser dans Accueil et résumé.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tâches</td> 
      <td> <p>Dans Accueil, votre configuration pour ce paramètre affecte la zone située à droite d’une tâche lorsqu’une personne clique sur la tâche. Et, dans une liste de tâches, cela affecte le panneau Résumé qui s’affiche sur le côté droit de la page lorsqu’une personne sélectionne une tâche, puis clique sur l’icône Ouvrir le résumé <img src="assets/summary-panel-icon.png">.</p> <p>Par exemple, vous pouvez déterminer les champs que les personnes voient dans la zone Détails lorsqu’elles sélectionnent des tâches dans Accueil :</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>Et lorsqu’elles sélectionnent une tâche dans le Résumé :</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problèmes</td> 
      <td> <p>Dans Accueil, votre configuration pour ce paramètre affecte la zone située à droite d’un problème lorsqu’une personne clique sur le problème.</p> <p>Dans une liste de problèmes, ce paramètre affecte le panneau Résumé qui s’affiche sur le côté droit de la page lorsqu’une personne sélectionne un problème, puis clique sur l’icône Ouvrir le résumé <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projets</td> 
      <td>Dans Accueil, lorsqu’une personne clique sur une approbation de projet qui lui est affectée, votre configuration pour ce paramètre affecte la zone située à droite de l’approbation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td>Dans Accueil, lorsqu’une personne clique sur une approbation de document qui lui est affectée, votre configuration pour ce paramètre affecte la zone située à droite de l’approbation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versions des documents</td> 
      <td>Dans Accueil, lorsqu’une personne clique sur une approbation qui lui est affectée pour une version spécifique d’un document, votre configuration pour ce paramètre affecte la zone située à droite de l’approbation.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Si une tâche n’est pas affectée, la personne affectée au modèle de disposition ne verra pas les personnalisations des champs dans le résumé.

1. (Le cas échéant) Si vous avez cliqué sur Tâches ou Problèmes à l’étape précédente, sélectionnez la catégorie de tâches ou de problèmes que vous souhaitez personnaliser.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Le cas échéant) Si le menu déroulant **Définir le bouton d’action principal** s’affiche (si vous sélectionnez **Tâches** ou **Problèmes** dans la liste de gauche), cliquez sur l’action principale (**Terminé** ou **Statut**) que vous souhaitez mettre à la disposition des personnes dans la zone Accueil et dans le panneau Résumé lorsqu’elles visualisent une tâche ou un problème.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Ajoutez ![](assets/add-item-plus-in-circle-blue.png) ou masquez ![](assets/close-or-hide---x.png) pour le type d’objet sélectionné.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Répétez les étapes 3 à 6 pour personnaliser la zone Accueil et le panneau Résumé pour tout autre type d’objet.
1. Cliquez sur **Paramètres globaux**, près du coin inférieur gauche, puis activez ou désactivez l’une des options suivantes liées aux objets Adobe Workfront dans Accueil et Résumé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher les mises à jour pour le travail</td> 
      <td>Affiche toutes les mises à jour effectuées sur une tâche ou un problème sélectionné dans Accueil ou Résumé. Cela inclut les mises à jour du système et les mises à jour effectuées par un utilisateur ou une utilisatrice. Les personnes peuvent toujours filtrer les mises à jour du système, comme décrit dans la section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Activer ou désactiver des mises à jour système</a> dans <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mettre à jour le travail</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consigner les heures de travail</td> 
      <td>Affiche l’option Consigner le temps passé sur le travail lorsqu’une tâche ou un problème est sélectionné, ce qui permet aux personnes de consigner le temps passé sur les tâches directement à partir des zones Accueil et Résumé.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher les documents associés au travail</td> 
      <td>Affiche une zone Documents dans Accueil et Résumé lorsqu’une tâche ou un problème est sélectionné, répertoriant tous les documents associés à la tâche ou au problème. Les personnes peuvent cliquer sur les documents pour les afficher dans une fenêtre d’aperçu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer l'horodatage</td> 
      <td>Masque les horodatages des champs de date suivants dans Accueil et Résumé :
       <ul>
        <li>Date d'achèvement prévue</li>
        <li>Date d’engagement</li>
        <li>Date d’envoi</li>
       </ul><p><b>NOTE</b> :</p> <p> Lorsque cette option est activée, les tâches arrivant en retard sont déplacées vers le regroupement Tard dans la liste des tâches à domicile en fonction de la date uniquement et non de l’heure.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

Pour plus d’informations sur les modèles de disposition, voir [Créer et gérer des modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
