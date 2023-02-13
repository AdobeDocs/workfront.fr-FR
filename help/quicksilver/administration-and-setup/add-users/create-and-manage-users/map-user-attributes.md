---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mappage des attributs utilisateur et configuration automatique des nouveaux utilisateurs
description: À l’aide de l’authentification unique (SSO), vous pouvez transmettre des attributs du Principal annuaire de votre fournisseur d’identité à vos utilisateurs Adobe Workfront. Vous pouvez également ajouter de nouveaux utilisateurs à Workfront à l’aide de l’option Configuration automatique (également appelée approvisionnement juste à temps ou JIT).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 3%

---

# Mappage des attributs utilisateur et configuration automatique des nouveaux utilisateurs

À l’aide de l’authentification unique (SSO), vous pouvez transmettre des attributs du Principal annuaire de votre fournisseur d’identité à vos utilisateurs Adobe Workfront. Vous pouvez également ajouter de nouveaux utilisateurs à Workfront à l’aide de l’option Configuration automatique (également appelée approvisionnement juste à temps ou JIT).

>[!NOTE]
>
>Cette option n’est pas disponible si votre organisation a été intégrée à Adobe Admin Console. Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.


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

## Conseils relatifs aux attributs de mappage

Gardez les éléments suivants à l’esprit lors du mappage des attributs :

* Toujours tester dans un environnement de test Aperçu ou un environnement de test d’actualisation client.
* Testez les comptes administrateur et non administrateur pour vérifier que vous mappez correctement les attributs.
* Les attributs sont mappés chaque fois qu’un utilisateur se connecte à Workfront par le biais de l’authentification unique, et pas seulement pendant l’approvisionnement automatique.

## Mappage des attributs utilisateur et configuration automatique des nouveaux utilisateurs

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Authentification unique (SSO)**.

1. Dans le **Type** menu déroulant, cliquez sur **SAML 2.0**.

1. Cliquez sur **Mappage des attributs utilisateur**.

   ![](assets/map-user-attributes.png)

1. (Facultatif) Si vous souhaitez que Workfront crée automatiquement de nouveaux utilisateurs à partir de votre répertoire Principal, cliquez sur **Configuration automatique des utilisateurs**.

   Cette fonctionnalité nécessite le mappage des attributs.

1. Dans la ligne des options qui s’affiche, mappez les attributs dont vous avez besoin pour vos utilisateurs Workfront.

   Vous pouvez mapper des attributs tels que Adresse, Gestionnaire, Rôle de tâche, Groupe d’accueil, etc.

   Les mappages d’attributs fonctionnent avec un ratio 1:1. Par exemple, vous ne pouvez pas définir chaque groupe auquel appartient un utilisateur. vous ne pouvez définir qu’une seule valeur par utilisateur.

   >[!IMPORTANT]
   >
   >Les attributs suivants sont requis pour chaque utilisateur :
   >      
   >* Prénom
   >* Nom de famille
   >* Adresse électronique

   >      
   >Il est déconseillé de mapper les niveaux d’accès dans les mappages d’attributs. Si vous le faites, soyez prudent lorsque vous définissez la valeur par défaut afin de vous assurer que vous ne supprimez pas l’accès administrateur par inadvertance.

   Le tableau suivant explique les champs que vous pouvez utiliser pour mapper des attributs :

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Attribut utilisateur Workfront</td> 
      <td>Sélectionnez le nom de l’attribut que vous mappez.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attribut de répertoire</td> 
      <td>Saisissez le libellé d’attribut SSO que vous souhaitez utiliser./td&gt; 
     </tr> 
     <tr> 
      <td role="rowheader">Valeur par défaut</td> 
      <td> <p>Après avoir choisi un attribut utilisateur Workfront, si la valeur est NULL lors de la connexion, ce champ renseigne la valeur par défaut correspondante dans le système. Saisissez une valeur ici uniquement si vous prévoyez d’appliquer des règles de mappage d’attributs (voir l’étape 7). La valeur par défaut agit comme une exception à ces règles.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatif) Cliquez sur **Règles** pour ajouter une règle à l’attribut .

   1. Dans la liste déroulante, sélectionnez le modificateur d’attribut à utiliser.
   1. Dans les 2 champs à droite, saisissez la valeur de l’attribut directory et la valeur avec laquelle vous souhaitez le remplacer.

      ![](assets/rule-fields.png)
   Vous pouvez cliquer sur **Ajouter une règle** pour ajouter d’autres règles à l’attribut .

1. (Facultatif) Pour mapper d’autres attributs utilisateur, cliquez sur **Ajouter un mappage** et répétez les étapes 6 à 7.
1. Cliquer sur **Enregistrer**.
