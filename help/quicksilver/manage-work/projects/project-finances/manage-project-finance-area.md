---
product-area: projects
navigation-topic: financials
title: Gérer les informations dans la zone Finances d’un projet
description: Gérer les informations dans la zone Finances d’un projet
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: 647788221b4acff1cfd5e0ce14d5b99cf90ceee0
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 14%

---

# Gérer les informations dans la zone Finances d’un projet

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Vous pouvez afficher ou modifier les informations financières d’un projet en accédant à la zone Finance de la section Détails du projet . Il existe un nombre limité de champs que vous pouvez afficher ou modifier dans cette zone. Pour plus d’informations sur la modification de toutes les informations d’un projet, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Affichage ou accès supérieur à Projets et données financières</p> <p>Modifier l’accès aux projets et aux données financières pour modifier les informations financières sur le projet</p> <p><b>NOTE</b></p>
   <p> Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations d’un projet ou d’une version ultérieure incluant des autorisations View Finance</p> <p>Gérer les autorisations du projet qui incluent Gérer les finances pour modifier les informations financières du projet</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Présentation de la zone Finance

Tenez compte des points suivants lors de l’affichage ou de la modification d’informations dans la zone Finance :

* Les informations financières disponibles dans la zone Finance des Détails du projet représentent les valeurs cumulées au niveau du projet à partir des tâches, ainsi que les informations entrées directement sur le projet. Certaines informations financières peuvent être gérées au niveau du projet ainsi qu’au niveau de la tâche.
* Vous devez disposer des autorisations d’affichage sur le projet ainsi que de l’accès aux données financières à partir de votre niveau d’accès afin de pouvoir afficher la zone Finance sur un projet.
* Vous devez disposer des autorisations de gestion sur le projet ainsi que de l’accès aux données financières à partir de votre niveau d’accès afin de pouvoir modifier les informations de la zone Finance . Cependant, nous recommandons que seul le propriétaire du projet modifie les informations sur cette zone .

## Affichage des informations financières sur un projet

1. Accédez à un projet.
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) dans le coin supérieur droit de la section Détails, puis cliquez sur **Finance**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront a configuré votre modèle de mise en page, la section Aperçu peut ne pas être répertoriée en premier, auquel cas elle est réduite. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Affichez les champs suivants dans la zone Finance du projet :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Méthode d'indice de performances</td> 
      <td> Contrôle la méthode utilisée par Workfront pour calculer les mesures de valeur obtenue. Il peut être basé sur les heures ou sur les coûts. <br>Pour plus d’informations sur le PIM, consultez l’article <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Définition de la méthode d’index de performance (PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">IPC/SPI/CSI</td> 
      <td> <p>Il s’agit de mesures de performances de projet qui indiquent les performances de votre projet à un moment donné. Leurs valeurs sont calculées selon la méthode de l’index de performance.<br>Pour plus d’informations, voir les articles suivants : </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calculer l’index de performance des coûts (IPC)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calculer l’index de performance de planification (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calculer l’index de performance de la planification des coûts (CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimation à l'achèvement</td> 
      <td> Coût total prévu de votre projet, représenté en heures si la méthode d’index de performance (PIM) est basée sur les heures et est représentée dans une valeur monétaire, si la méthode d’index de performance (PIM) est basée sur les coûts.<br>Pour plus d’informations sur le calcul de l’estimation à la fin, consultez l’article <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcul de l’estimation à la fin (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Il s’agit du budget défini pour le projet. Ceci est spécifié manuellement par le propriétaire du projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts fixes</td> 
      <td>Il s’agit des coûts d’exploitation du projet, indépendamment des autres activités du projet. Elles sont saisies manuellement par le propriétaire du projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts prévus</td> 
      <td>Coût estimé du projet, en fonction des Heures planifiées et des taux associés aux personnes désignées pour la tâche (rôles de tâche ou utilisateurs).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts réels</td> 
      <td>Tous les coûts du projet. Le coût réel est la somme de tous les coûts réels : le coût du travail (basé sur les Heures réelles et les taux associés aux rôles de travail ou aux utilisateurs qui les enregistrent), les dépenses et les coûts fixes, qui peuvent être associés à un projet ou à une tâche.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus fixes</td> 
      <td>Définissez les recettes attendues en fonction du planning du projet. Les recettes fixes sont spécifiées manuellement par le propriétaire du projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus prévus</td> 
      <td>Chiffre d’affaires prévisionnel attendu selon les Heures prévues et les taux associés aux personnes désignées pour la tâche (rôles de travail ou utilisateurs).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenu réel</td> 
      <td>Recettes réelles du projet basées sur les Heures réelles et les taux associés aux personnes désignées pour la tâche (rôles de tâche ou utilisateurs).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus facturés</td> 
      <td> <p>Recettes facturées aux clients ou à d’autres parties capturées dans les enregistrements de facturation. Pour plus d’informations sur les enregistrements de facturation, consultez l’article <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Créer des enregistrements de facturation</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## Modification des informations financières d’un projet

En tant que propriétaire de projet, vous pouvez modifier les informations du sous-onglet Finance d’un projet.

Pour modifier les informations sur le sous-onglet Finance de projet :

1. Accédez à un projet dont vous êtes le propriétaire.

   >[!NOTE]
   >
   >Pour effectuer les étapes suivantes, vous devez gérer les autorisations du projet. Nous recommandons également que seul le propriétaire du projet modifie le sous-onglet Finance du projet.

1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Cliquez sur l’icône **Modifier** ![](assets/edit-icon.png) dans le coin supérieur droit de la section Détails, puis cliquez sur **Finance** . La zone Finance s’ouvre alors pour modification.
1. Modifiez n’importe quel champ disponible pour modification, en cliquant une seule fois sur le champ ou en cliquant sur **+Ajouter** pour ajouter des informations à un champ vide.

   >[!TIP]
   >
   >Les champs ne peuvent pas être modifiés s’ils sont automatiquement calculés par Workfront ou si vous ne disposez pas d’autorisations de modification.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Mettez à jour l’un des champs ci-dessous.

   >[!NOTE]
   >
   >Selon la manière dont votre administrateur Workfront configure notre modèle de mise en page, les champs de la section Détails du projet peuvent être différents dans votre environnement. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Méthode d'indice de performances</td> 
      <td> <p>Contrôle la méthode utilisée par Workfront pour calculer les mesures de performances du projet. Il est configuré au niveau du système par votre administrateur, mais vous pouvez également le modifier au niveau du projet. Choisissez l’une des options suivantes :</p> 
       <ul> 
        <li><strong>Basé sur l’heure : </strong>Workfront utilise les heures planifiées dans le calcul de l’IPC et de l’EAC du projet, et l’EAC du projet s’affiche sous forme de nombre, en heures. </li> 
        <li><strong>Basé sur les coûts : </strong>Workfront utilise le coût de la main-d’oeuvre planifiée dans le calcul de l’IPC et du CAE du projet, et le CAE s’affiche sous forme de valeur monétaire. Lorsque vous sélectionnez cette option, assurez-vous que les personnes désignées pour les tâches (rôles de tâche ou utilisateurs) sont associées aux taux de coût.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimation à l'achèvement</td> 
      <td> <p>Représente le coût total prévu de votre projet ou de votre tâche une fois qu’elle s’est terminée. Il est configuré au niveau du système par votre administrateur, mais vous pouvez également le modifier au niveau du projet. Choisissez l’une des options suivantes :</p> 
       <ul> 
        <li><strong>Calculer au niveau du projet</strong> : les champs de contrôle d’accès de la tâche parent et du projet sont déterminés en saisissant les heures réelles/le coût réel de la main-d’oeuvre dans les formules du contrôle d’accès. Ce calcul inclut les Heures/coûts réels et les dépenses ajoutées directement à la tâche ou au projet parent.</li> 
        <li><strong>Cumul à partir des tâches/sous-tâches</strong> : les champs d’évaluation cumulés de la tâche parent et du projet sont déterminés en additionnant les champs d’évaluation cumulés de chaque tâche enfant. Ce calcul exclut les Heures/coûts réels et les dépenses ajoutées directement à la tâche ou au projet parent.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Indiquez le budget de ce projet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Coûts fixes</td> 
      <td>Indiquez le coût fixe de ce projet. Cela ne doit pas inclure de coûts de main-d'oeuvre ou de dépenses.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Revenus fixes</td> 
      <td> <p>Indiquez les recettes fixes de ce projet. Cela ne doit pas inclure les recettes provenant d’enregistrements de facturation facturés à des partenaires ou à des tiers.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Devise du projet</td> 
      <td> <p>Indiquez une devise pour ce projet, si elle diffère de la devise par défaut de votre système. La devise par défaut de votre système est définie par votre administrateur Workfront. Pour plus d’informations sur la configuration des taux d’exchange dans Workfront, consultez l’article <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configuration des taux d’exchange</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer les modifications**.
