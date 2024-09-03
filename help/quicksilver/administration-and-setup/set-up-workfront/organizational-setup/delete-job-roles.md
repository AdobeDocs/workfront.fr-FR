---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Supprimer des fonctions
description: Vous pouvez supprimer les fonctions que votre entreprise n’utilise plus. Nous vous recommandons de ne pas supprimer les fonctions si elles ont été associées à des éléments de travail par le passé. Pour conserver toutes vos informations historiques sur les affectations de travail, nous vous recommandons de désactiver les rôles plutôt que de les supprimer lorsqu’ils deviennent obsolètes. Pour plus d’informations sur la désactivation des rôles, voir Désactiver des fonctions.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 100%

---

# Supprimer des fonctions

Vous pouvez supprimer les fonctions que votre entreprise n’utilise plus. Nous vous recommandons de ne pas supprimer les fonctions si elles ont été associées à des éléments de travail par le passé.

Pour conserver toutes vos informations historiques sur les affectations de travail, nous vous recommandons de désactiver les rôles plutôt que de les supprimer lorsqu’ils deviennent obsolètes. Pour plus d’informations sur la désactivation des rôles, voir [Désactiver des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès administratif aux fonctions</p> <p><b>NOTE</b> : si votre accès n’est toujours pas activé, demandez à votre administrateur ou à votre administratrice [!DNL Workfront] si des restrictions supplémentaires au niveau de votre accès ont été définies. Pour plus d’informations sur la manière dont une équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Supprimer une fonction

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

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
