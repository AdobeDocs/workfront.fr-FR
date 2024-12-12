---
product-area: projects
navigation-topic: financials
title: Définir la méthode de l’indice de performance (PIM)
description: La méthode d’indice de performances (PIM) du projet contrôle la méthode utilisée par Adobe Workfront pour calculer les mesures de performances du projet, telles que l’Indice Coûts Performances (ICP), l’Indice Coûts Horaire Performances (CSI), l’Indice Horaire Performances (SPI) et l’estimation à l’achèvement (EAC).
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 100%

---

# Définir la méthode de l’indice de performance (PIM)

La méthode d’indice de performances (PIM) du projet contrôle la méthode utilisée par Adobe Workfront pour calculer les mesures de performances du projet, telles que l’Indice Coûts Performances (ICP), l’Indice Coûts Horaire Performances (CSI), l’Indice Horaire Performances (SPI) et l’estimation à l’achèvement (EAC).

Workfront calcule ces valeurs à l’aide des éléments suivants :

* Heures
* Coûts

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
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Accès en modification aux projets et aux données financières</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Autorisations de gestion pour le projet avec les autorisations de gestion financière</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considérations relatives à la PIM dans Workfront

* Votre administrateur ou administratrice Workfront ou un administrateur ou une administratrice de groupes configure par défaut la méthode d’indice de performances (PIM) en fonction des heures ou des coûts. Les calculs des mesures de performances changent en fonction de la définition de cette valeur par défaut. Pour plus d’informations sur la modification de la valeur par défaut pour le calcul de la PIM, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Les personnes responsables des projets peuvent également modifier le paramètre de la PIM, au niveau du projet, pour les projets individuels dans le sous-onglet Finances du projet. Pour modifier le sous-onglet Finances du projet, vous devez disposer d’autorisations de gestion sur le projet.

## Définir la méthode d’indice de performances (PIM) d’un projet

1. Accédez à un projet dont vous êtes la personne propriétaire.

   >[!IMPORTANT]
   >
   >Pour effectuer les étapes suivantes, vous devez disposer des autorisations de gestion sur le projet. Nous recommandons également que seule la personne propriétaire du projet modifie la zone Finances du projet.

1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis accédez à la zone **Finances**.
1. Double-cliquez sur la valeur dans le champ **Méthode d’indice de performances** pour la modifier.
1. Sélectionnez l’une des options suivantes dans le champ **Méthode d’indice de performances** :

   | Basé sur les heures | Workfront utilise le nombre d’heures prévues pour calculer l’ICP et l’EAC du projet, et l’EAC du projet s’affiche sous forme d’un nombre, en heures. |
   |---|---|
   | Basé sur les coûts | Workfront utilise le coût prévu de main d’œuvre dans le calcul de l’ICP et de l’EAC du projet, et l’EAC s’affiche sous forme de valeur monétaire. Lorsque vous sélectionnez cette option, assurez-vous que les personnes assignées à la tâche (fonctions ou utilisateurs et utilisatrices) sont associées aux taux de coûts. |

   {style="table-layout:auto"}

1. Cliquez sur **Enregistrer** **les modifications**.
