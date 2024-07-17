---
product-area: projects
navigation-topic: financials
title: Définir la méthode de l’indice de performance (PIM)
description: La méthode d’index de performance (PIM) du projet contrôle la méthode utilisée par Adobe Workfront pour calculer les mesures de performances du projet, telles que l’indice de performance des coûts (IPC), l’indice de performance de la planification des coûts (CSI), l’indice de performance de la planification (SPI) et l’estimation à la fin de la période d’exécution (EAC).
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 23%

---

# Définir la méthode de l’indice de performance (PIM)

La méthode d’index de performance (PIM) du projet contrôle la méthode utilisée par Adobe Workfront pour calculer les mesures de performances du projet, telles que l’indice de performance des coûts (IPC), l’indice de performance de la planification des coûts (CSI), l’indice de performance de la planification (SPI) et l’estimation à la fin de la période d’exécution (EAC).

Workfront calcule ces valeurs à l’aide des éléments suivants :

* Heures
* Coûts

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets et aux données financières</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations du projet avec les autorisations de gestion financière</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Considérations relatives à PIM dans Workfront

* Votre administrateur Workfront ou un administrateur de groupe configure par défaut la méthode d’index de performance (PIM) en fonction des heures ou des coûts. Les calculs des mesures de performances changent en fonction de la définition de cette valeur par défaut. Pour plus d’informations sur la façon de modifier la valeur par défaut pour calculer le PIM, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Les chefs de projet peuvent également modifier le paramètre de PIM, au niveau du projet, pour les projets individuels dans le sous-onglet Finance du projet. Pour modifier le sous-onglet Finance du projet, vous devez disposer des autorisations de gestion du projet.

## Définition de la méthode d’index de performance (PIM) pour un projet

1. Accédez à un projet dont vous êtes le propriétaire.

   >[!IMPORTANT]
   >
   >Pour effectuer les étapes suivantes, vous devez gérer les autorisations du projet. Nous recommandons également que seul le propriétaire du projet modifie la zone Finance du projet.

1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis accédez à la zone **Finance**.
1. Double-cliquez sur la valeur dans le champ **Méthode d’index de performance** pour la modifier.
1. Sélectionnez l’une des options suivantes dans le champ **Méthode d’index de performance** :

   | Basé sur les heures | Workfront utilise les heures prévues pour calculer l’IPC et le CAE du projet, et le CAE du projet s’affiche sous forme de nombre, en heures. |
   |---|---|
   | Basé sur les coûts | Workfront utilise le coût du travail planifié dans le calcul de l’IPC et du CAE du projet, et le CAE s’affiche sous forme de valeur monétaire. Lorsque vous sélectionnez cette option, assurez-vous que les personnes désignées pour les tâches (rôles de tâche ou utilisateurs) sont associées aux taux de coût. |

   {style="table-layout:auto"}

1. Cliquez sur **Enregistrer** **Modifications**.
