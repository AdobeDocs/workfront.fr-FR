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
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Partage d’un formulaire personnalisé

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients ou dans l’environnement Production pour les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Présentation de la version du deuxième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Vous pouvez configurer l’accès à un formulaire personnalisé pour contrôler qui (personne, rôle, groupe, équipe, entreprise) peut l’afficher, le partager et le modifier.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Formule Adobe Workfront</p> </td> 
   <td>Quelconque</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Accès administratif aux formulaires personnalisés</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Accès aux formulaires personnalisés {#access-to-custom-forms}

Par défaut, lorsque vous créez un formulaire personnalisé et que quelqu’un le joint à un objet, tout utilisateur affecté à l’objet peut afficher et remplir le formulaire. Cela inclut les utilisateurs disposant de licences de demande et d’utilisateurs externes.

Cependant, sur un objet pour lequel le formulaire personnalisé n’est pas déjà joint, un utilisateur (même s’il dispose d’un niveau d’accès de planificateur) ne peut pas le joindre à partir du menu déroulant Forms personnalisé, sauf si l’une des conditions suivantes est vraie :

* Une personne a partagé le formulaire personnalisé avec l’utilisateur ou avec son équipe, rôle de tâche, groupe ou entreprise, en accordant au moins l’autorisation Afficher avec l’option Joindre aux données personnalisées sélectionnée.
* L’utilisateur dispose d’une licence Plan et son niveau d’accès permet l’accès administratif aux formulaires personnalisés.

## Partage d’un formulaire personnalisé

Plutôt que de laisser un formulaire personnalisé dans l’état de partage par défaut (décrit à la section [Accès aux formulaires personnalisés](#access-to-custom-forms) dans cet article), vous pouvez configurer des niveaux d’accès spécifiques au formulaire pour certains utilisateurs, rôles de tâche, groupes, équipes et entreprises.

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Forms personnalisée**.
1. Sélectionnez le formulaire personnalisé, puis cliquez sur **Partager** <span class="preview">ou ![Icône Partager](assets/share-icon.png).</span>
1. Dans la zone qui s’affiche, sous **Octroyer un accès à un formulaire personnalisé**, commencez à saisir le nom de l’utilisateur, de l’équipe, du rôle de tâche, du groupe ou de la société avec lequel vous souhaitez partager le formulaire personnalisé, puis appuyez sur **Entrée** lorsque le nom s’affiche.
1. Pour ajuster l’accès de l’utilisateur, de l’équipe, du rôle de tâche, du groupe ou de la société que vous venez d’ajouter, cliquez sur le menu déroulant à droite du nom, puis configurez l’une des options disponibles suivantes, ainsi que l’un de ses paramètres avancés :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">L'afficher</td> 
      <td> <p>Possibilité d’afficher et de remplir le formulaire personnalisé sur les objets.</p> <p><b>REMARQUE</b>: pour les utilisateurs disposant de licences de travail, de révision et de demande, il s’agit de l’option la plus élevée disponible.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li><strong>Ajout à des données personnalisées</strong>: possibilité de joindre un formulaire personnalisé aux projets, tâches et problèmes pour lesquels ils disposent de l’autorisation Gérer .</li> 
        <li> <p><strong>Partager</strong>: possibilité de partager le formulaire personnalisé avec d’autres personnes du système</p> <p>Les utilisateurs disposant d’une licence de travail, de révision ou de demande peuvent partager un formulaire personnalisé uniquement par le biais de l’API ou d’un rapport de formulaires personnalisés. Pour plus d’informations, voir .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Le gérer</td> 
      <td> <p>Disponible uniquement pour les utilisateurs disposant d’une licence Plan. </p> <p>En plus de pouvoir ajouter le formulaire aux objets qu’il a accès à la modification, les utilisateurs peuvent également modifier entièrement le formulaire personnalisé, y compris ajouter, modifier et supprimer des champs.</p> <p>Cliquez sur <strong>Paramètres avancés</strong> pour indiquer si vous souhaitez autoriser les éléments suivants :</p> 
       <ul> 
        <li> <p><strong>Ajout à des données personnalisées</strong>: possibilité de joindre un formulaire personnalisé aux projets, tâches et problèmes pour lesquels ils disposent de l’autorisation Gérer .</p> </li> 
        <li><strong>Supprimer</strong>: supprime le formulaire personnalisé du système</li> 
        <li><strong>Partager</strong>: partage du formulaire personnalisé avec d’autres personnes du système</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Répétez les étapes 4 à 5 pour ajouter d’autres noms à la liste et configurer leurs options.
1. (Facultatif) Si vous souhaitez limiter l’accès au formulaire personnalisé (sur les objets auxquels il est associé) à ceux que vous avez spécifiés aux étapes précédentes, cliquez sur l’icône d’engrenage. ![](assets/gear-icon-settings-with-dn-arrow.jpg) dans le coin supérieur droit de la boîte de partage, puis cliquez sur **Suppression de l’accès à l’échelle du système**.

   Si vous changez d&#39;avis, vous pouvez cliquer sur **rendre visible à l’échelle du système ;** (option par défaut).

   >[!NOTE]
   >
   >* Lorsque vous affichez un formulaire personnalisé à l’échelle du système, vous autorisez uniquement les utilisateurs à le voir et à le remplir sur les objets auxquels ils sont affectés, et non à le joindre à d’autres objets. Vous pouvez accorder la possibilité de joindre le formulaire personnalisé à des objets à l’aide de l’option &quot;Joindre aux données personnalisées&quot; expliquée à l’étape 5.
   >* La plupart des entreprises souhaitent s’assurer que tous les membres du système peuvent remplir un formulaire personnalisé lorsqu’il est joint aux objets sur lesquels ils travaillent et afficher ses données dans les rapports. Si cela est vrai pour votre organisation, nous vous recommandons d’utiliser &quot;**rendre visible à l’échelle du système ;**.&quot; Lorsque l’option est configurée de cette manière, &quot;Visible à l’échelle du système&quot; s’affiche dans la boîte de dialogue :
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Si un formulaire personnalisé vous préoccupe, dans lequel les utilisateurs peuvent saisir des données sensibles lorsqu’il est joint à certains objets, limite le partage pour ces données. *objet* peut être préférable à la limitation de l’accès au formulaire lui-même.

1. Cliquer sur **Enregistrer**.

## Supprimer l’accès à un formulaire personnalisé

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Forms personnalisée**.
1. Sélectionnez le formulaire personnalisé, puis cliquez sur **Partager** <span class="preview">ou ![Icône Partager](assets/share-icon.png).</span>
1. Dans la zone qui s’affiche, cliquez sur le X situé à droite du nom de l’utilisateur, de l’équipe, du rôle, du groupe ou de la société dont vous ne souhaitez plus bénéficier d’un accès spécial au formulaire.
1. (Facultatif) Répétez l’étape précédente sur pour connaître les autres noms que vous souhaitez supprimer.
1. Cliquer sur **Enregistrer**.
