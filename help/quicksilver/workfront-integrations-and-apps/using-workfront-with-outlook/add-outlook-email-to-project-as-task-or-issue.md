---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Ajouter un e-mail Outlook à un projet en tant que tâche ou problème
description: Vous pouvez convertir des e-mails en tâches ou problèmes  [!DNL Adobe Workfront] . Après la conversion d’un e-mail, la tâche ou le problème apparaît dans le projet sélectionné au moment de la conversion.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 00755c27-9fc9-4357-a39b-4f9772484252
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 82%

---

# Ajouter un e-mail [!DNL Outlook] à un projet en tant que tâche ou problème

>[!IMPORTANT]
>
>[Microsoft est en train de désactiver la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le complément Workfront Outlook pour l&#39;authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et continuera à être déployée par phases jusqu’en octobre 2025.
>
>* **Une fois que Microsoft a complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionne plus.**
>
>Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière dont les jetons sont réactivés. Après le **30 juin 2025**, les administrateurs ne pourront plus réactiver les jetons eux-mêmes. Seule la prise en charge de Microsoft peut accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Les exceptions ne seront pas accordées.**

Vous pouvez convertir des e-mails en tâches ou problèmes [!DNL Adobe Workfront]. Après la conversion d’un e-mail, la tâche ou le problème apparaît dans le projet sélectionné au moment de la conversion.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] formule*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Conditions préalables

Votre équipe d’administration [!DNL Workfront] doit activer [!DNL Outlook for Office] avec [!DNL Workfront] pour que vous puissiez utiliser cette intégration.

## Ajouter un e-mail [!DNL Outlook] à un projet en tant que tâche ou problème

1. Sélectionnez l’e-mail [!DNL Outlook] que vous souhaitez convertir en tâche ou en problème.
1. Cliquez sur l’icône **[!DNL Workfront]** dans le coin supérieur droit de l’e-mail pour afficher le module complémentaire Workfront.

   Vous devrez peut-être cliquer sur la flèche pointant vers le bas dans le coin supérieur droit de votre e-mail pour accéder à l’icône [!DNL Workfront].

1. Cliquez sur l’icône **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) pour afficher la liste des options [!DNL Workfront] disponibles.



1. Cliquez sur **[!UICONTROL Ajouter au travail]**.

1. Sélectionnez le champ **[!UICONTROL Ajouter au projet]**.
1. Commencez à saisir le nom d’un projet dans le champ **[!UICONTROL Projet]**, puis sélectionnez-le lorsqu’il apparaît dans la liste.
1. Sélectionnez la case d’option **[!UICONTROL Tâche]** si vous souhaitez ajouter une tâche au projet sélectionné.

   Ou

   Sélectionnez la case d’option **[!UICONTROL Problème]** si vous souhaitez ajouter un problème au projet sélectionné.

1. (Facultatif) Spécifiez à qui affecter cette tâche ou ce problème dans le champ **[!UICONTROL Affecter ceci à]**.

   >[!TIP]
   >
   >Vous pouvez attribuer la tâche ou le problème à une équipe si vous souhaitez que plusieurs personnes en soient informées. Si les personnes membres de l’équipe ont activé les notifications par e-mail, elles recevront un e-mail concernant l’affectation de la nouvelle tâche ou du nouveau problème.


1. (Facultatif) Indiquez la **[!UICONTROL Date d’échéance]**. Cette date devient la [!UICONTROL Date d’achèvement prévue] de la tâche ou du problème.
1. (Facultatif) Mettez à jour les informations suivantes de l’e-mail avant de l’enregistrer en tant que tâche ou problème (les champs obligatoires sont précédés d’un astérisque).

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Task or Issue Name]</td>
        <td>Par défaut, le nom de la tâche est le même que l’objet de l’e-mail. Vous pouvez modifier le nom de la tâche selon vos besoins.</td>
        <td></td>
      </tr>
      <tr>
        <td>[!UICONTROL Description]</td>
        <td>Par défaut, la description est identique au corps de l’e-mail. Vous pouvez modifier la description selon vos besoins.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Attachments]</td>
        <td>Les pièces jointes sont enregistrées dans la zone [!UICONTROL Documents] de la tâche ou du problème. Vous pouvez supprimer les pièces jointes avant d’enregistrer l’e-mail en tant que tâche ou problème.</td>
      </tr>
   </table>

1. Cliquez sur **[!UICONTROL Ajouter]**.

   L’objet (tâche ou problème) est ajouté au projet spécifié.

1. (Facultatif) Cliquez sur **[!UICONTROL Afficher dans[!DNL Workfront]]** pour afficher la tâche dans l’application [!DNL Workfront] dans un nouvel onglet.

1. (Facultatif) Retournez sur [!DNL Outlook] et sélectionnez l’e-mail converti.

   En haut du panneau du module complémentaire [!DNL Workfront], vous remarquerez la confirmation avec un lien que l’e-mail a été ajouté à [!DNL Workfront] en tant que tâche ou problème. Le lien comprend la date à laquelle il a été converti.



