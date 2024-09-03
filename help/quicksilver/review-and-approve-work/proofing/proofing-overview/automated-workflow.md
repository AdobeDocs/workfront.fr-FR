---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Vue d’ensemble des workflows automatisés
description: Les workflows automatisés vous permettent de créer une série d’étapes de révision séquentielles ou parallèles, d’établir des dépendances entre ces étapes et de limiter leur visibilité à certains utilisateurs et utilisatrices. S’il existe des étapes interdépendantes dans votre processus de révision, les workflows automatisés déplacent automatiquement votre épreuve au travers des étapes, en informant les réviseurs et réviseuses et les approbateurs et approbatrices concernés tout au long du processus.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 100%

---

# Vue d’ensemble des workflows automatisés

<!-- Audited: 01/2024 -->

Les workflows automatisés vous permettent de créer une série d’étapes de révision séquentielles ou parallèles, d’établir des dépendances entre ces étapes et de limiter leur visibilité à certains utilisateurs et utilisatrices. S’il existe des étapes interdépendantes dans votre processus de révision, les workflows automatisés déplacent automatiquement votre épreuve au travers des étapes, en informant les réviseurs et réviseuses et les approbateurs et approbatrices concernés tout au long du processus. Pour plus d’informations sur la configuration d’un workflow automatisé, consultez [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Exemples :** les workflows automatisés vous aident à gérer des processus de révision d’épreuves complexes tels que :

* Lorsque différents groupes ou réviseurs et réviseuses doivent consulter le contenu dans un ordre spécifique.
* Lorsqu’il existe des dépendances dans l’activité des utilisateurs et des utilisatrices lors de la révision du contenu.
* Lorsque du contenu est révisé régulièrement par les mêmes groupes de personnes.
* Lorsque vous souhaitez contrôler la période pendant laquelle les réviseurs et réviseuses peuvent consulter le contenu.
* Lorsque vous souhaitez que certaines activités de révision restent privées.

## Étapes

Pour chaque étape du workflow automatisé, vous pouvez configurer des paramètres tels qu’une date d’échéance pour l’étape, un verrouillage de l’étape, un réviseur ou une réviseuse défini comme personne décideuse pour l’étape et un paramètre de confidentialité qui permet de restreindre à certaines personnes uniquement la consultation des commentaires des réviseurs et réviseuses sur l’étape.

Les étapes peuvent être activées manuellement, lors de la création de l’épreuve, lorsqu’une date d’échéance est atteinte, à une date et une heure spécifiques ou lorsqu’une décision est prise sur l’étape parent.

Les étapes peuvent être verrouillées manuellement, lorsque l’étape suivante débute, ou lorsque toutes les décisions ont été prises sur l’étape. Vous pouvez également choisir de ne jamais verrouiller une étape.

Vous pouvez affecter une personne décideuse principale à une étape. La décision de cette personne rend toutes les autres décisions prises sur l’étape inutiles.

Vous pouvez également choisir de n’exiger qu’une seule décision pour une étape. Lorsque vous choisissez cette option, le processus de révision de l’étape est indiqué comme terminé dès que n’importe quelle personne destinataire prend une décision sur l’étape.

Vous pouvez notifier tous les réviseurs et réviseuses de leur invitation à réviser le contenu lors du démarrage du processus de révision, ou vous pouvez choisir que chaque réviseur et réviseuse soit informé uniquement lors de l’activation de son étape.

## Étapes privées

Par défaut, les commentaires laissés par les réviseurs et réviseuses sur toutes les étapes sont visibles pour tous ceux qui révisent le contenu et qui reçoivent des notifications par e-mail et des résumés des commentaires concernant le processus de révision.

Si vous souhaitez empêcher certains groupes de réviseurs et réviseuses de voir les commentaires d’autres réviseurs et réviseuses, vous pouvez créer des étapes privées.

Les étapes privées ne sont visibles que par les réviseurs et réviseuses ajoutés à ces étapes. Elles sont également visibles par les utilisateurs et utilisatrices disposant de droits d’édition sur l’épreuve ou de droits d’édition sur tous les éléments créés dans le compte Adobe Workfront de votre entreprise (rôle Superviseur et supérieur, ou utilisateurs et utilisatrices disposant de profils personnalisés pour lesquels la modification des informations d’autres personnes est activée).

Les commentaires ajoutés par les participantes et les participants de l’étape privée ne sont pas inclus dans les notifications par e-mail et dans les résumés des commentaires de l’épreuve demandés par quiconque ne possède pas le droit de les consulter.

## Diagramme de workflow

Le diagramme de workflow est une représentation visuelle du processus de révision de votre épreuve. Il vous indique l’ordre des étapes et les dépendances entre les étapes lorsque vous créez une épreuve ou consultez les détails d’une épreuve. Toutes les étapes privées s’affichent avec un symbole en forme de clé.

![intro-to-aw-example-diagram.png](assets/intro-to-aw-example-diagram-350x199.png)

Dans les épreuves actives, les dépendances des étapes s’affichent avec une ligne grise en pointillés pour les étapes inactives ou une ligne noire continue pour les étapes actives. Les étapes s’affichent en vert si le processus d’approbation a été terminé dans le délai spécifié. Les étapes dont la date d’échéance approche s’affichent en orange et les étapes qui ont dépassé leur date d’échéance s’affichent en rouge.

![workflow_2.png](assets/workflow-2-350x183.png)

## Modèles de workflows automatisés

Si votre organisation utilise le même processus de révision pour plusieurs épreuves, votre administrateur ou administratrice Workfront peut créer des modèles de workflows automatisés pour faciliter la création des épreuves. Vous pouvez choisir un modèle de workflow automatisé lorsque vous configurez une épreuve pour lui ajouter les étapes et les réviseurs et réviseuses de ce modèle. Vous pouvez modifier si nécessaire le modèle appliqué à l’épreuve avant et après la création de l’épreuve.

Votre administrateur ou administratrice Workfront peut créer un nombre illimité de modèles en fonction des besoins de votre entreprise.

Pour en savoir plus sur la création, l’utilisation et la gestion de modèles, contactez votre administrateur ou administratrice Workfront.
