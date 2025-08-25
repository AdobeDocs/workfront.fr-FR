---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,sécurité,certificat,administration,exemption,configuration,métadonnées
navigation-topic: security
title: Renouveler le certificat de métadonnées Adobe Workfront SAML 2.0
description: Les serveurs Adobe Workfront utilisent le protocole SAML 2.0 pour l’authentification et l’autorisation. Une fois mis à jour, le nouveau certificat reste valide pendant un an. Lorsque le moment est venu de renouveler le certificat de votre fournisseur d’identité, vous recevez un avertissement dans Workfront vous informant que ce changement doit être effectué. En tant qu’administrateur ou administratrice de Workfront, vous pouvez gérer ce changement au niveau du système.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 90%

---

# Renouveler le certificat de métadonnées SAML 2.0 d’Adobe Workfront

>[!IMPORTANT]
>
>La procédure décrite sur cette page a été supprimée, car elle s’appliquait uniquement aux organisations qui n’avaient pas encore intégré Adobe Admin Console. Cette procédure n’est pas nécessaire pour les organisations sur le Adobe Admin Console.
>
>Comme toutes les organisations Workfront ont maintenant été intégrées à Adobe Admin Console, cet article sera supprimé prochainement.

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>La procédure décrite sur cette page ne s’applique qu’aux entreprise qui n’ont pas encore été intégrées à l’Admin Console. Si votre entreprise est intégrée à Adobe Admin Console, aucune action n’est nécessaire.
>
>Pour suivre la procédure correspondant à votre situation et à son intégration ou non à Adobe Admin Console, consultez la section [Différences en matière d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Les serveurs Adobe Workfront utilisent le protocole SAML 2.0 pour l’authentification et l’autorisation. Une fois mis à jour, le nouveau certificat reste valide pendant un an. Lorsque le moment est venu de renouveler le certificat de votre fournisseur d’identité, vous recevez un avertissement dans Workfront vous informant que ce changement doit être effectué. En tant qu’administrateur ou administratrice de Workfront, vous pouvez gérer ce changement au niveau du système.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre organisation repose sur Adobe IMS. Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
 <tr> 
  <td role="rowheader">Licence Adobe Workfront</td> 
  <td> <p>Nouveau : Standard </p>
 <p>ou</p> 
<p>Actuel : formule </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurer SAML 2.0 dans Workfront

Pour consulter le message d’avertissement et confirmer la mise à jour des métadonnées SAML 2.0 dans votre fournisseur d’identité, procédez comme suit :

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Authentification unique**.

1. Dans le menu déroulant **Type**, sélectionnez **SAML 2.0**.

1. Cliquez sur **Télécharger les métadonnées SAML 2.0**.

   Cette opération permet de télécharger le certificat Workfront renouvelé pour SAML 2.0, qui contient les métadonnées correctes pour votre serveur.

1. Dans votre fournisseur d’identité, copiez l’URL de votre ACS (Service consommateurs - Assertion) actuel (également connue sous le nom d’URL de réponse) dans un endroit sûr.

   >[!CAUTION]
   >
   >Avant de charger les métadonnées Workfront vers votre fournisseur d’authentification unique (SSO) à l’étape 6, copiez l’URL de votre ACS (Service consommateurs - Assertion) dans un endroit sûr. Cette URL, également connue sous le nom d’URL de réponse, se trouve sur la page de configuration Workfront de votre fournisseur SSO.
   >
   >
   >Si l’URL ACS est modifiée après le chargement des métadonnées Workfront, cela signifie que les métadonnées peuvent contenir une URL ACS incorrecte. Vous devez la remplacer par celle que vous avez copiée afin d’éviter l’échec de votre connexion SSO. Votre certificat mis à jour sera toujours correct après cette opération.

1. Dans le serveur de votre fournisseur d’identité, mettez à jour le nouveau certificat que vous avez téléchargé.
1. (Le cas échéant) Si l’URL ACS (Service consommateurs - Assertion) ou l’URL de la réponse a été modifiée dans votre fournisseur d’identité, remplacez-la par l’URL que vous avez copiée à l’étape 5.
1. Dans Workfront, sur la **page SSO (authentification unique)**, assurez-vous que l’option suivante est sélectionnée : **Le nouveau certificat Workfront a déjà été chargé sur le fournisseur d’identité**.

   >[!NOTE]
   >
   >* Cette option n’est visible que si toutes les conditions suivantes sont remplies :
   >   * Votre organisation est déjà configurée pour SAML 2.0.
   >   * Le certificat actuel arrive à expiration.
   >   * Le nouveau certificat est disponible.
   >* Lorsque ce champ est sélectionné, les administrateurs et administratrices de Workfront peuvent se connecter à Workfront avec leurs identifiants SSO ou Workfront.

1. Cliquer sur **Enregistrer**.

   Le message d’avertissement ne s’affiche plus, car vous avez confirmé le renouvellement du certificat SAML 2.0 sur le serveur de votre fournisseur d’identité.

1. Cliquez sur **Tester connexion** pour tester votre configuration.

   Vous devriez voir un message confirmant que la connexion a réussi.

Pour plus d’informations ou pour obtenir de l’aide pour la configuration manuelle des métadonnées, veuillez contacter notre équipe d’assistance, comme expliqué dans [Contacter l’assistance clientèle](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
