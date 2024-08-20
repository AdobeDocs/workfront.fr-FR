---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuration des paramètres de partage pour vos utilisateurs
description: En tant qu’administrateur Adobe Workfront ou administrateur Workfront Proof, vous pouvez configurer les comptes d’utilisateurs avec lesquels les bons à tirer peuvent être partagés, déterminer si les utilisateurs peuvent voir toutes les versions d’un bon à tirer et déterminer le moment auquel les utilisateurs ont accès aux éléments partagés.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 5%

---

# Configuration des paramètres de partage pour vos utilisateurs

En tant qu’administrateur Adobe Workfront ou administrateur Workfront Proof, vous pouvez configurer les comptes d’utilisateurs avec lesquels les bons à tirer peuvent être partagés, déterminer si les utilisateurs peuvent voir toutes les versions d’un bon à tirer et déterminer le moment auquel les utilisateurs ont accès aux éléments partagés.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : Premium ou Sélectionner</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>L’administrateur doit être sélectionné dans votre profil d’autorisation de BAT. Pour plus d’informations, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configuration de l’accès de vérification de l’utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configuration du partage avec d’autres comptes

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte**, puis sur l’onglet **Paramètres** .

1. Dans la section **Partage**, à droite de **Autoriser le partage avec**, cliquez sur **Configuration**.

1. Dans la liste déroulante qui s’affiche, sélectionnez une option pour indiquer si vous souhaitez rendre les bons à tirer disponibles pour tout le monde, restreindre le partage de vos bons à tirer à votre propre compte uniquement ou restreindre le partage à votre propre compte et à tout compte partenaire avec lequel vous collaborez.
1. Cliquez sur **Enregistrer.**

## Configurer la visibilité de toutes les versions d’un BAT partagé

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte**, puis sur l’onglet **Paramètres** .

1. Dans la section **Partage**, à droite de **Les destinataires peuvent afficher toutes les versions**, sélectionnez **Activer** ou **Désactiver** pour indiquer si vous souhaitez autoriser les destinataires à afficher toutes les versions d’un BAT dans la visionneuse de vérification lorsque l’URL du BAT est activée.

## Configuration de la visibilité du BAT en fonction de l’activité d’étape du workflow

Vous pouvez spécifier le moment où les bons à tirer avec un workflow automatisé sont visibles par les utilisateurs associés à une étape donnée.

>[!NOTE]
>
>* Cette option est disponible uniquement lors de l’utilisation de l’application Workfront Proof autonome. Elle n’est pas disponible lors de l’utilisation d’une instance Workfront Proof intégrée à Workfront ou lors de la vérification de l’intégrité dans Workfront.
>* Les utilisateurs ne reçoivent une notification par e-mail à propos du BAT qu’après son entrée dans l’étape à laquelle l’utilisateur est associé, quel que soit ce paramètre.
>

Pour configurer lorsque les bons à tirer avec un workflow automatisé sont visibles par les utilisateurs :

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte**, puis sur l’onglet **Paramètres** .

1. Dans la section **Partage** , activez ou désactivez la **visibilité du BAT en fonction de l&#39;activation de l&#39;étape**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Disabled</strong> (par défaut)</td> 
      <td>Les bons à tirer sont visibles par les utilisateurs au moment de la création du BAT.<br><p>Tout utilisateur associé à une étape du workflow pour le BAT peut voir le BAT dans les résultats de recherche immédiatement après la création du BAT.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enabled</strong> </td> 
      <td> <p>Les bons à tirer ne sont visibles par les utilisateurs qu’une fois l’étape à laquelle ils sont associés devient <strong>active.</strong></p> <p><b>NOTE</b> :   
        <ul> 
         <li><em style="font-style: normal;"> Une fois cette option activée, les bons à tirer existants sont toujours visibles par les utilisateurs qui pouvaient les afficher lors de leur création.</em> </li> 
         <li>Une fois qu’un utilisateur a accès à une version d’un BAT (car l’étape à laquelle l’utilisateur est associé devient active), il ne peut voir que la version dans laquelle l’étape est activée. Si une version précédente n’a jamais atteint l’étape à laquelle l’utilisateur est associé, l’utilisateur ne peut pas voir cette version du BAT.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
