---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Créer une épreuve de plusieurs pages
description: Vous pouvez combiner plusieurs fichiers en une seule épreuve de plusieurs pages. Les personnes chargées de la révision peuvent utiliser les outils de navigation de la visionneuse de relecture pour parcourir les pages d’une épreuve de plusieurs pages.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 98%

---

# Créer une épreuve de plusieurs pages

Vous pouvez combiner plusieurs fichiers en une seule épreuve de plusieurs pages. Les personnes chargées de la révision peuvent utiliser les outils de navigation de la visionneuse de relecture pour parcourir les pages d’une épreuve de plusieurs pages.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
    <p>Travail ou plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une épreuve de plusieurs pages

Lorsque cette option est activée, les fichiers statiques et les sites web sont disponibles dans une seule épreuve. Lorsque cette option est désactivée, tous les documents et sites web sont générés en tant qu’épreuves individuelles et vous pouvez charger jusqu’à 100 fichiers à la fois.

Pour créer un BAT multi-pages :

1. Accédez au projet, à la tâche ou au problème pour lequel vous souhaitez créer une épreuve, puis cliquez sur la section **Documents**.
1. Cliquez sur **Ajouter** > **Épreuve**.
1. Faites glisser et déposez les fichiers ou parcourez et sélectionnez-les dans votre explorateur de fichiers. Vous pouvez exporter jusqu’à 50 fichiers à la fois. Pour plus d’informations sur les limites de fichiers, voir la section [Remarques](#considerations) de cet article.

   >[!NOTE]
   >
   >Les fichiers interactifs, y compris les vidéos et les sites web interactifs, ne peuvent pas être combinés en une seule épreuve.

1. Sous **Épreuve unique**, activez l’option **Combiner tous les fichiers compatibles en une seule épreuve**.
1. Dans le champ **Nom de l’épreuve**, entrez un nouveau nom pour l’épreuve combinée.
1. (Facultatif) Dans la liste des fichiers que vous avez chargés, réorganisez les fichiers en les faisant glisser. L’ordre des fichiers est l’ordre des pages de l’épreuve combinée.
1. (Facultatif) Pour supprimer un seul fichier de la page Nouvelle épreuve, placez la souris sur le fichier et cliquez sur l’icône **Corbeille** qui apparaît à droite.

   Ou

   Pour supprimer tous les fichiers chargés en une seule fois, cliquez sur **Supprimer tout** dans le coin supérieur droit de la liste.

1. Une fois tous vos fichiers chargés, vous devez décider si vous souhaitez configurer une épreuve de base ou automatisée :

   * Avec une épreuve de base, vous pouvez ajouter autant d’approbateurs et d’approbatrices que vous le souhaitez à une épreuve, mais sans organisation en étapes. Toutes les personnes chargées de la révision que vous ajoutez peuvent accéder à l’épreuve dès que vous l’avez créée. Pour configurer une épreuve de base, voir [Créer une épreuve avancée avec un workflow de base](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Dans le cas d’une épreuve automatisée, l’épreuve passe d’une étape à l’autre et Adobe Workfront avertit chaque personne lorsqu’elle doit la réviser à son tour. Pour configurer une épreuve automatisée, voir [Créer une épreuve avancée avec un workflow automatisé](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Considérations {#considerations}

Tenez compte des points suivants lorsque vous combinez des fichiers en une seule épreuve :

* Vous pouvez charger jusqu’à 500 fichiers distincts.
* Vous pouvez combiner des fichiers statiques de différents types (par exemple, PDF, JPG, DOC, PPT, EXC), jusqu’à un total de 2 000 pages.
* Vous pouvez combiner des captures web statiques.
* Vous pouvez combiner des fichiers GIF ; toutefois, les GIF animés sont traités comme des fichiers statiques.
* Vous ne pouvez pas combiner des fichiers AV et des captures web interactives.
* L’image miniature de l’épreuve est extraite de la première page de l’épreuve (voir [Gérer les détails de l’épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Vous pouvez consulter les noms des fichiers qui ont été combinés pour créer l’épreuve sur la page Détails de l’épreuve. Pour plus d’informations, voir [Gérer les détails de l’épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Si l’option de téléchargement des fichiers originaux est activée sur l’épreuve, vous pouvez télécharger tous les fichiers qui ont été combinés pour créer l’épreuve au format .zip. Pour plus d’informations, voir [Télécharger les fichiers stockés dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
