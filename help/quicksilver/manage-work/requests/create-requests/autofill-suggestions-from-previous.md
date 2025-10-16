---
title: Renseigner automatiquement une requête avec les données des requêtes précédentes
content-type: reference
description: Vous pouvez utiliser l’IA pour remplir automatiquement les champs de la requête à l’aide des données de requêtes précédentes.
author: Becky
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
source-git-commit: 1b7964b533093c4eee20d69a74512a145e207e29
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 21%

---

# Renseigner automatiquement une requête avec les données des requêtes précédentes

L’IA peut vous aider à remplir automatiquement les champs de requête en fonction des requêtes précédentes. Vous pouvez approuver ou rejeter ces suggestions avant d’envoyer la demande.

La saisie automatique ne remplace aucun champ que vous avez déjà rempli.

Les utilisateurs ne reçoivent pas de suggestions de données auxquelles ils n’ont pas accès autrement.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Contributeur ou version ultérieure</p>
   <p>Requête ou supérieure</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p>  </td> 
  </tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td><p>Accès à l’ajout de demandes à une file d’attente</p> <p>Autorisation en affichage ou supérieure sur la demande existante</p> <p>Pour plus d’informations sur la configuration d’une file d’attente des demandes, voir <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Créer une file d’attente des demandes</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Obtention de suggestions lors du remplissage du formulaire

La saisie automatique peut suggérer des valeurs de champ lorsque vous remplissez le formulaire. Lorsque vous saisissez des valeurs dans les champs de requête, Workfront compare ces valeurs aux requêtes précédentes. Si la valeur saisie est étroitement corrélée à d’autres valeurs de champ dans des contextes similaires dans des requêtes précédentes, Workfront suggère ces valeurs.

Par exemple, si une clinique utilise toujours le même code de facturation, Workfront suggère ce code de facturation dans le champ approprié lorsque le nom de la clinique est saisi.

Pour utiliser des suggestions basées sur des requêtes précédentes :

1. Commencez à créer une demande.

   Pour obtenir des instructions, voir [Création et envoi de requêtes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Commencez à remplir les champs.

   Lorsque vous remplissez des champs, d’autres champs peuvent afficher des suggestions.

1. Pour chaque suggestion de champ, sélectionnez **Accepter** ou **Rejeter** pour ce champ.

   ![Accepter ou refuser la suggestion](assets/accept-reject-suggestion.png)

   Ou

   Sélectionnez **Accepter tout** ou **Rejeter tout** en haut de la page pour accepter ou rejeter toutes les suggestions.

   >[!NOTE]
   >
   >Toute suggestion non révisée sera automatiquement acceptée lorsque vous soumettrez la demande.
