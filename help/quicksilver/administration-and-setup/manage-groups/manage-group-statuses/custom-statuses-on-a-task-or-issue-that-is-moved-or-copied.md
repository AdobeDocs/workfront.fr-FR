---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Statuts personnalisés sur une tâche ou un problème qui est déplacé ou copié
description: Lorsque vous déplacez ou copiez une tâche ou un problème vers un autre projet, certains états de la tâche ou du problème peuvent se mettre à jour pour correspondre aux états utilisés par le groupe du projet de destination.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Statuts personnalisés sur une tâche ou un problème qui est déplacé ou copié

Lorsque vous déplacez ou copiez une tâche ou un problème vers un autre projet, certains états de la tâche ou du problème peuvent se mettre à jour pour correspondre aux états utilisés par le groupe du projet de destination. Cela dépend de l’existence ou non d’états avec la même clé dans ce groupe :

* Si un état de la tâche ou du problème possède la même clé qu’un état utilisé par le groupe du projet de destination, l’état de la tâche ou du problème reste le même.

   Si le libellé de ces deux états ne correspond pas, l’état de la tâche ou du problème hérite du libellé de l’état utilisé par le groupe du projet de destination.

* Si un état de la tâche ou du problème n’a pas le même état que l’état équivalent dans le groupe du projet de destination, l’état de la tâche ou du problème passe à l’état par défaut équivalent dans le groupe du projet de destination.

Pour plus d’informations sur les clés d’état, voir [Création ou modification d’un état de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
