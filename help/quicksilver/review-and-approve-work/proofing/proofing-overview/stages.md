---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Présentation des étapes de workflow automatisées
description: Les étapes de BAT sont des segments de temps dans lesquels différents utilisateurs passent en revue un BAT. Au fur et à mesure que le BAT passe d'une étape à l'autre, Adobe Workfront avertit les réviseurs de leur indiquer quand il est temps d'y travailler.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Présentation des étapes de workflow automatisées

Les étapes de BAT sont des segments de temps dans lesquels différents utilisateurs passent en revue un BAT. Au fur et à mesure que le BAT passe d&#39;une étape à l&#39;autre, Adobe Workfront avertit les réviseurs de leur indiquer quand il est temps d&#39;y travailler.

![stage_diagramme.png](assets/stages-diagram-350x63.png)

Les étapes se produisent dans deux situations différentes :

* [Création d’un BAT avec un workflow automatisé](#create-a-proof-with-an-automated-workflow)
* [Attribuer des échéances à différents opérateurs validants sur un BAT](#assign-deadlines-for-different-reviewers-on-a-proof)

## Création d’un BAT avec un workflow automatisé {#create-a-proof-with-an-automated-workflow}

Lorsque vous ajoutez un workflow automatisé à un BAT, vous configurez les étapes du travail de révision que vous souhaitez réaliser.

Lorsque vous configurez des étapes pour un BAT avec un workflow automatique :

* Vous pouvez configurer les étapes pour qu’elles s’exécutent consécutivement ou simultanément.
* Vous pouvez configurer certaines étapes pour qu’elles deviennent principales uniquement une fois l’étape précédente terminée.
* Vous pouvez rendre certaines scènes privées. Cela s’avère utile, par exemple, pour une agence qui examine un BAT avant qu’il ne soit partagé avec un client et qui ne souhaite pas que les commentaires qui en résultent soient visibles par le client.

Pour plus d’informations sur la création d’étapes pour un BAT avec un workflow automatisé, voir [Créer un BAT avancé avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>Si un utilisateur n’est pas inclus dans une étape, mais qu’il a accès au document et qu’il ouvre le BAT, le système crée une étape appelée *Workfront*.
>
>L’utilisateur qui a ouvert le BAT se voit attribuer le rôle spécifié dans Configuration > Révision et approbation > Rôles pour les non-destinataires qui ouvrent un BAT de document.

## Attribuer des échéances à différents opérateurs validants sur un BAT {#assign-deadlines-for-different-reviewers-on-a-proof}

Lorsque vous attribuez des échéances de validation différentes aux validants sur un BAT, le système crée une étape pour chaque échéance et regroupe les validants pour chaque échéance dans l&#39;étape correspondante. 

**Exemple :** Par exemple, si vous créez un BAT avec quatre réviseurs :

* Pour les réviseurs Olivia et Tony, vous spécifiez un délai de 14h00 dans quelques jours.
* Pour Aaron et Amy, vous spécifiez une date limite de 17h00 quelques jours plus tard.
* Vous ne spécifiez pas de date limite pour vous-même.

Le système crée une étape pour chacun de ces trois &quot;groupes&quot; de réviseurs :

![stage.png](assets/stages-350x239.png)

Si vous partagez le BAT avec un autre réviseur et ne spécifiez pas d’échéance, Workfront ajoute l’utilisateur à l’étape 3, où il n’y a pas d’échéance. 
