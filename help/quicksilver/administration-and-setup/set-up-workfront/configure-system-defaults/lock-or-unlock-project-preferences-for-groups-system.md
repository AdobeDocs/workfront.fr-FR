---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système
description: Des groupes de votre organisation peuvent nécessiter qu’une préférence de projet soit configurée différemment pour leurs workflows uniques. Vous pouvez déverrouiller la préférence pour tous les groupes de l’organisation afin qu’ils puissent la configurer eux-mêmes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 97%

---

# Verrouiller ou déverrouiller les préférences de projet pour tous les groupes du système

Des groupes de votre organisation peuvent nécessiter qu’une préférence de projet soit configurée différemment pour leurs workflows uniques. Vous pouvez déverrouiller la préférence pour tous les groupes de l’organisation afin qu’ils puissent la configurer eux-mêmes.

Lorsqu’une préférence est déverrouillée et que l’administrateur ou l’administratrice de groupes la modifie, les projets associés au groupe héritent de la configuration de cette préférence du paramètre au niveau du groupe au lieu du paramètre au niveau du système.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour plus d’informations sur la manière dont un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## À propos des préférences verrouillées et déverrouillées

Le verrouillage d’une préférence de projet, de tâche ou de problème que vous avez configurée au niveau du système garantit que toutes les personnes utilisent le même paramètre pour cette préférence. Bien que vous puissiez toujours reconfigurer une préférence que vous avez verrouillée, les administrateurs et administratrices de groupes ne peuvent pas la reconfigurer pour leurs groupes.

À l’inverse, le déverrouillage d’une préférence de projet, de tâche ou de problème permet aux administrateurs et administratrices de groupes de gérer avec plus de souplesse la manière dont leurs groupes utilisent ces éléments. Lorsqu’une préférence est déverrouillée, les administrateurs et administratrices de groupes peuvent la reconfigurer pour leurs groupes.

Si un champ ne comporte pas de bouton (bascule) de verrouillage/déverrouillage, il ne peut pas être déverrouillé pour que les administrateurs et administratrices de groupes configurent les paramètres au niveau du groupe. La configuration est uniquement disponible au niveau du système.

Pour obtenir des instructions sur le verrouillage ou le déverrouillage d’une préférence de projet, de tâche ou de problème au niveau du système, voir [Configurer les préférences de tâche et de problème à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Une fois qu’un administrateur ou qu’une administratrice [!DNL Workfront] a déverrouillé une préférence au niveau du système, toute personne membre de l’administration du groupe peut la configurer, puis la verrouiller pour s’assurer que toutes les personnes membres de son groupe et des sous-groupes inférieurs utilisent la même configuration. Cette fonction est similaire à la capacité qu’a un administrateur ou une administratrice  de configurer et de verrouiller une préférence pour toutes les personnes utilisant le système. [!DNL Workfront] Pour plus d’informations, voir [Configurer les préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et [Verrouiller ou déverrouiller une préférence de projet, de tâche ou de problème pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Déverrouiller une préférence de projet pour que les groupes puissent la configurer.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]**, puis sur **[!UICONTROL Projets]**.

1. Effectuez l’une des opérations suivantes :

   * Si vous souhaitez que les administrateurs et administratrices de groupes puissent configurer une préférence pour leurs groupes, déverrouillez-la ![](assets/unlock-toggle-button.png).
   * Si vous souhaitez que tous les groupes utilisent votre configuration pour une préférence, assurez-vous qu’elle est verrouillée (option par défaut).

     >[!IMPORTANT]
     >
     >Nous vous recommandons de communiquer avec l’ensemble des personnes qui administrent et utilisent le système afin de vous assurer que tous les besoins sont pris en compte lors de la configuration d’une préférence verrouillée. Lorsque vous la verrouillez, votre configuration est héritée par tous les groupes du système. De plus, si la préférence a été déverrouillée pour une période de temps donnée, votre configuration remplace celles que les administrateurs et administratrices de groupes ont pu effectuer.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
