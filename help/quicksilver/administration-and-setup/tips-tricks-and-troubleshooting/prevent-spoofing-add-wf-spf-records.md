---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Empêcher l’usurpation et ajouter des enregistrements  [!DNL Adobe Workfront] SPF
description: Si les utilisateurs ne reçoivent pas de  [!DNL Adobe Workfront] notifications par e-mail, vous devez ajouter des  [!DNL Workfront] enregistrements SPF à votre pare-feu. Vous devez collaborer avec votre équipe informatique pour ajouter des enregistrements SPF.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 25%

---

# Empêcher l’usurpation et l’ajout d’enregistrements SPF [!DNL Adobe Workfront]

## Problème

Si les utilisateurs ne reçoivent pas [!DNL Adobe Workfront] notifications électroniques, vous devez ajouter [!DNL Workfront] enregistrements SPF à votre pare-feu. Vous devez collaborer avec votre équipe informatique pour ajouter des enregistrements SPF.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

Si vous avez déjà ajouté les adresses IP à votre liste autorisée pour votre environnement de production comme décrit dans la section [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) et que les utilisateurs ne reçoivent toujours pas d’e-mails :

1. Ajoutez l’enregistrement SPF suivant à votre pare-feu :

   *spf.workfront.com*

   Cela ajoute automatiquement toutes les adresses IP [!DNL Workfront] à votre liste autorisée sur votre pare-feu et permet à tous les filtres anti-spam (qui utilisent des enregistrements SPF) de valider les serveurs [!DNL Workfront] comme expéditeurs valides pour votre domaine.

   >[!NOTE]
   >
   > Un enregistrement SPF est un enregistrement TXT qui fait partie d’un fichier de zone DNS. La modification de votre fichier de zone DNS n’est pas prise en charge.

1. Vous devez spécifier le type d’enregistrement SPF à configurer. Il s’agit des types d’enregistrements SPF valides :

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * exists (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Par exemple, &quot;v=spf1 a mx inclut : spf.workfront.com -all&quot;

Si vous ne pouvez pas ajouter d’enregistrements SPF à votre pare-feu en raison de la politique de l’entreprise, veuillez travailler avec votre représentant de l’assistance [!DNL Workfront].
