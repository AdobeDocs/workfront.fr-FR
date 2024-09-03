---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Questions fréquentes à propos des débuts
description: Trouvez les réponses aux questions fréquemment posées sur l’import et l’export de données Workfront à l’aide des Kickstarts.
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 98%

---

# Questions fréquentes à propos de Kick-Starts

Les questions les plus fréquemment posées sur les Kickstarts sont les suivantes :

## Pourquoi est-ce que je reçois cette erreur lorsque j’essaie d’importer un fichier Kickstart : « Votre fichier est correct, mais rien n’a été importé » ?

### Réponse

L’un des trois éléments suivants peut manquer dans le fichier Kickstart :

1. La colonne **isNew** doit avoir la valeur **TRUE** pour tous les éléments que vous souhaitez importer. **isNew** doit avoir la valeur **TRUE**, car vous ne pouvez importer de nouvelles données qu’avec un Kickstart. Vous ne pouvez pas modifier des données existantes via Kickstart. Vous pouvez avoir d’autres lignes dans la feuille de calcul avec **isNew = FALSE**, mais ces lignes ne seront pas importées.

1. Le fichier doit comporter une ligne vide avant le début des en-têtes de vos données.
1. Les feuilles Excel doivent avoir les noms corrects.

Lorsque vous travaillez avec des Kickstarts, nous vous recommandons de télécharger d’abord le modèle Kickstart, de le remplir manuellement avec les données correctes, puis de le réimporter dans Adobe Workfront.

Pour plus d’informations sur l’import de données correctes dans Workfront à l’aide de Kickstarts, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Pourquoi est-ce que je reçois cette erreur lorsque j’essaie d’importer des heures dans Workfront à l’aide d’un fichier Kickstart : « Utilisateur ou utilisatrice aux valeurs de clé primaire « null » introuvable » ?

### Réponse

L’erreur se réfère au GUID de la personne associée aux heures.

Afin d’y remédier, procédez comme suit :

1. Exporter un modèle Kickstart vierge pour l’objet **Heures** uniquement.\
   Pour plus d’informations sur l’export d’un fichier Kickstart vierge, voir « Exporter le modèle Kickstart » dans [Importer des données dans Adobe Workfront à l’aide d’un modèle Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copiez manuellement les données du Kickstart d’origine et collez-les dans le fichier vide.\
   Procédez ainsi pour chaque colonne.
1. Essayez d’importer à nouveau le fichier.\
   Le Kickstart devrait être importé sans encombre.

## Pourquoi le champ Pays ne s’affiche-t-il pas dans le profil d’utilisateur ou d’utilisatrice lors d’un import de Kickstart ?

### Problème

Lors de l’import d’un Kickstart d’utilisateur ou d’utilisatrice avec le champ **setCountry**, ces données ne sont pas transférées dans le pays indiqué sur le profil de la personne.

### Réponse

Si la personne est activée pour la gestion unifiée des utilisateurs et utilisatrices (UUM) ou le système de gestion des identités Adobe (IMS), le champ **Pays** n’accepte que les codes de pays comme valeurs (par exemple, US, GB, IN). Vérifiez que le champ **setCountry** de votre modèle Kickstart utilise des codes de pays comme valeurs avant de procéder à l’import.

Pour plus d’informations sur l’import de données correctes dans Workfront à l’aide de Kickstarts, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle Kickstart](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
