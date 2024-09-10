---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Supprimer fonctions
description: Vous pouvez supprimer les fonctions que votre entreprise n’utilise plus. Nous vous recommandons de ne pas supprimer les fonctions si elles ont été associées à des éléments de travail par le passé. Pour conserver toutes vos informations historiques sur les affectations de travail, nous vous recommandons de désactiver les rôles plutôt que de les supprimer lorsqu’ils deviennent obsolètes. Pour plus d’informations sur la désactivation des rôles, voir Désactiver des fonctions.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 98%

---

# Supprimer des fonctions

Vous pouvez supprimer les fonctions que votre entreprise n’utilise plus. Nous vous recommandons de ne pas supprimer les fonctions si elles ont été associées à des éléments de travail par le passé.

Pour conserver toutes vos informations historiques sur les affectations de travail, nous vous recommandons de désactiver les rôles plutôt que de les supprimer lorsqu’ils deviennent obsolètes. Pour plus d’informations sur la désactivation des rôles, voir [Désactiver des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouvelle : [!UICONTROL Standard]</p>
   <p>Ou</p>
   <p>Actuelle : [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Accès administratif aux rôles de tâche</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Supprimer une fonction

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Fonctions].**
1. Sélectionnez la fonction que vous souhaitez supprimer, puis cliquez sur **[!UICONTROL Supprimer].**
1. Si des objets (utilisateurs et utilisatrices, tâches, problèmes) sont affectés à la fonction, effectuez l’une des opérations suivantes :

   * **Remplacez la fonction par une autre fonction :** sélectionnez la nouvelle fonction dans la liste déroulante.

     Toutes les allocations de ressources actuelles et passées associées à la fonction supprimée sont transférées à la fonction sélectionnée.

     Les utilisateurs et utilisatrices auxquels une seule fonction a été attribuée sont réaffectés à la fonction sélectionnée. Les personnes auxquelles une fonction secondaire a été affectée ne sont pas réaffectées à la fonction sélectionnée.

   * **Supprimez la fonction et son allocation de ressources :** sélectionnez **[!UICONTROL Aucune]** dans la liste déroulante.

     >[!IMPORTANT]
     >
     >La suppression d’une fonction entraîne celle de toutes les allocations de ressources actuelles et passées qui sont liées à cette fonction pour tous les projets.

     Par exemple, si un objet (tâche ou problème) n’est affecté qu’à cette fonction, cet élément n’est plus affecté après la suppression de la fonction.

1. Cliquez sur **[!UICONTROL Oui, supprimer]**.
