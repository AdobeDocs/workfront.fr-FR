---
title: Vérifier des formules de champ calculé à l’aide de l’assistant AI
content-type: reference
description: Vous pouvez utiliser l’assistant d’intelligence artificielle pour résoudre les erreurs de vos expressions personnalisées non valides dans les champs calculés.
author: Becky
feature: Get Started with Workfront
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 09c05db7c6a5db7db74dd95ca323415f4318489d
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 16%

---

# Génération ou révision de formules de champ calculé à l’aide de l’assistant AI

Vous pouvez utiliser l’assistant d’IA pour générer des formules en fonction d’une invite que vous fournissez. Vous pouvez également résoudre les erreurs de vos expressions personnalisées non valides dans les champs calculés.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td><p>Nouveau : Prime ou Ultimate</p>
       <p>ou</p>
       <p>Actuel : non disponible</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Nouveau : Standard</p>
       <p>ou</p>
       <p>Actuel : non disponible</p></td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Générer une expression de champ calculé

## Modification d’une expression de champ calculée

Lorsque vous créez le champ calculé dans le créateur de formulaires personnalisé, un message d’erreur s’affiche sous le champ si la formule n’est pas valide.

![Erreur d’expression non valide](assets/invalid-expression.png)

L’assistant d’IA peut vous aider à réviser votre formule en une expression de champ calculé valide.

Pour réviser une expression de champ calculé non valide :

1. Cliquez sur l’icône **Assistant IA** ![Icône Assistant IA](assets/ai-assistant-icon.png) près du coin supérieur droit de l’écran.
1. dans la zone d’invite située au bas du panneau de l’assistant d’IA, saisissez une invite du type :
   `Rewrite this formula to remove the invalid expression error`
1. Copiez l’expression non valide à partir du créateur de formulaires personnalisé et collez-la dans la zone d’invite.
1. Appuyez sur **Entrée**.

   L’assistant d’IA peut prendre quelques instants pour générer la formule révisée, en fonction de la taille ou de la complexité de la formule.
1. Affichez la formule révisée dans le panneau de l’assistant d’IA.
1. (Facultatif) Copiez la formule révisée à partir du panneau de l’assistant d’IA, puis collez-la dans le champ calculé du créateur de formulaires personnalisé.

>[!NOTE]
>
>Nous vous recommandons de tester le champ calculé pour vous assurer qu’il récupère le résultat attendu.

Pour plus d’informations sur les champs calculés dans Workfront, voir [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

