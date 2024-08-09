---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système
description: Les groupes de votre entreprise peuvent avoir besoin d’une préférence de projet configurée différemment pour leurs workflows uniques. Vous pouvez déverrouiller la préférence pour tous les groupes de l’organisation afin qu’ils puissent la configurer par eux-mêmes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 13%

---

# Verrouillage ou déverrouillage des préférences de projet pour tous les groupes du système

Les groupes de votre entreprise peuvent avoir besoin d’une préférence de projet configurée différemment pour leurs workflows uniques. Vous pouvez déverrouiller la préférence pour tous les groupes de l’organisation afin qu’ils puissent la configurer par eux-mêmes.

Lorsqu’une préférence est déverrouillée et que l’administrateur du groupe la modifie, les projets associés au groupe obtiennent la configuration correspondant à cette préférence à partir du paramètre au niveau du groupe plutôt que du paramètre au niveau du système.

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
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## A propos des préférences verrouillées et déverrouillées

Le verrouillage d’un projet, d’une tâche ou d’une préférence d’émission que vous avez configurée au niveau du système garantit que chacun utilise le même paramètre pour cette préférence. Bien que vous puissiez toujours reconfigurer une préférence que vous verrouillez, les administrateurs de groupe ne peuvent pas la reconfigurer pour leurs groupes.

Inversement, le déverrouillage d’un projet, d’une tâche ou d’une préférence de problème offre aux administrateurs de groupe une plus grande flexibilité pour gérer la manière dont leurs groupes fonctionnent avec ces éléments. Lorsqu’une préférence est déverrouillée, les administrateurs de groupe peuvent la reconfigurer pour leurs groupes.

Si un champ ne comporte pas de bouton de verrouillage/déverrouillage, il ne peut pas être déverrouillé pour que les administrateurs de groupe configurent les paramètres au niveau du groupe. La configuration est uniquement disponible au niveau du système.

Pour plus d’informations sur le verrouillage ou le déverrouillage d’un projet, d’une tâche ou d’une préférence de problème au niveau du système, voir [ Configuration de la tâche à l’échelle du système et préférences d’émission](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Une fois qu’un administrateur [!DNL Workfront] a déverrouillé une préférence au niveau du système, tout administrateur de groupe peut la configurer, puis la verrouiller pour s’assurer que tous les membres de leur groupe et les sous-groupes ci-dessous utilisent la même configuration. Cela est parallèle à la possibilité qu’un administrateur [!DNL Workfront] doit configurer et verrouiller une préférence pour tous les utilisateurs du système. Pour plus d’informations, voir [Configuration des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et [Verrouillage ou déverrouillage d’un projet, d’une tâche ou d’une préférence de problème pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Déverrouiller une préférence de projet afin que les groupes puissent la configurer ;

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]**, puis sur **[!UICONTROL Projets]**.

1. Effectuez l’une des opérations suivantes :

   * Si vous souhaitez que les administrateurs de groupes puissent configurer une préférence pour leurs groupes, déverrouillez-la ![](assets/unlock-toggle-button.png).
   * Si vous souhaitez que tous les groupes utilisent votre configuration pour une préférence, assurez-vous qu’elle est verrouillée (il s’agit de la valeur par défaut).

     >[!IMPORTANT]
     >
     >Nous vous recommandons de communiquer avec les administrateurs et les utilisateurs de groupes dans tout le système pour vous assurer que tous les besoins sont pris en compte dans la configuration d’une préférence verrouillée. Lorsque vous le verrouillez, votre configuration pour elle est héritée par tous les groupes du système. Et si la préférence a été déverrouillée pendant une période quelconque, votre configuration remplace celles que les administrateurs de groupe peuvent avoir faites.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
