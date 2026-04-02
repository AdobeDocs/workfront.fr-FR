---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Configuration des collaborateurs d’IA
description: En tant qu’administrateur Adobe Workfront, vous pouvez configurer des collaborateurs IA et les affecter à des projets et à des tâches.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 25c4d4435cc3507ab2d163600a8c42be66efd4c2
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 7%

---

# Configuration des collaborateurs d’IA

{{highlighted-preview-article-level}}

Les collaborateurs AI permettent d’intégrer des agents AI à vos projets et tâches. Vous pouvez configurer un collaborateur d’IA, puis l’affecter comme vous le feriez à un utilisateur.

Par exemple, vous pouvez configurer un collaborateur en IA de type réviseur avec des directives de marque, puis affecter ce collaborateur à la révision d’un document.

Les types de collaborateurs IA disponibles sont les suivants :

* Réviseur : créez un collaborateur à l’aide de marques ou du cerveau de la marque, puis affectez-le en tant que réviseur de ressources.

  Pour plus d’informations, voir [Prise en main de Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

  >[!NOTE]
  >
  >Actuellement, Reviewer est le seul type de collaborateur IA disponible. D’autres fonctionnalités AI Collaborator seront disponibles à l’avenir.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Standard, Prime ou Ultimate</p></td> 
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



* Votre entreprise doit avoir un contrat Adobe Gen AI signé dans son dossier.

  Pour plus d’informations, consultez [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) dans l’article Assistant AI dans Workfront.
* Vous devez avoir configuré une marque dans Workfront avant de pouvoir l’utiliser pour un collaborateur d’IA de type réviseur.

  Pour obtenir des instructions, voir [Créer et gérer des marques pour le réviseur de contenu](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Créer un collaborateur d’IA de type réviseur

{{step-1-to-setup}}

1. Dans le volet de navigation de gauche, cliquez sur **Collaborateurs AI**.
1. Cliquez sur **Nouveau collaborateur** dans le coin supérieur droit de l’écran.
1. Cliquez sur **Réviseur**, puis sur **Continuer**.

   >[!NOTE]
   >
   >Actuellement, seul le type Réviseur est disponible. D’autres types de collaborateurs IA seront disponibles à l’avenir.

1. Dans le champ Nom du collaborateur, entrez le nom du collaborateur. Il s’agit du nom qui apparaît dans la liste des délégataires disponibles pour une tâche.
1. Choisissez si le collaborateur utilisera une marque ou un cerveau de marque pour ses évaluations.
1. (Conditionnel) Si le collaborateur en IA va utiliser un Brand Brain, sélectionnez le client qu’il utilisera.
1. (Conditionnel) Si le collaborateur de l’IA va utiliser une marque, sélectionnez la marque et les instructions qu’il suivra.
1. Cliquez sur **Enregistrer**.

## Gérer les collaborateurs d’IA

Vous pouvez modifier, copier et supprimer des collaborateurs IA existants.

{{step-1-to-setup}}

1. Dans le volet de navigation de gauche, cliquez sur **Collaborateurs AI**.
1. (Conditionnel) Pour modifier un espace de collaboration, cliquez sur le nom de l&#39;espace de collaboration que vous souhaitez modifier, apportez des modifications dans la fenêtre Modifier l&#39;espace de collaboration, puis cliquez sur **Enregistrer**.
1. (Conditionnel) Pour copier un espace de collaboration, cliquez sur l&#39;icône Copier ![icône Copier](assets/copy-ai-collaborator.png) dans la ligne de l&#39;espace de collaboration IA que vous souhaitez copier, cliquez sur le nom de la copie, apportez des modifications dans la fenêtre Modifier l&#39;espace de collaboration, puis cliquez sur **Enregistrer**.
1. (Conditionnel) Pour supprimer un espace de collaboration, cliquez sur l’icône Supprimer ![icône Supprimer](assets/delete-collaborator-icon.png) dans la ligne de l’espace de collaboration IA que vous souhaitez supprimer, puis cliquez sur **Supprimer**.
