---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: Configuration des collaborateurs d’IA
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer des collaborateurs IA et les affecter à des projets et à des tâches.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 3%
---
# Configuration des collaborateurs d’IA

Les collaborateurs AI permettent d’intégrer des agents AI à vos projets et tâches. Vous pouvez configurer un collaborateur d’IA, puis l’affecter comme vous le feriez à un utilisateur.

Par exemple, vous pouvez configurer un collaborateur en IA de type réviseur avec des directives de marque, puis affecter ce collaborateur à la révision d’un document.

Les types de collaborateurs IA disponibles sont les suivants :

* Réviseur AI : créez un collaborateur à l’aide de marques ou de Adobe Brand Intelligence, puis affectez-le en tant que réviseur de ressources.

  Pour plus d’informations, voir [Prise en main du réviseur de l’IA dédiée à Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Agent de travail : créez un collaborateur à l’aide de Copilote ou de Writer, puis affectez le collaborateur à une tâche pour effectuer un travail au niveau de la tâche.

  Pour plus d’informations, voir [Utilisation des agents de travail](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Select, Prime ou Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

### Pour les réviseurs d’IA :

* Votre entreprise doit avoir un contrat Adobe Gen AI signé dans son dossier.

  Pour plus d’informations, consultez [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) dans l’article Assistant AI dans Workfront.
* Vous devez avoir configuré une marque dans Workfront avant de pouvoir l’utiliser pour un réviseur de l’IA.

  Pour obtenir des instructions, voir [Créer et gérer des marques pour l’AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Pour utiliser Adobe Brand Intelligence pour un réviseur d’IA, votre entreprise doit utiliser l’expérience de révision et d’approbation unifiée dans Workfront.

  Pour plus d’informations, voir [Prise en main de la révision et de l’approbation unifiées](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

### Pour les agents de travail

Vous devez configurer un agent dans Claude, Copilot Studio ou Writer avant de pouvoir l&#39;utiliser comme agent de travail.

## Créer un réviseur d’IA

Les réviseurs d’IA peuvent être configurés pour utiliser les marques Workfront ou Adobe Brand Intelligence.

* **Marques** : les marques sont créées dans Workfront. Vous pouvez créer des marques dans Workfront en chargeant des fichiers PDF qui contiennent vos directives de marque ou en saisissant manuellement des éléments de marque.
* **&#x200B;**&#x200B;: lorsqu’un collaborateur d’IA révise une ressource à l’aide de Adobe Brand Intelligence, vous pouvez afficher les commentaires du réviseur d’IA dans Frame.io.


{{step-1-to-setup}}

1. Dans le volet de navigation de gauche, cliquez sur **Collaborateurs AI**.
1. Cliquez sur **Nouveau collaborateur** dans le coin supérieur droit de l’écran.
1. Cliquez sur **Réviseur**, puis sur **Continuer**.
1. Dans le champ Nom du collaborateur, entrez le nom du collaborateur. Il s’agit du nom qui apparaît dans la liste des délégataires disponibles pour une tâche.
1. Choisissez si le collaborateur utilisera une marque ou un Adobe Brand Intelligence pour ses révisions.
1. (Conditionnel) Si le collaborateur de l’IA va utiliser une marque, sélectionnez la marque et les instructions qu’il suivra.
1. Cliquer sur **Enregistrer**.

## Configuration d’un agent de travail

Les agents de travail sont des agents que vous pouvez affecter à des tâches dans Workfront. Vous configurez l’agent de travail avec un nom, un niveau d’accès et d’autres détails, puis vous l’affectez à une tâche comme vous le feriez pour un utilisateur.

Les agents de travail étant des agents, leurs actions et capacités sont configurées à l’emplacement où vous configurez vos agents. Actuellement, les agents utilisés comme agents de travail peuvent être créés dans Copilot Studio, Claude ou Writer.

Les agents de travail ne peuvent être affectés qu&#39;à des tâches et ne peuvent actuellement être affectés à des événements.

Pour obtenir une liste des bonnes pratiques à suivre lors de la création d’un agent pour travailler en tant qu’agent de travail, voir [Bonnes pratiques pour créer un agent pour un agent de travail](#best-practices-for-creating-an-agent-for-a-work-agent).

### Configuration d’un agent de travail dans Workfront

{{step-1-to-setup}}

1. Dans le volet de navigation de gauche, cliquez sur **Collaborateurs AI**.
1. Cliquez sur **Nouveau collaborateur** dans le coin supérieur droit de l’écran.
1. Sélectionnez **Agents de travail**, puis cliquez sur **Continuer**.
1. Dans le champ Nom du collaborateur de l’IA, saisissez un nom pour le collaborateur. Il s’agit du nom qui apparaît dans la liste des délégataires disponibles pour une tâche.
1. Dans le champ Description du collaborateur de l’IA, saisissez une description de l’objectif du collaborateur ou des actions qu’il effectue.
1. Dans le champ Niveau d&#39;accès , sélectionnez un niveau d&#39;accès pour ce collaborateur. Ce niveau d’accès contrôle ce que le collaborateur peut faire, de la même manière qu’un niveau d’accès contrôle ce qu’un utilisateur peut faire.
1. Dans la zone **Choisir l’origine de l’agent**, indiquez si vous souhaitez connecter un agent créé sur une plateforme commune telle que Copilot ou Writer, ou utiliser un agent personnalisé.
1. (Conditionnel) Si vous utilisez un agent provenant d’une plateforme commune, saisissez les détails d’authentification de la plateforme de l’agent :

   | Platform | Authentification requise |
   |---|---|
   | Copilot Studio | Secret de canal web |
   | Claude Managed Agents | Clé API anthropique<br>ID d’agent<br>ID d’environnement |
   | Rédacteur | Clé API<br>ID de l’application |

1. Cliquez sur **Tester la connexion**. Vous pouvez ainsi savoir si la connexion a été correctement configurée.
1. Dans la zone **Une fois le travail du collaborateur terminé, il peut** activer/désactiver les actions que vous souhaitez que le collaborateur effectue.
1. Cliquer sur **Enregistrer**.

Pour plus d’informations sur les agents de travail, y compris sur la manière de les affecter à des tâches, voir [Utiliser des agents de travail](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


### Bonnes pratiques relatives à la création d’un agent pour un agent de travail

Les bonnes pratiques suivantes peuvent s’avérer utiles lors de la création d’un agent à utiliser comme agent de travail dans Workfront. Pour afficher les bonnes pratiques, cliquez sur la section de l’application dans laquelle vous créez l’agent.

+++ Claude

1. Accédez à la console Claude sur [platform.claude.com](https://platform.claude.com/).
1. Créez une clé API.
   1. Sous Clés API, cliquez sur **Créer une clé** dans le coin supérieur droit.
   1. Indiquez un nom et une date d’expiration.
   1. Copiez la clé et enregistrez-la dans un endroit sûr et sécurisé. Vous aurez besoin de cette clé pour configurer l’agent de travail dans Workfront.

1. Créer un environnement.
   1. Sous **Agents gérés** > **Environnements**, cliquez sur **Créer un environnement** dans le coin supérieur droit.
   1. Indiquez un nom et un type d’hébergement, le cas échéant.
   1. Configurez les packages et métadonnées partagés selon les besoins. Les environnements peuvent être réutilisés sur plusieurs agents et permettent de partager des packages et des métadonnées.
      L’identifiant d’environnement s’affiche sous le nom de l’environnement dans le coin supérieur gauche.

1. Créez un agent.
   1. Sous Agents gérés > Agents, cliquez sur **Créer un agent** dans le coin supérieur droit.
   1. Attribuez un nom, un modèle, une invite système, des compétences et des outils, le cas échéant. Soyez explicite, car les agents de travail transmettent le contexte de la tâche à cet agent, qui exécute ensuite le travail.
      L’ID de l’agent s’affiche sous le nom de l’agent dans le coin supérieur gauche.

1. Configurez l’agent de travail dans Workfront.
   1. Saisissez votre clé API, votre identifiant d’environnement et votre identifiant d’agent
   1. Cliquez sur **Tester la connexion** pour vérifier.

1. Affectez l’agent de travail à une tâche Workfront.
   1. L’agent de travail se déclenche une fois toutes les tâches antérieures terminées.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Rédacteur

>[!NOTE]
>
> Vous pouvez utiliser un agent Principal en tant qu’agent de travail, mais les playbooks de Principal ne peuvent pas être utilisés en tant qu’agents de travail.

Lors de la création d’un agent à utiliser comme agent de travail dans Writer, nous recommandons le workflow suivant.

Vous trouverez des informations plus détaillées sur la création d’agents dans la [documentation du rédacteur](https://dev.writer.com/no-code/introduction).

1. Créez une application sans code dans Writer AI Studio.
1. Ajoutez un seul champ de saisie de texte. Vous pouvez utiliser le nom par défaut « Entrée de texte ».
1. Ajoutez des `@TextInput` à l’invite. Dans la section Invites de la configuration de l’application, assurez-vous que votre modèle d’invite référence la variable d’entrée. Sans cela, le modèle ne voit jamais les données de la tâche.
1. Ajustez votre invite pour générer la sortie immédiatement. Supprimez toutes les instructions qui demandent à l’utilisateur une clarification ou un contexte supplémentaire avant de répondre. Par exemple : « Lorsque vous recevez une entrée, traitez-la comme une requête de génération de contenu et générez immédiatement la sortie. Ne demandez pas d&#39;éclaircissements. »
1. Copiez votre clé API et votre ID d’application. Vous en aurez besoin pour configurer l’agent de travail dans Workfront.

   * Pour obtenir des instructions sur la configuration d’une clé API dans Writer, voir [Quickstart](https://dev.writer.com/home/quickstart) dans la documentation Writer.
   * Pour obtenir des instructions sur la configuration d’un ID d’application dans Writer, consultez la section [Appeler des agents sans code via l’API](https://dev.writer.com/home/applications) dans la documentation du Writer.

1. Configurez l’agent de travail dans Workfront. Dans le cadre de la configuration, saisissez votre clé API et votre ID d’application, puis cliquez sur **Tester la connexion** pour vérifier.
1. Affectez l’agent de travail à une tâche Workfront. L’agent de travail commence à travailler une fois que toutes les tâches antérieures de la tâche sont terminées.

+++

## Gérer les collaborateurs d’IA

Vous pouvez modifier, copier et supprimer des collaborateurs IA existants.

{{step-1-to-setup}}

1. Dans le volet de navigation de gauche, cliquez sur **Collaborateurs AI**.
1. (Conditionnel) Pour modifier un espace de collaboration, cliquez sur le nom de l&#39;espace de collaboration que vous souhaitez modifier, apportez des modifications dans la fenêtre Modifier l&#39;espace de collaboration, puis cliquez sur **Enregistrer**.
1. (Conditionnel) Pour supprimer un espace de collaboration, cliquez sur l’icône Supprimer ![icône Supprimer](assets/delete-collaborator-icon.png) dans la ligne de l’espace de collaboration IA que vous souhaitez supprimer, puis cliquez sur **Supprimer**.
