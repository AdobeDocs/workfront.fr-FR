---
title: Configurez la variable [!DNL Workfront] et [!DNL Frame.io] integration
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Comme [!DNL Adobe Workfront] administrateur, vous pouvez intégrer [!DNL Workfront] avec [!DNL Frame.io] et fournir à votre entreprise un moyen transparent de passer en revue et d’approuver les ressources.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 4%

---


# Configurez la variable [!DNL Workfront] et [!DNL Frame.io] integration

L’administrateur de Workfront active l’intégration entre Workfront et Frame.io en configurant le compte Frame.io par défaut dans la zone Configuration, puis en désignant les utilisateurs de Frame.io dans Workfront. Cela permet au coordinateur de projet de planifier et de lancer des travaux à l’aide de projets Workfront et de workflows de révision et d’approbation.


## Conditions d’accès

>[!IMPORTANT]
>
>Cette fonctionnalité est disponible uniquement pour les organisations qui ont été intégrées au [!DNL Adobe Admin Console].

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td>N’importe quelle
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licences</strong>
   </td>
   <td>Actuel : formule [!UICONTROL] <br>
   Nouveau : [!UICONTROL Standard]
   </td>
  </tr>

<tr>
   <td><strong>Paramétrages du niveau d'accès</strong>
   </td>
   <td>Vous devez être un [!DNL Workfront] administrateur.
   </td>
  </tr>

</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Configuration d’une valeur par défaut [!DNL Frame.io] account [!BADGE Bientôt disponible]{type=Informative}

Une fois la valeur par défaut [!DNL Frame.io] est configuré, tout projet créé dans [!DNL Workfront] Créez un projet miroir dans Frame.io.

>[!IMPORTANT]
>
>Cette fonctionnalité sera bientôt disponible. Pour l’instant, les comptes Frame.io sont ajoutés manuellement par l’équipe Workfront. Contactez votre représentant de compte d’Adobe pour obtenir de l’aide.

## Configuration d’un compte Frame.io unique avec un groupe Workfront

Vous pouvez connecter un seul groupe Workfront à un seul compte Frame.io différent du compte par défaut.

Pour configurer un seul compte Frame.io avec un groupe Workfront :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Groupes**.
1. Sélectionnez un groupe existant ou cliquez sur **Créer un groupe**.
1. Dans le panneau de gauche, cliquez sur **Connexion à Frame.io**.
1. Saisissez le jeton développeur de l’API.
1. Cliquez sur **Lancer la connexion**.
1. (Conditionnel) Si vous êtes administrateur de plusieurs comptes Frame.io, sélectionnez le compte à utiliser.

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

1. Sélectionnez un ou plusieurs utilisateurs, puis cliquez sur le bouton **Modifier** icon ![](assets/edit-icon.png).
1. Dans la section Accès , cochez la case Ajouter aux projets dans Frame.io , puis sélectionnez **Oui** dans le menu déroulant.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Si cette case n’est pas cochée, l’utilisateur conserve l’accès aux affectations antérieures et est ajouté aux projets Frame.io à partir de maintenant.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->

