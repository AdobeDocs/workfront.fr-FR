---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Partager un tableau de bord de zones de travail
description: Vous pouvez partager un tableau de bord Zone de travail avec d’autres utilisateurs d’Adobe Workfront afin qu’ils puissent l’afficher ou le modifier.
author: Jenny
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 13%

---

# Partager un tableau de bord de zones de travail

>[!IMPORTANT]
>
>La fonctionnalité Tableaux de bord de la zone de travail est actuellement disponible uniquement pour les utilisateurs participant à l’étape bêta. Il se peut que certaines parties de la fonction ne soient pas terminées ou ne fonctionnent pas comme prévu à cette étape. Veuillez soumettre tout commentaire concernant votre expérience en suivant les instructions de la section [Fournir un commentaire](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) de l’article de présentation de la version Beta des tableaux de bord de la zone de travail.<br>
>&#x200B;>Si vous avez des commentaires concernant un bug ou un problème technique éventuel, envoyez un ticket à l’assistance Workfront. Pour plus d’informations, voir [Contacter le service clientèle](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>&#x200B;>Notez que cette version bêta n’est pas disponible sur les fournisseurs de cloud suivants :
>
>* Apporter votre propre clé pour Amazon Web Services
>* Azure
>* Google Cloud Platform

Vous pouvez partager un tableau de bord Zone de travail avec d’autres utilisateurs d’Adobe Workfront afin qu’ils puissent l’afficher ou le modifier.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<p>Tous </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td> 
<p>Standard </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurations des niveaux d’accès</p></td> 
   <td><p>Afficher l’accès aux rapports, aux tableaux de bord et aux calendriers</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td><p>Autorisations d’affichage pour le tableau de bord afin de partager le tableau de bord</p>
   <p>Gérer les autorisations relatives au tableau de bord pour attribuer des autorisations relatives au tableau de bord</p>
  </td> 
  </tr>
</tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Remarques sur le partage des tableaux de bord

* Les tableaux de bord peuvent être partagés avec les utilisateurs, les équipes, les groupes, les fonctions ou les ressources de l’entreprise.

* Par défaut, le créateur d’un tableau de bord dispose des autorisations de niveau Gérer pour celui-ci.

* Les administrateurs système et les utilisateurs disposant d’une autorisation Gérer peuvent accorder un accès en lecture ou en gestion à un tableau de bord.

* Les utilisateurs disposant d’une autorisation d’affichage dans un tableau de bord peuvent accorder un accès en affichage à un tableau de bord.

* Lors du partage d’un tableau de bord, les ressources avec lesquelles il est partagé hériteront des autorisations relatives aux rapports affichés sur le tableau de bord.

* Lorsqu&#39;un tableau de bord est distribué par le biais d&#39;un modèle de mise en page, une autorisation d&#39;affichage automatique du tableau de bord (et de ses rapports) est accordée à toutes les ressources affectées au modèle de mise en page.


## Partager un tableau de bord de zones de travail


{{step1-to-dashboards}}

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord des zones de travail**.

1. Sur la page **Tableaux de bord de la zone de travail**, sélectionnez le tableau de bord à partager.

1. Dans le coin supérieur droit de la page, cliquez sur le bouton **Partager**. La boîte de dialogue **Partage de tableau de bord** s’affiche.

1. Dans le champ **Accorder l’accès à**, commencez à saisir le nom d’un utilisateur, d’une équipe, d’un rôle, d’un groupe ou d’une entreprise avec lequel vous souhaitez partager le tableau de bord Zone de travail, puis sélectionnez-le lorsqu’il apparaît dans la liste déroulante.

1. (Facultatif) Pour modifier l’accès d’une ressource au tableau de bord, cliquez sur **Afficher** en regard de son nom, puis sélectionnez **Gérer** dans la liste déroulante qui s’affiche.

   >[!NOTE]
   >
   > Lorsque les utilisateurs ne disposent pas des autorisations de modification d’un tableau de bord attribuées via leur niveau d’accès, ils ne peuvent pas se voir attribuer les autorisations de gestion d’un tableau de bord.

1. Répétez les étapes 5 à 6 pour chaque ressource avec laquelle vous souhaitez partager le tableau de bord.

1. Cliquez sur le bouton **Partager**. Les destinataires reçoivent une notification par e-mail les informant que le tableau de bord a été partagé avec eux, à laquelle ils peuvent désormais accéder à l’adresse **Tableaux de bord** > **Tableaux de bord de la zone de travail** > **Tableaux de bord partagés**.

   >[!NOTE]
   >
   > Les préférences individuelles des utilisateurs et les exclusions système pour les notifications par e-mail peuvent s’appliquer. <br>
   > Les notifications sont envoyées uniquement lorsqu’elles sont partagées directement avec un utilisateur. Le partage vers des groupes, des rôles, des entreprises et des équipes ne génère pas de notifications par e-mail.<br>
   > Les autorisations héritées d’un modèle de mise en page ne génèrent pas de notification par e-mail concernant l’accès au tableau de bord.
