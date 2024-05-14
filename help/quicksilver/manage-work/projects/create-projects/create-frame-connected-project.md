---
product-area: projects
navigation-topic: create-projects
title: Création d’un projet connecté à Frame.io
description: Un projet est une grande unité de travail dans Adobe Workfront. Vous pouvez créer des projets à partir de zéro, utiliser un modèle ou convertir des problèmes ou des tâches en projets.
author: Courtney
feature: Work Management
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 4%

---


# Création d’un projet connecté à Frame.io

L’intégration de Workfront et de Frame.io vous permet de créer des projets dans Workfront qui sont mis en miroir dans Frame.io, ce qui vous permet d’effectuer facilement des révisions et des validations.

Lorsqu’un projet Workfront est connecté à Frame.io, vous pouvez

* **Affecter des utilisateurs de Frame.io à des tâches**: les utilisateurs activés pour Frame.io sont avertis par e-mail lorsqu’ils sont affectés à une tâche Workfront, ce qui indique qu’il reste du travail à faire.
* **Partage du projet avec les utilisateurs de Frame.io**: lorsqu’un projet est partagé avec des utilisateurs activés pour Frame.io, ils ont accès au projet à l’intérieur de Workfront et de Frame.io.
* **Partage de contenu créatif avec Frame.io**: les coordinateurs de projet peuvent envoyer des instructions et du matériel de Workfront directement à l’utilisateur créatif de Frame.io à l’aide d’un dossier de projet de synchronisation unidirectionnelle. [!BADGE Bientôt disponible]{type=Informative}
* **Suivi de la progression de la tâche**: les créatifs peuvent envoyer des ressources terminées et marquer les tâches comme terminées, le tout sans quitter Frame.io.

## Conditions d’accès

>[!IMPORTANT]
>
>Cette fonctionnalité est disponible uniquement pour les organisations qui ont été intégrées au [!DNL Adobe Admin Console].

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Lorsque vous créez un projet, vous recevez automatiquement les autorisations de gestion du projet.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

* Configuration du compte Frame.io par défaut dans la zone de configuration de Workfront
* Activation des utilisateurs de Frame.io dans le profil utilisateur Workfront

Pour plus d’informations sur les conditions préalables ci-dessus, voir [Configurez la variable [!DNL Workfront] et [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).


## Créer un modèle de projet

Lors de la création d’un modèle, vous pouvez saisir les informations pour toutes les tâches et pour les paramètres futurs du projet. Ces informations seront ensuite transférées vers tout projet que vous créez à partir du modèle.

Les projets de Frame.io sont organisés par des équipes connectées aux groupes Workfront. Nous vous recommandons d’utiliser un modèle de projet pour créer des projets connectés, car vous pouvez définir le groupe de projets auparavant.

Si vous choisissez de créer entièrement le projet, Workfront ajoute automatiquement le groupe de projets par défaut et le projet Frame.io miroir est créé sous cette équipe par défaut dans Frame.io.

>[!NOTE]
>
>La mise à jour du groupe après la création du projet ne modifie pas l’équipe Frame.io.


### Créez le modèle et spécifiez le groupe de projets.

{{step1-to-templates}}

1. Cliquez sur **Nouveau modèle**.
1. Saisissez le nom du modèle, puis appuyez sur **Entrée** pour enregistrer le nom.
1. Dans le panneau de gauche, cliquez sur **Détails du modèle**.
1. Dans le **Association de modèles** , veillez à spécifier un groupe. Si vous n’ajoutez pas de groupe, le groupe de projets par défaut est ajouté et le projet dans Frame.io est créé sous l’équipe par défaut correspondante dans Frame.io.

Passez à la section suivante.

![](assets/template-group.png)

### Ajout de tâches et affectation d’utilisateurs activés Frame.io

1. Dans le panneau de gauche, cliquez sur **Tâches de modèle**.
1. Cliquez sur **Commencer à ajouter des tâches de modèle** pour ajouter rapidement des tâches à votre modèle. Vous pouvez configurer d’autres paramètres ultérieurement.

   Ou

   Cliquez sur **Nouvelle tâche de modèle** pour ajouter une tâche à la fois et configurer des paramètres supplémentaires.
   ![](assets/add-tasks-to-template.png)
1. Ajoutez un nom de tâche.
1. Dans le **Affectations** , affectez des utilisateurs ou des équipes. Si vous attribuez un utilisateur Frame.io activé, individuellement ou au sein d’une équipe, il se voit accorder un accès collaborateur au projet Frame.io et vous êtes informé par e-mail de la tâche dans le projet Frame.io. À partir de cet e-mail, ils peuvent rejoindre le projet Frame.io et commencer à travailler.
1. Répétez les étapes 1 et 2 si nécessaire.

Passez à la section suivante.

### Configuration des détails supplémentaires du modèle

Workfront dispose de puissantes fonctionnalités de gestion de projet. Il est recommandé d’utiliser la variable [Modifier des modèles de projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) pour configurer les zones suivantes du modèle :

* Vue d’ensemble
* Finances
* Formulaires personnalisés
* Paramètres du projet
* Paramètres des tâches
* Paramètres de l&#39;événement
* Accès

### Création d’un projet à partir du modèle

Une fois que vous avez créé un modèle, vous pouvez l’utiliser pour créer des projets.

{{step1-to-projects}}

1. Cliquez sur **Nouveau projet à partir du modèle**.
1. Dans la zone de recherche, commencez à saisir le nom du modèle dont vous avez besoin.
1. Sélectionnez le nom du modèle, puis cliquez sur **Utiliser un modèle**.
   ![](assets/find-your-template.png)
1. Ajustez les paramètres d’un projet selon vos besoins, puis cliquez sur **Créer un projet**.
1. Dans le panneau de gauche, cliquez sur **Documents**.
1. Utilisez le dossier de synchronisation unidirectionnelle pour partager automatiquement du contenu créatif avec Frame.io. [!BADGE Bientôt disponible]{type=Informative}

   >[!NOTE]
   >
   >Cette fonctionnalité est actuellement en cours de développement. Pour partager des informations avec les utilisateurs de Frame.io, téléchargez les fichiers dans l’onglet Document . Lorsque l’état du projet est défini sur Actuel, ces fichiers sont automatiquement transférés vers Frame.io.

1. Dans l’en-tête du projet, modifiez le projet à partir de **Planification** to **Actuel**.

Une fois le projet créé et les créatifs chargés les ressources terminées, vous pouvez affecter un processus de révision et d’approbation à la ressource dans Workfront. Pour plus d’informations, voir [Créer une demande d’approbation ou de révision de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->

## Création d’un projet à partir de zéro

Vous pouvez créer un projet à partir de zéro, si nécessaire.

>[!IMPORTANT]
>
>* Les projets de Frame.io sont organisés par des équipes connectées aux groupes Workfront. Nous vous recommandons d’utiliser un modèle de projet pour créer des projets connectés, car vous pouvez définir le groupe de projets auparavant.
>
>
>* Si vous choisissez de créer entièrement le projet, Workfront ajoute automatiquement le groupe de projets par défaut et le projet Frame.io miroir est créé sous cette équipe par défaut dans Frame.io.
>
>La mise à jour du groupe après la création du projet ne modifie pas l’équipe Frame.io.

### Création du projet

{{step1-to-projects}}

1. Cliquez sur **Nouveau projet**.
1. Saisissez le nom de votre projet, puis appuyez sur **Entrée** pour enregistrer le nom.

Passez à la section suivante.

### Ajout de tâches et affectation d’utilisateurs activés Frame.io

1. Dans le panneau de gauche, cliquez sur **Tâche**.
1. Cliquez sur **Commencer à ajouter des tâches** pour ajouter rapidement des tâches à votre projet. Vous pouvez configurer d’autres paramètres ultérieurement.

   Ou

   Cliquez sur **Nouvelle tâche** pour ajouter une tâche à la fois et configurer des paramètres supplémentaires.
   ![](assets/add-project-tasks.png)
1. Ajoutez un nom de tâche.
1. Dans le **Affectations** , affectez des utilisateurs ou des équipes. Si vous attribuez un utilisateur Frame.io activé, individuellement ou au sein d’une équipe, il se voit accorder un accès collaborateur au projet Frame.io et vous êtes informé par e-mail de la tâche dans le projet Frame.io. À partir de cet e-mail, ils peuvent rejoindre le projet Frame.io et commencer à travailler.
1. Répétez les étapes 1 et 2 si nécessaire.

Passez à la section suivante.

### Chargement de ressources créatives

1. Dans le panneau de gauche, cliquez sur **Documents**.
1. Utilisez le dossier de synchronisation unidirectionnelle pour partager automatiquement du contenu créatif avec Frame.io. [!BADGE Bientôt disponible]{type=Informative}

   >[!NOTE]
   >
   >Cette fonctionnalité est actuellement en cours de développement. Pour partager des informations avec les utilisateurs de Frame.io, téléchargez les fichiers dans l’onglet Document . Lorsque l’état du projet est défini sur Actuel, ces fichiers sont automatiquement transférés sur Frame.io.

Passez à la section suivante.

### Configuration des détails supplémentaires du projet

Workfront dispose de puissantes fonctionnalités de gestion de projet. Il est recommandé d’utiliser la variable [Modification de projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) article pour configurer les zones suivantes du projet :

* Vue d’ensemble
* Finances
* Formulaires personnalisés
* Paramètres du projet
* Paramètres des tâches
* Paramètres de l&#39;événement
* Accès

### Définir le projet sur actuel

1. Dans l’en-tête du projet, remplacez le projet de Planification par Actuel.
Une fois le projet créé et les créatifs chargés les ressources terminées, vous pouvez affecter un processus de révision et d’approbation à la ressource dans Workfront.

Une fois le projet créé et les créatifs chargés les ressources terminées, vous pouvez affecter un processus de révision et d’approbation à la ressource dans Workfront.

Pour plus d’informations, voir [Créer une demande d’approbation ou de révision de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->