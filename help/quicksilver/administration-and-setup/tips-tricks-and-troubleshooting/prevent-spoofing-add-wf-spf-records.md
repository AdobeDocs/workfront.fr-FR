---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Empêcher l'usurpation et ajouter  [!DNL Adobe Workfront]  enregistrements SPF
description: Si les utilisateurs et les utilisatrices ne reçoivent pas de notifications par e-mail  [!DNL Adobe Workfront] , vous devez ajouter des enregistrements SPF  [!DNL Workfront]  à votre pare-feu. Vous devez collaborer avec votre équipe informatique pour ajouter des enregistrements SPF.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
TQID: https://experienceleague.adobe.com/6VnF205aiahPEWdP2kPk-YXF8UfPwSJ0-yJ6nGq3-FM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 294
ht-degree: 97%

---

# Prévenir l’usurpation d’identité et ajouter des enregistrements SPF [!DNL Adobe Workfront]

## Problème

Si les utilisateurs et les utilisatrices ne reçoivent pas de notifications par e-mail [!DNL Adobe Workfront], vous devez ajouter des enregistrements SPF [!DNL Workfront] à votre pare-feu. Vous devez collaborer avec votre équipe informatique pour ajouter des enregistrements SPF.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

Si vous avez déjà ajouté les adresses IP à votre liste autorisée pour votre environnement de production, tel que décrit dans la section [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md), mais que les utilisateurs et utilisatrices ne reçoivent toujours pas d’e-mails :

1. Ajoutez l’enregistrement SPF suivant à votre pare-feu :

   *spf.workfront.com*

   Cela ajoute automatiquement toutes les adresses IP [!DNL Workfront] à votre liste autorisée sur votre pare-feu et permet à tous les filtres anti-spam (qui utilisent des enregistrements SPF) de valider les serveurs [!DNL Workfront] en tant qu’expéditeurs valides pour votre domaine.

   >[!NOTE]
   >
   > Un enregistrement SPF est un enregistrement TXT qui fait partie d’un fichier de zone DNS. La modification de votre fichier de zone DNS n’est pas prise en charge.

1. Vous devez spécifier le type d’enregistrement SPF à configurer. Les types d’enregistrements SPF valides sont les suivants :

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * exists (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Par exemple, « v=spf1 a mx inclut : spf.workfront.com -all »

Si vous ne pouvez pas ajouter d’enregistrements SPF à votre pare-feu en raison de la politique de l’entreprise, veuillez contacter la personne qui représente l’équipe de support [!DNL Workfront].
