---
user-type: administrator
product-area: system-administration;setup
title: Configurer les champs à suivre dans l’historique des modifications
description: En tant qu’administrateur Workfront, vous pouvez configurer les champs d’objet et les actions suivis par Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 20%

---

# Configurer les champs à suivre dans l’historique des modifications

{{highlighted-preview-article-level}}

Adobe Workfront génère des mises à jour système automatiques pour enregistrer les événements suivants :

* Modifications effectuées par les personnes dans un champ d’objet
* Actions effectuées par les personnes sur un objet

Ces mises à jour du système incluent les types d’informations suivants :

* Le changement qui a été apporté.
* Le nom de l’utilisateur ou l’utilisatrice qui a effectué la modification.
* La date et l’heure de la modification.

En tant qu’administrateur Workfront, vous pouvez configurer les champs d’objet et les actions suivis par Workfront.

Par exemple, vous pouvez demander à Workfront de suivre toutes les modifications apportées par les utilisateurs aux noms des problèmes sur l’ensemble du système. Toute modification du nom de l&#39;événement apparaît alors comme une entrée dans le journal de l&#39;historique des modifications. Pour plus d&#39;informations, voir [Afficher et gérer l&#39;historique des modifications](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Administrateur ou administratrice système</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limites du suivi des champs

Les limites du nombre de champs que vous pouvez suivre sont définies par votre package Workfront.

| Package Workfront | Nombre maximum de champs trackés |
|---------|----------|
| Sélectionner | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| Workflow Select | 1000 |
| Workflow Prime | 5000 |
| Workflow Ultimate | Illimité |

## Ajouter les champs dont vous souhaitez effectuer le suivi

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Suivi des modifications > Configuration**.
1. Dans l’écran Configuration, cliquez sur **Ajouter un champ**.
1. Dans la zone **Ajouter des champs**, sélectionnez un objet. Vous pouvez commencer à saisir le nom de l’objet, puis le sélectionner lorsqu’il apparaît dans la liste.
1. Sélectionnez ensuite les noms des champs dont vous souhaitez effectuer le suivi pour cet objet. Vous pouvez commencer à saisir le nom du champ, puis le sélectionner lorsqu’il apparaît dans la liste.

   Les champs personnalisés et les champs natifs sont disponibles pour l’objet .
   Les champs déjà suivis s’affichent tels que sélectionnés dans la liste.

   ![Ajouter des champs pour le suivi des modifications](assets/change-history-config-add-fields.png)

1. Après avoir sélectionné tous les champs dont vous souhaitez effectuer le suivi, cliquez sur **Ajouter**.

   Les champs sont ajoutés à la liste Champs suivis .

## Supprimer les champs dont vous ne souhaitez plus le suivi

Vous pouvez supprimer des champs que le système ne doit pas suivre pour un type d’objet particulier dans l’interface de Workfront.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Suivi des modifications > Configuration**.
1. Dans l’écran Configuration , sélectionnez le ou les champs dont vous souhaitez arrêter le suivi.

   Il se peut que le même nom de champ s’affiche plusieurs fois. Les champs sont regroupés par objet afin que vous puissiez localiser le champ correct. Vous pouvez également utiliser la zone de recherche située en haut de l’écran.

1. Sélectionnez **Supprimer** dans la barre d’actions située en bas de l’écran.
1. Cliquez sur **Supprimer** dans le message de confirmation.

   Les champs sont supprimés de la liste Champs suivis .


