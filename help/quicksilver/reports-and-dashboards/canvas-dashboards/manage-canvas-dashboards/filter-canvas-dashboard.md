---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrer un tableau de bord de la zone de travail
description: Vous pouvez appliquer un filtre à un tableau de bord de la zone de travail après sa création.
author: Courtney
feature: Reports and Dashboards
exl-id: 156e9d3f-49f6-4372-9749-c7124ff5baee
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 9%

---

# Filtrer un tableau de bord de la zone de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement uniquement disponible pour les utilisateurs participant à la phase Beta. Certaines parties de la fonction peuvent ne pas être complètes ou ne pas fonctionner comme prévu pendant cette étape. Veuillez soumettre vos commentaires concernant votre expérience en suivant les instructions de la section [Fournir des commentaires](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) dans l&#39;article de présentation de la version Beta des tableaux de bord Canvas.<br>
>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, voir [Contacter le service clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform


Vous pouvez appliquer un filtre à un tableau de bord de zone de travail contenant des invites. Une invite fonctionne comme un modificateur de filtre qui applique des critères de filtrage supplémentaires afin que vous puissiez affiner davantage vos résultats. Ces invites peuvent être modifiées à chaque application du filtre, ce qui vous permet d’ajuster les résultats affichés sans avoir à modifier les critères de filtre principaux du tableau de bord ou de chaque rapport individuel.

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

You must create a dashboard before it can be filtered.

Pour plus d’informations, voir [Créer un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Filtrer un tableau de bord

Pour filtrer un tableau de bord, procédez comme suit dans l’ordre indiqué :

* [Partie 1 : création d’un filtre de tableau de bord](#part-1-create-a-dashboard-filter)
* [Partie 2 : créer une invite de tableau de bord](#part-2-define-a-dashboard-prompt)
* [Partie 3 : appliquer une invite de tableau de bord](#step-3-apply-a-dashboard-prompt)

>[!NOTE]
>
>Le filtre de tableau de bord s’applique à tous les rapports pour lesquels les filtres de niveau tableau de bord ne sont pas désactivés.  Vous pouvez exclure des rapports individuels de l&#39;application de filtres au niveau du tableau de bord en développant le menu d&#39;actions pour chaque rapport et en sélectionnant l&#39;option **Désactiver les filtres**.


### Partie 1 : Création d’un filtre de tableau de bord

Avec un filtre de tableau de bord, vous pouvez appliquer un filtre commun à tous les rapports disponibles sur un tableau de bord sans avoir à modifier les filtres pour chaque rapport individuel.

>[!NOTE]
>
>Ces filtres peuvent uniquement être configurés par un utilisateur avec un accès Gérer au tableau de bord.


{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. On the **Canvas Dashboards** page, select the dashboard you want to apply a filter to.

1. In the upper-left corner of the dashboard details page, click **Filters**. The filters side panel opens.

1. Select **Edit filters**. The **Dashboard filters** dialog box opens.

1. (Facultatif) Pour ajouter une règle, procédez comme suit :

   1. Sélectionnez l’icône **Modifier** située à droite de la zone de la règle.

      ![Edit icon](assets/edit-icon.png)

   1. Click **Add condition** and then add the following information:
      * Select a field that you want to filter by.
      * Select an option (or filter modifier) to define what kind of condition the field must meet.

   1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OR.

1. Passez à [Partie 2 : créer une invite de tableau de bord](#part-2-define-a-dashboard-prompt).


### Partie 2 : Définition d’une invite de tableau de bord

Une invite du tableau de bord permet aux utilisateurs d’appliquer des filtres personnalisés supplémentaires aux rapports disponibles sur le tableau de bord.

>[!NOTE]
>
>Les options d’invite du tableau de bord peuvent uniquement être configurées par un utilisateur avec un accès Gérer au tableau de bord.

1. To add a prompt, follow the steps below:

   1. Select **Add prompt**. Les nouveaux champs apparaissent sur le côté droit de l’écran.

   1. Enter a label in the **Customize label** field.

   1. Select the field that you want the prompt to be based on by typing the name of the field and then selecting it when it appears in the list. 

1. Pour ajouter une invite personnalisée, procédez comme suit :

   1. Sélectionnez **Ajouter une invite personnalisée**. Les nouveaux champs s’affichent dans la partie droite de l’écran.

   1. (Facultatif) Saisissez un nouveau libellé dans le champ **Personnaliser le libellé**. Par défaut, le libellé *Nouvelle invite personnalisée* est attribué.

   1. Click **Add new option**.

   1. Enter the prompt name in the **Option Value** field.

   1. Cliquez sur **Ajouter une condition** puis spécifiez le champ à utiliser comme filtre et le modificateur qui définit le type de condition auquel le champ doit répondre.

      >[!NOTE]
      >
      >La condition d’une invite personnalisée ne peut être modifiée qu’en mode texte. Cela permet d’appliquer plusieurs conditions dans un seul champ.


   1. (Facultatif) Cliquez sur **Ajouter un groupe de filtres** pour ajouter un autre ensemble de critères de filtrage. L’opérateur par défaut entre les visionneuses est AND. Cliquez sur l’opérateur pour le remplacer par OU.

1. Cliquez sur **Enregistrer** pour appliquer le filtre au tableau de bord.

1. Passez à [Partie 3 : appliquer une invite de tableau de bord](#step-3-apply-a-dashboard-prompt).

### Étape 3 : application d’une invite de tableau de bord

Tous les utilisateurs ayant accès à un tableau de bord peuvent appliquer une invite de tableau de bord à un tableau de bord de zone de travail une fois que le filtre et les invites ont été créés.

{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Sur la page **Tableaux de bord Canvas**, sélectionnez le tableau de bord auquel vous souhaitez appliquer l&#39;invite.

1. Dans le coin supérieur gauche de la page de détails du tableau de bord, cliquez sur **Filtres**. The filters side panel opens.

1. In the **Show records where...** section, choose a condition for one or all the prompts displayed. The prompt is applied and a **Dashboard filters applied** tag appears in the corner of the report widget.
   ![Select condition](assets/prompts-list.png)

1. Cliquez sur l&#39;icône **Fermer** ![Fermer](assets/close-icon.png) dans le coin supérieur droit pour masquer le panneau.


