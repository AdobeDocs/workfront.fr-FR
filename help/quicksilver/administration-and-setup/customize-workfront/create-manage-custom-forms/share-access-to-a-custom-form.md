---
title: Partage d’un formulaire personnalisé
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez configurer l’accès à un formulaire personnalisé afin de contrôler qui peut l’afficher, le partager et le modifier.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 3e6ae76eea2e12fc7fc3a45dad753261a7bad628
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 51%

---

# Partager un formulaire personnalisé

{{preview-fast-release-general}}

Vous pouvez configurer l’accès à un formulaire personnalisé afin de contrôler qui (personne, rôle, groupe, équipe, entreprise, profil d’entreprise) peut l’afficher, le partager et le modifier.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr>  
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Accéder aux formulaires personnalisés {#access-to-custom-forms}

Par défaut, lorsqu’un formulaire personnalisé est joint à un objet, tous les utilisateurs et toutes les utilisatrices à qui cet objet est affecté ont la possibilité de l’afficher et de le remplir. Cela inclut les utilisateurs disposant de licences Contributeur ou Requête et les utilisateurs externes.

Cependant, sur un objet pour lequel le formulaire personnalisé n’est pas déjà joint, un utilisateur ou une utilisatrice (même si un niveau d’accès de planification lui a été accordé) ne peut pas le joindre à partir du menu déroulant des formulaires personnalisés, sauf si l’une des conditions suivantes est vraie :

* <span class="preview">Quelqu&#39;un a partagé le formulaire personnalisé en tant que « Tout le monde dans le système peut afficher et joindre »</span>
* Quelqu’un a partagé le formulaire personnalisé avec l’utilisateur ou avec son équipe, fonction, groupe, entreprise ou profil d’entreprise en accordant au moins l’autorisation Afficher avec l’option Joindre aux données personnalisées sélectionnée
* L’utilisateur dispose d’une licence Standard ou Plan et son niveau d’accès permet un accès administratif aux formulaires personnalisés

<!--

## Share a custom form from the list of forms

Rather than leaving a custom form in the default sharing state (described in [Access to custom forms](#access-to-custom-forms) in this article), you can configure specific levels of access to the form for certain users, job roles, groups, teams, and companies.

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Select the custom form, then click ![Share icon](assets/share-icon.png).
1. In the box that displays, under **Give custom form access to**, start typing the name of the user, team, job role, group, company, or business profile you want to share the custom form with, then press **Enter** when the name displays.
1. To adjust access for the user, team, job role, group, company, or business profile you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View it</td> 
      <td> <p>This option provides the ability to view and fill out the custom form on objects. At the object level, users must also have at least Contribute access with the <strong>Edit custom form</strong> advanced setting enabled. For example, if the form is attached to a project, users must have Contribute access to that project, or they will not be able to fill out the form.</p>
      
      <p><b>NOTE</b>: For users with Light and Contributor licenses (or Work, Review, and Request licenses), this is the highest available option.</p>
      
      <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow the following:</p> 
       <ul> 
        <li><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</li> 
        <li> <p><strong>Share</strong>: Ability to share the custom form with others in the system</p> <p>Users with a Light or Contributor license (or Work, Review, or Request license) can share a custom form only through the API or a custom forms report.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage it</td> 
      <td> <p>This option available only for users with a Standard or Plan license. </p> <p>In addition to being able to add the form to objects they have access to edit, users can also fully edit the custom form, including adding, editing, and deleting fields.</p> <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow following:</p> 
       <ul> 
        <li> <p><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</p> </li> 
        <li><strong>Delete</strong>: Delete the custom form from the system</li> 
        <li><strong>Share</strong>: Share the custom form with others in the system</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Repeat Steps 4-5 to add other names to the list and configure their options.
1. (Optional) If you want to limit access to the custom form (on objects where it's attached) to those you have specified in the previous steps, click the gear icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) in the upper right corner of the sharing box, then click **Remove system-wide access**.

   If you change your mind, you can click **Make this visible system-wide** (the default option).

   >[!NOTE]
   >
   >* When you make a custom form visible system-wide, you allow users only to see and fill it out on objects they are assigned to, not to attach it to other objects. You can grant the ability to attach the custom form to objects using the option "Attach to custom data" explained under step 5.
   >* Most organizations want to ensure that everyone in the system can fill out a custom form when it's attached to objects they work on and view its data in reports. If this is true for your organization, we recommend that you use **Make this visible system-wide**. When the option is configured this way, "Visible System-Wide" displays in the dialog box:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >If you are concerned about a custom form where users might enter sensitive data when it is attached to certain objects, limiting sharing for those *objects* might be better rather than limiting access to the form itself.

1. Click **Save**.

-->

## Partager un formulaire personnalisé

Plutôt que de laisser un formulaire personnalisé à l’état de partage par défaut (décrit dans [Accès aux formulaires personnalisés](#access-to-custom-forms) dans cet article), vous pouvez configurer des niveaux d’accès spécifiques au formulaire pour certains utilisateurs, fonctions, groupes, équipes, sociétés et profils professionnels.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Sélectionnez le formulaire personnalisé dans la liste, puis cliquez sur ![icône Partager](assets/share-icon.png).

   Ou

   Ouvrez un formulaire personnalisé ou créez un formulaire personnalisé. Cliquez ensuite sur **Partager** en haut à droite du concepteur de formulaire.

1. Dans la zone de partage, sous **Accorder l’accès au formulaire personnalisé à**, commencez à saisir le nom de l’utilisateur, de l’équipe, de la fonction, du groupe, de la société ou du profil professionnel avec lequel vous souhaitez partager le formulaire personnalisé, puis appuyez sur **Entrée** lorsque le nom s’affiche.
1. Pour ajuster l’accès pour l’utilisateur, l’équipe, la fonction, le groupe, l’entreprise ou le profil d’entreprise que vous venez d’ajouter, cliquez sur le menu déroulant à droite du nom, puis configurez l’une des options disponibles suivantes et l’un de ses paramètres avancés :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Afficher</td> 
      <td> <p>Cette option permet d’afficher et de remplir le formulaire personnalisé sur des objets. Au niveau de l’objet, les utilisateurs doivent également avoir au moins un accès de type Contributeur avec le paramètre avancé <strong>Modifier le formulaire personnalisé</strong> activé. Par exemple, si le formulaire est joint à un projet, les utilisateurs doivent avoir un accès de type Contributeur à ce projet, sinon ils ne pourront pas remplir le formulaire.</p>

   <p><b>NOTE</b> : pour les titulaires d’une licence Contribution et Light (ou travail, révision et demande), il s’agit de l’option la plus élevée disponible.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li><strong>Joindre aux données personnalisées</strong> : possibilité de joindre un formulaire personnalisé aux projets, tâches et problèmes pour lesquels ils disposent de l’autorisation de gestion.</li> 
        <li> <p><strong>Partager</strong> : possibilité de partager le formulaire personnalisé avec d’autres personnes dans le système.</p> <p>Les titulaires d’une licence Contribution ou Light (ou travail, révision ou demande) peuvent partager un formulaire personnalisé uniquement par le biais de l’API ou d’un rapport de formulaires personnalisés.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gérer</td> 
      <td> <p>Cette option est disponible uniquement pour les utilisateurs disposant d’une licence Standard ou Plan. </p> <p>En plus de pouvoir ajouter le formulaire aux objets auxquels ils ont un accès en modification, les utilisateurs et utilisatrices peuvent également modifier entièrement le formulaire personnalisé, notamment ajouter, modifier et supprimer des champs.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li> <p><strong>Joindre aux données personnalisées</strong> : possibilité de joindre un formulaire personnalisé aux projets, tâches et problèmes pour lesquels ils disposent d’un accès Gérer.</p> </li> 
        <li><strong>Supprimer</strong> : supprimer le formulaire personnalisé du système</li> 
        <li><strong>Partager</strong> : partager un formulaire personnalisé avec d’autres personnes du système</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez les étapes 5 et 6 pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Si vous souhaitez limiter l’accès au formulaire personnalisé (sur les objets auxquels il est associé) aux personnes que vous avez spécifiées aux étapes précédentes, cliquez sur la flèche de liste déroulante sous **Qui a accès**, puis sélectionnez **Accessible par les personnes invitées uniquement**.

   Si vous changez d’avis, vous pouvez sélectionner **Visible par tous dans le système**.

   >[!NOTE]
   >
   >* Lorsque vous affichez un formulaire personnalisé sur tout le système, vous autorisez uniquement les personnes à le consulter et à le remplir sur les objets auxquels ils sont affectés, et non à le joindre à d’autres objets. Vous pouvez accorder la possibilité de joindre le formulaire personnalisé à des objets à l’aide de l’option « Joindre aux données personnalisées », décrite à l’étape 6.
   >* La plupart des entreprises souhaitent s’assurer que toutes les personnes du système peuvent remplir un formulaire personnalisé lorsqu’il est joint aux objets sur lesquels ils travaillent et afficher ses données dans les rapports. Si votre entreprise est concernée, nous vous recommandons d’utiliser **Visible par tous dans le système**.
   >* <span class="preview">Si vous sélectionnez **Tout le monde dans le système peut afficher et joindre**, tous les utilisateurs peuvent joindre le formulaire à d’autres objets.</span>
   >
   ><span class="preview">Exemple d’image dans l’environnement de prévisualisation :</span>
   >![Partager un formulaire personnalisé](assets/share-custom-forms-all-can-attach.png)
   >   
   >Exemple d’image dans l’environnement de production :
   >![Partager un formulaire personnalisé](assets/share-custom-form-in-designer.png)
   >   
   >Si vous vous inquiétez au sujet d’un formulaire personnalisé dans lequel les utilisateurs peuvent saisir des données sensibles lorsqu’il est joint à certains objets, limiter le partage de ces *objets* peut s’avérer plus efficace que limiter l’accès au formulaire lui-même.

1. Cliquer sur **Enregistrer**.

## Supprimer l’accès à un formulaire personnalisé

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Sélectionnez le formulaire personnalisé dans la liste, puis cliquez sur ![icône Partager](assets/share-icon.png).
1. Dans la zone de partage, cliquez sur le menu déroulant situé à droite du nom de l’utilisateur, de l’équipe, du rôle, du groupe, de la société ou du profil d’entreprise dont vous ne souhaitez plus disposer d’un accès spécial au formulaire, puis sélectionnez **Supprimer**.
1. (Facultatif) Répétez l’étape précédente pour les autres noms que vous souhaitez supprimer.
1. Cliquez sur **Enregistrer**.

