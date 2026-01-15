---
title: Personnalisation de la terminologie de l’interface utilisateur à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un modèle de mise en page pour modifier les libellés de certains objets qui s’affichent dans Workfront afin de correspondre aux termes utilisés dans votre organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 90%

---

# Personnaliser la terminologie de l’interface d’utilisation à l’aide d’un modèle de mise en page

En tant qu’administrateur ou administratrice Adobe Workfront, vous pouvez utiliser un modèle de mise en page pour modifier les libellés de certains objets qui s’affichent dans Workfront afin de correspondre aux termes utilisés dans votre organisation.

Après avoir enregistré un modèle de mise en page dans lequel vous avez modifié la terminologie, puis avoir effectué une déconnexion et reconnexion à Workfront, les libellés que vous avez modifiés apparaissent à l’endroit où les libellés par défaut apparaissent dans la plupart des zones de Workfront :

* Menu principal
* Toutes les zones accessibles à partir du menu principal
* Tous les onglets
* Tous les menus
* Les éléments de Report Builder et de création de rapports (vues, filtres et regroupements)
* Boutons Enregistrer
* Fichiers exportés
* E-mails
* Applications mobiles

>[!NOTE]
>
>* La zone du module complémentaire Outlook n’affiche pas les libellés personnalisés.
>* Vous pouvez rencontrer des problèmes de grammaire et d’autres problèmes lorsque vous personnalisez des libellés. Par exemple, si vous remplacez « Problème » par « Demande », l’expression « Une demande » peut se trouver dans l’interface d’utilisation. Pour plus d’informations, voir [Implications de la personnalisation des noms d’objet](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) dans l’article [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>

Pour plus d’informations sur les modèles de mise en page, voir [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Créer et modifier des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de mise en page à des utilisateurs et utilisatrices, voir [Attribuer un modèle de mise en page à des utilisateurs et utilisatrices](../use-layout-templates/assign-users-to-layout-template.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.</p>
        <p>Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser la terminologie de l’interface utilisateur

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur **Définir la terminologie** près du coin supérieur droit de la page.
1. Effectuez l’une des opérations suivantes :

   * Pour utiliser un autre terme fourni par Workfront, cliquez sur la flèche vers le bas ![Flèche vers le bas](assets/dropdown-arrow.png) en regard du libellé, puis cliquez sur le libellé secondaire de votre choix dans la liste déroulante.

     >[!NOTE]
     >
     >Les autres libellés fournis dans les listes déroulantes sont pris en charge dans les versions de Workfront localisées pour les langues autres que l’anglais.

   * Pour fournir votre propre alternative personnalisée au libellé affiché pour un objet, cliquez sur **Définir un nom personnalisé** à droite du libellé, puis saisissez le **Singulier** et le **Pluriel** du terme personnalisé. Cliquez sur **Réinitialiser** si vous changez d’avis.

     Vous pouvez personnaliser les noms d’objet suivants :

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Objets Workfront</p></td>
        <td>
          <p>Portfolio</p>
          <p>Programme</p>
          <p>Projet</p>
          <p>Tâche</p>
          <p>Problème</p>
          <p>Objectif</p>
          <p>Résultat</p>
          <p>Activité</p>
         </ul></td>
        <td><p>Pour plus d’informations sur ces objets, voir <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Présentation des objets dans Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Objets des Objectifs Workfront</p></td>
        <td>
         <ul>
          <p>Objectif</p>
          <p>Résultat</p>
          <p>Activité</p>
         </ul></td>
        <td><p>Ces objets nécessitent une licence supplémentaire. Pour plus d’informations, voir <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Vue d’ensemble d’Ojectifs Adobe Workfront</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Objets du planificateur de scénarios Workfront</p></td>
        <td>
         <ul>
          <p>Initiative</p>
          <p>Scénario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Ces objets nécessitent une licence supplémentaire. Pour plus d’informations, voir <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Commencer avec le planificateur de scénarios</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Lorsque vous avez terminé, cliquez sur **Terminé**.

   >[!TIP]
   >
   >Après avoir cliqué sur Terminé (et même après avoir enregistré votre modèle de mise en page), vous pouvez toujours revenir aux paramètres Définir la terminologie et cliquer sur Réinitialiser en regard des termes personnalisés pour les renvoyer à leur statut par défaut.

1. Continuez à personnaliser le modèle de mise en page. Vous pouvez cliquer sur **Appliquer** à tout moment pour enregistrer votre progression.

   Ou

   Si vous avez terminé la personnalisation, cliquez sur **Enregistrer et fermer**.

1. Pour afficher vos changements de terminologie :

   1. Déconnectez-vous puis reconnectez-vous à Workfront.
   1. Fermez tous les onglets du navigateur que vous avez ouverts pour votre environnement Workfront.

   >[!IMPORTANT]
   >
   >Cela est également requis pour toute personne qui a utilisé le modèle de mise en page avant d’apporter des modifications à la terminologie.

Pour plus d’informations sur les modèles de mise en page, voir [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
