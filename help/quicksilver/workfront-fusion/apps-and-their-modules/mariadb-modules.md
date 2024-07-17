---
title: Modules MariaDB
description: Dans un scénario  [!DNL Adobe Workfront Fusion] , vous pouvez automatiser les workflows qui utilisent  [!DNL MariaDB] et les connecter à plusieurs applications et services tiers.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 50%

---

# Modules [!DNL MariaDB]

Dans un scénario [!DNL Adobe Workfront Fusion], vous pouvez automatiser les workflows qui utilisent [!DNL MariaDB] et les connecter à plusieurs applications et services tiers.

Si vous avez besoin d’instructions sur la création d’un scénario, voir [Créer un scénario dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Pour plus d’informations sur les modules, consultez [Modules dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Conditions d’accès

Pour utiliser les fonctionnalités décrites dans cet article, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] forfait*</td>
  <td> <p>[!UICONTROL Pro] ou un forfait supérieur</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licence*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licence**</td> 
   <td>
   <p>Exigences de licence actuelle : aucune exigence de licence [!DNL Workfront Fusion]</p>
   <p>Ou</p>
   <p>Exigence de licence héritée : [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences du produit actuel : si vous disposez du forfait [!DNL Adobe Workfront] [!UICONTROL Select] ou [!UICONTROL Prime], votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article. [!DNL Workfront Fusion] est inclus dans le forfait [!DNL Workfront] [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Exigences du produit hérité : votre entreprise doit acheter [!DNL Adobe Workfront Fusion] et [!DNL Adobe Workfront] pour utiliser les fonctionnalités décrites dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez vote administrateur ou administratrice [!DNL Workfront].

Pour plus d’informations sur les licences [!DNL Adobe Workfront Fusion], consultez les [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser des modules [!DNL MariaDB], vous devez disposer d’un compte [!DNL MariaDB].

## Connecter [!DNL MariaDB] à [!DNL Workfront Fusion]

Vous pouvez créer une connexion à votre compte [!DNL MariaDB] directement à partir de l’intérieur d’un module [!DNL MariaDB].

1. Dans un module [!DNL MariaDB], cliquez sur **[!UICONTROL Ajouter]** en regard du champ [!UICONTROL Connexion].
1. Configurez les champs suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Saisissez un nom pour la nouvelle connexion.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Saisissez l’adresse IP ou le nom d’hôte de l’instance de base de données. Cet hôte doit être accessible en dehors de votre réseau.</p> <p>Exemple : <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>Le port par défaut est 3306. Si vous utilisez un port non standard, définissez ce nombre sur votre port. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Database Name]</td> 
      <td>Saisissez le nom de la base de données avec laquelle vous souhaitez interagir.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Username]</td> 
      <td>Saisissez votre nom d’utilisateur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Password]</td> 
      <td>Saisissez votre mot de passe.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **[!UICONTROL Continuer]** pour créer la connexion et retourner au module.

## [!DNL MariaDB] Modules et leurs champs

Lorsque vous configurez des modules [!DNL MariaDB], [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. Des champs [!DNL MariaDB] supplémentaires peuvent également s’afficher, en fonction des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, consultez [Mapper les informations d’un module à un autre dans  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Exécution d’une requête (avancée)

Ce module d’action récupère les informations de votre base de données, en fonction d’une requête que vous fournissez.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour plus d'informations sur la connexion de votre compte [!DNL MariaDB] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connexion [!DNL MariaDB] à [!DNL Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>Saisissez la requête SQL que le module doit utiliser pour récupérer les données.</p> <p>Important : Les variables utilisées dans la requête ne sont pas assainies. Assurez-vous d’assainir correctement les variables pour empêcher l’injection SQL.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Sélectionner des lignes d’une table (avancé)]

Ce module lit les enregistrements de votre base de données.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Pour plus d'informations sur la connexion de votre compte [!DNL MariaDB] à [!DNL Workfront Fusion], reportez-vous à la section <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connexion [!DNL MariaDB] à [!DNL Workfront Fusion]</a> de cet article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table]</td> 
   <td> <p>Sélectionnez la table contenant les enregistrements à lire.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Configurez le filtre selon lequel vous souhaitez sélectionner des lignes.</p> 
    <ul> 
     <li> <p>Sélectionnez le champ par lequel effectuer la recherche.</p> </li> 
     <li> <p>Sélectionnez l’opérateur à utiliser pour votre recherche.</p> </li> 
     <li> <p>Saisissez ou mappez la valeur à rechercher.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort] </td> 
   <td> <p>Pour chaque niveau par lequel vous souhaitez trier les résultats, cliquez sur <strong>[!UICONTROL Ajouter un élément]</strong>, puis sélectionnez le champ par lequel vous souhaitez trier les résultats et indiquez si vous souhaitez trier les résultats par ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Saisissez ou mappez le nombre maximal d’enregistrements que le module doit renvoyer pour chaque cycle d’exécution du scénario.</p> </td> 
  </tr> 
 </tbody> 
</table>
