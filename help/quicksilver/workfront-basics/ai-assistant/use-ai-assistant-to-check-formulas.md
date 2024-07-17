---
title: Révision des formules de champ calculé à l’aide de l’assistant AI
content-type: reference
description: Vous pouvez utiliser l’assistant d’intelligence artificielle pour résoudre les erreurs de vos expressions personnalisées non valides dans les champs calculés.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 6dd2fd4d688514540265fa3b0d2634194fb6a7ab
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Révision des formules de champ calculé à l’aide de l’assistant AI

Vous pouvez utiliser l’assistant d’intelligence artificielle pour résoudre les erreurs de vos expressions personnalisées non valides dans les champs calculés.

Lorsque vous créez le champ calculé dans le créateur de formulaires personnalisé, un message d’erreur s’affiche sous le champ si la formule n’est pas valide.

![Erreur d’expression non valide](assets/invalid-expression.png)

L’assistant d’IA peut vous aider à réviser votre formule en une expression de champ calculé valide.

## Modification d’une expression de champ calculée

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

Pour plus d’informations sur les champs calculés dans Workfront, voir [Ajout de données calculées à un formulaire personnalisé avec l’ancien créateur de formulaires](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
