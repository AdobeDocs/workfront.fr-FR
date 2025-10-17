---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Comment les groupes héritent des statuts
description: 'Voici les statuts disponibles pour un groupe :'
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 99%

---

# Héritage des statuts par les groupes

Voici les statuts disponibles pour un groupe :

* Statuts personnalisés créés pour le groupe, comme expliqué dans [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Statuts hérités du système et des niveaux supérieurs de la hiérarchie du groupe, comme expliqué dans cet article.

## Héritage des statuts

Votre groupe hérite des statuts lorsque l’une des situations suivantes se produit :

* Vous créez le groupe.
* Un administrateur ou une administratrice verrouille un statut dans un groupe de niveau supérieur.
* Un administrateur ou une administratrice supprime un autre groupe et choisit votre groupe pour le remplacer.

Le tableau ci-dessous explique chacune de ces circonstances.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Création de votre groupe</td> 
   <td> <p>Lorsque vous créez un nouveau groupe, il hérite automatiquement :</p> 
    <ul> 
     <li>des statuts déverrouillés dans le groupe d’un niveau supérieur, si le nouveau groupe est un sous-groupe ;</li> 
    </ul> 
    <ul> 
     <li>des statuts verrouillés au niveau du système.</li> 
    </ul> 
     <b>EXEMPLE</b></span></span> 
     <p>Supposons qu’un groupe appelé Marketing comporte deux sous-groupes appelés Communications marketing et Image de marque.</p> 
     <p>Un administrateur ou une administratrice du groupe Marketing crée un nouveau statut personnalisé appelé Découverte.</p> 
     <p>Plus tard, vous créez un nouveau sous-groupe sous le groupe Marketing et l’appellez Publicité.</p> 
     <p>Votre sous-groupe hérite du statut Découverte parce que vous avez créé le groupe après que l’autre administrateur ou administratrice a créé le statut Découverte déverrouillé.</p> 
     <p>Comme les sous-groupes Communications marketing et Image de marque existaient déjà sous le groupe Marketing lorsque cela s’est produit, ils n’héritent pas du statut Découverte déverrouillé.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Verrouillage d’un statut à un niveau supérieur par un administrateur ou une administratrice</td> 
   <td> <p>Lorsqu’un administrateur ou une administratrice Workfront verrouille un statut au niveau du système, votre groupe en hérite avec tous les autres groupes du système.</p> <p>De même, lorsqu’un administrateur ou une administratrice verrouille un statut pour un groupe supérieur au vôtre, votre groupe en hérite ainsi que tous les autres sous-groupes inférieurs au groupe supérieur.</p> <p><b>REMARQUE</b> : par la suite, si un administrateur ou une administratrice déverrouille l’un de ces statuts au niveau du système ou dans un groupe supérieur au vôtre, votre groupe conserve le statut dont il a hérité précédemment. Il s’agit désormais d’une version distincte du statut, que vous pouvez personnaliser en fonction de votre groupe.</p> 
    <p><b>EXEMPLE</b></p>
    <p>L’administrateur ou l’administratrice du groupe Marketing verrouille le statut Découverte mentionné ci-dessus pour s’assurer que les trois sous-groupes en bénéficient.</p> 
    <p>Avec votre groupe Publicité, les groupes Communications marketing et Image de marque ont désormais le statut Découverte. Ils en ont hérité lorsqu’ils ont été verrouillés dans le groupe Marketing supérieur.</p> 
    <p>L’administrateur ou l’administratrice du groupe Marketing déverrouille ensuite le statut Découverte afin que les trois sous-groupes disposent de leur propre version du statut Découverte. Vous et les administrateurs ou administratrices des deux autres groupes pouvez maintenant personnaliser le statut Découverte pour répondre aux besoins de vos groupes.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Suppression d’un groupe par un administrateur ou une administratrice</td> 
   <td> <p>Lorsqu’un administrateur ou une administratrice supprime un groupe et choisit le vôtre pour le remplacer dans le système, votre groupe hérite des statuts personnalisés du groupe supprimé s’ils n’existent pas déjà dans votre groupe.</p> 
   <p><b>EXEMPLE </b></p>
     <p>Un groupe appelé Messages doit fusionner avec votre groupe Publicité. Un administrateur ou une administratrice Workfront supprime donc le groupe Messages et choisit votre groupe pour le remplacer.</p> 
     <p>Le groupe Messages avait un statut unique appelé En cours de traitement. Votre groupe Publicité dispose désormais de ce statut.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Héritage des configurations de statut

Lorsque vous créez un groupe de premier niveau, il hérite des configurations suivantes du niveau système. Lorsque vous créez un sous-groupe, il hérite des configurations suivantes du groupe immédiatement supérieur.

* Configurations de statut par défaut

  Pour plus d’informations à ce sujet, voir [Utiliser des statuts personnalisés comme statuts par défaut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Configurations de l’ordre d’affichage des statuts

  Pour plus d’informations à ce sujet, voir [Réorganiser les statuts de niveau système et de groupe](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Si quelqu’un modifie ces configurations après la création de votre groupe, ses statuts ne sont pas affectés.
