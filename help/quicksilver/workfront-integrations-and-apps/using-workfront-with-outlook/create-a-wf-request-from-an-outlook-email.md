---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Créez un [!DNL Adobe Workfront] demande d’un courrier électronique Outlook
description: Vous pouvez créer un [!DNL Adobe Workfront] à partir d’un courrier électronique dans Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Créez un [!DNL Adobe Workfront] d’une [!UICONTROL Outlook] email

Vous pouvez créer un [!DNL Adobe Workfront] à partir d’un courrier électronique dans Outlook.

Lorsque vous créez une [!DNL Workfront] sur la base d’un email, le contenu de l’email (y compris l’objet et le corps) est inclus par défaut dans la requête.

>[!NOTE]
>
>Vous ne pouvez pas créer un [!DNL Workfront] requête d’un partage [!UICONTROL Outlook] boîte aux lettres.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Conditions préalables

Votre [!DNL Workfront] L’administrateur doit activer [!DNL Outlook for Office] avec [!DNL Workfront] avant de pouvoir utiliser cette intégration.

## Créez une requête à partir d’une [!DNL Outlook] email

Pour créer une [!DNL Workfront] Demander à [!DNL Outlook]:

1. Sélectionnez l&#39;email contenant les informations que vous souhaitez inclure dans un [!DNL Workfront] requête.
1. Cliquez sur le bouton **[!DNL Workfront]** dans le coin supérieur droit de l’e-mail pour afficher le module complémentaire Workfront.\
   Vous devrez peut-être cliquer sur la flèche pointant vers le bas dans le coin supérieur droit de votre email pour accéder à la variable [!DNL Workfront] icône .

1. Cliquez sur le bouton **[!UICONTROL Menu]** pour afficher la liste des [!DNL Workfront] options.

   ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png)

1. Cliquez sur **[!UICONTROL Envoyer la requête]**.
1. Dans le **[!UICONTROL Sélection d’un type de requête]** , sélectionnez la file d’attente de requête dans laquelle vous souhaitez envoyer la requête.

   ![o365_addin_submitrequest.png](assets/o365-addin-submitrequest.png)

1. Indiquez les informations suivantes :\
   Selon la configuration de la file d’attente des demandes, les champs disponibles peuvent varier. Pour obtenir la liste complète et la description des champs possibles, voir [Créer et envoyer [!DNL Adobe Workfront] requests](../../manage-work/requests/create-requests/create-submit-requests.md) article.

   * **[!UICONTROL Objet]:** Spécifiez l’objet de la requête. Par défaut, l&#39;objet de l&#39;email est utilisé.
   * **[!UICONTROL Description]:** Spécifiez une description pour la requête. Par défaut, le corps de l&#39;email est utilisé.
   * **[!UICONTROL Documents]:** Joignez tous les documents que vous souhaitez inclure dans la requête. Vous pouvez joindre des documents par glisser-déposer ou en cliquant sur **[!UICONTROL Sélectionner un fichier]** et accédez au document et sélectionnez-le.\

      Par défaut, tous les documents joints au courrier électronique sont inclus dans la demande.

1. Cliquez sur **[!UICONTROL Envoyer la requête]**.\
   La demande est envoyée à [!DNL Workfront], dans la file d’attente de requête spécifiée.

1. (Facultatif) Revenez à [!DNL Outlook], puis sélectionnez l’email d’origine.\
   En haut de la [!DNL Workfront] module complémentaire, notez la confirmation avec un lien que le courrier électronique a été ajouté à Workfront en tant que demande. Le lien comprend la date à laquelle il a été converti.\
   ![perspectives_submit_as_a_request.png](assets/outlook-submitted-as-a-request-350x130.png)
