---
title: Affichage des informations de connexion de l’utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez déterminer la fréquence à laquelle les utilisateurs se connectent à Workfront, ainsi que la dernière fois où ils se sont connectés, en indiquant que vous souhaitez inclure ces informations dans la vue d’une liste d’utilisateurs ou dans un rapport destiné aux utilisateurs.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 21%

---

# Afficher les informations de connexion de l’utilisateur ou de l’utilisatrice

Vous pouvez déterminer la fréquence à laquelle les utilisateurs se connectent à Adobe Workfront, ainsi que la dernière fois qu’ils se sont connectés, en indiquant que vous souhaitez inclure ces informations dans la vue d’une liste d’utilisateurs ou dans un rapport destiné aux utilisateurs.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur ou administratrice système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder l’accès administratif complet à un utilisateur ou une utilisatrice</a>. </p> </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Parmi ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être administrateur ou administratrice d’un groupe dont l’utilisateur est membre.</p> <p>Pour plus d’informations sur le paramètre <b>Utilisateurs et utilisatrices</b> dans un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs et utilisatrices</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Comment Workfront enregistre les informations de connexion

Workfront enregistre les informations suivantes sur les utilisateurs qui se connectent au système :

* **Nombre de connexions** : Workfront comptabilise un utilisateur qui se connecte à l’application une fois toutes les 24 heures. Si un utilisateur se connecte plusieurs fois à l’aide de différents navigateurs, ordinateurs ou appareils mobiles, Workfront comptabilise toutes les connexions qui se sont produites au cours d’une journée comme une seule connexion. Le nombre de connexions contient des informations commençant par la date de création de l’utilisateur.
* **Date de dernière connexion** : dernière date à laquelle un utilisateur s’est connecté. La date de chaque connexion à partir d’un navigateur, d’un périphérique mobile ou d’une autre application est enregistrée dans ce champ.

La connexion à Workfront de l’une des façons suivantes compte comme une connexion à Workfront :

* Application Web Workfront
* Les applications mobiles Workfront (appareils iOS ou Android)
* Toute intégration Workfront prise en charge avec une autre application tierce (Slack, Jira)
* Toute intégration personnalisée entre Workfront et une autre application tierce.
* API WORKFRONT

  >[!NOTE]
  >
  >La connexion à Workfront par le biais de l’API Workfront est disponible uniquement pour les organisations qui ne sont pas encore intégrées à Adobe Business Platform.

## Affichage des informations d’utilisation dans une liste d’utilisateurs ou un rapport

Vous pouvez afficher le nombre de connexions et les champs Date de dernière connexion dans la vue d’une liste d’utilisateurs ou dans un rapport pour les utilisateurs.\
Pour plus d&#39;informations sur la création d&#39;un rapport, voir [Création d&#39;un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour afficher les informations d’utilisation dans la vue d’une liste d’utilisateurs :

1. Accédez à une liste d’utilisateurs dans Workfront.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Cliquez sur **Ajouter la colonne** près du coin inférieur droit de l’écran.
1. Dans le champ **Afficher dans cette colonne**, commencez à saisir **Nombre de connexions**, puis sélectionnez-le lorsqu’il apparaît dans la liste sous **Utilisateur**.

1. Cliquez sur **Ajouter une colonne** encore une fois.
1. Dans le champ **Afficher dans la colonne**, commencez à saisir **Date de dernière connexion**, puis sélectionnez-le lorsqu’il apparaît dans la liste sous **Utilisateur**.

1. (Facultatif) Cliquez sur **Options avancées**, puis sélectionnez un **format de champ** dans le menu déroulant pour inclure l’heure ou le jour de la semaine de la dernière connexion dans votre colonne.

1. Cliquez sur **Enregistrer la vue**.\
   La vue inclut des informations sur le nombre de fois où les utilisateurs se sont connectés et le dernier moment où ils se sont connectés.
