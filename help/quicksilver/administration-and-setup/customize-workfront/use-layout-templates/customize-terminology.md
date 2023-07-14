---
title: Personnalisation de la terminologie de l’interface utilisateur à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur d’Adobe Workfront, vous pouvez utiliser un modèle de mise en page pour modifier les libellés de certains objets qui s’affichent dans Workfront afin de correspondre aux termes utilisés dans votre entreprise.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 3%

---

# Personnalisation de la terminologie de l’interface utilisateur à l’aide d’un modèle de mise en page

En tant qu’administrateur d’Adobe Workfront, vous pouvez utiliser un modèle de mise en page pour modifier les libellés de certains objets qui s’affichent dans Workfront afin de correspondre aux termes utilisés dans votre entreprise.

Après avoir enregistré un modèle de mise en page dans lequel vous avez modifié la terminologie, puis vous être déconnecté de Workfront et de nouveau connecté, les libellés que vous avez modifiés apparaissent à l’endroit où les libellés par défaut apparaissent dans la plupart des zones de Workfront :

* Menu principal
* Toutes les zones accessibles à partir du menu principal
* Tous les onglets
* Tous les menus
* Eléments de Report Builder et de reporting (vues, filtres et regroupements)
* Bouton Enregistrer
* Fichiers exportés
* E-mails
* Applications mobiles

>[!NOTE]
>
>* La zone du module complémentaire Outlook n’affiche pas les libellés personnalisés.
>* Vous pouvez rencontrer des problèmes de grammaire et d’autres problèmes lorsque vous personnalisez des étiquettes. Par exemple, si vous remplacez &quot;Problème&quot; par &quot;Requête&quot;, l’expression &quot;Une requête&quot; peut se trouver dans l’interface utilisateur. Pour plus d’informations, voir [Implications de la personnalisation des noms d’objet](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) dans l’article [Présentation des objets dans Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

Pour plus d’informations sur les modèles de mise en page, voir [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

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
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur système.
Pour les exécuter pour un groupe, vous devez être un responsable de ce groupe.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnalisation de la terminologie de l’interface utilisateur

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur **Définir la terminologie** près du coin supérieur droit de la page.
1. Effectuez l’une des opérations suivantes :

   * Pour utiliser un autre terme fourni par Workfront, cliquez sur la flèche vers le bas  ![](assets/dropdown-arrow.png) en regard du libellé, cliquez sur l’autre libellé de votre choix dans la liste déroulante.

     >[!NOTE]
     >
     >Les autres libellés fournis dans les listes déroulantes sont pris en charge dans les versions de Workfront localisées pour les langues autres que l’anglais.

   * Pour fournir votre propre alternative personnalisée au libellé affiché pour un objet, cliquez sur **Définition d’un nom personnalisé** à droite du libellé, puis saisissez la valeur **Singular** et **Plural** formulaires du terme personnalisé. Vous pouvez cliquer sur **Réinitialiser** si vous changez d&#39;avis.

     Vous pouvez personnaliser les noms d’objet suivants :

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
        <td><p>Pour plus d’informations sur ces objets, voir <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Présentation des objets dans Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Objets Workfront Objectifs</p></td>
        <td>
         <ul>
          <p>Objectif</p>
          <p>Résultat</p>
          <p>Activité</p>
         </ul></td>
        <td><p>Ces objets nécessitent une licence supplémentaire. Pour plus d’informations, voir <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Présentation des objectifs d’Adobe Workfront</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Objets du planificateur de scénario Workfront</p></td>
        <td>
         <ul>
          <p>Initiative</p>
          <p>Scénario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Ces objets nécessitent une licence supplémentaire. Pour plus d’informations, voir <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Prise en main du planificateur de scénarios</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Lorsque vous avez terminé, cliquez sur **Terminé**.

   >[!TIP]
   >
   >Après avoir cliqué sur Terminé (et même après avoir enregistré votre modèle de mise en page), vous pouvez toujours revenir aux paramètres Définir la terminologie et cliquer sur Réinitialiser en regard des termes personnalisés pour les renvoyer à leur état par défaut.

1. Continuez à personnaliser le modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

1. Pour afficher vos changements de terminologie :

   1. Déconnectez-vous puis reconnectez-vous à Workfront.
   1. Fermez tous les onglets du navigateur que vous avez ouverts pour votre environnement Workfront.

   >[!IMPORTANT]
   >
   >Cela est également requis pour toute personne qui a utilisé le modèle de mise en page avant d’apporter des modifications à la terminologie.

Pour plus d’informations sur les modèles de mise en page, voir [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
