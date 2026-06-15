---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: La décision de l'approbateur affiche un tiret dans le rapport Approbation de l'épreuve
description: Un trait d’union dans le champ Décision de l’approbateur du rapport Approbation de l’épreuve indique qu’un destinataire n’a plus de rôle décisionnel concernant l’épreuve.
author: Courtney
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 9c6e8d04c1faa2902cab870a03a68f0cb14da3aa
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 0%

---

# La décision de l&#39;approbateur affiche un tiret dans le rapport Approbation de l&#39;épreuve

## Problème

Dans le rapport Approbation de l’épreuve , le champ Décision de l’approbateur d’un destinataire affiche un trait d’union (-) même si le champ Date de décision affiche une date et que la valeur du champ En attente de décision est Faux.

![La décision de l&#39;approbateur affiche un tiret dans le rapport Approbation de l&#39;épreuve](assets/approver-decision-hyphen.png)

## Cause

Un trait d’union dans le champ Décision de l’approbateur signifie que le destinataire n’a plus de rôle décisionnel concernant le BAT. Cela peut se produire dans les situations suivantes :

* Le destinataire a été ajouté à l’épreuve, a pris une décision et a été ensuite supprimé du workflow. Si le destinataire revient sur le BAT, le système de relecture enregistre la visite en tant que modification de décision. Le destinataire n&#39;étant plus un approbateur, le système enregistre la nouvelle décision sous forme de trait d&#39;union.
* Le rôle d&#39;épreuve du destinataire a été remplacé par un rôle qui n&#39;inclut pas de droits d&#39;approbation, tel que Réviseur. Pour plus d’informations sur les actions que chaque rôle peut entreprendre sur une épreuve, voir [Présentation des rôles d’épreuve](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md).
* Le profil d&#39;autorisation d&#39;épreuve du destinataire a été rétrogradé après sa décision.

## Signification de cette expression dans vos rapports

Le trait d’union est intentionnel. Il vous indique que le système n’attend pas que le destinataire approuve le BAT et que ce dernier n’a plus de rôle décisionnel concernant le BAT.

Le champ Date de décision affiche toujours la date de l’activité de décision la plus récente du destinataire, mais la décision du destinataire n’est plus comptabilisée dans le rapport.

Pour plus d&#39;informations sur la création et l&#39;utilisation du rapport Approbation de l&#39;épreuve, voir [ Utiliser le rapport Approbation de l&#39;épreuve ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/proof-approval-report.md).


