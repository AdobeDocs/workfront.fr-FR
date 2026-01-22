---
title: Supprimer types d’enregistrements
description: Vous pouvez supprimer des types d’enregistrement lorsqu’ils ne sont plus pertinents. La suppression des types d’enregistrement supprime également toutes les informations associées aux types d’enregistrement, telles que leurs enregistrements, champs et vues.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 5bccad02f90fd99135b50c5a929913b16cc5b809
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 21%

---


<!--keep the global record type reference in yellow till January 2026-->

# Supprimer des types d’enregistrements

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Vous pouvez supprimer des types d’enregistrement lorsqu’ils ne sont plus pertinents.

Cependant, la suppression des types d’enregistrement supprime également toutes les informations associées aux types d’enregistrement. Pour plus d’informations, consultez la section [Remarques concernant la suppression de types d’enregistrement](#considerations-when-deleting-record-types) de cet article.

Pour plus d’informations sur les types d’enregistrements, voir [ Présentation des types d’enregistrements ](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Conditions d’accès

+++ Développez pour afficher les conditions d’accès requises pour la fonctionnalité de cet article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Package Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Tout Workfront et tout package Planning</p></li>
Ou
<li><p>Tout workflow et tout package Planning</p></li></ul>

<p>Pour supprimer des types d’enregistrements globaux :</p>
<ul><li><p>Tout package Workfront et un package Planning Plus</p></li>
Ou
<li><p>Tout workflow et un package Planning Prime ou Ultimate</p></li></ul>

<p>Pour plus d’informations sur les composants inclus dans chaque package Workfront Planning, contactez votre représentant de compte Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licence Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Autorisations d’objet</p></td> 
   <td>   <p>Gérer les autorisations d’un espace de travail</p>  
   <p>L’administration système a accès à tous les espaces de travail, y compris ceux qu’elle n’a pas créés.</p>  </td> 
  </tr>  
</tbody> 
</table>

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Exigences d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## Remarques concernant la suppression de types d’enregistrement

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Vous ne pouvez supprimer que les types d’enregistrement des espaces de travail pour lesquels vous disposez d’autorisations de gestion.
* La suppression des types d’enregistrement supprime les informations suivantes qui leur sont associées :

   * Tous les enregistrements de ce type
   * Tous les champs associés au type d’enregistrement
   * Toutes les vues (y compris les filtres, les regroupements et les critères de tri) du type d’enregistrement
* Le type d’enregistrement est supprimé pour toutes les personnes accédant à l’espace de travail.
* La suppression des types d’enregistrements et leurs informations associées est irréversible.
* Il est recommandé de recréer les champs et les enregistrements associés au type d’enregistrement que vous souhaitez supprimer sur un autre type d’enregistrement avant de les supprimer.

* Vous ne pouvez pas supprimer un type d&#39;enregistrement global qui a été ajouté à d&#39;autres espaces de travail.

  Pour plus d’informations, consultez la section [Supprimer des types d’enregistrements globaux](#delete-global-record-types) dans cet article.

## Supprimer des types d’enregistrements

{{step1-to-planning}}

1. Cliquez sur l’espace de travail dont vous souhaitez supprimer les types d’enregistrements,

   Ou

   Depuis un espace de travail, développez la flèche pointant vers le bas à droite d’un nom d’espace de travail existant, recherchez un espace de travail, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   L’espace de travail et les types d’enregistrement s’affichent.
1. Utilisez l’une des méthodes suivantes :

   * Pointez sur la carte de type d’enregistrement, cliquez sur le menu **Plus**, puis **Supprimer**.
   * Cliquez sur la carte du type d’enregistrement à supprimer, puis, dans la page du type d’enregistrement, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) à droite du nom du type d’enregistrement, puis cliquez sur **Supprimer**.

     >[!TIP]
     >
     >Vous ne pouvez pas supprimer un type d’enregistrement global de l’espace de travail secondaire où il a été ajouté à partir de la page du type d’enregistrement. Vous pouvez uniquement la supprimer de la carte de type d’enregistrement dans l’espace de travail.

     ![Confirmation de suppression définitive du type d’enregistrement](assets/permanently-delete-record-type-confirmation.png)


1. Saisissez **delete** dans la zone de confirmation, puis cliquez sur **Supprimer définitivement**. Cette opération n’est pas sensible à la casse.

   Le type d&#39;enregistrement sélectionné, ainsi que ses champs, les enregistrements associés et les vues sont supprimés et ne peuvent pas être récupérés.

## Supprimer les types d’enregistrements globaux

Les scénarios suivants existent lors de la suppression de types d’enregistrements globaux :

* Si un type d’enregistrement configuré comme global n’a pas encore été ajouté à un autre espace de travail, vous pouvez le supprimer de son espace de travail d’origine.

* Si un type d’enregistrement configuré en tant que type d’enregistrement global a été ajouté à au moins un autre espace de travail, vous ne pouvez pas le supprimer de son espace de travail d’origine. Vous devez d’abord supprimer (en supprimant) le type d’enregistrement global des espaces de travail secondaires où ils ont été ajoutés, puis vous pouvez supprimer définitivement le type d’enregistrement global de son espace de travail d’origine.

### Supprimer un type d’enregistrement global de l’espace de travail d’origine

Vous pouvez supprimer un type d’enregistrement de son espace de travail d’origine s’il n’est plus pertinent.

Tous les enregistrements et champs sont également supprimés et ne peuvent pas être récupérés.

1. Accédez au type d’enregistrement global dans son espace de travail d’origine.

1. (Conditionnel) Effectuez l’une des opérations suivantes, selon que le type d’enregistrement global a été ajouté ou non aux espaces de travail secondaires :

   * Si le type d’enregistrement n’a pas été ajouté à un espace de travail secondaire, cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) sur la carte du type d’enregistrement ou à droite du nom du type d’enregistrement sur sa page, puis cliquez sur **Supprimer**.
   * Si le type d’enregistrement a été ajouté à au moins un autre espace de travail secondaire, accédez d’abord à l’espace de travail secondaire et supprimez l’enregistrement global de cet espace.

     Pour plus d’informations, consultez la section [Supprimer un type d’enregistrement global d’un espace de travail secondaire](#delete-a-global-record-type-from-a-secondary-workspace) dans cet article.

1. (Conditionnel) Continuez la suppression du type d’enregistrement, comme décrit dans la section [Supprimer des types d’enregistrement](#delete-record-types-1) de cet article.

   Les événements suivants se produisent :

   * Le type d’enregistrement global est supprimé de l’espace de travail d’origine et le type d’enregistrement, ses enregistrements et champs ne peuvent pas être récupérés.
   * Tous les enregistrements globaux des espaces de travail secondaires et leurs enregistrements sont également supprimés de cet espace de travail.

### Supprimer un type d’enregistrement global d’un espace de travail secondaire

Vous pouvez supprimer un type d’enregistrement que vous avez ajouté à partir d’un autre espace de travail si nécessaire.

Tenez compte des points suivants :

* Lorsque vous supprimez un type d’enregistrement global d’un espace de travail secondaire, il reste dans l’espace de travail d’origine.

* Lorsque vous supprimez un type d’enregistrement global d’un espace de travail secondaire, les éléments suivants sont également supprimés :

   * Les enregistrements ajoutés depuis l’espace de travail secondaire sont supprimés de l’espace de travail secondaire et de l’espace de travail d’origine et ne peuvent pas être récupérés.

  <!--Coming later: * The fields added from the secondary workspace.-->

* Les types d’enregistrements globaux supprimés de leurs espaces de travail secondaires ne peuvent pas être récupérés.

* Le type d’enregistrement d’origine reste dans son espace de travail d’origine ainsi que dans les autres espaces de travail où il a été ajouté.

* Les vues ajoutées au type d’enregistrement dans l’espace de travail secondaire sont conservées et sont visibles dans d’autres espaces de travail, si elles sont partagées avec vous.

Pour supprimer un type d’enregistrement global d’un espace de travail secondaire :

1. Accédez au type d’enregistrement global dans son espace de travail secondaire.

1. (Facultatif) Cliquez sur le menu **Plus** ![Plus](assets/more-menu.png) sur la carte du type d’enregistrement, puis cliquez sur **Supprimer**.
1. (Conditionnel) Saisissez **delete** dans le champ fourni, puis cliquez sur **Supprimer définitivement**.

   ![Supprimer la boîte de confirmation de type d&#39;enregistrement global secondaire](assets/delete-secondary-global-record-type.png)

   Les événements suivants se produisent :

   * Le type d’enregistrement créé à partir d’un type d’enregistrement global est supprimé de l’espace de travail secondaire sélectionné.
   * Le type d’enregistrement d’origine et ses champs restent dans leur espace de travail d’origine.
   * Le type d’enregistrement reste dans tous les autres espaces de travail où il a été ajouté.
   * Les enregistrements <!--and fields--> ajoutés au type d’enregistrement de l’espace de travail secondaire sont supprimés. Tous les autres enregistrements ajoutés à partir d’espaces de travail supplémentaires où le type d’enregistrement global a été ajouté sont conservés dans leurs espaces de travail respectifs et dans l’espace de travail d’origine. &lt;!: les champs sont conservés dans les espaces de travail où ils ont été ajoutés.


