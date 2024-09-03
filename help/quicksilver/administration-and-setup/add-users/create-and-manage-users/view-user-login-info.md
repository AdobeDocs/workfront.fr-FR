---
title: Affichage des informations de connexion de l’utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez déterminer la fréquence à laquelle les utilisateurs et utilisatrices se connectent à Workfront, ainsi que leur dernière connexion, en indiquant que vous souhaitez inclure ces informations dans la vue d’une liste d’utilisateurs et d’utilisatrices ou dans un rapport destiné aux utilisateurs et utilisatrices.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 99%

---

# Afficher les informations de connexion de l’utilisateur ou de l’utilisatrice

Vous pouvez déterminer la fréquence à laquelle les utilisateurs et utilisatrices se connectent à Adobe Workfront, ainsi que leur dernière connexion, en indiquant que vous souhaitez inclure ces informations dans la vue d’une liste d’utilisateurs et d’utilisatrices ou dans un rapport destiné aux utilisateurs et utilisatrices.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès Administrateur ou administratrice système. Pour plus d’informations, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès d’administration complet à un utilisateur ou une utilisatrice</a>. </p> </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Parmi ces deux options, si l’option <b>Administratrion des utilisateurs et utilisatrices (utilisateurs et utilisatrices du groupe)</b> est activée, vous devez être administrateur ou administratrice de groupes d’un groupe dont l’utilisateur ou l’utilisatrice est membre.</p> <p>Pour plus d’informations sur le paramètre <b>Utilisateurs et utilisatrices</b> d’un niveau d’accès, consultez <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Octroyer un accès aux utilisateurs et utilisatrices</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Enregistrement des informations de connexion par Workfront

Workfront enregistre les informations suivantes sur les utilisateurs et utilisatrices qui se connectent au système :

* **Nombre de connexions** : Workfront comptabilise un utilisateur ou une utilisatrice qui se connecte à l’application une fois toutes les 24 heures. Si un utilisateur ou une utilisatrice se connecte plusieurs fois à l’aide de différents navigateurs, ordinateurs ou appareils mobiles, Workfront comptabilise toutes les connexions effectuées au cours d’une journée comme une seule connexion. Le nombre de connexions contient des informations dont la date de création de l’utilisateur ou de l’utilisatrice.
* **Date de dernière connexion** : dernière date à laquelle une personne s’est connectée. La date de chaque connexion à partir d’un navigateur, d’un appareil mobile ou d’une autre application est enregistrée dans ce champ.

Se connecter à Workfront de l’une des façons suivantes compte comme une connexion à Workfront :

* Application web Workfront
* Applications mobiles Workfront (appareils iOS ou Android)
* Toute intégration Workfront prise en charge avec une autre application tierce (Slack, Jira)
* Toute intégration personnalisée entre Workfront et une autre application tierce
* API Workfront

  >[!NOTE]
  >
  >La connexion à Workfront par le biais de l’API Workfront est disponible uniquement pour les organisations qui ne sont pas encore intégrées à Adobe Business Platform.

## Afficher les informations d’utilisation dans une liste d’utilisateurs et d’utilisatrices ou un rapport

Vous pouvez afficher le nombre de connexions et les champs Date de dernière connexion dans la vue d’une liste d’utilisateurs et d’utilisatrices ou dans un rapport destiné aux utilisateurs et utilisatrices.\
Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour afficher les informations d’utilisation dans la vue d’une liste d’utilisateurs et d’utilisatrices, procédez comme suit :

1. Accédez à une liste d’utilisateurs et d’utilisatrices dans Workfront.
1. Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne** près du coin inférieur droit de l’écran.
1. Dans le champ **Afficher dans cette colonne**, commencez à saisir **Nombre de connexions**, puis sélectionnez-le lorsqu’il apparaît dans la liste sous **Utilisateur ou utilisatrice**.

1. Cliquez sur **Ajouter une colonne** encore une fois.
1. Dans le champ **Afficher dans la colonne**, commencez à saisir **Dernière date de connexion**, puis sélectionnez-la lorsqu’elle apparaît dans la liste sous **Utilisateur ou utilisatrice**.

1. (Facultatif) Cliquez sur **Options avancées**, puis sélectionnez un **format du champ** dans le menu déroulant pour inclure l’heure ou le jour de la semaine de la dernière connexion dans votre colonne.

1. Cliquez sur **Enregistrer la vue**.\
   La vue inclut des informations relatives au nombre de fois où les utilisateurs et utilisatrices se sont connectés et à la date de leur dernière connexion.
