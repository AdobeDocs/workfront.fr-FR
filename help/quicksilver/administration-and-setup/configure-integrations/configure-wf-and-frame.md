---
title: Configuration de l'intégration  [!DNL Workfront] et [!DNL Frame.io]
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: En tant qu'administrateur  [!DNL Adobe Workfront] , vous pouvez intégrer  [!DNL Workfront]  à  [!DNL Frame.io]  et offrir à votre entreprise un moyen transparent de passer en revue et d'approuver les ressources.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: 0d737bc410f3db4eeff52fa8954acdb8a0eb1a6e
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 23%

---

# Configuration de l’intégration [!DNL Workfront] et [!DNL Frame.io]

L’administrateur de Workfront active l’intégration entre Workfront et Frame.io en configurant le compte Frame.io par défaut dans la zone Configuration, puis en désignant les utilisateurs de Frame.io dans Workfront. Cela permet au coordinateur de projet de planifier et de lancer des travaux à l’aide de projets Workfront et de workflows de révision et d’approbation.


## Conditions d’accès

>[!IMPORTANT]
>
>Cette fonctionnalité est disponible uniquement pour les entreprises qui ont été intégrées à [!DNL Adobe Admin Console].

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td>Plan <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td>N’importe quelle
   </td>
  </tr>
  <tr>
   <td>Licences <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td>Actuel : [!UICONTROL Plan] <br>
 Nouveau : [!UICONTROL Standard]
   </td>
  </tr>

<tr>
   <td><strong> Configurations de niveau d’accès</strong>
   </td>
   <td>Vous devez être un administrateur ou une administratrice [!DNL Workfront].
   </td>
  </tr>

</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Configurer un compte [!DNL Frame.io] par défaut [!BADGE Bientôt disponible]{type=Informative}

Une fois qu’un compte [!DNL Frame.io] par défaut est configuré, tous les projets créés dans [!DNL Workfront] ont un projet miroir créé dans Frame.io.

>[!IMPORTANT]
>
>Cette fonctionnalité sera bientôt disponible. Pour l’instant, les comptes Frame.io sont ajoutés manuellement par l’équipe Workfront. Contactez votre représentant de compte d’Adobe pour obtenir de l’aide.

## Configuration d’un compte Frame.io unique avec un groupe Workfront

Vous pouvez connecter un seul groupe Workfront à un seul compte Frame.io différent du compte par défaut.

Pour configurer un seul compte Frame.io avec un groupe Workfront :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Sélectionnez un groupe existant ou cliquez sur **Créer un groupe**.
1. Dans le panneau de gauche, cliquez sur **Se connecter à Frame.io**.
1. Saisissez le jeton de développement d’API.
1. Cliquez sur **Lancer la connexion**.
1. (Le cas échéant) Si vous êtes administrateur ou administratrice de plusieurs comptes Frame.io, sélectionnez le compte à utiliser.

## Activation de Frame.io

Les utilisateurs de Workfront qui utilisent régulièrement Frame.io doivent être marqués comme des utilisateurs de Frame.io. Les administrateurs de Workfront peuvent désigner des utilisateurs de Frame.io dans le profil utilisateur de Workfront.

>[!TIP]
>
>Nous recommandons d’activer les utilisateurs qui travaillent régulièrement dans des outils de création et de charger des ressources pour révision et approbation en tant qu’utilisateurs de Frame.io.

Lorsqu’un utilisateur est marqué comme utilisateur Frame.io dans Workfront et est ajouté à un projet :

* Ils sont ajoutés en tant que collaborateur dans Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Ils peuvent envoyer des ressources de Frame.io à Workfront pour révision et approbation formelles.
* Ils peuvent afficher des informations dans le dossier de synchronisation unidirectionnelle à partir de Workfront. [!BADGE Bientôt disponible]{type=Informative}

Pour activer les utilisateurs de Frame.io :

{{step-1-to-users}}

1. Sélectionnez un ou plusieurs utilisateurs, puis cliquez sur l’icône **Modifier** ![](assets/edit-icon.png).
1. Dans la section Accès , cochez la case Ajouter aux projets dans Frame.io , puis sélectionnez **Oui** dans le menu déroulant.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Si cette case n’est pas cochée, l’utilisateur conserve l’accès aux affectations antérieures et est ajouté aux projets Frame.io à partir de maintenant.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
