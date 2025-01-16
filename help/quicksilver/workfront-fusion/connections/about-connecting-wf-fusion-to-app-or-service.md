---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Vue d’ensemble des connexions
description: La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement. Cet article est obsolète, mais contient un lien vers le nouvel article qui couvre cette fonctionnalité.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 88%

---

# Vue d’ensemble des connexions

>[!IMPORTANT]
>
>La documentation d’Adobe Workfront Fusion a été déplacée vers un nouvel emplacement.
>
>Les informations contenues dans cet article se trouvent désormais dans les articles suivants :
>
>* [Présentation de la connexion](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/connection-overview.html)
>* [Gérer les connexions](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/manage-connections.html)
>
>Mettez à jour les signets.
>
>Cet article n’est plus mis à jour et sera supprimé prochainement.

<!-- Audited: 3/2024-->

Pour la plupart des applications, [!DNL Workfront Fusion] nécessite une connexion, avec laquelle il peut communiquer avec le service tiers donné en fonction des paramètres du scénario.

Par exemple, si vous souhaitez créer un scénario qui récupère des informations de [!DNL Workfront], vous devez accorder l’autorisation d’accès à [!DNL Workfront Fusion] pour accéder à votre compte [!DNL Workfront].

Une connexion représente l’autorisation et les droits utilisés par Fusion pour accéder à l’application. Vous pouvez créer une ou plusieurs connexions pour chaque application et utiliser la même connexion dans plusieurs modules ou scénarios.

La plupart des connexions ne sont utilisées que pour une seule application. Par exemple, une connexion  ne peut pas être utilisée dans un module Salesforce. [!DNL Workfront] Certaines applications  peuvent partager des connexions. [!DNL Adobe] Pour plus de détails, consultez les articles relatifs à ces applications, répertoriés dans [Applications et leurs modules](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

Les connexions sont gérées au niveau de l’équipe. Tous les membres d’une équipe ont accès aux connexions de l’équipe et les utilisateurs et utilisatrices en dehors d’une équipe n’ont pas accès aux connexions de l’équipe.

## Conditions d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p><p>Ou</p><p>Actuelle : [!UICONTROL Work] ou niveau supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Actuelle : aucune exigence de licence [!DNL Workfront Fusion] requise.</p>
   <p>Ou</p>
   <p>Héritée : n’importe laquelle. </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Nouveau :</p> <ul><li>Forfait [!DNL Workfront] [!UICONTROL Select] ou [!UICONTROL Prime] : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</li><li>Forfait [!DNL Workfront] [!UICONTROL Ultimate] : [!DNL Workfront Fusion] est inclus.</li></ul>
   <p>Ou</p>
   <p>Actuel : votre entreprise doit acheter [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Droits d’accès

Pour chaque connexion,  ne nécessite que les droits d’accès nécessaires au déroulement du scénario concerné. [!DNL Workfront Fusion] Par exemple, si vous créez un scénario pour répertorier des documents à partir de ,  ne demande pas l’autorisation d’obtenir le contenu des documents. [!DNL Google Docs][!DNL Workfront Fusion] Par la suite, si vous constatez que vous devez accéder au contenu des documents, vous pouvez mettre à jour la connexion ou en créer une qui puisse accéder à ce contenu.

Tous les services ne vous permettent pas de limiter l’accès à des tâches spécifiques. Dans ces cas,  doit exiger des droits d’accès complets. [!DNL Workfront Fusion] Pour plus d’informations sur la manière de limiter l’accès de [!DNL Workfront Fusion] à votre compte enregistré pour ces services, consultez la documentation spécifique à l’application répertoriée dans [Applications et leurs modules](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Gérer les connexions

Vous pouvez gérer toutes les connexions à partir de la zone [!UICONTROL Connexions].

>[!NOTE]
>
>Les connexions appartiennent à des équipes. Si vous ne trouvez pas la connexion que vous recherchez, vérifiez que vous consultez l’équipe appropriée.
>
>Pour sélectionner une nouvelle équipe :
>
>* Cliquez sur le nom de l’équipe dans le panneau de navigation de gauche, puis sélectionnez une nouvelle équipe.
>
>    Ou
>
>* Cliquez sur Vue d’ensemble de l’équipe dans le panneau de navigation de gauche, puis sur la flèche déroulante en regard du nom de l’équipe près du haut de la page. Sélectionnez une nouvelle équipe.

1. Pour ouvrir la zone [!UICONTROL Connexions], cliquez sur <b>[!UICONTROL Connexions]</b> dans le panneau de navigation de gauche.
1. (Facultatif) Indiquez l’environnement et le type de connexion en cliquant sur les listes déroulantes Environnement et Type et en sélectionnant une option.
1. (Facultatif) Pour afficher les autorisations accordées à [!DNL Workfront Fusion] pour une connexion, cliquez sur l’icône Afficher ![Afficher les autorisations de connexion](assets/view-connection-permissions.png) de cette connexion.
1. (Facultatif) Pour renommer une connexion, mettez en surbrillance son nom et saisissez le nouveau nom.
1. (Facultatif) Pour réautoriser une connexion, cliquez sur **Réautoriser** pour cette connexion.
1. (Facultatif) Pour supprimer une connexion, cliquez sur **Supprimer** pour cette connexion.
1. (Facultatif) Pour vérifier que la connexion au service a bien été établie, cliquez sur **Vérifier** pour la connexion.



## Renouveler une connexion

[!DNL Workfront Fusion] obtient généralement des droits d’accès à un service donné pendant une période illimitée. Certaines applications exigent que l’autorisation d’accès soit renouvelée après un certain temps. Dans ce cas, [!DNL Workfront Fusion] vous avertit par e-mail peu de temps avant l’expiration de ses droits d’accès.

Pour renouveler une connexion :

1. Cliquez sur le bouton **[!UICONTROL Réautoriser]** dans la zone **[!UICONTROL Connexions]**.
