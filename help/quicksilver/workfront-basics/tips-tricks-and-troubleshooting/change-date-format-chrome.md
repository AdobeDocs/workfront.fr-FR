---
filename: change-date-format-chrome
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Modifier le format des dates dans [!DNL Adobe Workfront]
description: Pour modifier le format de date des dates dans  [!DNL Adobe Workfront] vous devez modifier les paramètres de langue dans votre navigateur.
feature: Get Started with Workfront
exl-id: 9fac92fb-e3d1-4537-b324-4b35447cef28
source-git-commit: e9a96b6952ca3f128cc723df68787f40c8dcf604
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 2%

---

# Modifier le format des dates dans [!DNL Adobe Workfront]

<!--this article used to be called "Change the date format in Adobe Workfront when using Chrome". The team decieded to make it more generic and hide the steps. Also see drafted content below-->

Vous pouvez modifier le format de date des dates dans [!DNL Adobe Workfront], par exemple [!UICONTROL Date d’achèvement planifiée], [!UICONTROL Date d’achèvement réelle] ou [!UICONTROL Date d’achèvement prévue].

Par exemple, vous pouvez remplacer le format de date _JJ/MM/AAAA_ par _MM/JJ/AAAA_ ou inversement.
Vous pouvez également remplacer le format de date _MM/JJ/AA_ par _Lun JJ, AAAA_.

Vous pouvez modifier les formats de date dans Workfront comme suit, selon les modifications que vous souhaitez afficher et l’endroit où vous souhaitez les voir.

* Pour modifier tous les formats de date pour toutes les pages de [!DNL Workfront] en fonction de votre emplacement et de votre langue, vous devez modifier les paramètres de langue dans votre navigateur.

  Par exemple, si la langue par défaut de votre navigateur est définie sur *[!UICONTROL Anglais (États-Unis)]*, les dates s’affichent dans les formats suivants :

   * MM/JJ/AAAA
   * Lun JJ, AAAA

  Pour modifier les paramètres de langue dans [!DNL Chrome] ou tout autre navigateur, vous devez modifier les paramètres de ce navigateur. Les étapes de modification des paramètres d’un navigateur varient d’un navigateur à l’autre. Reportez-vous aux zones [!UICONTROL Aide], [!UICONTROL Préférences] ou [!UICONTROL Paramètres] de votre navigateur pour savoir comment modifier ses paramètres.

* Pour modifier le format des dates uniquement dans les rapports et vues, vous devez mettre à jour le paramètre [!UICONTROL Format du champ] dans la zone [!UICONTROL Options avancées] d’une colonne, lors de la création du rapport ou de la vue. Cela ne modifie pas le format de date en fonction de l’emplacement ou de la langue. Il modifie le format des dates dans le contexte du même emplacement ou de la même langue.

  ![](assets/field-format-in-advanced-options-of-a-view-highlighted.png)

  Pour plus d’informations, consultez [Créer un rapport personnalisé](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Pour modifier le format des dates dans toutes les notifications électroniques sortantes pour l’ensemble de votre organisation, vous devez mettre à jour le paramètre [!UICONTROL Paramètres régionaux par défaut de l’e-mail] dans la zone [!UICONTROL Informations sur le client] de [!UICONTROL Configuration].

  ![](assets/default-email-locale-field.png)

  Pour plus d’informations, voir [Configuration des informations de base pour votre système](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Pour modifier le format de toutes les dates dans toutes les notifications électroniques sortantes pour un seul utilisateur, vous devez mettre à jour le paramètre [!UICONTROL Paramètre régional du courrier électronique] dans la zone [!UICONTROL Modifier la personne], lors de la modification du profil d’un utilisateur.

  ![](assets/email-locale-for-user-profile-highlighted.png)

  Pour plus d’informations, voir [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--drafted because we should not document steps for a third-party application

To change your language settings in Chrome:

1. Click the 3-dots in the top right corner of your Chrome interface, then click **Settings**.
1. On the left area of the Settings page, expand **Advanced**, then click **Languages**.  
   Or  
   Search for *language*&nbsp;at the top of the Settings page, then click **Languages**.

1. In the **Language** list, locate the language and region that use your preferred date format.

   **Example:** If you speak English and you want the date format to be MM/DD/YYYY, you would select **English (United States)**. If you speak English and you want the date format to be DD/MM/YYY, you would select **English (United Kingdom)**.

1. (Conditional) If the language and region you want to use are not visible in the list, click **Add languages** to add it to the list.
1. Click the 3-dot menu next to the language and region you want to use, then click **Move to the top**.
1. Return to the Workfront interface, then refresh the page.  
   The date format is now updated in projects and other areas of Workfront that use MM/DD/YYYY or DD/MM/YYYY format when displaying dates.

   -->
