---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gestion des cartes de taux
description: Les cartes de taux vous permettent de définir plusieurs taux de facturation par rôle, en fonction de l’emplacement.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Gestion des cartes de taux

{{highlighted-preview-article-level}}

Les cartes de taux vous permettent de définir plusieurs taux de facturation par rôle, en fonction de l’emplacement. Vous pourriez avoir un rôle professionnel de Designer basé à Paris et un second basé à New York, chacun avec des taux de facturation différents. Cependant, un emplacement n’est pas requis pour les rôles de tâche sur une carte de taux. Un taux de facturation pour un rôle de tâche (et éventuellement un emplacement) sur une carte de taux peut également inclure des dates d’entrée en vigueur.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>Nouveau plan : [!UICONTROL Standard] </p>
       <p>ou</p> 
       <p>Formule actuelle : [!UICONTROL Formule] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès à [!UICONTROL Financial Data]</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Pour modifier une carte de taux partagée avec vous, vous devez disposer des autorisations Gérer sur la carte de taux.</td> 
  </tr> 
 </tbody> 
</table>

## Ajouter une carte de taux

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte de taux**].
1. Cliquez sur [!UICONTROL **Nouvelle carte de taux**], puis saisissez le nom de la carte de taux dans la variable [!UICONTROL **Carte de taux**] pour remplacer &quot;Untitled Rate Card&quot;.
1. Sur l’écran de la carte, cliquez sur [!UICONTROL **Ajout d’un rôle de tâche**].
1. Dans la boîte de dialogue, sélectionnez une [!UICONTROL **Rôle de tâche**] pour définir les taux de facturation.

   Le taux de facturation par défaut affiche le taux au niveau du système pour ce rôle de tâche, le cas échéant.

   ![Boîte de dialogue Nouveau taux de facturation](assets/location-rate-for-rate-card.png)

1. Sélectionnez une [!UICONTROL **Devise**] pour le rôle de tâche.
1. (Facultatif) Sélectionnez une [!UICONTROL **Emplacement**] pour le rôle de tâche.
1. Dans le [!UICONTROL **Taux de facturation 1**] , saisissez le taux de facturation de cet emplacement. Cliquez ensuite sur [!UICONTROL **Enregistrer**] pour remplacer le taux de facturation une fois.

   Ou

   Cliquez sur [!UICONTROL **Taux d’ajout**] pour ajouter d’autres taux de facturation spécifiques à un emplacement avec des dates d’entrée en vigueur.

1. (Conditionnel) Si vous ajoutez plusieurs taux de facturation pour cet emplacement, saisissez les informations suivantes :

   * **[!UICONTROL Taux de facturation 1], 2, etc.:** La valeur du taux de facturation pour la période.
   * **[!UICONTROL Date de début]:** Date à laquelle le remplacement de taux commence.
   * **[!UICONTROL Date de fin]:** Date à laquelle le remplacement de taux se termine.

     Le taux de facturation 1 ne comporte pas de date de début et le dernier taux de facturation n’a pas de date de fin. Certaines dates sont ajoutées automatiquement. Par exemple, si le taux de facturation 1 ne comporte pas de date de fin et que vous ajoutez le taux de facturation 2 avec une date de début le 1er mai 2023, une date de fin du 30 avril 2023 est ajoutée au taux de facturation 1 afin qu’il n’y ait pas d’écart.

1. Cliquer sur [!UICONTROL **Enregistrer**].
1. (Facultatif) Pour ajouter un autre taux de facturation, soit pour le même rôle de tâche à un autre emplacement, soit pour un rôle de tâche distinct, cliquez sur [!UICONTROL **Ajout d’un rôle de tâche**].
1. (Facultatif) Pour modifier un taux de facturation, sélectionnez-le dans la carte de taux et cliquez sur le bouton **Modifier** Icône

## Copier une carte de taux

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte de taux**].
1. Cochez la case en regard de la carte de taux dans la liste et cliquez sur le bouton **Copier** icon ![Icône Copier](assets/copy-icon.png).

   Une carte de taux en double est ajoutée. Cliquez sur le nom de la carte de taux dans la liste pour en modifier le nom.

## Suppression d’une carte de taux entière

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte de taux**].
1. Cochez la case en regard de la carte de taux dans la liste et cliquez sur le bouton **Supprimer** icon ![Icône Supprimer](assets/delete.png).

   >[!NOTE]
   >
   >Une carte de taux associée à un projet sera supprimée du projet.
