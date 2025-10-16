---
title: Partage d’un formulaire personnalisé
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Vous pouvez configurer l’accès à un formulaire personnalisé pour contrôler qui (personne, rôle, groupe, équipe, entreprise) peut l’afficher, le partager et le modifier.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 89%

---

# Partager un formulaire personnalisé

Vous pouvez configurer l’accès à un formulaire personnalisé pour contrôler qui (personne, rôle, groupe, équipe, entreprise) peut l’afficher, le partager et le modifier.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
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

Par défaut, lorsqu’un formulaire personnalisé est joint à un objet, tous les utilisateurs et toutes les utilisatrices à qui cet objet est affecté ont la possibilité de l’afficher et de le remplir. Cela inclut les utilisateurs et les utilisatrices disposant de licences Demande et les utilisateurs et utilisatrices externes.

Cependant, sur un objet pour lequel le formulaire personnalisé n’est pas déjà joint, un utilisateur ou une utilisatrice (même si un niveau d’accès de planification lui a été accordé) ne peut pas le joindre à partir du menu déroulant des formulaires personnalisés, sauf si l’une des conditions suivantes est vraie :

* Le formulaire personnalisé est maintenant accessible à l’utilisateur ou à l’utilisatrice, à son équipe, sa fonction, son groupe ou même à l’organisation, avec au moins les autorisations d’affichage, suite à la sélection de l’option « Joindre aux données personnalisées ».
* L’utilisateur ou l’utilisatrice dispose d’une licence Plan et son niveau d’accès lui accorde l’accès administratif aux formulaires personnalisés.

## Partager un formulaire personnalisé à partir de la liste des formulaires

Plutôt que de laisser un formulaire personnalisé dans le statut de partage par défaut (décrit dans [Accès aux formulaires personnalisés](#access-to-custom-forms) dans cet article), vous pouvez configurer des niveaux spécifiques d’accès au formulaire pour certains utilisateurs et utilisatrices, fonctions, groupes, équipes et entreprises.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Sélectionnez le formulaire personnalisé, puis cliquez sur l’![icône Partager](assets/share-icon.png).
1. Dans la zone qui s’affiche, sous **Accorder l’accès à un formulaire personnalisé**, commencez à saisir le nom de la personne, de l’équipe, de la fonction, du groupe ou de l’entreprise avec lequel vous souhaitez partager le formulaire personnalisé, puis appuyez sur **Entrée** lorsque le nom s’affiche.
1. Pour ajuster l’accès de l’utilisateur ou de l’utilisatrice, de l’équipe, de la fonction, du groupe ou de la société que vous venez d’ajouter, cliquez sur le menu déroulant à droite du nom, puis configurez l’une des options disponibles suivantes, ainsi que l’un de ses paramètres avancés :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">L'afficher</td> 
      <td> <p>Cette option permet d’afficher et de remplir le formulaire personnalisé sur des objets. Au niveau de l’objet, les utilisateurs doivent également avoir au moins un accès de type Contributeur avec le paramètre avancé <strong>Modifier le formulaire personnalisé</strong> activé. Par exemple, si le formulaire est joint à un projet, les utilisateurs doivent avoir un accès de type Contributeur à ce projet, sinon ils ne pourront pas remplir le formulaire.</p>

   <p><b>NOTE</b> : pour les titulaires d’une licence Contribution et Light (ou travail, révision et demande), il s’agit de l’option la plus élevée disponible.</p>

   <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li><strong>Joindre aux données personnalisées</strong> : possibilité de joindre un formulaire personnalisé aux projets, tâches et problèmes pour lesquels ils disposent de l’autorisation de gestion.</li> 
        <li> <p><strong>Partager</strong> : possibilité de partager le formulaire personnalisé avec d’autres personnes dans le système.</p> <p>Les titulaires d’une licence Contribution ou Light (ou travail, révision ou demande) peuvent partager un formulaire personnalisé uniquement par le biais de l’API ou d’un rapport de formulaires personnalisés.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le gérer</td> 
      <td> <p>Cette option est disponible uniquement pour les utilisateurs disposant d’une licence Standard ou Plan. </p> <p>En plus de pouvoir ajouter le formulaire aux objets auxquels ils ont un accès en modification, les utilisateurs et utilisatrices peuvent également modifier entièrement le formulaire personnalisé, notamment ajouter, modifier et supprimer des champs.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li> <p><strong>Joindre aux données personnalisées</strong> : possibilité de joindre un formulaire personnalisé aux projets, tâches et problèmes pour lesquels ils disposent d’un accès Gérer.</p> </li> 
        <li><strong>Supprimer</strong> : supprimer le formulaire personnalisé du système</li> 
        <li><strong>Partager</strong> : partager un formulaire personnalisé avec d’autres personnes du système</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez les étapes 4 à 5 pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Si vous souhaitez limiter les autorisations d’accès au formulaire personnalisé (sur les objets auxquels il est joint) que vous avez accordées aux étapes précédentes, cliquez sur l’icône d’engrenage ![](assets/gear-icon-settings-with-dn-arrow.jpg) dans le coin supérieur droit de la zone de partage, puis cliquez sur **Supprimer l’accès à tout le système**.

   Si vous changez d’avis, vous pouvez cliquer sur **Rendre ceci visible sur tout le système** (option par défaut).

   >[!NOTE]
   >
   >* Lorsque vous rendez un formulaire personnalisé visible dans tout le système, vous autorisez les utilisateurs et les utilisatrices à l’afficher et à le remplir uniquement sur les objets auxquels ils sont affectés, mais pas à le joindre à d’autres objets. Vous pouvez accorder la possibilité de joindre le formulaire personnalisé à des objets à l’aide de l’option « Joindre aux données personnalisées » expliquée à l’étape 5.
   >* La plupart des entreprises souhaitent s’assurer que toutes les personnes du système peuvent remplir un formulaire personnalisé lorsqu’il est joint aux objets sur lesquels ils travaillent et afficher ses données dans les rapports. Si votre entreprise et concernée, nous vous recommandons d’activer l’option **Rendre cet élément visible à l’échelle du système**. Lorsque l’option est configurée ainsi, « Visible sur tout le système » s’affiche dans la boîte de dialogue :
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Si un formulaire personnalisé risque d’amener les utilisateurs et les utilisatrices à saisir des données sensibles lorsqu’il est joint à certains objets, il est préférable de limiter le partage pour ces *objets* plutôt que de limiter l’accès au formulaire proprement dit.

1. Cliquer sur **Enregistrer**.

## Partager un formulaire personnalisé à partir du concepteur de formulaires

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Ouvrez un formulaire personnalisé ou créez un formulaire personnalisé.
1. Cliquez sur **Partager** en haut à droite du concepteur de formulaires lorsque le formulaire est prêt à être partagé.
1. Dans la zone qui s’affiche, sous **Accorder l’accès à un formulaire personnalisé**, commencez à saisir le nom de la personne, de l’équipe, de la fonction, du groupe ou de l’entreprise avec lequel vous souhaitez partager le formulaire personnalisé, puis appuyez sur **Entrée** lorsque le nom s’affiche.
1. Pour ajuster l’accès de l’utilisateur ou de l’utilisatrice, de l’équipe, de la fonction, du groupe ou de la société que vous venez d’ajouter, cliquez sur le menu déroulant à droite du nom, puis configurez l’une des options disponibles suivantes, ainsi que l’un de ses paramètres avancés :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">L'afficher</td> 
      <td> <p>Cette option permet d’afficher et de remplir le formulaire personnalisé sur des objets. Au niveau de l’objet, les utilisateurs doivent également avoir au moins un accès de type Contributeur avec le paramètre avancé <strong>Modifier le formulaire personnalisé</strong> activé. Par exemple, si le formulaire est joint à un projet, les utilisateurs doivent avoir un accès de type Contributeur à ce projet, sinon ils ne pourront pas remplir le formulaire.</p>

   <p><b>NOTE</b> : pour les titulaires d’une licence Contribution et Light (ou travail, révision et demande), il s’agit de l’option la plus élevée disponible.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li><strong>Joindre aux données personnalisées</strong> : possibilité de joindre un formulaire personnalisé aux projets, tâches et problèmes pour lesquels ils disposent de l’autorisation de gestion.</li> 
        <li> <p><strong>Partager</strong> : possibilité de partager le formulaire personnalisé avec d’autres personnes dans le système.</p> <p>Les titulaires d’une licence Contribution ou Light (ou travail, révision ou demande) peuvent partager un formulaire personnalisé uniquement par le biais de l’API ou d’un rapport de formulaires personnalisés.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le gérer</td> 
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
   >* La plupart des entreprises souhaitent s’assurer que toutes les personnes du système peuvent remplir un formulaire personnalisé lorsqu’il est joint aux objets sur lesquels ils travaillent et afficher ses données dans les rapports. Si votre entreprise est concernée, nous vous recommandons d’utiliser **Visible par tous dans le système**. Lorsque l’option est configurée de cette manière, « Visible sur tout le système » s’affiche dans la boîte de dialogue :
   >   
   >![Partager un formulaire personnalisé](assets/share-custom-form-in-designer.png)
   >   
   >Si un formulaire personnalisé risque d’amener les utilisateurs et les utilisatrices à saisir des données sensibles lorsqu’il est joint à certains objets, il est préférable de limiter le partage pour ces *objets* plutôt que de limiter l’accès au formulaire proprement dit.

1. Cliquer sur **Enregistrer**.

## Supprimer l’accès à un formulaire personnalisé de la liste des formulaires

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Formulaires personnalisés**.
1. Sélectionnez le formulaire personnalisé, puis cliquez sur l’![icône Partager](assets/share-icon.png).
1. Dans la zone qui s’affiche, cliquez sur le bouton X situé à droite du nom de la personne, de l’équipe, du rôle, du groupe ou de l’entreprise dont vous ne souhaitez plus qu’il dispose d’un accès spécial au formulaire.
1. (Facultatif) Répétez l’étape précédente pour les autres noms que vous souhaitez supprimer.
1. Cliquer sur **Enregistrer**.
