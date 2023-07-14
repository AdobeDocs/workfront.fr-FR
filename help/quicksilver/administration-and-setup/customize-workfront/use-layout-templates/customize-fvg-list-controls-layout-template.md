---
title: Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: En tant qu’administrateur Workfront, vous pouvez utiliser un modèle de mise en page pour spécifier les commandes de liste qui apparaissent dans les menus déroulants Filtre, Affichage et Regroupement. Ces menus apparaissent au-dessus des listes dans Workfront, telles que la liste des tâches d’un projet.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page

En tant qu’administrateur Adobe Workfront, vous pouvez utiliser un modèle de mise en page pour spécifier les commandes de liste qui s’affichent dans les menus déroulants Filtre, Affichage et Regroupement . Ces menus apparaissent au-dessus des listes dans Workfront, telles que la liste des tâches d’un projet :

![](assets/filter-view-grouping-layout-templates.png)

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

## Personnaliser les contrôles de liste Filtrer, Afficher et Regroupement :

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur la flèche vers le bas ![](assets/down-arrow-blue.png) under **Personnalisation des éléments affichés par les utilisateurs**, puis cliquez sur **Listes** dans le menu déroulant qui s’affiche.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Cliquez sur la flèche vers le bas ![](assets/down-arrow-blue.png) under **Sélectionner une liste à personnaliser**, puis sélectionnez le type d’objet Workfront pour lequel vous souhaitez personnaliser les contrôles des listes Filtrer, Afficher et Regroupement.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Si vous sélectionnez Projets comme liste à personnaliser, puis désactivez Projets actifs ou Projets personnels dans la section Filtre , les utilisateurs ne verront plus ou ne pourront plus utiliser ce filtre :
   >
   >* Dans la liste des filtres qui s’affichent lorsqu’ils cliquent sur l’icône de filtre ![](assets/filter-nwepng.png) au-dessus d’une liste :
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* Dans l’en-tête de la zone Projets :
   >   
   >  ![](assets/disable-filter-pills.png)

1. (Facultatif) Si vous souhaitez modifier le filtre, la vue ou le regroupement par défaut pour le modèle de mise en page, passez la souris sur le filtre, la vue ou le regroupement, puis cliquez sur **Définir comme valeur par défaut**.

   Les valeurs par défaut que vous choisissez déterminent quels utilisateurs de filtrage, d’affichage et de regroupement verront dans les listes de Workfront lorsque le modèle de mise en page leur sera attribué. Si vous ne modifiez pas ces valeurs par défaut, les utilisateurs voient toutes les listes comme suit :

   * **Filtres**: Tous
   * **Affichage**: Standard (le cas échéant) certaines listes n’ont pas cette vue)
   * **Regroupement**: Rien

   Vous pouvez masquer les options Toutes, Standard et Rien après avoir sélectionné d’autres valeurs par défaut (voir Étape 5), mais elles ne peuvent pas être supprimées.

   Vous pouvez supprimer toute autre option utilisée par défaut, mais vous devez d’abord sélectionner une autre option par défaut.

   Pour plus d’informations sur la suppression de filtres, de vues et de regroupements, voir [Créer, modifier et partager des filtres, des vues et des regroupements par défaut](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Masquez et ajoutez des contrôles de liste comme suit :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Masquer un contrôle de liste</td> 
      <td> <p>Décochez ou décochez la case en regard du contrôle de liste à masquer ou à afficher.</p> <p>Si une case à cocher est grisée, vous ne pouvez pas masquer cette commande de liste. La valeur par défaut <img src="assets/default-pill.png"> pour chaque contrôle de liste est grisé, car vous ne pouvez pas masquer le paramètre actuellement configuré comme valeur par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajouter un contrôle de liste personnalisé</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Cliquez sur <strong>Ajouter un filtre</strong>, <strong>Ajouter une vue</strong>ou <strong>Ajouter un groupement</strong> au bas de la liste Filtre, Affichage ou Regroupement. Dans la zone qui s’affiche, commencez à saisir le nom d’un contrôle de liste personnalisé existant précédemment créé pour votre organisation, puis cliquez sur le nom lorsqu’il apparaît.</li> 
         <li value="2"> Si vous souhaitez que le nouveau contrôle de liste personnalisé soit défini comme filtre, affichage ou regroupement par défaut pour le modèle de mise en page, cliquez sur <strong>Définir comme valeur par défaut</strong>. </li> 
         <li value="3"> <p>Cliquez sur <strong>Ajouter</strong> lorsque vous avez terminé.</p> <p><b>NOTE</b>: <p>Les utilisateurs peuvent ajouter des contrôles de liste personnalisés à leurs propres listes. Si vous ajoutez des contrôles de liste personnalisés dans un modèle de mise en page, vos contrôles de liste sont ajoutés et les leurs sont déplacés vers le bas du panneau. les vôtres ne remplacent pas les leurs.</p> <p>Cela est également vrai si vous affectez l’utilisateur à un nouveau modèle de mise en page qui comporte des contrôles de liste personnalisés. </p> <p>Pour plus d’informations sur la personnalisation des contrôles de liste, voir <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Présentation des filtres dans Adobe Workfront</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Présentation des vues dans Adobe Workfront</a>, et <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Présentation des regroupements dans Adobe Workfront</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continuez à personnaliser le modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Vous pouvez cliquer à tout moment sur Enregistrer pour enregistrer votre progression, puis continuer à modifier le modèle ultérieurement.
