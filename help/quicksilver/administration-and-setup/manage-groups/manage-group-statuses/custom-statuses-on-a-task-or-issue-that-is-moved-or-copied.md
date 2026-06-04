---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Statuts personnalisés sur une tâche ou un événement déplacé ou copié
description: Lorsque vous déplacez ou copiez une tâche ou un problème vers un autre projet, certains statuts de la tâche ou du problème peuvent se mettre à jour pour correspondre aux statuts utilisés par le groupe du projet de destination.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
TQID: https://experienceleague.adobe.com/GzG3KBfUw05edjA0DVRtODyGprG2mKVjOuUV2L5eWto
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 211
ht-degree: 94%

---

# Statuts personnalisés pour une tâche ou un problème déplacé ou copié

Lorsque vous déplacez ou copiez une tâche ou un problème vers un autre projet, certains statuts de la tâche ou du problème peuvent se mettre à jour pour correspondre aux statuts utilisés par le groupe du projet de destination. Cela dépend de l’existence ou non de statuts ayant la même clé dans ce groupe :

* Si un statut de la tâche ou du problème possède la même clé qu’un statut utilisé par le groupe du projet de destination, le statut de la tâche ou du problème reste le même.

  Si le libellé de ces deux statuts ne correspond pas, le statut de la tâche ou du problème hérite du libellé du statut utilisé par le groupe du projet de destination.

* Si un statut de la tâche ou du problème n’a pas le même statut que celui équivalent dans le groupe du projet de destination, le statut de la tâche ou du problème passe au statut par défaut équivalent dans le groupe du projet de destination.

Pour plus d’informations sur les clés de statut, consultez la section [Créer ou modifier un statut de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
