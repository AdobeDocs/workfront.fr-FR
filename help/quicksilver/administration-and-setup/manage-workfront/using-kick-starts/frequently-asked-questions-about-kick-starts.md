---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Questions fréquentes à propos des débuts
description: Trouvez des réponses aux questions fréquentes sur l’importation et l’exportation de données Workfront à l’aide de Démarrages de session.
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 1%

---

# Questions fréquentes à propos des débuts

Vous trouverez ci-dessous les questions fréquemment posées à propos des débuts :

## Pourquoi cette erreur s’affiche-t-elle lorsque j’essaie d’importer un fichier de démarrage rapide : &quot;Votre fichier était correct, mais rien n’a été importé ?&quot;

### Réponse

L’un des trois éléments suivants peut ne pas figurer dans le fichier de démarrage :

1. La colonne **isNew** doit être définie sur **TRUE** pour tous les éléments que vous souhaitez importer. **isNew** doit être **TRUE** car vous ne pouvez importer de nouvelles données qu’avec un coup de pied-de-départ. Vous ne pouvez pas modifier des données existantes par le biais du démarrage rapide. Vous pouvez avoir d’autres lignes dans la feuille de calcul avec **isNew = FALSE**, mais ces lignes ne seront pas importées.

1. &#x200B; Le fichier doit comporter une ligne vide avant le démarrage des en-têtes de vos données.
1. &#x200B; Les feuilles Excel doivent avoir le ou les noms appropriés.

Lorsque vous travaillez avec les Kick-Starts, nous vous recommandons d’abord télécharger le modèle de démarrage rapide, de le renseigner manuellement avec les données correctes, puis de l’importer à nouveau dans Adobe Workfront.

Pour plus d’informations sur l’importation correcte des données dans Workfront à l’aide de démarrage rapide, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Pourquoi cette erreur s’affiche-t-elle lorsque j’essaie d’importer les heures dans Workfront à l’aide d’un fichier de démarrage rapide : &quot;Utilisateur avec la ou les valeurs de clé primaire &quot;null&quot; introuvable&quot; ?&quot;

### Réponse

L’erreur fait référence au GUID de l’utilisateur associé aux heures.

Pour résoudre ce problème :

1. Exportez un modèle de démarrage rapide vierge pour l’objet **Hours** uniquement.\
   Pour plus d’informations sur l’exportation d’un fichier de démarrage rapide vierge, voir &quot;Exportation du modèle de démarrage rapide&quot; dans [Importation de données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copiez manuellement les données du démarrage initial et collez-les dans le fichier vide.\
   Effectuez cette opération pour chaque colonne.
1. Essayez de réimporter le nouveau fichier.\
   L’importation du lancement doit réussir.

## Pourquoi le champ Pays n’est-il pas renseigné sur le profil utilisateur dans un import de démarrage rapide ?

### Problème

Lors de l’import d’un coup de pied-de-pied de l’utilisateur avec le champ **setCountry**, ces données ne sont pas transmises au pays sur le profil utilisateur.

### Réponse

Si l’utilisateur est activé pour Unified User Management (UUM) ou Adobe Identity Management System (IMS), le champ **Country** accepte uniquement les valeurs de code de pays (par exemple, US, GB, IN). Vérifiez que le champ **setCountry** de votre modèle de démarrage rapide utilise des valeurs de code de pays avant l’importation.

Pour plus d’informations sur l’importation correcte des données dans Workfront à l’aide de démarrage rapide, voir [Importer des données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
