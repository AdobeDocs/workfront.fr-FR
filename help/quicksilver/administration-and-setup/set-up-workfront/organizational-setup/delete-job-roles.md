---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Suppression de rôles de tâche
description: Vous pouvez supprimer les rôles de tâche que votre entreprise n’utilise plus. Nous vous recommandons de ne pas supprimer les rôles de tâche s’ils ont été associés à des tâches par le passé. Pour conserver toutes vos informations historiques sur les affectations de travail, nous vous recommandons de désactiver les rôles plutôt que de les supprimer lorsqu’ils deviennent obsolètes. Pour plus d’informations sur la désactivation des rôles, voir Désactivation des rôles de tâche.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Suppression de rôles de tâche

Vous pouvez supprimer les rôles de tâche que votre entreprise n’utilise plus. Nous vous recommandons de ne pas supprimer les rôles de tâche s’ils ont été associés à des tâches par le passé.

Pour conserver toutes vos informations historiques sur les affectations de travail, nous vous recommandons de désactiver les rôles plutôt que de les supprimer lorsqu’ils deviennent obsolètes. Pour plus d’informations sur la désactivation des rôles, voir [Désactivation des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux rôles de tâche</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Suppression d’un rôle de tâche

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Rôles de tâche].**
1. Sélectionnez le rôle de tâche à supprimer, puis cliquez sur **[!UICONTROL Supprimer].**
1. Si des objets (utilisateurs, tâches, problèmes) sont affectés au rôle de tâche, effectuez l’une des opérations suivantes :

   * **Remplacez le rôle de tâche par un autre rôle de tâche :** Sélectionnez le nouveau rôle de tâche dans la liste déroulante.

      Toutes les affectations de ressources actuelles et antérieures associées au rôle de tâche supprimé sont transférées vers le rôle de tâche que vous sélectionnez.

      Les utilisateurs auxquels un seul rôle de tâche est affecté sont réaffectés au rôle de tâche que vous sélectionnez ; les utilisateurs auxquels un rôle de tâche secondaire est affecté ne sont pas réaffectés au rôle de tâche que vous sélectionnez.

   * **Supprimez le rôle de tâche et son allocation de ressources :** Sélectionner **[!UICONTROL Aucun]** dans la liste déroulante.

      >[!IMPORTANT]
      >
      >La suppression d’un rôle de tâche supprime toutes les affectations de ressources actuelles et antérieures associées à ce rôle de tâche pour tous les projets.

      &#x200B; Par exemple, si une tâche ou un problème n’est affecté qu’à ce rôle de tâche, la tâche ou le problème n’est pas attribué une fois le rôle de tâche supprimé.

1. Cliquez sur  **[!UICONTROL Oui, la supprimer]**.
