---
title: Personnalisation du panneau Résumé à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Vous pouvez utiliser un modèle de mise en page pour configurer ce que voient les utilisateurs lorsqu’ils cliquent sur une tâche ou un problème dans le résumé. Chaque configuration que vous effectuez à l’aide des étapes ci-dessous affecte le panneau Résumé. Ces personnalisations ne s’appliquent pas au panneau Résumé du document.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 43cf88c533b80324266f0660648c6a1ab13ca8fc
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 59%

---

# Personnalisation du panneau Résumé à l’aide d’un modèle de mise en page


Vous pouvez utiliser un modèle de mise en page pour configurer ce que voient les utilisateurs lorsqu’ils cliquent sur une tâche ou un problème dans le résumé. Chaque configuration que vous effectuez à l’aide des étapes ci-dessous affecte le panneau Résumé. Ces personnalisations ne s’appliquent pas au panneau Résumé du document.

Vous pouvez configurer les éléments suivants :

* Les champs qui s’affichent pour une tâche ou un problème dans la zone Détails et dans quel ordre.
* Si les mises à jour, le temps consigné, les documents joints et les horodatages s’affichent pour une tâche ou un problème sélectionné.

Vous pouvez également personnaliser les champs affichés par les personnes dans la zone Accueil lorsque les personnes cliquent sur l’approbation d’un projet, l’approbation de document ou l’approbation de version du document qui leur est affectée.

Pour plus d’informations sur le panneau Résumé, voir [Vue d’ensemble du résumé](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

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

## Personnalisation du panneau Résumé à l’aide d’un modèle de mise en page

1. Commencez à travailler sur un modèle de disposition, comme décrit dans la section [Créer et gérer des modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow.png) sous **Personnaliser ce que les utilisateurs voient**, puis cliquez sur **Panneau de résumé**.

1. Dans la liste de gauche, cliquez sur le type d’objet (**Tâches**, **Problèmes**, **Projets**, **Documents** ou **Document Versions**) que vous souhaitez personnaliser dans le panneau Résumé.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tâches</td> 
      <td><p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problèmes</td> 
      <td><p>Dans une liste de problèmes, ce paramètre affecte le panneau Résumé qui s’affiche sur le côté droit de la page lorsqu’une personne sélectionne un problème, puis clique sur l’icône Ouvrir le résumé <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projets</td> 
      <td><p>Dans Accueil, lorsqu’une personne clique sur une approbation de projet qui lui est affectée, votre configuration pour ce paramètre affecte la zone située à droite de l’approbation.</p>
      <p>IMPORTANT : il s’agit d’une fonction obsolète. Toute modification apportée à cette zone est liée à une fonctionnalité supprimée par Workfront. Cette option sera supprimée de Workfront avec une mise à jour de maintenance ultérieure.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td><p>Dans Accueil, lorsqu’une personne clique sur une approbation de document qui lui est affectée, votre configuration pour ce paramètre affecte la zone située à droite de l’approbation.</p>
      <p>IMPORTANT : il s’agit d’une fonction obsolète. Toute modification apportée à cette zone est liée à une fonctionnalité supprimée par Workfront. Cette option sera supprimée de Workfront avec une mise à jour de maintenance ultérieure.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versions des documents</td> 
      <td><p>Dans Accueil, lorsqu’une personne clique sur une approbation qui lui est affectée pour une version spécifique d’un document, votre configuration pour ce paramètre affecte la zone située à droite de l’approbation.</p>
      <p>IMPORTANT : il s’agit d’une fonction obsolète. Toute modification apportée à cette zone est liée à une fonctionnalité supprimée par Workfront. Cette option sera supprimée de Workfront avec une mise à jour de maintenance ultérieure.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Si une tâche n’est pas affectée, la personne affectée au modèle de disposition ne verra pas les personnalisations des champs dans le résumé.

1. (Le cas échéant) Si vous avez cliqué sur Tâches ou Problèmes à l’étape précédente, sélectionnez la catégorie de tâches ou de problèmes que vous souhaitez personnaliser.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Conditionnel) Si le menu déroulant **Définir le bouton d’action principale** s’affiche (si vous sélectionnez **Tâches** ou **Problèmes** dans la liste de gauche), cliquez sur l’action principale (**Terminé** ou **État**) que vous souhaitez mettre à la disposition des utilisateurs dans le panneau Résumé lorsqu’ils affichent une tâche ou un problème.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Ajoutez ![](assets/add-item-plus-in-circle-blue.png) ou masquez ![](assets/close-or-hide---x.png) pour le type d’objet sélectionné.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Répétez les étapes 3 à 6 pour personnaliser le panneau Résumé pour tout autre type d’objet.
1. Cliquez sur **Paramètres globaux**, près du coin inférieur gauche, puis activez ou désactivez l’une des options suivantes liées aux objets Adobe Workfront dans le résumé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher les mises à jour pour le travail</td> 
      <td>Affiche toutes les mises à jour effectuées sur une tâche ou un problème sélectionné dans le panneau Résumé. Cela inclut les mises à jour du système et les mises à jour effectuées par un utilisateur ou une utilisatrice. Les personnes peuvent toujours filtrer les mises à jour du système, comme décrit dans la section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Activer ou désactiver des mises à jour système</a> dans <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mettre à jour le travail</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consigner les heures de travail</td> 
      <td>Affiche l’option Consigner le temps passé sur le travail lorsqu’une tâche ou un problème est sélectionné, ce qui permet aux personnes de consigner le temps passé sur les tâches directement à partir des zones Accueil et Résumé.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher les documents associés au travail</td> 
      <td>Affiche une zone Documents dans le panneau Résumé lorsqu’une tâche ou un problème est sélectionné, répertoriant tous les documents associés à la tâche ou au problème. Les personnes peuvent cliquer sur les documents pour les afficher dans une fenêtre d’aperçu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer l'horodatage</td> 
      <td>Masque les horodatages des champs de date suivants dans le panneau Résumé :
       <ul>
        <li>Date d'achèvement prévue</li>
        <li>Date d’engagement</li>
        <li>Date d’envoi</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

Pour plus d’informations sur les modèles de disposition, voir [Créer et gérer des modèles de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
