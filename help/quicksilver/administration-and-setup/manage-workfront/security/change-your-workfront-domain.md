---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Modification de votre domaine Adobe Workfront
description: En tant qu’administrateur Adobe Workfront et contact de support Workfront autorisé, vous pouvez demander de l’aide à l’équipe de support Workfront pour modifier le domaine Workfront de votre entreprise.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b9e088a0cdb32f3e8c565ea17f4613dda104bd7b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Modification de votre domaine Adobe Workfront

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, il n’est pas possible de modifier votre domaine Workfront.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, reportez-vous à la section [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En tant qu’administrateur Adobe Workfront et contact de support Workfront autorisé, vous pouvez demander de l’aide à l’équipe de support Workfront pour modifier le domaine Workfront de votre entreprise.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Demande de modification de domaine

1. Cliquez sur le bouton **Assistance** sur la page Workfront One , puis commencez à créer un cas d’assistance.
1. Dans le **Description** , incluez le nouveau domaine que vous souhaitez, ainsi que la période pendant laquelle vous souhaitez que le nouveau domaine soit mis en ligne.
1. Terminez de remplir les cases du cas d’assistance, puis cliquez sur **Envoyer**.

Vous pouvez également appeler l’assistance Workfront pour obtenir de l’aide sur le changement de domaine.

## Mettre à jour le nouveau domaine si vous êtes client SSO

Si votre entreprise utilise la connexion unique, les étapes suivantes sont requises une fois que votre domaine Workfront a été modifié.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Dans la barre latérale gauche, cliquez sur **Système** > **Informations sur le client** et assurez-vous que votre domaine est mis à jour sur la page Informations sur le client .

1. Dans la barre latérale gauche, cliquez sur **Système** > **Authentification unique (SSO)**.

1. Cliquez sur **Téléchargement des métadonnées SAML 2.0**.
1. Une fois le fichier téléchargé, ouvrez-le et assurez-vous des éléments suivants :

   1. **entityID** pointe vers le nouveau domaine.
   1. Tous les emplacements dans **`<md:AssertionConsumerService>`** pointe vers le nouveau domaine.

1. Fournissez le fichier de métadonnées téléchargé à votre fournisseur d’identité afin qu’il puisse être mis à jour de son côté.
1. Assurez-vous que le domaine est mis à jour pour toutes les intégrations Workfront utilisées par votre organisation.
