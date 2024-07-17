---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Présentation des connexions
description: Pour la plupart des applications, il est nécessaire de créer une connexion, par laquelle  [!DNL Adobe Workfront Fusion]  peut communiquer avec le service tiers donné en fonction des paramètres du scénario spécifique.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 8%

---

# Présentation des connexions

<!-- Audited: 3/2024-->

Pour la plupart des applications, [!DNL Workfront Fusion] nécessite une connexion, par laquelle il peut communiquer avec le service tiers donné en fonction des paramètres du scénario spécifique.

Par exemple, si vous souhaitez créer un scénario qui récupère des informations de [!DNL Workfront], vous devez accorder l’autorisation d’accès à [!DNL Workfront Fusion] pour accéder à votre compte [!DNL Workfront].

Une connexion représente l’autorisation et les autorisations utilisées par Fusion pour accéder à l’application. Vous pouvez créer une ou plusieurs connexions pour chaque application et utiliser la même connexion dans plusieurs modules ou scénarios.

La plupart des connexions ne sont utilisées que pour une seule application. Par exemple, une connexion [!DNL Workfront] ne peut pas être utilisée dans un module [!UICONTROL Salesforce]. Certaines applications [!DNL Adobe] peuvent partager des connexions. Pour plus d’informations, reportez-vous aux articles relatifs à ces applications, répertoriés dans la section [Applications et leurs modules](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

Les connexions sont gérées au niveau de l’équipe. Tous les membres d’une équipe ont accès aux connexions de l’équipe et les utilisateurs en dehors d’une équipe n’ont pas accès aux connexions de l’équipe.

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Actuel : aucune exigence de licence [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Hérité : Tout </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Nouveau :</p> <ul><li>Formule [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront] : [!DNL Workfront Fusion] est inclus.</li></ul>
   <p>Ou</p>
   <p>Actuel : votre organisation doit acheter [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Droits d’accès

Pour chaque connexion, [!DNL Workfront Fusion] ne nécessite que les droits d’accès nécessaires pour terminer un scénario donné. Par exemple, si vous créez un scénario pour répertorier les documents de [!DNL Google Docs], [!DNL Workfront Fusion] ne demande pas l’autorisation d’obtenir le contenu des documents. Par la suite, si vous constatez que vous devez accéder au contenu des documents, vous pouvez mettre à jour la connexion ou en créer une qui puisse accéder à ce contenu.

Tous les services ne permettent pas de limiter l’accès à des tâches spécifiques. Dans ce cas, [!DNL Workfront Fusion] doit exiger des droits d’accès complets. Pour plus d’informations sur la façon de restreindre l’accès [!DNL Workfront Fusion] à votre compte enregistré pour ces services, consultez la documentation spécifique à l’application répertoriée dans [Applications et leurs modules](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Gestion des connexions

Vous pouvez gérer toutes les connexions à partir de la zone [!UICONTROL Connexions].

>[!NOTE]
>
>Les connexions appartiennent à des équipes. Si vous ne trouvez pas la connexion que vous recherchez, vérifiez que vous consultez l’équipe appropriée.
>
>Pour sélectionner une nouvelle équipe :
>
>* Cliquez sur le nom de l’équipe dans le volet de navigation de gauche, puis sélectionnez une nouvelle équipe.
>
>    Ou
>
>* Cliquez sur Aperçu de l’équipe dans le volet de navigation de gauche, puis cliquez sur la flèche déroulante en regard du nom de l’équipe près du haut de la page. Sélectionnez une nouvelle équipe.

1. Pour ouvrir la zone [!UICONTROL Connexions], cliquez sur <b>[!UICONTROL Connexions]</b> dans le volet de navigation de gauche.
1. (Facultatif) Indiquez l’environnement et le type de connexion en cliquant sur la liste déroulante Environnement et Type et en sélectionnant une option.
1. (Facultatif) Pour afficher les autorisations accordées à [!DNL Workfront Fusion] pour une connexion, cliquez sur l’icône Afficher ![Afficher les autorisations de connexion](assets/view-connection-permissions.png) pour cette connexion.
1. (Facultatif) Pour renommer une connexion, mettez en surbrillance son nom et saisissez le nouveau nom.
1. (Facultatif) Pour réautoriser une connexion, cliquez sur **Réautoriser** pour cette connexion.
1. (Facultatif) Pour supprimer une connexion, cliquez sur **Supprimer** pour cette connexion.
1. (Facultatif) Pour vérifier que la connexion au service a bien été établie, cliquez sur **Vérifier** pour la connexion.



## Renouveler une connexion

[!DNL Workfront Fusion] obtient généralement des droits d’accès à un service donné pendant une période illimitée. Certaines applications exigent que l’autorisation d’accès soit renouvelée après un certain temps. Dans ce cas, [!DNL Workfront Fusion] vous avertit par e-mail peu de temps avant l’expiration de ses droits d’accès.

Pour renouveler une connexion :

1. Cliquez sur le bouton **[!UICONTROL Réautoriser]** dans la zone **[!UICONTROL Connexions]** .
