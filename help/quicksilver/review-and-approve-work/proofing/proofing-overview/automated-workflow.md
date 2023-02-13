---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Présentation des processus automatisés
description: Les processus automatisés vous permettent de créer une série d’étapes de révision séquentielles ou parallèles, d’établir des dépendances entre ces étapes et de limiter leur visibilité à certains utilisateurs. S’il existe des étapes interdépendantes dans votre processus de révision, les workflows automatisés déplacent automatiquement votre BAT au cours des étapes, en informant les réviseurs et les approbateurs concernés tout au long du processus. Pour plus d’informations sur la configuration d’un workflow automatisé, voir Création d’un BAT avancé avec un workflow automatisé.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Présentation des processus automatisés

Les processus automatisés vous permettent de créer une série d’étapes de révision séquentielles ou parallèles, d’établir des dépendances entre ces étapes et de limiter leur visibilité à certains utilisateurs. S’il existe des étapes interdépendantes dans votre processus de révision, les workflows automatisés déplacent automatiquement votre BAT au cours des étapes, en informant les réviseurs et les approbateurs concernés tout au long du processus. Pour plus d’informations sur la configuration d’un processus automatisé, voir [Créer un BAT avancé avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Exemples :**  Les workflows automatisés vous aident à gérer des processus de révision de BAT complexes tels que

* Lorsque différents groupes ou opérateurs validants doivent consulter le contenu dans un ordre spécifique
* Lorsqu’il existe des dépendances entre l’activité des utilisateurs lorsqu’ils examinent le contenu
* Lorsque le contenu est révisé régulièrement par les mêmes groupes de personnes
* Lorsque vous souhaitez contrôler la période pendant laquelle les réviseurs examinent le contenu
* Lorsque vous souhaitez que certaines activités de révision restent privées

## Étapes

Pour chaque étape du processus automatisé, vous pouvez configurer des paramètres tels qu’une échéance pour l’étape, un verrou sur l’étape, un réviseur défini comme décideur de l’étape et un paramètre de confidentialité permettant uniquement à certaines personnes d’afficher les commentaires des réviseurs sur l’étape.

Les étapes peuvent être activées manuellement, lors de la création du BAT, lors de l’atteinte d’une échéance, d’une date et d’une heure spécifiques ou lorsqu’une décision est prise sur la scène parent.

Les étapes peuvent être verrouillées manuellement, ainsi que lorsque l’étape suivante commence ou lorsque toutes les décisions sont prises sur l’étape. Vous pouvez également choisir de ne jamais verrouiller une scène.

Vous pouvez nommer un Principal décideur pour une étape. La décision de cette personne rend inutiles toutes les autres décisions pour l’étape.

De même, vous pouvez choisir de n’exiger que la décision pour une étape. Lorsque vous procédez de la sorte, le processus de révision de l’étape est marqué comme terminé une fois que l’un des destinataires a pris sa décision sur l’étape.

Vous pouvez notifier tous les réviseurs de leur invitation à réviser le contenu au début du processus de révision, ou vous pouvez demander à chaque réviseur d’être informé uniquement lorsque son étape est activée.

## Etapes privées

Par défaut, les commentaires laissés par les réviseurs à toutes les étapes sont visibles pour tous ceux qui visualisent le contenu et reçoivent des notifications par e-mail et des résumés de commentaires sur le processus de révision.

Si vous souhaitez empêcher certains groupes de réviseurs de voir les commentaires d’autres réviseurs, vous pouvez créer des scènes privées.

Les scènes privées ne sont visibles que par les réviseurs ajoutés à ces scènes. Elles sont également visibles par les utilisateurs disposant de droits d’édition sur le BAT ou ayant des droits d’édition sur tous les éléments créés dans le compte Adobe Workfront de votre organisation (superviseur et supérieur ou utilisateurs avec des profils personnalisés pour lesquels la modification des informations d’autres personnes est activée).

Les commentaires ajoutés par les participants de la scène privée ne sont pas inclus dans les notifications par email et les résumés des commentaires du BAT demandés par quiconque n’a pas les droits de les afficher.

## Diagramme de workflow

Le diagramme de workflow est une représentation visuelle du processus de révision de votre BAT. Il vous montre l’ordre des scènes et les dépendances entre les scènes lorsque vous créez ou affichez les détails d’un BAT. Toutes les scènes privées s’affichent avec un symbole de clé.

![intro-to-aw-example-diagramme.png](assets/intro-to-aw-example-diagram-350x199.png)

Dans les bons à tirer en direct, les dépendances des étapes s’affichent avec une ligne grise en pointillé pour les étapes inactives ou une ligne noire continue pour les principales étapes. Les étapes s’affichent en vert si le processus de validation a été terminé dans le délai spécifié. Les étapes approchant leurs échéances s’affichent en orange et les étapes au-delà de leur date limite s’affichent en rouge.

![workflow_2.png](assets/workflow-2-350x183.png)

## Modèles de workflow automatisés

Si votre entreprise utilise le même processus de révision pour plusieurs BAT, votre administrateur Workfront peut créer des modèles de workflow automatisé pour faciliter la création des BAT. Vous pouvez choisir un modèle de workflow automatisé lorsque vous configurez un BAT pour ajouter les phases et les validants de ce modèle au BAT. Vous pouvez modifier le modèle appliqué au BAT si nécessaire avant et après la création du BAT.

Votre administrateur Workfront peut créer un nombre illimité de modèles en fonction des besoins de votre entreprise.

Pour en savoir plus sur la création, l’utilisation et la gestion des modèles, consultez votre administrateur Workfront.
