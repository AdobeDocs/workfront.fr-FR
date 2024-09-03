---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Définir une épreuve avec un workflow automatisé dans  [!DNL Workfront Proof]
description: Il s’agit d’une répétition des informations contenues dans l’article « Configurer des épreuves dans Workfront ». Consolidez ici ou là. Peut-être mieux ici.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 100%

---

# Définir une épreuve avec un workflow automatisé dans [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Cet article fait référence à la fonctionnalité du produit autonome [!DNL Workfront Proof]. Pour plus d’informations sur la relecture dans [!DNL Adobe Workfront], voir [Relecture](../../../review-and-approve-work/proofing/proofing.md).

Le workflow automatisé facilite la gestion de la révision et de l&#39;approbation des contenus lorsque vous avez des processus de révision complexes ou si vous envoyez régulièrement des contenus à réviser aux mêmes groupes de personnes.

Vous créez l’épreuve, puis elle passe d’une étape à l’autre jusqu’à l’approbation finale. Les utilisateurs et utilisatrices concernés sont avertis lorsqu’ils sont tenus d’effectuer une approbation.

![stages_diagram.png](assets/stages-diagram-350x81.png)

Vous pouvez ajouter un workflow automatisé à une épreuve lors du chargement du document, ou après son chargement.

## Créer une épreuve avec un workflow automatisé

1. Commencez à créer l’épreuve.
1. Dans la section **[!UICONTROL Partager]**, cliquez sur **[!UICONTROL Utiliser un workflow automatisé]**.

   Vous pouvez désélectionner cette option pour revenir à un workflow standard.

1. (Facultatif) Si vous souhaitez utiliser un modèle de workflow automatisé que votre administrateur ou administratrice [!DNL Workfront] a configuré et partagé avec vous, sélectionnez-le dans le menu déroulant **[!UICONTROL Sélectionner un modèle de workflow]**.

   >[!NOTE]
   >
   >Votre capacité à modifier le modèle dépend des paramètres du modèle configurés par l’administrateur ou administratrice [!DNL Workfront]. Si la possibilité de modifier le modèle est désactivée, seule la personne propriétaire du modèle peut le modifier.

1. Indiquez les informations suivantes pour configurer la première étape du workflow automatisé :

   * **[!UICONTROL Nom] :** le nom de l’étape apparaît sur le diagramme de workflow et est inclus dans les notifications par e-mail envoyées aux réviseurs et réviseuses.
   * **[!UICONTROL Date d’échéance] :** la fonctionnalité de ce champ diffère selon l’option sélectionnée dans la liste déroulante **[!UICONTROL Date d’échéance calculée à partir de]**.

   * **[!UICONTROL À partir de la création de l’épreuve] :** sélectionnez la date d’échéance pour l’épreuve.
   * **[!UICONTROL À partir de l’activation de l’étape] :** sélectionnez le nombre de jours ouvrables qui seront ajoutés à la date d’activation de l’étape pour définir automatiquement une date d’échéance pour l’épreuve.
   * **[!UICONTROL Activer l’étape] :** pour chaque étape de votre workflow, vous pouvez décider quand elle doit être activée. Pour votre première étape, les options suivantes sont disponibles.

      * Lors de la création des épreuves
      * À une date et une heure précises
      * Manuellement

        Des options supplémentaires sont disponibles pour les étapes suivantes. Ces options nécessitent une étape parent. Il s’agit de :
      * Une fois que la date d’échéance précédente est atteinte.
      * Toutes les décisions sont approuvées ou approuvées avec modifications.
      * Toutes les décisions sont approuvées.
      * Toutes les décisions sont prises.
   * **[!UICONTROL Date d’échéance calculée à partir de] :** l’option que vous sélectionnez dans cette liste déroulante affecte les options disponibles dans le champ **[!UICONTROL Date d’échéance]**.

   * **[!UICONTROL Création d’une épreuve] :** dans le champ **[!UICONTROL Date d’échéance]**, sélectionnez la date d’échéance pour l’épreuve.

   * **[!UICONTROL Activation de l’étape] :** dans le champ **[!UICONTROL Date d’échéance]**, sélectionnez le nombre de jours ouvrables qui seront ajoutés à la date d’activation de l’étape pour définir automatiquement une date d’échéance pour l’épreuve.

   * **[!UICONTROL Verrouiller l’étape] :** permet de sélectionner le moment où l’étape peut être verrouillée.
   * **[!UICONTROL Personne décisionnaire principale] :** sélectionnez la personne décisionnaire principale de l’étape. Les personnes décisionnaires ne sont disponibles dans la liste déroulante qu’après l’ajout de réviseurs et réviseuses à l’étape.
   * **[!UICONTROL Une seule décision requise] :** sélectionnez cette option pour que la révision soit terminée après que l’une des personnes décisionnaires a pris sa décision.

     Cette option n’est pas disponible si vous avez désigné un utilisateur ou une utilisatrice dans le menu déroulant **[!UICONTROL Personne décisionnaire principale]**.

   * **[!UICONTROL Étape privée] :** lorsque cette option est sélectionnée, les commentaires et les décisions ne sont pas visibles pour les personnes qui ne sont pas ajoutées à cette étape ou qui ne font pas partie de la supervision, de l’administration ou de l’administration de facturation dans le compte.


1. (Facultatif) Ajoutez des réviseurs et réviseuses à l’étape.
1. Tenez compte des éléments suivants lorsque vous ajoutez des réviseurs et réviseuses :

   * Une personne chargée dela révision ne peut être ajoutée à une épreuve qu’une seule fois. (Vous ne pouvez pas ajouter la même personne à plus d’une étape de l’épreuve).
   * Les personnes en charge de la révision qui sont ajoutées à une étape privée ne peuvent voir que l’étape à laquelle elles ont été ajoutées dans l’épreuve et les commentaires faits dans cette étape.
   * Par défaut, l’ajout d’un utilisateur ou d’une utilisatrice à une étape lui donne accès pour afficher l’épreuve à partir du moment où l’épreuve est créée.\

     L’administrateur ou l’administratrice du système peut configurer le système de vérification pour empêcher des personnes d’accéder à l’épreuve jusqu’à ce que le workflow entre dans l’étape où la personne a été ajoutée. Pour plus d’informations, consultez les ressources suivantes :

1. (Facultatif) Cliquez sur **[!UICONTROL Nouvelle étape]**, puis répétez les étapes 4 et 5 pour ajouter plusieurs étapes au workflow automatisé.
1. Poursuivez la création de l’épreuve en spécifiant les informations nécessaires dans les sections [!UICONTROL Organiser] et [!UICONTROL Autres paramètres] de la page [!UICONTROL Nouvelle épreuve], comme décrit dans la section

## Diagrammes de workflows automatisés

Lors de la configuration du workflow pour votre épreuve, vous remarquerez qu’un diagramme est créé. Chaque étape que vous ajoutez à votre épreuve apparaîtra dans le diagramme, indiquant clairement les dépendances entre les étapes. Les étapes privées sont marquées avec une icône de clé.

Le diagramme est flottant, ce qui signifie qu’il restera visible, même si vous faites défiler la page vers le bas.

Si vous n’avez pas besoin de voir le diagramme, vous pouvez le masquer (1).

![Diagram.png](assets/diagram-350x93.png)

## Ajouter une étape

Vous pouvez ajouter une étape supplémentaire à un workflow que vous êtes en train de créer ou de modifier.

1. Si vous ajoutez une étape à une épreuve existante, accédez à la page Détails de l’épreuve, tel que décrit dans la section [Gérer les détails de l’épreuve dans  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Dans la section **[!UICONTROL Workflow]**, cliquez sur **[!UICONTROL Nouvelle étape]**.

1. Spécifiez les informations relatives à l’étape, comme indiqué au point 4 de la section [!UICONTROL Créer une épreuve avec un workflow automatisé] de cet article.
1. Cliquez sur **[!UICONTROL Ajouter une étape]**, puis cliquez sur **[!UICONTROL Terminé]**.

## Supprimer une étape

1. Cliquez sur l’icône de la corbeille présente en haut à droite de l’étape (1).\
   L’icône apparaît lorsque vous survolez l’étape.\
   ![deleting_a_stage.png](assets/deleting-a-stage-350x250.png)

## Paramètres de l’étape

* **[!UICONTROL Nom de l’étape]** : apparaît sur le diagramme de workflow et est inclus dans les notifications par e-mail envoyées aux équipes de révision.
* **[!UICONTROL Activer l’étape]** : pour chaque étape de votre workflow, vous pouvez décider du moment où elle doit être activée. Pour la première étape, les options suivantes sont disponibles :

   * Lors de la création des épreuves
   * À une date et une heure précises
   * Manuellement
   * Seules ces trois options sont disponibles pour la première étape. Les autres options seront disponibles lorsque vous ajouterez une deuxième étape. Elles nécessitent la sélection d’une étape parent.
   * Après l’échéance précédente (nécessite de choisir une étape parent).
   * Toutes les décisions sont approuvées ou [!UICONTROL approuvées avec modifications] (nécessite de choisir une étape parent).
   * Toutes les décisions sont approuvées (nécessite de choisir une étape parent).
   * Toutes les décisions sont prises (nécessite de choisir une étape parent).

* **[!UICONTROL Échéance] :** vous pouvez choisir le mode de calcul de la date limite à chaque étape d’un workflow. Les options sont les suivantes :

   * À partir de la création de l’épreuve : dans le champ [!UICONTROL Échéance] (9), vous pouvez sélectionner la date limite de l’épreuve.
   * À partir de l’activation de l’étape : dans le menu déroulant [!UICONTROL Échéance], vous pouvez sélectionner le nombre de jours ouvrables qui seront ajoutés à la date d’activation de l’étape pour fixer automatiquement une date limite pour l’épreuve.

* **[!UICONTROL Verrouiller] :** il existe plusieurs options qui déterminent le moment où une étape peut être verrouillée. Les options sont les suivantes :

   * Verrouillage manuel
   * Jamais
   * Lorsque l’étape suivante commence.
   * Lorsque toutes les décisions sont prises.

**[!UICONTROL Personne décisionnaire principale]** : vous définissez qui est la personne décisionnaire principale de l’étape. Les personnes décisionnaires disponibles n’apparaissent dans la liste qu’une fois les équipes de révision ajoutées à l’étape.

>[!NOTE]
>
>Si vous choisissez une personne décisionnaire principale, l’option « Une seule décision requise » ne sera plus disponible à cette étape.

* **[!UICONTROL Une seule décision requise]** : vous pouvez activer cette option sur une étape. Cela signifie que la révision sera terminée lorsque l’une des personnes décisionnaires aura pris sa décision.
* **[!UICONTROL Confidentialité] :** chaque étape peut être rendue privée. Si une étape est privée, les commentaires et les décisions ne seront pas visibles par les personnes qui n’ont pas été ajoutées à cette étape ou qui ne font pas partie de la supervision, de l’administration ou de l’administration de facturation dans le compte. Pour plus d’informations, voir [Vue d’ensemble des workflows automatisés](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Ajouter des réviseurs et réviseuses à une étape

1. Saisissez un nom de contact ou une adresse e-mail dans le champ situé au bas de chaque étape.
1. Cliquez sur l’icône verte Plus pour les ajouter.
1. Définissez le rôle sur l’épreuve.
1. Définissez l’alerte par e-mail.
1. Lors de la mise en place de la première étape, vous avez également la possibilité de modifier la personne propriétaire de l’épreuve.

   >[!NOTE]
   >
   >* Une personne chargée dela révision ne peut être ajoutée à une épreuve qu’une seule fois. Vous ne pouvez pas ajouter la même personne à plus d’une étape de l’épreuve.
   >* Les personnes en charge de la révision qui ne sont pas ajoutées à une étape privée ne peuvent pas voir l’étape sur l’épreuve ou les commentaires faits dans cette étape.


## Convertir une épreuve en un workflow automatisé

Vous pouvez convertir une épreuve de base en workflow automatisé.

1. Cliquez sur **[!UICONTROL Convertir en workflow automatisé]** sur la page [!UICONTROL Détails de l’épreuve].
Une fois l’épreuve retravaillée par le workflow automatisé, toutes les étapes sont actives et publiques, et l’option [!UICONTROL Verrouiller l’étape] est définie par défaut sur Manuel. Toutes les étapes restent entre les mains des personnes et de leurs paramètres.

   * « Activer l’étape » est réglée sur « À la création de l’épreuve » à chaque étape.
   * L’option « Date d’échéance calculée à partir » est définie sur « À la création de l’épreuve » à chaque étape.
   * Si l’option « Une seule décision » a été sélectionnée pour l’épreuve de base, elle l’est à toutes les étapes.
   * Si une [!UICONTROL personne décisionnaire principale] a été sélectionnée pour l’épreuve de base, les étapes avec cette personne destinataire sont définies comme étant les siennes et toutes les autres sont définies sur Aucun.
   * Le nom de l’étape reste le même.

## Ajouter un modèle supplémentaire à un workflow automatisé existant

Une fois qu’une épreuve de base a été convertie en workflow automatisé, vous pouvez y ajouter des modèles supplémentaires.

1. Sur la page Détails de l’épreuve, dans la section Workflow, cliquez sur **[!UICONTROL Ajouter un modèle].**

   * Les paramètres du modèle déterminent ce qui peut être fait avec une épreuve à laquelle ce modèle a été ajouté. Par exemple, si les options [!UICONTROL Ajouter une étape et Ajouter des personnes aux étapes] sont désactivées dans le modèle, les boutons [!UICONTROL ajouter une étape] et [!UICONTROL partager l’épreuve] ne seront pas visibles.
   * Si l’option [!UICONTROL Ajouter une étape] est désactivée dans le modèle donné, le bouton [!UICONTROL Ajouter un modèle] n’est pas visible après son ajout.
   * Lorsqu’une personne est ajoutée à une étape dans un modèle de workflow automatisé, mais qu’elle est déjà présente dans l’épreuve, si ce modèle est appliqué, le système supprimera automatiquement cette personne de l’étape. Si personne d’autre n’a été ajouté à cette étape particulière, l’erreur suivante s’affiche, car le système ne permet pas d’ajouter une étape vide au workflow.

     ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
