---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Créer une Forms d’admission de projets
description: Vous pouvez utiliser les formulaires de réception de projets pour simplifier le processus de création de projets dans Workfront
author: Becky
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
source-git-commit: 5ff71313c550d949079e7426b657a0a4e19a656c
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 6%

---

# Créer des formulaires de saisie de projet

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Les formulaires de réception de projets sont un type de formulaire de demande qui permet aux utilisateurs de demander des projets. Les projets sont créés à partir du formulaire, sans qu’il soit nécessaire de créer un projet à partir d’un événement envoyé.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Nouvelle licence : Standard </p>
   Ou
   <p>Licence actuelle : plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront pour créer des formulaires de réception de projets. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autres produits</td> 
   <td> <p>Votre entreprise doit avoir acheté Workfront Planning pour utiliser les fonctionnalités de Planning telles que les automatisations.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fonctionnalités et limites de Project Intake Forms

### Fonctionnalités

Les formulaires de réception de projets comprennent les fonctionnalités suivantes :

#### Automatismes de Workfront Planning

Les formulaires de saisie de projet Workfront prennent en charge l’automatisation de planification Workfront pour configurer les propriétés créées spécifiques au projet.

Pour plus d’informations sur les automatisations de Planning, voir [Configurer les automatisations de Planning d’Adobe Workfront](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Configuration de la validation

Les formulaires de réception de projets incluent la possibilité de configurer des approbateurs pour les demandes envoyées.

### Limites

#### Types de champ pris en charge

Forms d’entrée de projet peut inclure des champs de n’importe quel formulaire personnalisé avec le type d’objet Projet.

Les types de champs suivants ne sont actuellement pas pris en charge dans Project Intake Forms :

* Section
* Formule
* Agrégation des données
* Agrégation des données sur une seule ligne
* Connexion de planning
* Les références de champs natifs qui font référence aux champs natifs du projet, qui sont en lecture seule (par exemple, `workRequiredExpression`)

#### Demande d’expérience

Les formulaires de réception de projets ne peuvent être utilisés qu’avec la nouvelle expérience de demande.

Pour plus d’informations sur la nouvelle expérience de demande, voir [Création et envoi de demandes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

#### Partage

Les formulaires de réception de projets ne prennent pas en charge le partage public. Les options de partage sont les suivantes :

* **Tout le monde** : tout le monde dans le système peut utiliser le formulaire pour envoyer une demande de projet.
* **Utilisateurs spécifiés** : vous pouvez sélectionner les utilisateurs spécifiques qui ont accès au formulaire de demande de projet.

## Créer un formulaire de saisie de projet

{{step1-to-requests}}

1. Activez le paramètre **Basculer vers une nouvelle expérience** dans le coin supérieur droit de l’écran.
1. Cliquez sur **Formulaires de demande** dans le coin supérieur droit de l’écran.

   >[!NOTE]
   >
   >Étant donné que seuls les administrateurs Workfront peuvent créer des formulaires de réception, le bouton Formulaires de demande n’est visible que par les administrateurs.

   Une liste des formulaires de demande actuellement disponibles s’affiche. Cela inclut les formulaires de demande de Workfront Planning.

1. Cliquez sur **Nouveau formulaire de demande** dans le coin supérieur droit de l’écran.
1. Saisissez un nom pour le formulaire de demande. Par défaut, le nom du formulaire est **Formulaire sans titre**.
1. Sélectionnez le type d’objet **Projet** en haut de la liste déroulante. Actuellement, il s’agit du seul type de projet Workfront disponible. Les autres éléments de la liste appartiennent à Workfront Planning.
1. (Facultatif) Ajoutez une **Description** pour le formulaire de demande.
1. Cliquez sur **Créer**. Le formulaire de demande pour le type d’enregistrement sélectionné s’ouvre dans l’onglet Formulaire .

   Le créateur de formulaires de saisie de projet s’ouvre sur l’onglet Formulaire .

   Le formulaire de saisie contient par défaut les informations suivantes :

   * **Section par défaut** : il s’agit du saut de section par défaut que Workfront applique au formulaire de demande. Tous les champs d’enregistrement s’affichent dans la zone **Section par défaut**.
   * Champ **Subject** : champ qui identifiera la demande dans Workfront. La configuration et la valeur du champ Objet ne sont pas modifiables.
   * Tous les champs associés aux projets.

     Les champs contenus dans le formulaire de demande seront visibles pour toutes les personnes soumettant une demande de projet.

1. Pour ajouter des champs au formulaire, cliquez sur le type de champ dans le volet de navigation de gauche, puis sélectionnez le champ.
1. (Facultatif) Pour supprimer un champ, pointez sur le champ du formulaire à supprimer, puis cliquez sur l’icône **x** pour le supprimer.
1. (Facultatif) Pour supprimer la **section Par défaut** du formulaire, procédez comme suit :

   1. Supprimez tous les champs de la section Par défaut.
   1. Cliquez sur l’onglet **Éléments de contenu** et ajoutez une nouvelle section, puis ajoutez un nom pour la section.
   1. Ajoutez des champs à la nouvelle section.
   1. Cliquez sur l’icône **x** pour supprimer la **section par défaut**.
1. Cliquez sur n’importe quel champ, puis utilisez les commandes du panneau de droite du formulaire pour définir leur taille ou l’une des informations suivantes :

   * **Libellé** : il s&#39;agit du nom du champ tel qu&#39;il apparaîtra sur le formulaire de demande. Le nom du champ d’enregistrement n’est pas modifié.
   * **Instructions** : ajoutez plus d’informations sur le champ .
   * **Rendre un champ obligatoire** : lorsqu’il est sélectionné, le champ doit avoir une valeur. Dans le cas contraire, le formulaire ne peut pas être envoyé.
   * **Ajouter une logique** : définissez les conditions qui doivent être remplies pour que le champ s’affiche ou soit masqué.

   >[!TIP]
   >
   >   Le type de champ de chaque champ s’affiche dans la partie supérieure du panneau de droite, une fois que vous avez sélectionné le champ dans le formulaire.
   >     

1. (Facultatif) Cliquez sur l’onglet **Éléments de contenu** sur le côté gauche du formulaire, puis ajoutez l’un des éléments suivants :

   * **Texte descriptif**
   * **Saut de section**

   Pour plus d’informations sur la création d’un formulaire personnalisé, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Cliquez sur l’onglet **Automatisations** sur le côté gauche du formulaire, puis effectuez l’une des opérations suivantes :

   * Sélectionner un modèle de projet
   * Joindre des formulaires personnalisés
   * Définir un propriétaire de projet
   * Ajouter le projet à un portefeuille ou à un programme

   Toutes les sélections que vous effectuez ici seront appliquées aux projets créés à partir de ce formulaire de saisie.

1. (Facultatif) Cliquez sur **Aperçu** pour voir comment le formulaire s’affichera pour les autres utilisateurs lorsqu’ils l’utiliseront pour envoyer un nouvel enregistrement.

1. (Facultatif) Cliquez sur l’onglet **Configuration**, puis ajoutez au moins un utilisateur ou une équipe&lt; au champ **Approbateurs** pour approuver les nouvelles demandes de ce formulaire de réception.

   * Lorsque vous associez un formulaire de réception à des approbateurs, toute nouvelle demande doit d&#39;abord être approuvée par tous les approbateurs avant de générer un projet.
   * Vous pouvez ajouter un ou plusieurs approbateurs à un formulaire de réception.
   * Si au moins un approbateur rejette la demande, celle-ci est rejetée et le projet n’est pas créé.
   * Tous les approbateurs doivent prendre une décision avant qu&#39;un projet ne soit approuvé ou rejeté.
   * Si une équipe est définie en tant qu&#39;approbateur, une seule décision est requise de la part de l&#39;équipe.

     Pour plus d’informations sur l’ajout d’approbations à des formulaires de demande, voir [ Ajouter une approbation à un formulaire de demande ](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du formulaire dans l’en-tête, puis cliquez sur **Modifier** pour mettre à jour le nom du formulaire.

1. Cliquez sur **Publier** pour publier le formulaire et obtenir un lien unique pour celui-ci.

   Les événements suivants se produisent :

   * Le bouton **Publier** est supprimé.
   * Le bouton **Dépublier** est ajouté au formulaire. Cliquez dessus pour empêcher l’accès au formulaire.
   * Un bouton **Partager** est ajouté au formulaire.
   * Le formulaire est alors disponible dans la zone Demandes du menu principal de Workfront.

1. Cliquez sur **Partager** pour partager le formulaire avec d’autres personnes.
1. Cliquez sur la flèche pointant vers la gauche du nom du formulaire dans l’en-tête pour fermer le formulaire.

   La vue du tableau **Formulaires de demande** s’ouvre et le formulaire y est ajouté.

1. (Facultatif) Passez la souris sur le nom d’un formulaire de demande en mode Tableau, puis cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du formulaire, puis cliquez sur l’une des options suivantes :

   * **Modifier le formulaire** : cliquez sur cette option pour modifier davantage les informations du formulaire.
   * **Dépublier** : cliquez sur cette option pour dépublier le formulaire et le supprimer de la zone des Demandes dans Workfront.
   * **Partager** : cliquez sur cette option pour modifier la personne qui a accès au formulaire.
   * **Copier le lien** : cliquez sur cette option pour copier rapidement le lien du formulaire de demande sans ouvrir le formulaire.
   * **Supprimer** : cliquez sur cette icône pour supprimer le formulaire. Toutes les demandes et tous les enregistrements ajoutés à l’aide du formulaire ne sont pas supprimés. Le formulaire ne peut pas être récupéré.

   >[!NOTE]
   >
   >Vous pouvez identifier les formulaires de saisie de projet en mode Tableau, car ils affichent « Projet » dans la colonne Type d’objet.

1. Cliquez sur la flèche pointant vers la gauche de **Formulaires de demande** dans l’en-tête pour fermer le tableau des formulaires de demande.

