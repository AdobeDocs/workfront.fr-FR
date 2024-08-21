---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Modification de votre domaine Adobe Workfront
description: En tant qu’administrateur Adobe Workfront et contact de support Workfront autorisé, vous pouvez demander de l’aide à l’équipe de support Workfront pour modifier le domaine Workfront de votre entreprise.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 34%

---

# Modification de votre domaine Adobe Workfront

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées à Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, il n’est pas possible de modifier votre domaine Workfront.
>
>Pour obtenir une liste de procédures qui varient selon que votre organisation a été intégrée ou non à Adobe Admin Console, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront Fusion/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En tant qu’administrateur Adobe Workfront et contact de support Workfront autorisé, vous pouvez demander de l’aide à l’équipe de support Workfront pour modifier le domaine Workfront de votre entreprise.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Demande de modification de domaine

1. Commencez à créer un ticket d’assistance sur Experience League.
1. Dans la zone **Description**, incluez le nouveau domaine que vous souhaitez, ainsi que la période pendant laquelle vous souhaitez que le nouveau domaine soit mis en ligne.
1. Terminez de remplir les cases du cas d’assistance, puis cliquez sur **Submit**.

Vous pouvez également appeler l’assistance Workfront pour obtenir de l’aide sur le changement de domaine.

## Mettre à jour le nouveau domaine si vous êtes client SSO

Si votre entreprise utilise la connexion unique, les étapes suivantes sont requises une fois que votre domaine Workfront a été modifié.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

{{step-1-to-setup}}

1. Dans la barre latérale gauche, cliquez sur **Système** > **Informations client** et assurez-vous que votre domaine est mis à jour sur la page Informations client.

1. Dans la barre latérale gauche, cliquez sur **Système** > **Connexion unique (SSO)**.

1. Cliquez sur **Télécharger les métadonnées SAML 2.0**.
1. Une fois le fichier téléchargé, ouvrez-le et assurez-vous des éléments suivants :

   1. **entityID** pointe vers le nouveau domaine.
   1. Tous les emplacements dans **`<md:AssertionConsumerService>`** pointent vers le nouveau domaine.

1. Fournissez le fichier de métadonnées téléchargé à votre fournisseur d’identité afin qu’il puisse être mis à jour de son côté.
1. Assurez-vous que le domaine est mis à jour pour toutes les intégrations Workfront utilisées par votre organisation.
