---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Modifications de taux de notifications push pour les projets
description: Une carte tarifaire représente l’accord contractuel avec votre client dans lequel des taux horaires sont définis pour les fonctions qui termineront le travail. Dans une carte tarifaire, vous pouvez définir plusieurs taux de facturation par fonction, en fonction des attributs.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
source-git-commit: d645aeb9d2d49432b49b6f2e2c4748f50075c42b
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 13%

---

# Modifications du taux de notification push pour les projets

Lorsqu’une carte tarifaire est associée à un <!--or a staffing plan--> de projet, les taux sur la carte tarifaire peuvent toujours être ajustés. Vous pouvez ensuite transférer ces taux vers les projets auxquels la carte tarifaire est associée. Si vous n’appliquez pas les nouveaux taux, les taux d’origine restent dans le projet.
<!-- and staffing plans -->
<!-- or staffing plan -->

Pour plus d’informations sur l’association d’une carte tarifaire à un projet, voir [Associer une carte tarifaire à un projet](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Modifier l’accès aux [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td>Pour modifier une carte tarifaire partagée avec vous, vous devez disposer des autorisations de niveau Gérer sur la carte tarifaire.</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modifications du taux de notification push pour les projets

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Carte tarifaire**].
1. Cliquez sur le nom de la carte tarifaire dans la liste Cartes tarifaires .
1. Sur l’écran Carte tarifaire > Fonctions et taux , vérifiez que les taux sont corrects et modifiez les taux selon vos besoins.
1. Cliquez sur [!UICONTROL **Pousser les modifications**].
1. Dans la boîte de dialogue [!UICONTROL **Appliquer à tous les projets**], tous les projets qui utilisent cette carte tarifaire sont sélectionnés par défaut. Si vous ne souhaitez pas qu&#39;un projet applique les modifications de taux, vous devez le désélectionner.

   <!--/staffing plans-->
   <!--and staffing plans -->
   <!--or staffing plan -->

   >[!NOTE]
   >
   >Seuls les projets dont les taux des cartes tarifaires sont obsolètes s’affichent dans la boîte de dialogue. Si un projet utilise cette carte tarifaire et que les taux sont actuels sur le projet, elle ne s’affiche pas.

1. Cliquer sur [!UICONTROL **Enregistrer**].

   Les nouveaux taux sont désormais répercutés sur les projets <!--and staffing plans -->qui utilisent la carte tarifaire).
