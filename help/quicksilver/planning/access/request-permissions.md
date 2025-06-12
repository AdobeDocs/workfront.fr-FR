---
title: Demande d’autorisations pour une vue ou un Workspace
description: Lorsqu’une personne partage un lien vers une vue ou un espace de travail auquel vous n’avez pas accès, vous pouvez demander des autorisations pour pouvoir l’ouvrir. Cet article explique les étapes à suivre pour demander l’accès à une vue ou à un espace de travail lorsque vous rencontrez un lien partagé que vous ne pouvez pas ouvrir.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 14%

---

# Demander des autorisations pour une vue ou un espace de travail

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

>[!IMPORTANT]
>
>La fonctionnalité décrite dans cet article n’est disponible que lorsque votre organisation a intégré l’expérience unifiée Adobe.
>
>Pour plus d’informations, voir [Adobe Unified Experience pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


Vous pouvez demander des autorisations pour une vue ou un espace de travail lorsqu&#39;une personne partage un lien avec vous vers la vue ou l&#39;espace de travail auquel vous n&#39;avez pas accès.

Demander des autorisations pour une vue est similaire à demander des autorisations pour un espace de travail.

Cet article décrit comment demander l’accès à une vue ou à un espace de travail lorsqu’une personne partage un lien avec vous et que vous ne pouvez pas accéder à la page partagée.

Pour plus d’informations sur l’octroi d’autorisations aux vues et aux espaces de travail, consultez les articles suivants :

* [Partager des affichages](/help/quicksilver/planning/access/share-views.md)
* [Partager des espaces de travail](/help/quicksilver/planning/access/share-workspaces.md)


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produits</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planification d’Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Formule Adobe Workfront*</p></td> 
   <td> 
<p>L’un des plans Workfront suivants :</p> 
<ul><li>Sélectionner</li> 
<li>Principal</li> 
<li>Final</li></ul> 
<p>Workfront Planning n’est pas disponible pour les plans Workfront hérités</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront Planning*</p></td> 
   <td> 
<p>Tous </p> 
<p>Pour plus d’informations sur les éléments inclus dans chaque plan de planification Workfront, contactez votre gestionnaire de compte Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Plateforme Adobe Workfront</p></td> 
   <td> 
<p>L’instance de Workfront de votre organisation doit être intégrée à l’expérience unifiée Adobe pour pouvoir accéder à Workfront Planning.</p> 
<p><b>IMPORTANT</b></p>
<p>Les utilisateurs de votre organisation peuvent demander des autorisations pour les vues et les espaces de travail uniquement lorsque votre organisation a intégré l’expérience unifiée Adobe. </p>
<p>Pour plus d’informations, voir <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience pour Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront*</p></td> 
   <td><p> Standard, Léger ou Contributeur</p>
   <p>Workfront Planning n’est pas disponible pour les licences Workfront héritées</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuration du niveau d’accès</p></td> 
   <td> <p>Il n’existe aucun contrôle de niveau d’accès pour Adobe Workfront Planning.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>  <p>Une fois votre demande d’autorisation accordée, vous pouvez obtenir les autorisations suivantes :</p>
   <ul><li><p>Affichage ou gestion d’une vue</p></li>
   <li><p>Affichage, contribution ou gestion d’un espace de travail</p></li></ul>  
   <p>Seuls les utilisateurs disposant d’autorisations de niveau Gérer pour un espace de travail et une vue peuvent partager une vue publiquement.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modèle de mise en page</p></td> 
   <td> 
   <p>Dans l’environnement de production, tous les utilisateurs, y compris les administrateurs système, doivent être affectés à un modèle de mise en page qui inclut les zones Planning.</p>
   <div class="preview">
<p> Dans l’environnement de Prévisualisation, les utilisateurs disposant d’une licence Light ou Contributor doivent se voir attribuer un modèle de mise en page qui inclut l’option Planification dans les domaines suivants :</p>
   <ul><li>Menu principal</li>
   <li>Panneau de gauche de projets, portefeuilles et programmes</li>
   </ul>
   <p>Pour plus d’informations, voir <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Créer et gérer des modèles de disposition</a>.</p>
   <p>Les zones Planning sont activées par défaut pour les utilisateurs standard et les administrateurs système.</p></div>
   </td> 
  </tr> 
</tbody> 
</table>

* Pour plus d’informations sur les exigences d’accès à Workfront, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Demander des autorisations pour une vue ou un espace de travail

Demander des autorisations pour une vue est similaire à demander une autorisation pour un espace de travail.

Lorsqu&#39;une personne partage avec vous un lien vers un espace de travail ou une vue auquel vous n&#39;avez pas accès :

1. Cliquez sur le lien partagé avec vous pour la vue ou l&#39;espace de travail.

   Une page **Vous n’avez pas accès** s’affiche pour vous informer que vous n’avez pas accès à la vue ou à l’espace de travail.

   ![Demander l’accès à la vue](assets/request-access-to-view.png)

1. (Conditionnel) Si le lien partagé correspond à une vue de l&#39;espace de travail auquel vous avez accès, cliquez sur **Ouvrir avec la vue existante**. Si vous disposez des autorisations nécessaires pour accéder à l’espace de travail, la page de type d’enregistrement s’ouvre dans la vue par défaut.

1. (Facultatif et conditionnel) Si vous ne disposez pas des autorisations nécessaires pour afficher l’espace de travail, ajoutez un message personnalisé dans la zone disponible, puis cliquez sur **Demander l’accès**.

   Tous les utilisateurs disposant d’autorisations de niveau Gérer pour l’affichage ou l’espace de travail reçoivent les notifications suivantes pour la demande d’accès :
   * Une notification in-app
     ![Notification in-app pour la demande d’accès](assets/in-app-notification-for-access-request.png)
   * Notification par e-mail
     ![Notification électronique pour la demande d’accès](assets/email-notification-for-access-request.png)

1. (Conditionnel) Lorsque le gestionnaire de l’affichage ou de l’espace de travail vous accorde des autorisations pour l’affichage ou l’espace de travail, vous recevez une notification par e-mail et une notification in-app avec une confirmation que l’autorisation a été accordée. <!--check this - I was not able to test this, but Isk confirmed.-->
