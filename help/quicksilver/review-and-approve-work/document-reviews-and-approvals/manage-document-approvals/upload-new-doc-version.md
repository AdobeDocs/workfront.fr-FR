---
product-area: documents
navigation-topic: approvals
title: Charger une nouvelle version du document et demander une approbation
description: Vous pouvez charger une nouvelle version du document et demander l’approbation d’autres utilisateurs dans Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 162f63d52c97c6d4894d35565c68eb2858369b53
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 54%

---

# Charger une nouvelle version du document et demander une approbation

Si un document marqué a besoin d’être retravaillé lors d’une révision précédente, vous pouvez charger une nouvelle version dans le document d’origine et commencer une nouvelle série d’approbations. Une fois que vous avez chargé une nouvelle version du document, les versions précédentes sont verrouillées.

Si le nom de fichier de la nouvelle version est différent de celui de la version précédente, Workfront affiche le document avec le nom de fichier le plus récent.

Lorsqu&#39;une nouvelle version est ajoutée à un document avec des approbations en attente, l&#39;approbation de la version précédente indique Retiré. Le processus d’approbation précédent se termine, même si certains participants n’ont pas encore pris de décision.

Si la dernière version du document est supprimée, les versions précédentes restent verrouillées. Si vous devez modifier une version précédente, vous devez la déverrouiller manuellement.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Actuelle : demande ou niveau supérieur</p>
   ou
   <p>Nouvelle : contributeur ou supérieure</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès Modifier à l’objet associé au document</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Faire glisser et déposer pour ajouter une nouvelle version

>[!NOTE]
>
>Glisser-déposer ne fonctionne pas avec Internet Explorer.

1. Accédez à la zone Documents dans laquelle le document est chargé.
1. Depuis votre poste de travail ou un onglet de navigateur distinct, faites glisser la nouvelle version du document au-dessus de la version existante dans Workfront.

   Lorsque vous faites glisser la nouvelle version, vous pouvez pointer sur un dossier de documents Workfront pour l’ouvrir. Vous pouvez ensuite faire défiler vers le haut ou vers le bas en faisant glisser les fichiers vers le haut ou le bas de l’écran.

1. Déposez la nouvelle version au-dessus du fichier existant sur l’onglet **Documents**.

1. Une fois le document téléchargé, cliquez dessus et ouvrez le panneau Résumé du document .

1. Faites défiler la page jusqu’à la section **Approbations** dans le volet Résumé du document, puis cliquez sur **Ajouter**.

![](assets/doc-summary-add-approvers.png)

1. (Facultatif) Définissez une date limite pour l’approbation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant l’échéance spécifiée.

1. Pour ajouter rapidement des réviseurs et des approbateurs à partir de la version précédente, cliquez sur le bouton d’ajout en regard de leurs noms répertoriés ci-dessous.
   <!--need screenshot when working-->

1. (Facultatif) modifiez le rôle de l’approbateur/réviseur.

1. Pour ajouter de nouveaux approbateurs et validants, cliquez sur **Réviseur** ou **Approbateur** et commencez à saisir l’utilisateur, l’utilisatrice ou l’équipe.

   ![](assets/add-approver-and-deadline.png)
