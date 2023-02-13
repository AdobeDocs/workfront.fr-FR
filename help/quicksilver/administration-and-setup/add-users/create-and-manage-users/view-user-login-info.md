---
title: Affichage des informations de connexion de l’utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez déterminer la fréquence à laquelle les utilisateurs se connectent à Workfront, ainsi que la dernière fois où ils se sont connectés, en indiquant que vous souhaitez inclure ces informations dans la vue d’une liste d’utilisateurs ou dans un rapport destiné aux utilisateurs.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Affichage des informations de connexion de l’utilisateur

Vous pouvez déterminer la fréquence à laquelle les utilisateurs se connectent à Adobe Workfront, ainsi que la dernière fois qu’ils se sont connectés, en indiquant que vous souhaitez inclure ces informations dans la vue d’une liste d’utilisateurs ou dans un rapport destiné aux utilisateurs.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez disposer de l’une des options suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur système. Pour plus d’informations, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>. </p> </li> 
     <li> <p><b>Utilisateurs</b> paramètre de votre niveau d’accès configuré sur <b>Modifier</b> accès, avec <b>Créer</b> et au moins l’une des deux <b>Administration des utilisateurs</b> options activées sous <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>de ces deux options, si Utilisateur <b>Administration (utilisateurs de groupe)</b> est activé, vous devez être administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> <p>Pour plus d’informations sur la variable <b>Utilisateurs</b> paramétrer un niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Accorder l’accès aux utilisateurs</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Comment Workfront enregistre les informations de connexion

Workfront enregistre les informations suivantes sur les utilisateurs qui se connectent au système :

* **Nombre de connexions**: Workfront comptabilise un utilisateur qui se connecte à l’application une fois toutes les 24 heures. Si un utilisateur se connecte plusieurs fois à l’aide de différents navigateurs, ordinateurs ou appareils mobiles, Workfront comptabilise toutes les connexions qui se sont produites au cours d’une journée comme une seule connexion. Le nombre de connexions contient des informations commençant par la date de création de l’utilisateur.
* **Date de dernière connexion**: Dernière date à laquelle un utilisateur s’est connecté. La date de chaque connexion à partir d’un navigateur, d’un périphérique mobile ou d’une autre application est enregistrée dans ce champ.

La connexion à Workfront de l’une des façons suivantes compte comme une connexion à Workfront :

* Application Web Workfront
* Les applications mobiles Workfront (appareils iOS ou Android)
* Toute intégration Workfront prise en charge avec une autre application tierce (Slack, Jira)
* Toute intégration personnalisée entre Workfront et une autre application tierce.
* API Workfront

   >[!NOTE]
   >
   >La connexion à Workfront par le biais de l’API Workfront est disponible uniquement pour les organisations qui ne sont pas encore intégrées à Adobe Business Platform.

## Affichage des informations d’utilisation dans une liste d’utilisateurs ou un rapport

Vous pouvez afficher le nombre de connexions et les champs Date de dernière connexion dans la vue d’une liste d’utilisateurs ou dans un rapport pour les utilisateurs.\
Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour afficher les informations d’utilisation dans la vue d’une liste d’utilisateurs :

1. Accédez à une liste d’utilisateurs dans Workfront.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** près du coin inférieur droit de l’écran.
1. Dans le **Afficher dans cette colonne** champ, commencer à saisir **Nombre de connexions**, puis sélectionnez-le lorsqu’il apparaît dans la liste sous **Utilisateur**.

1. Cliquez sur **Ajouter une colonne** encore une fois.
1. Dans le **Afficher dans la colonne** champ, commencer à saisir **Date de dernière connexion**, puis sélectionnez-le lorsqu’il apparaît dans la liste sous **Utilisateur**.

1. (Facultatif) Cliquez sur **Options avancées**, puis sélectionnez une **Format du champ** dans le menu déroulant pour inclure l’heure ou le jour de la semaine de la dernière connexion dans votre colonne.

1. Cliquez sur **Enregistrer la vue**.\
   La vue inclut des informations sur le nombre de fois où les utilisateurs se sont connectés et le dernier moment où ils se sont connectés.
