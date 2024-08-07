---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,sécurité,certificat,Admin,Exonération,configurer,métadonnées
navigation-topic: security
title: Renouvellement du certificat de métadonnées Adobe Workfront SAML 2.0
description: Les serveurs Adobe Workfront utilisent le protocole SAML 2.0 pour l’authentification et l’autorisation. Une fois mis à jour, le nouveau certificat reste valide pendant un an. Lorsqu’il est temps pour vous de renouveler le certificat sur votre fournisseur d’identité, vous recevez un avertissement dans Workfront vous informant que cette modification doit se produire. En tant qu’administrateur Workfront, vous pouvez gérer cette modification au niveau du système.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 21%

---

# Renouvellement du certificat de métadonnées Adobe Workfront SAML 2.0

>[!IMPORTANT]
>
>La procédure décrite sur cette page s’applique uniquement aux organisations qui n’ont pas encore été intégrées à Admin Console. Si votre entreprise a été intégrée à Adobe Admin Console, aucune action n’est nécessaire.
>
>Pour obtenir une liste de procédures qui varient selon que votre organisation a été intégrée ou non à Adobe Admin Console, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront Fusion/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Les serveurs Adobe Workfront utilisent le protocole SAML 2.0 pour l’authentification et l’autorisation. Une fois mis à jour, le nouveau certificat reste valide pendant un an. Lorsqu’il est temps pour vous de renouveler le certificat sur votre fournisseur d’identité, vous recevez un avertissement dans Workfront vous informant que cette modification doit se produire. En tant qu’administrateur Workfront, vous pouvez gérer cette modification au niveau du système.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise est activée avec Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

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
  <td> <p>Nouvelle : standard </p>
 <p>ou</p> 
<p>Actuelle : formule </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuration de SAML 2.0 dans Workfront

Pour passer en revue le message d’avertissement et reconnaître la mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité :

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) en haut à droite d’Adobe Workfront, puis cliquez sur **Configurer** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Connexion unique**.

1. Dans le menu déroulant **Type**, sélectionnez **SAML 2.0**.

1. Cliquez sur **Télécharger les métadonnées SAML 2.0**.

   Cela télécharge le certificat Workfront renouvelé pour SAML 2.0, qui contient les métadonnées correctes pour votre serveur.

1. Dans votre fournisseur d’identité, copiez l’URL actuelle d’Assertion Consumer Service (ACS) (également appelée URL de réponse) dans un endroit sûr.

   >[!CAUTION]
   >
   >Avant de charger les métadonnées Workfront vers votre fournisseur de connexion unique (SSO) à l’étape 6, copiez l’URL actuelle du service client d’assertion (ACS) vers un emplacement sécurisé. Cette URL, également appelée URL de réponse, se trouve sur la page de configuration Workfront de votre fournisseur d’authentification unique.
   >
   >
   >Si l’URL ACS change après le chargement des métadonnées Workfront, cela signifie que les métadonnées peuvent contenir une URL ACS incorrecte. Vous devez la redéfinir sur celle que vous avez copiée afin d’éviter de rompre votre connexion à authentification unique. Votre certificat mis à jour sera toujours correct après cette opération.

1. Sur votre serveur de fournisseur d’identité, mettez à jour le nouveau certificat que vous avez téléchargé.
1. (Conditionnel) Si l’URL ACS (Assertion Consumer Service) ou l’URL de réponse a changé dans votre fournisseur d’identité, redéfinissez-la sur l’URL que vous avez copiée à l’étape 5.
1. Dans Workfront, sur la **page de connexion unique (SSO)**, assurez-vous que cette option est sélectionnée : **Le nouveau certificat Workfront a déjà été téléchargé vers le fournisseur d’identité**.

   >[!NOTE]
   >
   >* Cette option n’est visible que si tous les éléments suivants s’appliquent :
   >   * Votre organisation est déjà configurée pour SAML 2.0.
   >   * Le certificat actuel est prêt à expirer.
   >   * Le nouveau certificat est disponible
   >* Lorsque ce champ est sélectionné, les administrateurs Workfront peuvent se connecter à Workfront avec leurs informations d’identification d’authentification unique ou leurs informations d’identification Workfront.

1. Cliquer sur **Enregistrer**.

   Le message d’avertissement ne s’affiche plus, car vous avez accusé réception du renouvellement du certificat SAML 2.0 sur le serveur de votre fournisseur d’identité.

1. Cliquez sur **Tester la connexion** pour tester votre configuration.

   Un message s’affiche pour confirmer que la connexion a réussi.

Pour plus d’informations ou pour obtenir de l’aide sur la configuration manuelle des métadonnées, contactez notre équipe d’assistance, comme expliqué dans la rubrique [Contacter le service clientèle](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
