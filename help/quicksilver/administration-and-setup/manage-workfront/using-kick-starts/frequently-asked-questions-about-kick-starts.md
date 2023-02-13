---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Questions fréquentes sur les débuts
description: Trouvez des réponses aux questions fréquentes sur l’importation et l’exportation de données Workfront à l’aide de Démarrages de session.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Questions fréquentes sur les débuts

Vous trouverez ci-dessous les questions fréquentes sur les débuts :

## Pourquoi cette erreur s’affiche-t-elle lorsque j’essaie d’importer un fichier de démarrage rapide : &quot;Votre fichier était correct, mais rien n&#39;a été importé ?&quot;

### Réponse

L’un des trois éléments suivants peut ne pas figurer dans le fichier de démarrage :

1. Le **isNew** doit être définie sur **TRUE** pour tous les éléments à importer. **isNew** must **TRUE** car vous ne pouvez importer de nouvelles données qu’avec un coup de pied de page. Vous ne pouvez pas modifier des données existantes par le biais du démarrage rapide. Vous pouvez insérer d’autres lignes dans la feuille de calcul avec **isNew = FALSE** mais ces lignes ne seront pas importées.

1. &#x200B; Le fichier doit comporter une ligne vide avant le démarrage des en-têtes de vos données.
1. &#x200B; Les feuilles Excel doivent avoir le ou les noms appropriés.

Lorsque vous travaillez avec les Kick-Starts, nous vous recommandons d’abord télécharger le modèle de démarrage rapide, de le renseigner manuellement avec les données correctes, puis de l’importer à nouveau dans Adobe Workfront.

Pour plus d’informations sur l’importation correcte des données dans Workfront à l’aide de Démarrages de session, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Pourquoi cette erreur s’affiche-t-elle lorsque j’essaie d’importer des heures dans Workfront à l’aide d’un fichier de démarrage rapide : &quot;Utilisateur avec la ou les valeurs de clé Principale &quot;null&quot; introuvable ?&quot;

### Réponse

L’erreur fait référence au GUID de l’utilisateur associé aux heures.

Pour résoudre ce problème :

1. Exportez un modèle de démarrage rapide vierge pour le **Heures** uniquement.\
   Pour plus d’informations sur l’exportation d’un fichier de démarrage rapide vierge, voir &quot;Exportation du modèle de démarrage rapide&quot; dans  [Importer des données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copiez manuellement les données du démarrage initial et collez-les dans le fichier vide.\
   Effectuez cette opération pour chaque colonne.
1. Essayez de réimporter le nouveau fichier.\
   L’importation du lancement doit réussir.

## Pourquoi le champ Pays n’est-il pas renseigné sur le profil utilisateur dans un import de démarrage rapide ?

### Problème

Lors de l’importation d’un coup de pied-de-pied de l’utilisateur avec le champ **setCountry**, ces données ne sont pas transmises au pays sur le profil utilisateur.

### Réponse

Si l’utilisateur est activé pour Unified User Management (UUM) ou Adobe Identity Management System (IMS), la variable **Pays** accepte uniquement les valeurs de code de pays (par exemple, US, GB, IN). Vérifiez que la variable **setCountry** dans votre modèle de démarrage rapide (Kick-Start), utilisez des valeurs de code de pays avant l’importation.

Pour plus d’informations sur l’importation correcte des données dans Workfront à l’aide de Démarrages de session, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
