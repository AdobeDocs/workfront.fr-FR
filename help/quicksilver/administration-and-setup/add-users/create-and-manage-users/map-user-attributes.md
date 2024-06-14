---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mapper les attributs d’utilisateurs et d’utilisatrices
description: À l’aide de l’authentification unique, vous pouvez transmettre des attributs d’Active Directory de votre fournisseur d’identité à vos utilisateurs Adobe Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 5%

---

# Mapper les attributs d’utilisateurs et d’utilisatrices

<!--Audited 2/2024-->

À l’aide de l’authentification unique, vous pouvez transmettre des attributs d’Active Directory de votre fournisseur d’identité à vos utilisateurs Adobe Workfront.

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
   <td><p>Nouveau : Standard</p><p>Ou</p><p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conseils relatifs aux attributs de mappage

Gardez les éléments suivants à l’esprit lors du mappage des attributs :

* Toujours tester dans un environnement de test Aperçu ou un environnement de test d’actualisation client.
* Testez les comptes administrateur et non administrateur pour vérifier que vous mappez correctement les attributs.
* Les attributs mappés sont appliqués chaque fois qu’un utilisateur se connecte par le biais d’une authentification unique.

  Exemple : si vous mappez &quot;nom&quot; et mettez à jour leur nom dans Workfront sans mettre à jour la valeur de leur fournisseur d’identité, le nom sera remplacé pour correspondre à la valeur de ce qui se trouve dans le fournisseur d’identité lors de la prochaine connexion de l’utilisateur.

## Mappage des attributs utilisateur pour votre organisation

La procédure de mappage des attributs varie selon que votre organisation utilise l’expérience unifiée Adobe.

Pour déterminer si votre organisation utilise l’expérience unifiée Adobe, examinez l’URL que vous utilisez pour accéder à Workfront.

| URL | Expérience Adobe |
|---|---|
| (NomSociété).my.workfront.com | Expérience classique |
| experience.adobe.com | Adobe d’une expérience unique |

* [Mise en correspondance des attributs utilisateur dans l’expérience classique](#map-user-attributes-in-the-classic-experience)
* [Mise en correspondance des attributs utilisateur dans l’expérience unifiée Adobe](#map-user-attributes-in-the-adobe-unified-experience)

### Mise en correspondance des attributs utilisateur dans l’expérience classique

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Authentification unique (SSO)**.

1. Dans le **Type** menu déroulant, cliquez sur **SAML 2.0**.

1. Cliquez sur **Mappage des attributs utilisateur**.

   ![](assets/map-user-attributes.png)

1. Dans la ligne des options qui s’affiche, mappez les attributs dont vous avez besoin pour vos utilisateurs Workfront.

   Vous pouvez mapper des attributs tels que Adresse, Gestionnaire, Rôle de tâche, Groupe d’accueil, etc.

   Les mappages d’attributs fonctionnent avec un ratio 1:1. Par exemple, vous ne pouvez pas définir chaque groupe auquel appartient un utilisateur ; vous ne pouvez en définir qu’un par utilisateur.

   >[!IMPORTANT]
   >
   >Il est déconseillé de mapper les niveaux d’accès dans les mappages d’attributs. Si vous le faites, soyez prudent lorsque vous définissez la valeur par défaut pour vous assurer de ne pas supprimer l’accès administrateur par inadvertance.

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
      <td>Saisissez le libellé d’attribut SSO que vous souhaitez utiliser.</td> 
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

   Cliquez sur **Ajouter une règle** pour ajouter d’autres règles à l’attribut .

1. (Facultatif) Pour mapper d’autres attributs utilisateur, cliquez sur **Ajouter un mappage** et répétez les étapes 6 à 7.
1. Cliquer sur **Enregistrer**.

### Mise en correspondance des attributs utilisateur dans l’expérience unifiée Adobe

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-left.png) dans le coin supérieur gauche d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Authentification unique (SSO)**.

1. Sélectionnez la variable **Adobe** .

1. (Facultatif et conditionnel) Si le mappage des attributs de votre organisation a été configuré dans l’expérience classique et que vous souhaitez copier ce mappage d’attributs dans l’expérience unifiée Adobe, cliquez sur **Migrer les mappages**. Vous pouvez ensuite ignorer, supprimer ou modifier ces mappages.

   >[!NOTE]
   >
   >Nous vous recommandons de migrer les mappages la première fois que vous configurez des mappages dans l’expérience unifiée Adobe. Il n’y a aucun mal à migrer à nouveau plus tard, mais migrer plus d’une fois n’est pas nécessaire.

1. Pour créer un mappage d’attributs, cliquez sur **Ajouter un mappage**.

1. Cliquez sur la flèche en regard du nom du champ Workfront et sélectionnez l’option [!DNL Workfront] champ à mapper.

1. (Facultatif) Si vous souhaitez créer plusieurs règles pour un champ donné, cliquez sur la flèche en regard de **Toujours** et sélectionnez l’opérateur que la règle doit utiliser.

1. (Conditionnel) Si vous avez sélectionné un opérateur en plus de Toujours, sélectionnez le champ Workfront et la valeur auxquels s’applique l’opérateur.

   >[!NOTE]
   >
   >Les opérateurs `Is Truthy` et `Is Falsy` ne requièrent pas de valeurs.

1. Indiquez si vous souhaitez appliquer la valeur d’un attribut dans votre gestionnaire d’identités au champ Workfront ou si vous souhaitez appliquer une valeur constante spécifique.

1. Saisissez le nom du champ du gestionnaire d’identités à appliquer ou le texte de la valeur constante à appliquer.

1. (Facultatif) Pour ajouter d’autres règles pour le même champ Workfront, cliquez sur **Ajouter une nouvelle règle** et suivez les étapes 4 à 9.

   >[!IMPORTANT]
   >
   > * Toute règle sous une règle Toujours est ignorée. Si vous disposez d’une règle Toujours , vous devez la déplacer au bas de la liste des règles. Vous pouvez déplacer les règles dans la liste en cliquant sur le menu à trois points situé à droite de la règle et en déplaçant la règle vers le haut ou vers le bas.
   > * Pour créer une règle au milieu de la liste, cliquez sur le menu à trois points en regard de la règle que vous souhaitez placer au-dessus ou en dessous de la nouvelle règle, puis sélectionnez **Ajouter une règle au-dessus de** ou **Ajouter une règle ci-dessous**.

1. Pour supprimer une règle, cliquez sur le menu à trois points en regard de la règle à supprimer, puis sélectionnez **Supprimer**.
1. Pour supprimer un mappage, cliquez sur le bouton **Supprimer** qui se trouve sur la carte pour ce mappage.

1. Pour enregistrer, faites défiler la page jusqu’au haut de la page et cliquez sur **Enregistrer**.


