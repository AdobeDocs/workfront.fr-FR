---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Planifier la remise automatique d’un rapport
description: Planifier la remise automatique d’un rapport
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 2%

---

# Planifier la remise automatique d’un rapport

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Vous pouvez planifier la remise automatique des rapports aux utilisateurs selon un calendrier défini ou envoyer manuellement les rapports ponctuellement. Lorsque vous envoyez un rapport d’Adobe Workfront, l’utilisateur reçoit un courrier électronique contenant le rapport Workfront en pièce jointe distincte.

Pour plus d’informations, y compris les limites de taille qui peuvent affecter la distribution de vos rapports, voir [Présentation de la diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer, vous devez créer un rapport. Pour en savoir plus sur la création de rapports, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Planification de la remise d’un rapport

Pour planifier la remise automatique d’un rapport, modifier ou supprimer une remise existante d’un rapport : &#x200B;

1. Accédez à un rapport dont vous souhaitez planifier la remise.

   >[!NOTE]
   >
   >Les diffusions de rapports ne contiennent pas d’invites. Si vous souhaitez limiter les données dans une diffusion de rapport, il est recommandé d&#39;appliquer des filtres sur le rapport que vous souhaitez envoyer.

1. Cliquez sur **Actions de rapport**, puis **Envoyer le rapport**.

   Le **Envoyer le rapport** s’affiche.

   >[!TIP]
   >
   >Pour envoyer manuellement un rapport à un moment donné, accédez au rapport, puis cliquez sur **Actions de rapport** > **Envoyer le rapport** > **Envoyer maintenant**.

1. Sélectionnez la **Diffusions répétées** .
1. (Conditionnel) Pour modifier une diffusion de rapport qui se répète, sélectionnez la diffusion de rapport dans le **Diffusions répétées** .
1. Indiquez les informations suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Envoyer à</p> </td> 
      <td> <p>Commencez à saisir le nom de l’utilisateur, du groupe, de l’équipe ou du rôle auquel vous souhaitez envoyer le rapport, puis cliquez sur le nom qui s’affiche dans la liste déroulante.</p> <p>Ou</p> <p>Indiquez l’adresse électronique d’une personne externe au système Workfront à qui vous souhaitez accéder au rapport.</p> <p>Répétez cette procédure pour envoyer le rapport à plusieurs utilisateurs, groupes, équipes ou rôles.</p> <p>Note:  <p>Tenez compte des points suivants lors de l’ajout de destinataires de diffusion de rapports :</p> 
        <ul> 
         <li>Si votre entreprise limite les notifications Workfront à des domaines de messagerie spécifiques, vous pouvez uniquement envoyer des rapports aux adresses électroniques répertoriées dans la liste autorisée de messagerie.<p>Pour plus d’informations sur la façon dont un administrateur Workfront met à jour la liste autorisée de messagerie, voir la section <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configuration de votre liste autorisée de messagerie</a>.</p></li> 
         <li> <p>L'ajout d'un grand nombre d'utilisateurs en tant que destinataires peut entraîner l'échec de la diffusion. Si vous rencontrez des diffusions en échec, vous pouvez planifier plusieurs diffusions de rapports avec des groupes d’utilisateurs plus petits.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Objet de l'e-mail</p> </td> 
      <td> <p>Indiquez l’objet de la notification par courrier électronique.</p> <p>Par défaut, l'objet de l'email est :</p> <p><em>Rapport Workfront : [Nom du rapport] [Date]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Message électronique</p> </td> 
      <td> <p>Spécifiez un message à inclure dans le courrier électronique.</p> <p>Par défaut, le message électronique est :</p> <p><em>Le rapport [fréquence du rapport] [nom du rapport] généré par Workfront le [date] est joint.</em> </p> <p>Remarque : Pour les rapports livrés sous la forme d’un fichier Excel uniquement, le message suivant est également ajouté à l’email : "Veuillez noter qu’avec les types de fichiers MS Excel (XLS), il existe une limite (65 530) de liens hypertextes pris en charge par ces types de fichiers. Si vous dépassez ces limites, votre fichier ne s’ouvre pas et il est recommandé de le renvoyer sans hyperliens. Revenez au planificateur de rapports pour supprimer les liens hypertexte et renvoyer le rapport." L’expression "veuillez revenir au planificateur de rapports" est un lien renvoyant au rapport.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Diffuser ce rapport avec les droits d'accès de</p> </td> 
      <td> <p>Commencez à saisir le nom d’un utilisateur ayant accès au rapport, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante. Les utilisateurs qui reçoivent le rapport auront le même niveau d’accès que l’utilisateur spécifié ici.<br> Pour plus d’informations, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Exécution et diffusion d’un rapport avec les droits d’accès d’un autre utilisateur</a>.</p> <p>Remarque : Ce champ ne prend pas en charge les caractères génériques. Par exemple, l’utilisation du caractère générique $$User.ID n’exécute pas le rapport avec les droits d’accès de l’utilisateur qui reçoit le rapport.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Format</p> </td> 
      <td> <p>Sélectionnez le format souhaité pour le rapport remis :</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Si vous sélectionnez cette option, vous pouvez formater la sortie à l’aide de l’option <strong>Format du papier</strong> et <strong>Orientation</strong> qui s’affichent.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inclure des liens</p> </td> 
      <td> <p>Cette option est disponible uniquement lorsque <strong>MS Excel</strong> est sélectionné dans la variable <strong>Format</strong> menu déroulant. Lorsque cette option est activée, tous les liens hypertexte sont inclus dans le document Excel exporté.</p> <p>Les documents contenant plus de 65 530 liens ne peuvent pas être ouverts. Si le document exporté contient plus de 65 530 liens, désélectionnez cette option.</p> <p>Cette option est activée par défaut.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Résumé</p> </td> 
      <td> <p>Affiche un résumé du moment où la diffusion se répète.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se répète</p> </td> 
      <td> <p>Indiquez si le rapport doit être diffusé tous les jours, toutes les semaines, tous les mois ou tous les ans.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se répète tous les</p> </td> 
      <td> <p>Sélectionnez la fréquence de répétition de la diffusion. La valeur que vous sélectionnez pour cette option est basée sur l’option sélectionnée dans la variable <strong>Répéter</strong> liste déroulante.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Heure</p> </td> 
      <td> <p>Sélectionnez l'heure de la journée d'envoi de la diffusion.</p> <p>Conseil : Les chargements du système pouvant avoir une incidence sur les heures de remise des rapports, un délai peut s’écouler entre l’heure planifiée et l’heure de remise réelle. Si vous avez besoin d'un rapport livré selon une heure spécifique, nous vous recommandons de planifier la diffusion avant le moment où elle est nécessaire. Par exemple, nous vous recommandons de planifier la diffusion un jour avant la date à laquelle elle est nécessaire.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se répète le</p> </td> 
      <td> <p>Cette option est disponible lorsque la variable <strong>Répéter</strong> est définie sur l’une des options suivantes : <strong>Hebdomadaire</strong> ou <strong>Mensuel</strong>:</p> 
       <ul> 
        <li> <p>Lorsque la variable <strong>Répéter</strong> est définie sur <strong>Hebdomadaire</strong>: Sélectionnez les jours de la semaine où la diffusion est envoyée.</p> </li> 
        <li> <p>Lorsque la variable <strong>Répéter</strong> est définie sur <strong>Mensuel</strong>: Indiquez si la diffusion est envoyée le jour du mois, le jour de la semaine ou le dernier jour du mois (ces options utilisent la date que vous avez sélectionnée dans la variable <strong>Commence par</strong> ).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Commence le</p> </td> 
      <td>Sélectionnez la date de début de la diffusion planifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se termine le</p> </td> 
      <td>Sélectionnez la date de fin de la diffusion planifiée.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Jamais</p> </td> 
      <td>Sélectionner <strong>Jamais</strong> si vous souhaitez que la diffusion planifiée dure indéfiniment.</td> 
     </tr> 
    </tbody> 
   </table>

1. Cliquez sur **Enregistrer** pour enregistrer la diffusion du rapport.

   Le rapport s’affiche dans la variable **Diffusions répétées** (dans la section **Envoyer le rapport** ) et elle sera envoyée à l’heure planifiée.

   Pour plus d’informations sur les limites de taille qui peuvent affecter la distribution de vos rapports, reportez-vous aux sections [Limites de diffusion des rapports](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) et [Limites d’exportation](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. (Facultatif) Pour supprimer une diffusion planifiée :

   1. Dans le **Diffusions répétées** , cliquez sur la diffusion planifiée, puis sur **Supprimer**.
   1. Cliquez sur **Supprimer** pour confirmer.

## Présentation vidéo

Consultez la vidéo suivante pour savoir comment planifier la remise d’un rapport. Cette vidéo a été enregistrée dans Workfront Classic. Cependant, le contenu s’applique également à la nouvelle expérience Workfront.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
