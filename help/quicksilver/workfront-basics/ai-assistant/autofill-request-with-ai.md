---
title: Remplir automatiquement une demande à l’aide de l’IA
content-type: reference
description: Vous pouvez utiliser l’IA pour remplir automatiquement les champs de requête.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Remplir automatiquement une demande à l’aide de l’IA

L’IA peut vous aider à remplir automatiquement les champs de requête. Il peut suggérer des valeurs de champ en fonction de requêtes précédentes ou les analyser à partir de texte tel que des e-mails.

Vous pouvez approuver ou rejeter ces envois avant d’envoyer la demande.

Le remplissage automatique ne remplace aucun champ que vous avez déjà renseigné.

## Obtention de suggestions lors du remplissage du formulaire

Le remplissage automatique peut suggérer des valeurs de champ lorsque vous remplissez le formulaire. Lorsque vous saisissez des valeurs dans les champs de requête, Workfront compare ces valeurs aux requêtes précédentes. Si la valeur saisie est étroitement corrélée à d’autres valeurs de champ dans des contextes similaires dans des requêtes précédentes, Workfront suggère ces valeurs.

Par exemple, si une clinique utilise toujours le même code de facturation, Workfront suggère ce code de facturation dans le champ approprié lorsque le nom de la clinique est saisi.

Pour utiliser des suggestions basées sur des requêtes précédentes :

1. Commencez à créer une demande.

   Pour obtenir des instructions, voir [Création et envoi de requêtes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Commencez à remplir les champs.

   Lorsque vous remplissez des champs, d’autres champs peuvent afficher des suggestions.

1. Pour chaque suggestion de champ, sélectionnez **Accepter** ou **Rejeter** sous ce champ.

   Ou

   Sélectionnez **Accepter tout** ou **Rejeter tout** en haut de la page pour accepter ou rejeter toutes les suggestions.

## Obtenir des suggestions à partir d’une invite de texte

Le remplissage automatique peut suggérer des valeurs de champ en fonction du texte, tel que les e-mails. Vous collez un bloc de texte, puis Workfront traite le texte pour suggérer des valeurs de champ en fonction du texte.

Par exemple, si l’e-mail inclut « L’échéance est le 1er juin » et que le formulaire de demande comporte un champ pour la date d’échéance, Workfront suggère le 1er juin pour cette valeur de champ.

Ce type de suggestion vérifie également les demandes précédentes pour des contextes similaires. Par exemple, si l’invite indique que la demande concerne un certain client, Workfront peut localiser et saisir automatiquement l’adresse de facturation de ce client, en fonction des demandes précédentes.

Vous pouvez coller du texte à appliquer à l’ensemble du formulaire ou à une seule section du formulaire.

Pour utiliser des suggestions basées sur une invite de texte collée :

1. Commencez à créer une demande.

   Pour obtenir des instructions, voir [Création et envoi de requêtes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Pour appliquer l’invite de texte à l’ensemble du formulaire, cliquez sur **Remplissage automatique avec l’IA** dans le coin supérieur droit de l’écran.

   Ou

   Pour appliquer l’invite de texte à une seule section, cliquez sur l’icône AI ![icône AI](assets/request-prompt-icon.png) à côté du nom de la section.

1. Collez le texte dans la zone d’invite.
1. Cliquez sur **Remplir le formulaire**.

   Workfront génère des suggestions pour le formulaire.
1. Pour chaque suggestion de champ, sélectionnez **Accepter** ou **Rejeter** sous ce champ.

   Ou

   Sélectionnez **Accepter tout** ou **Rejeter tout** en haut de la page pour accepter ou rejeter toutes les suggestions.

