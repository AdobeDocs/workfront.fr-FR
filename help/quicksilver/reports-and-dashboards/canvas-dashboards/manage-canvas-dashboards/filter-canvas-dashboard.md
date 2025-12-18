---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrer un tableau de bord de zone de travail
description: Vous pouvez appliquer un filtre à un tableau de bord de la zone de travail après sa création.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 156e9d3f-49f6-4372-9749-c7124ff5baee
source-git-commit: 39a8d670baa19aa37e29b0312e6c9a296569f44c
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 10%

---

# Filtrer un tableau de bord de zone de travail

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elles sont disponibles uniquement dans l’environnement de prévisualisation pour les clientes et les clients.</span>

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, voir [Contacter le service clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform


Vous pouvez appliquer un filtre à un tableau de bord Zone de travail qui contient des invites. Une invite fonctionne comme un modificateur de filtre qui applique des critères de filtrage supplémentaires afin que vous puissiez réduire encore davantage vos résultats. Ces invites peuvent être modifiées à chaque application du filtre, ce qui permet d&#39;ajuster les résultats affichés sans avoir à modifier les principaux critères de filtre du tableau de bord ou de chaque rapport.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tous </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td><p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td><p>Gestion des autorisations relatives au tableau de bord</p>
  </td> 
  </tr> 
</tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

Vous devez créer un tableau de bord avant de pouvoir le filtrer.

Pour plus d’informations, voir [Créer un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Filtrer un tableau de bord

Pour filtrer un tableau de bord, procédez comme suit dans l’ordre indiqué :

* [Partie 1 : création d’un filtre de tableau de bord](#part-1-create-a-dashboard-filter)
* [Partie 2 : créer une invite de tableau de bord](#part-2-define-a-dashboard-prompt)
* [Partie 3 : appliquer une invite de tableau de bord](#step-3-apply-a-dashboard-prompt)

>[!NOTE]
>
>Le filtre de tableau de bord s’applique à tous les rapports pour lesquels les filtres au niveau du tableau de bord ne sont pas désactivés.  Vous pouvez exclure des rapports individuels de l’application des filtres au niveau du tableau de bord en développant le menu d’actions pour chaque rapport et en sélectionnant l’option **Désactiver les filtres**.


### Partie 1 : création d’un filtre de tableau de bord

Un filtre de tableau de bord permet d’appliquer un filtre commun à tous les rapports disponibles sur un tableau de bord sans avoir à modifier les filtres de chaque rapport individuel.

>[!NOTE]
>
>Ces filtres ne peuvent être configurés que par un utilisateur disposant d’un accès de niveau Gérer au tableau de bord.


{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Sur la page **Tableaux de bord de la zone de travail**, sélectionnez le tableau de bord auquel vous souhaitez appliquer un filtre.

1. Dans le coin supérieur gauche de la page des détails du tableau de bord, cliquez sur **Filtres**. Le panneau latéral Filtres s’ouvre.

1. Sélectionnez **Modifier les filtres**. La boîte de dialogue **Filtres de tableau de bord** s’ouvre.

1. (Facultatif) Pour ajouter une règle, procédez comme suit :

   1. Sélectionnez l’icône **Modifier** située à droite de la zone de la règle.

      ![icône Modifier](assets/edit-icon.png)

   1. Cliquez sur **Ajouter une condition** puis ajoutez les informations suivantes :
      * Sélectionnez un champ en fonction duquel effectuer le filtrage.
      * Sélectionnez une option (ou un modificateur de filtre) pour définir le type de condition auquel le champ doit répondre.

   1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Passez à [Partie 2 : créer une invite de tableau de bord](#part-2-define-a-dashboard-prompt).


### Partie 2 : définir une invite de tableau de bord

Une invite de tableau de bord permet aux utilisateurs et utilisatrices d’appliquer des filtres personnalisés supplémentaires aux rapports disponibles sur le tableau de bord.

>[!NOTE]
>
>Les options d’invite du tableau de bord ne peuvent être configurées que par un utilisateur disposant de l’autorisation Gérer l’accès au tableau de bord.

1. Pour ajouter une invite, procédez comme suit :

   1. Sélectionnez **Ajouter une invite**. Les nouveaux champs s’affichent dans la partie droite de l’écran.

   1. Saisissez un libellé dans le champ **Personnaliser le libellé**.

   1. Sélectionnez le champ sur lequel vous souhaitez baser l’invite en saisissant le nom du champ, puis en le sélectionnant lorsqu’il apparaît dans la liste. 

1. Pour ajouter une invite personnalisée, procédez comme suit :

   1. Sélectionnez **Ajouter une invite personnalisée**. Les nouveaux champs s’affichent dans la partie droite de l’écran.

   1. (Facultatif) Saisissez un nouveau libellé dans le champ **Personnaliser le libellé**. Par défaut, le libellé *Nouvelle invite personnalisée* est attribué.

   1. Cliquez sur **Ajouter une nouvelle option**.

   1. Saisissez le nom de l’invite dans le champ **Valeur de l’option**.

   1. Cliquez sur **Ajouter une condition** puis spécifiez le champ à utiliser comme filtre et le modificateur qui définit le type de condition auquel le champ doit répondre.

      >[!NOTE]
      >
      >La condition d’une invite personnalisée ne peut être modifiée qu’en mode texte. Cela permet d’appliquer plusieurs conditions dans un seul champ.


   1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Cliquez sur **Enregistrer** pour appliquer le filtre au tableau de bord.

1. Passez à [Partie 3 : appliquer une invite de tableau de bord](#step-3-apply-a-dashboard-prompt).

### Étape 3 : appliquer une invite de tableau de bord

Tous les utilisateurs ayant accès à un tableau de bord peuvent appliquer une invite de tableau de bord à un tableau de bord de la zone de travail une fois le filtre et les invites créés.

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Sur la page **Tableaux de bord de la zone de travail**, sélectionnez le tableau de bord auquel vous souhaitez appliquer l’invite.

1. Dans le coin supérieur gauche de la page des détails du tableau de bord, cliquez sur **Filtres**. Le panneau latéral Filtres s’ouvre.

1. Dans la section **Afficher les enregistrements où...**, choisissez une condition pour une ou toutes les invites affichées. L’invite est appliquée et une balise **Filtres de tableau de bord appliqués** s’affiche dans le coin du widget de rapport.
   ![Sélectionner la condition](assets/prompts-list.png)

1. Cliquez sur l’icône **Fermer** ![Icône Fermer](assets/close-icon.png) dans le coin supérieur droit pour masquer le panneau.

<span class="preview">

## Filtrer un tableau de bord par type de devise

Vous pouvez basculer entre différents types de devise au niveau du tableau de bord. Les rapports qui contiennent des champs de devise seront mis à jour pour refléter le type de devise sélectionné.

>[!NOTE]
>
>Les champs de devise peuvent être verrouillés au niveau du rapport. Si un champ de devise est verrouillé, le type de devise de ce rapport ne change pas lorsque vous modifiez le type de devise du tableau de bord.

Pour modifier le type de devise du tableau de bord :

1. Cliquez sur le menu déroulant Devise dans le coin supérieur droit de la page des détails du tableau de bord.
1. Sélectionnez le type de devise souhaité dans la liste.

   ![liste déroulante modifier la devise](assets/filter-by-currency.png)

</span>