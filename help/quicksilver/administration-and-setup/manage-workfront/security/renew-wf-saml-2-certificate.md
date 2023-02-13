---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,sécurité,certificat,Admin,Exonération,configurer,métadonnées
navigation-topic: security
title: Renouvellement du certificat de métadonnées Adobe Workfront SAML 2.0
description: La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au Admin Console. Si votre organisation a été intégrée à Adobe Admin Console, vous devez effectuer cette action via Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Renouvellement du certificat de métadonnées Adobe Workfront SAML 2.0

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées au Admin Console. Si votre entreprise a été intégrée à Adobe Admin Console, aucune action n’est nécessaire.
>
>Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Admin Console, reportez-vous à la section [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Les serveurs Adobe Workfront utilisent le protocole SAML 2.0 pour l’authentification et l’autorisation. Une fois mis à jour, le nouveau certificat reste valide pendant un an. Lorsqu’il est temps pour vous de renouveler le certificat sur votre fournisseur d’identité, vous recevez un avertissement dans Workfront vous informant que cette modification doit se produire. En tant qu’administrateur Workfront, vous pouvez gérer cette modification au niveau du système.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

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

## Configuration de SAML 2.0 dans Workfront

Pour passer en revue le message d’avertissement et reconnaître la mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité :

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Authentification unique**.

1. Dans le **Type** menu déroulant, sélectionnez **SAML 2.0**.

1. Cliquez sur **Téléchargement des métadonnées SAML 2.0**.

   Cela télécharge le certificat Workfront renouvelé pour SAML 2.0, qui contient les métadonnées correctes pour votre serveur.

   >[!CAUTION]
   >
   >Avant de charger les métadonnées Workfront vers votre fournisseur de connexion unique (SSO) à l’étape 5, copiez l’URL actuelle du service client d’assertion (ACS) vers un emplacement sécurisé. Cette URL, également appelée URL de réponse, se trouve sur la page de configuration Workfront de votre fournisseur d’authentification unique.
   >
   >
   >Si l’URL ACS change après le chargement des métadonnées Workfront, cela signifie que les métadonnées peuvent contenir une URL ACS incorrecte. Vous devez la redéfinir sur celle que vous avez copiée afin d’éviter de rompre votre connexion à authentification unique. Votre certificat mis à jour sera toujours correct après cette opération.

1. Accédez à votre serveur de fournisseur d’identité et mettez à jour le nouveau certificat que vous avez téléchargé.
1. Dans Workfront, sur la **Page de connexion unique (SSO)**, assurez-vous que cette option est sélectionnée : **Le nouveau certificat Workfront a déjà été chargé dans le fournisseur d’identité.**.

   Lorsque ce champ est sélectionné, les administrateurs Workfront peuvent se connecter à Workfront avec leurs informations d’identification d’authentification unique ou leurs informations d’identification Workfront.

1. Cliquer sur **Enregistrer**.

   Le message d’avertissement ne s’affiche plus, car vous avez accusé réception du renouvellement du certificat SAML 2.0 sur le serveur de votre fournisseur d’identité.

1. Cliquez sur **Tester la connexion** pour tester votre configuration.

   Un message s’affiche pour confirmer que la connexion a réussi.

Pour plus d’informations ou pour obtenir de l’aide sur la configuration manuelle des métadonnées, veuillez contacter notre équipe d’assistance, comme expliqué dans la section [Contacter le service clientèle](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
