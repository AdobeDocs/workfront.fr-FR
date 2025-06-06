---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Ajouter un e-mail Outlook en tant que tâche à votre liste de travail
description: Vous pouvez convertir les e-mails  [!DNL Outlook]  en tâches  [!DNL Adobe Workfront] . Une fois qu’un e-mail a été converti, la tâche est disponible dans votre liste de travaux de la zone Accueil.
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 76%

---

# Ajouter un e-mail [!DNL Outlook] en tant que tâche à votre liste de travaux

>[!IMPORTANT]
>
>[Microsoft est en train de désactiver la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le complément Workfront Outlook pour l&#39;authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et continuera à être déployée par phases jusqu’en octobre 2025.
>
>* **Une fois que Microsoft a complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionne plus.**
>
>Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière dont les jetons sont réactivés. Après le **30 juin 2025**, les administrateurs ne pourront plus réactiver les jetons eux-mêmes. Seule la prise en charge de Microsoft peut accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Les exceptions ne seront pas accordées.**


Vous pouvez convertir les e-mails [!DNL Outlook] en tâches [!DNL Adobe Workfront]. Une fois qu’un e-mail a été converti, la tâche est disponible dans votre liste de [!UICONTROL travaux] dans la zone [!UICONTROL Accueil].

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

Votre administrateur ou administratrice [!DNL Workfront] doit activer [!DNL Outlook for Office] avec [!DNL Workfront] avant de pouvoir utiliser cette intégration.

## Ajouter un e-mail [!DNL Outlook] tant que tâche à votre liste de travaux

1. Sélectionnez l’e-mail dans [!DNL Outlook] que vous souhaitez convertir en tâche.
1. Cliquez sur l’icône **[!DNL Workfront]** dans le coin supérieur droit de l’e-mail pour afficher le module complémentaire [!DNL Workfront].\
   Vous devrez peut-être cliquer sur la flèche pointant vers le bas dans le coin supérieur droit de votre e-mail pour accéder à l’icône [!DNL Workfront].

1. Cliquez sur l’icône **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) pour afficher la liste des options [!DNL Workfront] disponibles.\


1. Cliquez sur **[!UICONTROL Ajouter au travail]**.\

1. Désélectionnez le champ **[!UICONTROL Ajouter au projet]**.
1. (Facultatif) Vous pouvez mettre à jour les informations suivantes de l’e-mail avant de l’enregistrer en tant que tâche :

   * **[!UICONTROL Nom de la tâche] :** par défaut, le nom de la tâche est identique à celui de l’objet de l’e-mail. Vous pouvez modifier le nom de la tâche selon vos besoins.
   * **[!UICONTROL Description] :** par défaut, la description est identique à celle du corps de l’e-mail. Vous pouvez modifier la description selon vos besoins.
   * **[!UICONTROL Pièces jointes] :** toutes les pièces jointes aux e-mails sont enregistrées dans la zone [!UICONTROL Documents] de la tâche. Vous pouvez supprimer toutes les pièces jointes avant d’enregistrer l’e-mail comme tâche.

1. Cliquez sur **[!UICONTROL Ajouter]**.\
   La tâche est ajoutée à la [!UICONTROL Liste de travaux] dans votre zone Accueil sans date d’engagement.

1. (Facultatif) Cliquez sur **[!UICONTROL Afficher dans Workfront]** pour afficher la tâche dans l’application [!DNL Workfront] dans un nouvel onglet.

1. (Facultatif) Revenez à [!DNL Outlook], puis sélectionnez l’e-mail d’origine.\
   En haut du panneau du module complémentaire [!DNL Workfront], remarquez la confirmation avec un lien qui indique que l’e-mail a été ajouté à Workfront en tant que tâche. Le lien comprend la date à laquelle il a été converti.\
