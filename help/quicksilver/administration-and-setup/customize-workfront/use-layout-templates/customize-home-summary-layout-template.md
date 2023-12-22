---
title: Personnalisation de l’accueil et du résumé à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Vous pouvez utiliser un modèle de mise en page pour configurer ce que voient les utilisateurs lorsqu’ils cliquent sur une tâche ou un problème dans Accueil et dans le résumé. Chaque configuration que vous effectuez en suivant les étapes ci-dessous affecte de la même manière la zone Accueil et le panneau Résumé. Ces personnalisations ne s’appliquent pas au panneau Résumé du document.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: abaabf12d63ea1e279d14ad8467ac239e6c211b1
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 2%

---

# Personnalisation de l’accueil et du résumé à l’aide d’un modèle de mise en page

Vous pouvez utiliser un modèle de mise en page pour configurer ce que voient les utilisateurs lorsqu’ils cliquent sur une tâche ou un problème dans Accueil et dans le résumé. Chaque configuration que vous effectuez en suivant les étapes ci-dessous affecte de la même manière la zone Accueil et le panneau Résumé. Ces personnalisations ne s’appliquent pas au panneau Résumé du document.

Vous pouvez configurer les éléments suivants :

* Quels champs s’affichent pour une tâche ou un problème dans la zone Détails et dans quel ordre ?
* Si les mises à jour, l’heure consignée, les documents joints et les horodatages s’affichent pour une tâche ou un problème sélectionné

Vous pouvez également personnaliser les champs affichés par les utilisateurs dans la zone Accueil lorsque les utilisateurs cliquent sur l’approbation d’un projet, l’approbation de document ou l’approbation de version de document qui leur est affectée.

Pour plus d’informations sur la zone d’accueil, voir [Utilisation de la zone Accueil](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). Pour plus d’informations sur le panneau Résumé, voir [Aperçu du résumé](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Pour plus d’informations sur la création de modèles de mise en page, voir [Création et gestion des modèles de mise en page](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Création et modification des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs pour que les modifications que vous avez apportées soient visibles par d’autres utilisateurs. Pour plus d’informations sur l’attribution d’un modèle de mise en page aux utilisateurs, voir [Affecter des utilisateurs à un modèle de mise en page](../use-layout-templates/assign-users-to-layout-template.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur système.
Pour les exécuter pour un groupe, vous devez être un responsable de ce groupe.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnalisation de l’accueil et du résumé à l’aide d’un modèle de mise en page

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow.png) under **Personnalisation des éléments affichés par les utilisateurs**, puis cliquez sur **Accueil et résumé**.

1. Dans la liste qui s’affiche à gauche, cliquez sur le type d’objet (**Tâche**, **Problèmes**, **Projets**, **Documents**, ou **Versions de document**) que vous souhaitez personnaliser dans Accueil et Résumé.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tâches</td> 
      <td> <p>Dans Accueil, votre configuration pour ce paramètre affecte la zone située à droite d’une tâche lorsqu’un utilisateur clique sur la tâche. Et, dans une liste de tâches, cela affecte le panneau Résumé qui s’affiche sur le côté droit de la page lorsqu’un utilisateur sélectionne une tâche, puis clique sur l’icône Ouvrir le résumé . <img src="assets/summary-panel-icon.png">.</p> <p>Par exemple, vous pouvez déterminer les champs que les utilisateurs voient dans la zone Détails lorsqu’ils sélectionnent des tâches dans Accueil :</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>Et lorsqu’ils sélectionnent une tâche dans le Résumé :</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problèmes</td> 
      <td> <p>Dans Accueil, votre configuration pour ce paramètre affecte la zone située à droite d’un problème lorsqu’un utilisateur clique sur le problème.</p> <p>Dans une liste de problèmes, ce paramètre affecte le panneau Résumé qui s’affiche sur le côté droit de la page lorsqu’un utilisateur sélectionne un problème, puis clique sur l’icône Ouvrir le résumé . <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projets</td> 
      <td>Dans Accueil, lorsqu’un utilisateur clique sur une approbation de projet qui lui est affectée, votre configuration pour ce paramètre affecte la zone située à droite de la validation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td>Dans Accueil, lorsqu’un utilisateur clique sur une approbation de document qui lui est affectée, votre configuration pour ce paramètre affecte la zone située à droite de la validation.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Versions des documents</td> 
      <td>Dans Accueil, lorsqu’un utilisateur clique sur une approbation qui lui est affectée pour une version spécifique d’un document, votre configuration pour ce paramètre affecte la zone située à droite de la validation.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Si une tâche n’est pas affectée, l’utilisateur affecté au modèle de mise en page ne verra pas les personnalisations des champs dans le résumé.

1. (Conditionnel) Si vous avez cliqué sur Tâches ou Problèmes à l’étape précédente, sélectionnez la catégorie de tâches ou de problèmes que vous souhaitez personnaliser.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Conditionnel) Si la variable **Bouton Définir l’action principale** s’affiche dans le menu déroulant (si vous sélectionnez **Tâche** ou **Problèmes** dans la liste de gauche), cliquez sur l’action principale (**Terminé** ou **État**) que vous souhaitez mettre à la disposition des utilisateurs dans la zone Accueil et dans le panneau Résumé lorsqu’ils visualisent une tâche ou un problème.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Ajouter ![](assets/add-item-plus-in-circle-blue.png) ou masquer ![](assets/close-or-hide---x.png) pour le type d’objet sélectionné.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Répétez les étapes 3 à 6 pour personnaliser la zone d’accueil et le panneau Résumé pour tout autre type d’objet.
1. Cliquez sur **Paramètres globaux**, près du coin inférieur gauche, puis activez ou désactivez l’une des options suivantes liées aux objets Adobe Workfront dans Accueil et Résumé :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher les mises à jour pour le travail</td> 
      <td>Affiche toutes les mises à jour effectuées sur une tâche ou un problème sélectionné dans Accueil ou Résumé. Cela inclut les mises à jour du système et les mises à jour effectuées par un utilisateur. Les utilisateurs peuvent toujours filtrer les mises à jour du système, comme décrit dans la section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Activation ou désactivation des mises à jour système</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mise à jour du travail</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Consigner les heures de travail</td> 
      <td>Affiche l’option Temps passé sur le travail lorsqu’une tâche ou un problème est sélectionné, ce qui permet aux utilisateurs de consigner le temps passé sur les tâches directement à partir des zones Accueil et Résumé.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afficher les documents associés au travail</td> 
      <td>Affiche une zone Documents dans Accueil et Résumé lorsqu’une tâche ou un problème est sélectionné, répertoriant tous les documents associés à la tâche ou au problème. Les utilisateurs peuvent cliquer sur les documents pour les afficher dans une fenêtre d’aperçu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Masquer l'horodatage</td> 
      <td>Masque les horodatages des champs de date suivants dans Accueil et Résumé :
       <ul>
        <li>Date d'achèvement prévue</li>
        <li>Date d'engagement</li>
        <li>Date d’envoi</li>
       </ul><p><b>REMARQUE</b>: lorsque cette option est activée, les tâches arrivant en retard sont déplacées vers le regroupement En retard dans la liste des tâches à domicile en fonction de la date uniquement et non de l’heure.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

Pour plus d’informations sur les modèles de mise en page, voir [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
