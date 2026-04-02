---
content-type: overview
product-area: projects
navigation-topic: financials
title: Généralités sur la hiérarchie des revenus et des coûts
description: Cet article décrit le processus détaillé permettant de déterminer les taux de facturation et de coûts appropriés pour les fonctions et les utilisateurs pour le type de revenu et de coût Utilisateur et Rôle par heure.
author: Lisa
feature: Work Management
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '3519'
ht-degree: 0%

---

# Présentation de la hiérarchie des revenus et des coûts

{{highlighted-preview-article-level}}

{{ultimate-package}}

Pour fournir des calculs financiers précis, Workfront utilise les taux de facturation appropriés lors du calcul du chiffre d’affaires d’une tâche ou d’un projet. La fonction et les taux d’utilisation doivent être bien définis à tous les niveaux pour obtenir des calculs financiers précis.

Les sections de cet article décrivent le processus étape par étape pour déterminer les taux de facturation et de coûts appropriés pour les fonctions et les utilisateurs pour l&#39;utilisateur et le type de revenu horaire par rôle et le type de coût.

Pour plus d’informations sur les taux de facturation, les types de revenus et la manière dont les revenus sont calculés, voir [Présentation de la facturation et des revenus](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Généralités sur les dates de validité

Les administrateurs de Workfront peuvent éventuellement définir des dates d’entrée en vigueur qui déterminent à quel moment les taux de facturation, les taux de coût et d’autres attributs financiers prennent effet dans le système. Par exemple, une fonction ou un utilisateur peut avoir un taux de facturation par défaut de 50 $. Si des dates d&#39;entrée en vigueur étaient appliquées, ce taux de 50 $ pourrait expirer le 31 mars, et un nouveau taux de 55 $ commencerait automatiquement le 1er avril.

Pour les calculs de revenus prévus, les taux de facturation sont basés sur la date des heures prévues. Les heures prévues sont réparties uniformément sur la durée de la tâche. Dans l’exemple précédent, les heures prévues pour le 31 mars ou une date antérieure utilisent le taux de 50 $ et les heures prévues pour le 1er avril ou une date ultérieure utilisent le taux de 55 $.

Pour les calculs des revenus réels, les taux de facturation sont basés sur la date des heures consignées. Dans l’exemple précédent, les heures enregistrées le 31 mars ou avant utilisent le taux de 50 $, et les heures enregistrées le 1er avril ou après utilisent le taux de 55 $.

>[!NOTE]
>
>Les affectations de tâches ne sont pas définies avec des dates d&#39;effet. Au lieu de cela, les affectations extraient les taux applicables du système, que ce soit à partir d&#39;une carte tarifaire, d&#39;un profil utilisateur ou d&#39;un remplacement au niveau de l&#39;affectation. Les dates de validité garantissent que le taux correct est appliqué en fonction de la durée du travail, mais elles ne définissent pas directement les affectations.

## Présentation de la fonction pour la facturation

Une **fonction pour la facturation** est définie pour un utilisateur au niveau de l’affectation ou du projet. Elle s’applique uniquement aux utilisateurs et ne peut pas être utilisée sur d’autres fonctions. Par exemple, la fonction principale d’un utilisateur ou d’une utilisatrice est Designer, mais pour une tâche ou un projet, il ou elle agit en tant que cadre Designer, et le taux doit refléter cela.

Une fonction au niveau de l’affectation pour la facturation est réservée à cette affectation spécifique et n’est pas automatiquement appliquée aux autres affectations de l’utilisateur. Une fonction au niveau du projet pour la facturation s’applique à toutes les affectations de l’utilisateur pour ce projet. Vous pouvez le remplacer au niveau de l’affectation individuelle, si nécessaire.

Lorsqu’une fonction pour la facturation est appliquée au niveau de l’affectation de l’utilisateur ou du projet, le taux associé à la fonction pour la facturation peut être utilisé à la place des taux d’utilisateur ou de fonction dans le calcul des revenus. La fonction de facturation n’est disponible que lorsque le type de revenu Utilisateur et Rôle par heure est utilisé.

>[!NOTE]
>
>Bien qu’un utilisateur puisse agir avec un rôle différent à des fins de facturation, le calcul des coûts continue d’utiliser sa fonction principale. La fonction de facturation n’affecte que les calculs de facturation.

Pour plus d’informations, voir [Configurer une fonction pour la facturation](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

## Présentation des taux conservés

L&#39;indicateur **Conserver les informations sur les taux de facturation du projet** sur un projet contrôle si le système utilise les informations de facturation pour les affectations au moment où la carte tarifaire est finalisée, ou autorise les modifications en fonction des modifications au cours du projet. Toute modification apportée à la fonction, au salaire, à la carte tarifaire ou à d&#39;autres informations relatives à la facturation de l&#39;utilisateur n&#39;aura aucune incidence sur les taux de facturation des affectations. Les taux sont conservés en fonction de la carte tarifaire finale au moment de l&#39;activation de l&#39;indicateur de projet. Ces propriétés d’affectation (telles que la fonction et le salaire) sont toujours mises à jour, ce qui garantit que le coût réel de l’affectation est exact.

Lorsque l’indicateur est activé, le système verrouille les taux de facturation effectifs à la date (définis sur la carte tarifaire finalisée jointe au projet) pour la durée du projet.

L&#39;indicateur peut être activé sur un projet lorsque le travail a commencé et que des affectations et des heures existent déjà. À ce moment-là :

* Le taux de carte tarifaire approuvé final devient la source des taux de facturation pour toutes les affectations de projet.
* Toutes les affectations passées, actuelles et futures sont recalculées à l&#39;aide des taux approuvés finaux.
* Les valeurs réelles et prévues sont recalculées.

>[!NOTE]
>
>Une fois que l’indicateur est activé pour conserver les taux de facturation, il ne peut pas être désactivé à moins que le projet n’ait aucune affectation et aucune heure. Cela permet de s’assurer que tous les rapports financiers reflètent les taux contractuels réels.
>Lorsque l’indicateur est désactivé, le système permet de recalculer ou d’ajuster dynamiquement les taux de facturation. Toute mise à jour du rôle, du salaire ou du taux de facturation de l’utilisateur est immédiatement répercutée sur le taux de facturation de l’affectation.

Pour plus d’informations, voir [Modifier les projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) et [Gérer les cartes tarifaires](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Revenu prévu - Utilisateur et rôle, par heure

Lorsque le type de revenu de la tâche est Utilisateur et rôle par heure, Workfront utilise les hiérarchies de taux d’utilisateur et de taux de fonction pour déterminer le taux de facturation du revenu prévu.

Cette image présente le flux de la hiérarchie des revenus prévus :

![Revenu prévu pour le type de revenu horaire de l’utilisateur et du rôle](assets/planned-revenue-chart.png)

Lorsqu’un utilisateur est affecté à la tâche, Workfront effectue une recherche selon cette hiérarchie :

1. Le système recherche d’abord un taux conservé sur l’affectation de l’utilisateur.

   Un taux conservé suit toujours la hiérarchie, mais il est gelé lorsque le projet est conservé. Pour plus d’informations, voir [Présentation des taux conservés](#overview-of-preserved-rates).

1. Ensuite, le système recherche le taux de facturation sur une carte tarifaire, pour la fonction principale ou la fonction pour la facturation de l’utilisateur affecté à la tâche. Si un taux existe et qu&#39;il est verrouillé, il est utilisé dans le calcul des revenus.

   Si un taux existe sur la carte tarifaire et qu’il est déverrouillé, le système n’utilise pas ce taux et recherche le taux suivant dans la hiérarchie.

1. Ensuite, le système recherche le taux de remplacement au niveau de l’affectation pour l’utilisateur. Il s’agit d’un taux ajouté manuellement lié à l’affectation spécifique et qui remplace tous les autres taux pour l’utilisateur de cette affectation (à l’exception d’un taux verrouillé par carte tarifaire). Si un taux est trouvé, il est utilisé dans le calcul des revenus.
1. Ensuite, le système recherche une fonction pour la facturation au niveau de l’affectation de tâche.

   La fonction pour la facturation est uniquement destinée à une affectation spécifique et s’applique à l’affectation au lieu du taux de fonction principale de l’utilisateur. Par exemple, la fonction principale d’un utilisateur ou d’une utilisatrice est Designer, mais pour une tâche, il ou elle agit en tant que cadre Designer avec un taux de facturation plus élevé.

   Workfront recherche la fonction pour le taux de facturation :

   * Le système recherche d’abord le taux de facturation de la fonction pour la facturation à partir de l’affectation (Senior Designer dans l’exemple), en prenant en compte les dates d’entrée en vigueur. Elle s’affiche dans la zone Taux > Facturation du projet, dans un regroupement **Taux Source : Remplacements > Type de ressource : Fonction**. Il s’agit d’un taux de remplacement pour le projet.
   * Ensuite, le système recherche la fonction pour le taux de facturation à partir d’une carte tarifaire, en prenant en compte les dates d’entrée en vigueur. Vous pourrez le voir dans la zone Taux > Facturation du projet, dans un regroupement **Rate Source : Carte tarifaire associée > Type de ressource : Fonction**.
   * Si le taux de la fonction pour la facturation ne figure pas sur le projet ou sur la carte tarifaire, le système recherche le taux de la fonction au niveau du système (Senior Designer dans l’exemple), en prenant en compte les dates d’entrée en vigueur.
   * Si une fonction pour la facturation est affectée et qu’aucun des taux des étapes précédentes n’est trouvé, le taux de facturation est de 0.

     >[!NOTE]
     >
     >Lorsqu’une fonction pour la facturation est affectée, mais que le taux de facturation est de 0, il s’agit d’un indicateur permettant de revoir la configuration du taux. Un taux de 0 signifie qu’aucun taux pour cette fonction (Senior Designer dans l’exemple) n’a été configuré dans Workfront. Vous devez ajouter des taux pour la fonction ou supprimer la fonction pour la facturation de l’affectation.
     >
     >Comme les tâches héritent des taux de fonctions du projet lorsque ces taux sont disponibles au niveau du projet, tout taux provenant d’une recherche de la fonction pour la facturation du projet aurait déjà été localisé lorsque Workfront a recherché dans la fonction pour la facturation au niveau de l’affectation de la tâche. La recherche au niveau du projet d’une fonction pour la facturation reste dans la hiérarchie de recherche.

1. Si aucune fonction de facturation n&#39;était disponible au niveau de l&#39;affectation de tâche, le système recherche alors le taux de facturation du projet pour l&#39;utilisateur spécifique affecté à la tâche, en tenant compte des dates de validité. Vous pourrez le voir dans la zone Taux > Facturation du projet, dans un regroupement **Taux Source : Remplacements > Type de ressource : Utilisateur**. Il s’agit d’un taux de remplacement pour le projet.
1. Ensuite, le système recherche le taux de facturation au niveau du système sur le profil de l’utilisateur, en prenant en compte les dates d’entrée en vigueur.
1. Ensuite, le système recherche le taux de facturation de la fonction principale de l’utilisateur (Designer dans l’exemple).

   * Le système recherche d’abord le taux de facturation du projet, pour la fonction principale de l’utilisateur, en prenant en compte les dates d’entrée en vigueur. Elle s’affiche dans la zone Taux > Facturation du projet, dans un regroupement **Taux Source : Remplacements > Type de ressource : Fonction**. Il s’agit d’un taux de remplacement pour le projet.
   * Ensuite, le système recherche le taux de fonction à partir d’une carte tarifaire, en tenant compte des dates d’entrée en vigueur. Vous pourrez le voir dans la zone Taux > Facturation du projet, dans un regroupement **Rate Source : Carte tarifaire associée > Type de ressource : Fonction**.
   * Ensuite, le système recherche le taux de fonctions au niveau du système, en prenant en compte les dates d’entrée en vigueur.

1. Si aucun de ces taux n’est trouvé, le taux de facturation est de 0.

Lorsque l’utilisateur n’est pas affecté à la tâche, Workfront recherche les taux de fonctions en fonction de cette hiérarchie :

1. Le système recherche d’abord un taux conservé sur l’affectation pour la fonction.
1. Le système recherche le taux de facturation sur une carte tarifaire pour la fonction affectée à la tâche. Si un taux existe et qu&#39;il est verrouillé, il est utilisé dans le calcul des revenus.

   Si un taux existe sur la carte tarifaire et qu’il est déverrouillé, le système n’utilise pas ce taux et recherche le taux suivant dans la hiérarchie.

1. Ensuite, le système recherche le taux de remplacement de la tâche d’affectation pour la fonction. Il s’agit d’un taux ajouté manuellement pour la fonction sur l’affectation spécifique et qui remplace tous les autres taux pour la fonction sur cette tâche. Si un taux est trouvé, il est utilisé dans le calcul des revenus.
1. Ensuite, le système recherche le taux de facturation de la fonction affectée à la tâche.

   * Le système recherche d’abord le taux de facturation du projet pour la fonction, en prenant en compte les dates d’entrée en vigueur. Elle s’affiche dans la zone Taux > Facturation du projet, dans un regroupement **Taux Source : Remplacements > Type de ressource : Fonction**. Il s’agit d’un taux de remplacement pour le projet.
   * Ensuite, le système recherche le taux de fonction à partir d’une carte tarifaire, en tenant compte des dates d’entrée en vigueur. Vous pourrez le voir dans la zone Taux > Facturation du projet, dans un regroupement **Rate Source : Carte tarifaire associée > Type de ressource : Fonction**.
   * Ensuite, le système recherche le taux de fonctions au niveau du système, en prenant en compte les dates d’entrée en vigueur.

1. Si aucun de ces taux n’est trouvé, le taux de facturation est de 0.

## Revenu réel - Utilisateur et rôle, par heure

Lorsque le type de revenu de la tâche est Utilisateur et Rôle par heure, Workfront utilise deux hiérarchies pour déterminer le taux de facturation du revenu réel. Le taux de facturation est basé sur les heures de connexion de l’utilisateur à une tâche.

L’« utilisateur » dans les hiérarchies est la personne affectée à la tâche. Le « propriétaire » est la personne dont le temps est enregistré pour la tâche, même s’il n’est pas affecté à la tâche. Par exemple, Michael est affecté à une tâche, mais Joanna termine le travail parce que Michael était malade. Le responsable peut consigner le temps par rapport à la tâche et définir le propriétaire des heures consignées sur Joanna. Les valeurs de revenus prévus sont basées sur l&#39;affectation de Michael et le taux dans la hiérarchie, mais les valeurs de revenus réels sont basées sur le taux de Joanna.

Cette image présente le flux de la hiérarchie réelle des revenus :

![Revenu réel pour le type de coût horaire de l&#39;utilisateur et du rôle](assets/actual-revenue-chart.png)

### Lorsque le propriétaire des heures consignées et l’utilisateur affecté à la tâche sont le même

Workfront recherche d’abord un taux de facturation par affectation d’utilisateur. Si un utilisateur n’est pas affecté à la tâche, il recherche un taux de facturation par affectation de fonction.

La hiérarchie de ce scénario est identique à celle du chiffre d&#39;affaires prévu. Voir [Revenu prévu - Utilisateur et rôle par heure](#planned-revenue--user-and-role-hourly) pour ce workflow.

### Lorsque le propriétaire des heures consignées n&#39;est pas l&#39;utilisateur affecté à la tâche

Workfront effectue une recherche dans les propriétés utilisateur du propriétaire selon cette hiérarchie :

1. Le système recherche d’abord un taux conservé sur l’affectation pour le propriétaire.
1. Ensuite, le système recherche le taux de facturation sur une carte tarifaire, pour la fonction principale du propriétaire. Si un taux existe et qu&#39;il est verrouillé, il est utilisé dans le calcul des revenus.

   Si un taux existe sur la carte tarifaire et qu’il est déverrouillé, le système n’utilise pas ce taux et recherche le taux suivant dans la hiérarchie.

1. Ensuite, le système recherche le taux de facturation du projet, pour le propriétaire, en tenant compte des dates d’entrée en vigueur. Cela s’affiche dans la zone Taux > Facturation du projet, dans un Source de taux : Remplacements > Type de ressource : Regroupement d’utilisateurs. Il s’agit d’un taux de remplacement pour le projet.
1. Ensuite, le système recherche une fonction pour la facturation au niveau du projet.

   La fonction de facturation est uniquement destinée à un projet spécifique et s’applique au projet au lieu du taux de fonctions principales du propriétaire. Par exemple, la fonction principale du propriétaire est Designer, mais pour un projet, il agit en tant que Designer principal avec un taux de facturation plus élevé.

   Workfront recherche la fonction pour le taux de facturation :

   * Le système recherche d’abord la fonction pour le taux de facturation à partir d’une carte tarifaire, en prenant en compte les dates d’entrée en vigueur. Vous pourrez le voir dans la zone Taux > Facturation du projet, dans un regroupement **Rate Source : Carte tarifaire associée > Type de ressource : Fonction**.
   * Si le taux de la fonction pour la facturation ne figure pas sur la carte tarifaire, le système recherche le taux de la fonction au niveau du système (Senior Designer dans l’exemple), en prenant en compte les dates d’entrée en vigueur.
   * Si une fonction pour la facturation est affectée et qu’aucun des taux des étapes précédentes n’est trouvé, le taux de facturation est de 0.

     >[!NOTE]
     >
     >Lorsqu’une fonction pour la facturation est affectée, mais que le taux de facturation est de 0, il s’agit d’un indicateur permettant de revoir la configuration du taux. Un taux de 0 signifie qu’aucun taux pour cette fonction (Senior Designer dans l’exemple) n’a été configuré dans Workfront. Vous devez ajouter des taux pour la fonction ou supprimer la fonction pour la facturation du projet.

1. Ensuite, le système recherche le taux de facturation au niveau du système sur le profil utilisateur du propriétaire, en prenant en compte les dates d’entrée en vigueur.
1. Ensuite, le système recherche le taux de facturation de la fonction principale du propriétaire (Designer dans l’exemple).

   * Le système recherche d&#39;abord le taux de facturation du projet, pour la fonction principale du propriétaire, en tenant compte des dates d&#39;entrée en vigueur. Elle s’affiche dans la zone Taux > Facturation du projet, dans un regroupement **Taux Source : Remplacements > Type de ressource : Fonction**. Il s’agit d’un taux de remplacement pour le projet.
   * Ensuite, le système recherche le taux de fonction à partir d’une carte tarifaire, en tenant compte des dates d’entrée en vigueur. Vous pourrez le voir dans la zone Taux > Facturation du projet, dans un regroupement **Rate Source : Carte tarifaire associée > Type de ressource : Fonction**.
   * Ensuite, le système recherche le taux de fonctions au niveau du système, en prenant en compte les dates d’entrée en vigueur.

1. Si aucun de ces taux n’est trouvé, le taux de facturation est de 0.

## Coût prévu - Utilisateur et rôle, par heure

Lorsque le type de coût de la tâche est Utilisateur et Rôle par heure, Workfront utilise les hiérarchies de taux d&#39;utilisateur et de rôle de tâche pour déterminer le taux du coût prévu.

Cette image présente le flux de la hiérarchie des coûts planifiés :

![Coût prévu pour le type de coût horaire Utilisateur et Rôle](assets/planned-cost-chart.png)

Lorsqu’un utilisateur est affecté à la tâche, Workfront effectue une recherche selon cette hiérarchie :

1. Le système recherche le taux de remplacement de la tâche d&#39;affectation pour l&#39;utilisateur. Il s’agit d’un taux ajouté manuellement pour l’utilisateur concernant l’affectation spécifique et qui remplace tous les autres taux pour l’utilisateur concernant cette tâche. Si un taux est trouvé, il est utilisé dans le calcul des coûts.
1. Ensuite, le système recherche le taux de coût du projet, pour l&#39;utilisateur spécifique affecté à la tâche, en prenant en compte les dates de validité. Vous pourrez le voir dans la zone Taux > Coût du projet, dans un regroupement **Taux Source : Remplacements > Type de ressource : Utilisateur**. Il s’agit d’un taux de remplacement pour le projet.
1. Ensuite, le système recherche le taux de coût au niveau du système sur le profil de l’utilisateur, en prenant en compte les dates d’entrée en vigueur.
1. Ensuite, le système recherche le taux de coût de la fonction principale de l’utilisateur avec la combinaison d’attributs affectés, en fonction du score de l’attribut.
1. Si aucun de ces taux n&#39;est trouvé, le taux de coût est 0.

Lorsque l’utilisateur n’est pas affecté à la tâche, Workfront recherche les taux de coût des fonctions selon cette hiérarchie :

1. Le système recherche le taux de remplacement de la tâche d&#39;affectation pour la fonction. Il s’agit d’un taux ajouté manuellement pour la fonction sur l’affectation spécifique et qui remplace tous les autres taux pour la fonction sur cette tâche. Si un taux est trouvé, il est utilisé dans le calcul des coûts.
1. Ensuite, le système recherche le taux de coût des fonctions au niveau du système avec la combinaison d’attributs affectés, en fonction du score de l’attribut et en tenant compte des dates d’entrée en vigueur.
1. Si aucun de ces taux n&#39;est trouvé, le taux de coût est 0.

## Coût réel - Utilisateur et rôle, par heure

Lorsque le type de coût de la tâche est Utilisateur et Rôle par heure, Workfront utilise deux hiérarchies pour déterminer le taux de facturation du coût réel. Le taux de facturation est basé sur les heures de connexion de l’utilisateur à une tâche.

L’« utilisateur » dans les hiérarchies est la personne affectée à la tâche. Le « propriétaire » est la personne dont le temps est enregistré pour la tâche, même s’il n’est pas affecté à la tâche. Par exemple, Michael est affecté à une tâche, mais Joanna termine le travail parce que Michael était malade. Le responsable peut consigner le temps par rapport à la tâche et définir le propriétaire des heures consignées sur Joanna. Les valeurs de revenus prévus sont basées sur l&#39;affectation de Michael et le taux dans la hiérarchie, mais les valeurs de revenus réels sont basées sur le taux de Joanna.

Cette image présente le flux de la hiérarchie des coûts réels :

![Coût réel pour l&#39;utilisateur et le type de coût horaire du rôle](assets/actual-cost-chart.png)

### Lorsque le propriétaire des heures consignées et l’utilisateur affecté à la tâche sont le même

Workfront recherche d’abord un taux de coût par affectation d’utilisateur. Si un utilisateur n’est pas affecté à la tâche, il recherche un taux de coût par affectation de fonction.

La hiérarchie de ce scénario est identique à celle des coûts planifiés. Voir [Coût prévu - Utilisateur et rôle par heure](#planned-cost--user-and-role-hourly) pour ce workflow.

### Lorsque le propriétaire des heures consignées n&#39;est pas l&#39;utilisateur affecté à la tâche

Workfront effectue une recherche dans les propriétés utilisateur du propriétaire selon cette hiérarchie :

1. Le système recherche le taux de coût du projet, pour le propriétaire, en tenant compte des dates d&#39;entrée en vigueur. Vous pourrez le voir dans la zone Taux > Coût du projet, dans un regroupement **Taux Source : Remplacements > Type de ressource : Utilisateur**. Il s’agit d’un taux de remplacement pour le projet.
1. Ensuite, le système recherche le taux de coût au niveau du système sur le profil utilisateur du propriétaire, en prenant en compte les dates d’entrée en vigueur.
1. Ensuite, le système recherche le taux de coût de la fonction principale du propriétaire (Designer dans l’exemple).

   * Le système recherche d&#39;abord le taux de coût du projet, pour la fonction principale du propriétaire, en tenant compte des dates d&#39;entrée en vigueur. Elle s&#39;affiche dans la zone Taux > Coût du projet, dans un regroupement **Taux Source : Remplacements > Type de ressource : Fonction**. Il s’agit d’un taux de remplacement pour le projet.
   * Ensuite, le système recherche le taux de fonction à partir d’une carte tarifaire, en tenant compte des dates d’entrée en vigueur. Vous pourrez le voir dans la zone Taux > Coût du projet, dans un regroupement **Taux Source : Carte tarifaire associée > Type de ressource : Fonction**.
   * Ensuite, le système recherche le taux de fonctions au niveau du système, en prenant en compte les dates d’entrée en vigueur.

1. Si aucun de ces taux n’est trouvé, le taux de facturation est de 0.

