---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuration des paramètres de partage pour vos utilisateurs
description: En tant qu’administrateur ou administratrice Adobe Workfront ou Workfront Proof, vous pouvez configurer les comptes des utilisateurs et utilisatrices avec lesquels les épreuves peuvent être partagées, déterminer si les utilisateurs et utilisatrices peuvent voir toutes les versions d’une épreuve et déterminer le moment auquel les utilisateurs et utilisatrices ont accès aux éléments partagés.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 98%

---

# Configurer les paramètres de partage pour vos utilisateurs et utilisatrices

En tant qu’administrateur ou administratrice Adobe Workfront ou Workfront Proof, vous pouvez configurer les comptes des utilisateurs et utilisatrices avec lesquels les épreuves peuvent être partagées, déterminer si les utilisateurs et utilisatrices peuvent voir toutes les versions d’une épreuve et déterminer le moment auquel les utilisateurs et utilisatrices ont accès aux éléments partagés.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Plan actuel : Pro ou version supérieure</p> <p>ou</p> <p>Formule héritée : Premium ou Select</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>L’option d’administration doit être sélectionnée dans votre profil d’autorisation d’épreuve. Pour plus d’informations, voir la section <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurer l’accès à la relecture d’un utilisateur ou d’une utilisatrice</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Configurer le partage avec d’autres comptes

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte**, puis cliquez sur l’onglet **Paramètres**.

1. Dans la section **Partage**, à droite de **Autoriser le partage avec**, cliquez sur **Configuration**.

1. Dans la liste déroulante qui s’affiche, sélectionnez une option pour indiquer si vous souhaitez rendre les épreuves disponibles pour toutes les personnes, restreindre le partage de vos épreuves à votre propre compte uniquement ou restreindre le partage à votre propre compte et à tout compte partenaire avec lequel vous collaborez.
1. Cliquez sur **Enregistrer**.

## Configurer la visibilité de toutes les versions d’une épreuve partagée

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte**, puis cliquez sur l’onglet **Paramètres**.

1. Dans la section **Partage**, à droite de **Les personnes destinataires peuvent voir toutes les versions**, sélectionnez **Activer** ou **Désactiver** pour indiquer si vous souhaitez autoriser les personnes destinataires à voir toutes les versions d’une épreuve dans la visionneuse de relecture lorsque l’URL de l’épreuve est activée.

## Configurer la visibilité de l’épreuve en fonction de l’activité d’étape du workflow

Vous pouvez spécifier le moment où les épreuves avec un workflow automatisé sont visibles par les utilisateurs et utilisatrices associés à une étape donnée.

>[!NOTE]
>
>* Cette option est disponible uniquement lors de l’utilisation de l’application Workfront Proof autonome ; elle n’est pas disponible lors de l’utilisation d’une instance Workfront Proof intégrée à Workfront ou lors de la relecture dans Workfront.
>* Les utilisateurs et utilisatrices ne reçoivent une notification par e-mail à propos de l’épreuve qu’après son entrée dans l’étape à laquelle la personne est associée, quel que soit ce paramètre.
>

Pour configurer quand les épreuves avec un workflow automatisé sont visibles par les utilisateurs et utilisatrices, procédez comme suit :

{{step1-to-proofing}}

1. Cliquez sur **Paramètres** > **Paramètres du compte**, puis cliquez sur l’onglet **Paramètres**.

1. Dans la section **Partage**, activez ou désactivez **Visibilité de l’épreuve en fonction de l’activation de l’étape**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Désactivé</strong> (par défaut)</td> 
      <td>Les épreuves sont visibles par les utilisateurs et utilisatrices au moment de la création de l’épreuve.<br><p>Toute personne associée à une étape du workflow pour l’épreuve peut voir l’épreuve dans les résultats de recherche immédiatement après la création de l’épreuve.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Activé</strong> </td> 
      <td> <p>Les épreuves ne sont visibles par les utilisateurs et utilisatrices que lorsque l’étape à laquelle ils sont associés devient <strong>active.</strong></p> <p><b>NOTE</b> :   
        <ul> 
         <li><em style="font-style: normal;">Une fois cette option activée, les épreuves existantes restent visibles pour les utilisateurs et utilisatrices qui pouvaient les afficher lors de leur création.</em> </li> 
         <li>Une fois qu’un utilisateur ou une utilisatrice a accès à une version d’une épreuve (car l’étape à laquelle la personne est associée devient active), l’utilisateur ou l’utilisatrice ne peut voir que la version dans laquelle l’étape est activée. Si une version précédente n’a jamais atteint l’étape à laquelle la personne est associée, la personne ne peut pas voir cette version de l’épreuve.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
