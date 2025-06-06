---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Créer une demande  [!DNL Adobe Workfront]  à partir d’un e-mail Outlook
description: Vous pouvez créer une demande  [!DNL Adobe Workfront]  à partir d’un e-mail dans Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 77%

---

# Créer une demande [!DNL Adobe Workfront] à partir d’un e-mail [!UICONTROL Outlook]

>[!IMPORTANT]
>
>[Microsoft est en train de désactiver la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le complément Workfront Outlook pour l&#39;authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et continuera à être déployée par phases jusqu’en octobre 2025.
>
>* **Une fois que Microsoft a complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionne plus.**
>
>Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière dont les jetons sont réactivés. Après le **30 juin 2025**, les administrateurs ne pourront plus réactiver les jetons eux-mêmes. Seule la prise en charge de Microsoft peut accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Les exceptions ne seront pas accordées.**

Vous pouvez créer une demande [!DNL Adobe Workfront] à partir d’un e-mail dans Outlook.

Lorsque vous créez une demande [!DNL Workfront] basée sur un e-mail, le contenu de l’e-mail (y compris l’objet et le corps) est inclus par défaut dans la demande.

>[!NOTE]
>
>Vous ne pouvez pas créer une demande [!DNL Workfront] à partir d’une boîte aux lettres partagée [!UICONTROL Outlook].

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

Votre administrateur ou administratrice [!DNL Workfront] doit activer [!DNL Outlook for Office] avec [!DNL Workfront] avant que vous ne puissiez utiliser cette intégration.

## Créer une demande à partir d’un e-mail [!DNL Outlook]

Pour créer une demande [!DNL Workfront] à partir d’[!DNL Outlook], procédez comme suit :

1. Sélectionnez l’e-mail qui contient les informations que vous souhaitez inclure dans une demande [!DNL Workfront].
1. Cliquez sur l’icône **[!DNL Workfront]** dans le coin supérieur droit de l’e-mail pour afficher le module complémentaire Workfront.\
   Il se peut que vous deviez cliquer sur la flèche pointant vers le bas en haut à droite de votre e-mail pour accéder à l’icône [!DNL Workfront].

1. Cliquez sur l’icône **[!UICONTROL Menu]** ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png) pour afficher la liste des options [!DNL Workfront] disponibles.

1. Cliquez sur **[!UICONTROL Envoyer la demande]**.
1. Dans le champ **[!UICONTROL Sélectionner un type de demande]**, sélectionnez la file d’attente des demandes dans laquelle vous souhaitez soumettre la demande.

1. Indiquez les informations suivantes :\
   Les champs disponibles peuvent varier en fonction de la configuration de la file d’attente des demandes. Pour une liste complète et une description des champs possibles, voir l’article [Créer et soumettre des demandes  [!DNL Adobe Workfront] ](../../manage-work/requests/create-requests/create-submit-requests.md).

   * **[!UICONTROL Objet] :** indiquez un objet pour la demande. Par défaut, l’objet de l’e-mail est utilisé.
   * **[!UICONTROL Description] :** spécifiez une description pour la demande. Par défaut, le corps de l’e-mail est utilisé.
   * **[!UICONTROL Documents] :** joignez tous les documents que vous souhaitez inclure dans la demande. Vous pouvez joindre des documents en les faisant glisser et en les déposant, ou en cliquant sur **[!UICONTROL Sélectionner un fichier]** et en recherchant et sélectionnant le document.

     Par défaut, tous les documents joints à l’e-mail sont inclus dans la demande.

1. Cliquez sur **[!UICONTROL Soumettre la demande]**.\
   La demande est soumise à [!DNL Workfront], dans la file d’attente des demandes spécifiée.

1. (Facultatif) Retournez sur [!DNL Outlook] et sélectionnez l’e-mail original.\
   En haut du panneau du complément [!DNL Workfront], remarquez la confirmation, avec un lien, que l’e-mail a été ajouté à Workfront en tant que demande. Le lien comprend la date à laquelle il a été converti.\
