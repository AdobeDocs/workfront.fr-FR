---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuration des paramètres de BAT par défaut
description: Ces paramètres vous permettent de définir des valeurs par défaut qui s’appliquent à toutes les épreuves créées par vos utilisateurs et utilisatrices. Toutefois, les utilisateurs et utilisatrices peuvent remplacer la plupart de ces paramètres lors de la création d’une épreuve.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: 5676910e53f1c4f49cab196e42bfbce8704887ca
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 99%

---

# Configurer les paramètres d’épreuve par défaut

Ces paramètres vous permettent de définir des valeurs par défaut qui s’appliquent à toutes les épreuves créées par vos utilisateurs et utilisatrices. Toutefois, les utilisateurs et utilisatrices peuvent remplacer la plupart de ces paramètres lors de la création d’une épreuve.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td>
   <p>Nouveau : Standard</p>
   ou
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront. Pour plus d’informations sur les administrateurs et administratrices Workfront, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder un accès administratif complet à un utilisateur ou une utilisatrice</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configurer les paramètres par défaut des nouvelles épreuves

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Épreuves** > **Paramètres des épreuves**.
1. Dans la section **Nouvelles valeurs par défaut de l’épreuve**, configurez les paramètres suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Destinataires</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger une connexion</td> 
      <td> <p>Les réviseurs et les réviseuses doivent se connecter à l’aide de leur adresse e-mail et de leur mot de passe avant de pouvoir consulter les épreuves créées dans le compte de votre organisation. Lorsque cette option est activée, les utilisateurs et utilisatrices ne peuvent pas partager l’épreuve avec les réviseurs et les réviseuses invités.</p> <p><b>IMPORTANT</b> : lorsque cette option est activée, la connexion est requise pour toutes les épreuves qui viennent d’être créées.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copier le propriétaire à partir de l’épreuve originale pour les nouvelles versions</td> 
      <td> <p>La personne propriétaire de la première version d’une épreuve est également propriétaire de toutes les versions consécutives de l’épreuve, quel que soit la personne qui a créé ces versions. Ce paramètre est activé par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Autoriser les utilisateurs à supprimer leurs commentaires sur l’épreuve</td> 
      <td>Les utilisateurs et utilisatrices peuvent supprimer leurs propres commentaires. Ce paramètre est activé par défaut.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exiger que les décisions soient signées de manière électronique </td> 
      <td> <p>Les décisionnaires sont invités à saisir leur identifiant de connexion Workfront lorsqu’ils prennent une décision sur une épreuve.</p> <p><b>IMPORTANT</b> : lorsque cette option est activée, les utilisateurs et utilisatrices ne peuvent pas partager l’épreuve avec des réviseurs et des réviseuses invités qui n’ont pas d’informations de connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Échéance</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Définir l’échéance par défaut</td> 
      <td> <p>Le système applique cette échéance à toutes les nouvelles épreuves de votre compte qui n’ont pas de workflow automatisé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informer les destinataires avant que l’épreuve ne soit à risque</td> 
      <td>Les destinataires sont informés par e-mail avant que l’épreuve ne soit considérée comme à risque en fonction de la date d’échéance spécifiée ci-dessus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Notifications par e-mail</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informer les destinataires lorsqu’ils sont ajoutés à une épreuve</td> 
      <td>Les destinataires sont informés par e-mail lorsqu’ils sont ajoutés à une épreuve.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquer sur **Enregistrer**.

## Configurer les décisions sur les épreuves

Les utilisateurs et utilisatrices peuvent utiliser les décisions sur les épreuves pour indiquer le statut de l’épreuve après son examen.

>[!NOTE]
>
>La logique qui sous-tend les décisions sur les épreuves sert à calculer le statut général d’un workflow d’épreuve s’il y a plusieurs décisions de différents niveaux. Les décisions « Approuvé » et « Approuvé avec modifications » déclenchent l’étape suivante d’un workflow automatique.

Pour configurer les décisions sur les épreuves :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Épreuves** > **Paramètres des épreuves**.
1. Dans la section **Décisions**, vous pouvez

   1. **Renommer la décision** : cliquez sur le texte à l’intérieur de la zone de décision et commencez à taper le nouveau libellé de la décision.

      >[!TIP]
      >
      >Conservez la logique d’une décision lorsque vous la renommez. Par exemple, la décision par défaut Rejeté peut être remplacée par *Nouvelle version requise*, mais ne doit pas être remplacée par *Envoyer aux imprimantes*.

      ![](assets/rename-decision-350x109.png)

   1. **Réorganiser l’ordre des décisions** : faites glisser les zones de décision dans l’ordre dans lequel vous souhaitez qu’elles apparaissent dans la visionneuse de relecture.

      ![](assets/move-decision-350x110.png)

   1. **Masquer une décision** : pointez sur la zone de décision et cliquez sur l’icône Masquer dans le coin supérieur droit.

      ![](assets/hide-decision-350x109.png)

1. (Facultatif) Pour revenir aux valeurs par défaut de Workfront, cliquez sur **Rétablir les paramètres par défaut**.
1. Cliquer sur **Enregistrer**.
