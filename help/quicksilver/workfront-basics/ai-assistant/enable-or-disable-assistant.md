---
title: Activer ou désactiver l’assistant IA.
content-type: reference
description: Vous pouvez contrôler les niveaux d’accès de votre organisation qui ont accès à l’assistant AI.
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 14%

---

# Activer ou désactiver l’assistant IA.

En tant qu’administrateur ou administratrice Workfront, vous pouvez contrôler quels utilisateurs et utilisatrices de votre organisation ont activé l’assistant AI. Cela est géré par le biais de niveaux d’accès.

Vous devez activer l’assistant AI pour votre organisation avant de pouvoir l’activer pour un niveau d’accès.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Activer ou désactiver l’assistant d’IA pour votre organisation

Pour activer l’assistant d’IA pour votre entreprise :

{{step-1-to-setup}}

1. Sélectionnez **Système** dans le volet de navigation de gauche, puis sélectionnez **Préférences**.
1. Faites défiler l’écran jusqu’à la section **Préférences IA**.
1. Activez le bouton bascule **Activer l’IA**.

>[!IMPORTANT]
>
>Vous devez disposer d’un accord Gen AI signé enregistré avec Adobe avant de pouvoir utiliser l’assistant AI.
>Pour plus d’informations sur le contrat Gen AI, consultez la section [Signer le contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) dans l’article Assistant AI de Workfront.

## Activer ou désactiver l’assistant AI pour un niveau d’accès

Pour activer l’assistant AI pour un niveau d’accès donné :

{{step-1-to-setup}}

1. Sélectionnez **Niveaux d’accès** dans le volet de navigation de gauche.
1. Sélectionnez le niveau d’accès souhaité, puis cliquez sur l’icône **Modifier** ![Modifier](assets/edit-icon.png) au-dessus de la liste.
1. Dans la zone **Définir des restrictions supplémentaires...** de la case **Modifier le niveau d’accès**, désélectionnez la case **Désactiver l’assistant Workfront AI**.
1. Cliquer sur **Enregistrer**.
1. Répétez les étapes 3 à 5 pour chaque niveau d’accès pour lequel vous souhaitez activer l’assistant AI.



>[!NOTE]
>
>* L’assistant AI est désactivé par défaut pour les utilisateurs non-administrateurs.
>* Si un non-administrateur interagit avec l’icône de l’assistant AI dans Workfront, le contrat de l’assistant AI s’affiche, demandant au non-administrateur d’accepter les conditions générales. S’ils acceptent le contrat, ils peuvent utiliser l’assistant AI même si celui-ci est désactivé dans leur modèle de mise en page.

