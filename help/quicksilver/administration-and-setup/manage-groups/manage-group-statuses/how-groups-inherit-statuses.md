---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Héritage de statuts par les groupes
description: 'Lorsque vous répertoriez les états disponibles pour un groupe, les éléments suivants s’affichent :'
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 1%

---

# Héritage de statuts par les groupes

Lorsque vous répertoriez les états disponibles pour un groupe, les éléments suivants s’affichent :

* États personnalisés créés pour le groupe, comme expliqué dans la section [Créer ou modifier un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Les états hérités du système et des niveaux supérieurs de la hiérarchie des groupes, comme expliqué dans cet article.

## Hériter des statuts

Votre groupe hérite des états lorsque l’un des événements suivants se produit :

* Vous créez le groupe.
* Un administrateur verrouille un état dans un groupe de niveau supérieur.
* Un administrateur supprime un autre groupe et choisit votre groupe pour le remplacer.

Le tableau ci-dessous explique chacune de ces circonstances.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Lorsque vous créez un groupe</td> 
   <td> <p>Lorsque vous créez un groupe, il hérite automatiquement des éléments suivants :</p> 
    <ul> 
     <li>Statuts déverrouillés dans le groupe à un niveau supérieur, si le nouveau groupe est un sous-groupe.</li> 
    </ul> 
    <ul> 
     <li>Statuts verrouillés au niveau du système .</li> 
    </ul> 
     <b>EXEMPLE :</b></span></span> 
     <p>Supposons qu’un groupe appelé Marketing comporte deux sous-groupes appelés Communications marketing et Valorisation de marque.</p> 
     <p>Un administrateur de groupe du groupe Marketing crée un état personnalisé appelé Discovery.</p> 
     <p>Par la suite, vous créez un sous-groupe sous le groupe Marketing et vous l’appelez Advertising.</p> 
     <p>Votre sous-groupe hérite de l’état Découverte car vous avez créé le groupe après que l’autre administrateur a créé l’état Découverte déverrouillée.</p> 
     <p>Comme les sous-groupes Communications marketing et Valorisation de marque existaient déjà sous le groupe Marketing lorsque cela s’est produit, ils n’héritent pas de l’état Découverte déverrouillée.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Lorsqu’un administrateur verrouille un état à un niveau supérieur</td> 
   <td> <p>Lorsqu’un administrateur Workfront verrouille un état au niveau du système, votre groupe l’hérite avec tous les autres groupes du système.</p> <p>De même, lorsqu’un administrateur verrouille l’état d’un groupe situé au-dessus de votre groupe, celui-ci l’hérite avec tous les autres sous-groupes situés en-dessous du groupe supérieur.</p> <p><b>REMARQUE</b> : par la suite, si un administrateur déverrouille l’un de ces états au niveau du système ou dans un groupe situé au-dessus de votre groupe, votre groupe conserve l’état qu’il a hérité précédemment. Il s’agit maintenant d’une version distincte de l’état et vous pouvez la personnaliser uniquement pour votre groupe.</p> 
    <p><b>EXEMPLE :</b></p>
    <p>L’administrateur du groupe marketing verrouille l’état Discovery mentionné ci-dessus pour s’assurer que les trois sous-groupes le possèdent.</p> 
    <p>Avec votre groupe Advertising, les groupes Communications marketing et Valorisation de marque ont désormais le statut Découverte . Ils l’héritaient lorsqu’il était verrouillé dans le groupe marketing situé au-dessus d’eux.</p> 
    <p>L’administrateur du groupe marketing déverrouille ensuite l’état Découverte afin que les trois sous-groupes disposent de leur propre version de l’état Découverte . Désormais, vous et les administrateurs des 2 autres groupes pouvez personnaliser l’état de la détection pour répondre aux besoins de vos groupes.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Lorsqu’un administrateur supprime un groupe</td> 
   <td> <p>Lorsqu’un administrateur supprime un groupe et choisit le vôtre de prendre sa place dans le système, votre groupe hérite des statuts personnalisés du groupe supprimé s’il n’existe pas déjà dans votre groupe.</p> 
   <p><b>EXEMPLE : </b></p>
     <p>Un groupe appelé Messagerie doit fusionner avec votre groupe Advertising. Par conséquent, un administrateur Workfront supprime le groupe Messagerie et choisit votre groupe pour le remplacer.</p> 
     <p>Le groupe de messagerie avait un statut unique appelé In Process. Ce statut est désormais disponible pour votre groupe Advertising.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Héritage des configurations de statut

Lorsque vous créez un groupe de niveau supérieur, il hérite des configurations suivantes du niveau système. Lorsque vous créez un sous-groupe, il hérite des configurations suivantes du groupe supérieur suivant.

* Configurations d’état par défaut

  Pour plus d’informations à ce sujet, voir [Utilisation d’états personnalisés comme états par défaut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Paramétrages de l’ordre d’affichage des états

  Pour plus d’informations à ce sujet, voir [Réorganiser les états au niveau du système et du groupe](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Si quelqu’un modifie ces configurations après la création de votre groupe, ses états ne sont pas affectés.
