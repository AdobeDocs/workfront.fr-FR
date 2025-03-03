---
title: Afficher les informations de connexion de l’utilisateur
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Vous pouvez déterminer la fréquence à laquelle les utilisateurs et utilisatrices se connectent à Workfront, ainsi que leur dernière connexion, en indiquant que vous souhaitez inclure ces informations dans la vue d’une liste d’utilisateurs et d’utilisatrices ou dans un rapport destiné aux utilisateurs et utilisatrices.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 93%

---

# Afficher les informations de connexion de l’utilisateur ou de l’utilisatrice

Vous pouvez déterminer la fréquence à laquelle les utilisateurs et utilisatrices se connectent à Adobe Workfront, ainsi que leur dernière connexion, en indiquant que vous souhaitez inclure ces informations dans la vue d’une liste d’utilisateurs et d’utilisatrices ou dans un rapport destiné aux utilisateurs et utilisatrices.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

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
   <td><p>Nouveau : Standard</p><p>Ou</p><p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez disposer de l’une des autorisations suivantes :</p> 
    <ul> 
     <li> <p>Niveau d’accès de l’administrateur système. </li> 
     <li> <p>Le paramètre <b>Utilisateurs et utilisatrices</b> de votre niveau d’accès doit être configuré sur l’accès <b>Modifier</b>, avec l’option <b>Créer</b> et au moins l’une des deux options d’<b>Administration des utilisateurs et utilisatrices</b> activées dans <b>Ajuster vos paramètres</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De ces deux options, si l’option <b>Administration des utilisateurs (utilisateurs du groupe)</b> est activée, vous devez être un administrateur de groupe d’un groupe dont l’utilisateur est membre.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
