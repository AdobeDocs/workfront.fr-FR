---
title: Politique de prise en charge d’AtTask OnPremise
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: Adobe Workfront est passé à un modèle "Software-as-A-Service" à 100 % et a cessé de vendre des logiciels on-premise le 31 décembre 2011. À compter de 2014, AtTask OnPremise n’est plus pris en charge, à l’exception des problèmes liés aux clés de licence. L’application on-premise n’est plus disponible au téléchargement ou à l’installation.
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 32%

---

# Politique de prise en charge d’AtTask OnPremise

Adobe Workfront est passé à un modèle &quot;Software-as-A-Service&quot; à 100 % et a cessé de vendre des logiciels on-premise le 31 décembre 2011. À compter de 2014, AtTask OnPremise n’est plus pris en charge, à l’exception des problèmes liés aux clés de licence. L’application on-premise n’est plus disponible au téléchargement ou à l’installation.

Si vous disposez déjà de l’application et devez réinstaller OnPremise, téléchargez le guide d’installation .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

Téléchargez des instructions sur la configuration SSL/TSL.

## Conditions d’accès

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
   <td> <p>Vous devez être un administrateur Workfront. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Mise à jour de la clé de licence OnPremise

Si vous avez besoin d’une nouvelle clé de licence, contactez le service clientèle de Workfront au 844-306-HELP(4357).

Une fois que vous avez obtenu une nouvelle clé de licence,

1. Arrêtez le serveur atTask.
1. Renommez le fichier license.key actuel (situé dans le dossier AtTaskDoc).
1. Copiez le nouveau fichier license.key en place.
1. Redémarrez le serveur atTask.

Cet article comprend les pièces jointes suivantes :
