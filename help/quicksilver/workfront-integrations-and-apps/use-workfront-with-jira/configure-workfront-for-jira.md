---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurer  [!DNL Adobe Workfront for Jira]
description: Vous pouvez utiliser  [!DNL Adobe Workfront for Jira]  pour intégrer votre  [!DNL Jira]  et les systèmes  [!DNL Workfront] .
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '2454'
ht-degree: 95%

---

# Configurer [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>Pour offrir des intégrations plus stables et plus évolutives, nous passons à une approche d’intégration moderne et flexible à l’aide de Workfront Automation and Integration (Fusion). Dans le cadre de ce processus de transition, l’intégration Workfront for Jira ne sera plus disponible après le **28 février 2026**.
>
>Nous vous recommandons d’utiliser l’automatisation et l’intégration de Workfront pour les besoins d’intégration de votre organisation à Jira.
>
>Pour une présentation de l’automatisation et de l’intégration de Workfront, consultez [Présentation d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Pour plus d’informations sur les fonctionnalités spécifiques des modules d’automatisation et d’intégration de Workfront pour Jira, voir [Modules logiciels Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Vous pouvez utiliser [!DNL Adobe Workfront for Jira] pour intégrer vos systèmes [!DNL Jira] et [!DNL Workfront].

Après l’installation du module complémentaire, vous pouvez définir des workflows qui créent des problèmes [!DNL Jira] automatiquement lorsque des éléments de travail [!DNL Workfront] sont créés. Les éléments des deux applications sont liés et certaines de leurs informations sont automatiquement mises à jour dans les deux systèmes.

Tous les utilisateurs et utilisatrices de [!DNL Workfront] et [!DNL Jira] peuvent bénéficier de cette intégration. Ils n’ont besoin d’une licence que pour le système dans lequel ils travaillent le plus, et non pour les deux systèmes.

Ce module complémentaire est disponible à la fois pour les versions [!UICONTROL Serveur] et [!UICONTROL OnDemand] (ou [!UICONTROL Cloud]) du logiciel [!DNL Jira].

Pour une liste de versions [!DNL Jira] que [!DNL Workfront for Jira] prend actuellement en charge, voir [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) à l’adresse [!DNL Atlassian Marketplace].

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Tous</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Accès Jira</td> 
   <td> <p>Accès pour l’administration système</p> <p>Important : nous vous recommandons de créer des comptes d’administrateur système distincts dans Jira et Workfront à dédier à cette intégration, plutôt que d’utiliser des comptes existants qui peuvent être associés aux utilisateurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de pouvoir configurer [!DNL Workfront for Jira], vous devez :

* installer [!DNL Workfront for Jira].
Pour obtenir des instructions sur l’installation de [!DNL Workfront for Jira], voir [Installer  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurer [!DNL Workfront for Jira]

En configurant [!DNL Workfront for Jira], vous pouvez effectuer ce qui suit :

* Définir les déclencheurs qui vont créer des éléments [!DNL Jira] lorsque des éléments [!DNL Workfront] sont créés.
* Spécifier les champs à synchroniser entre les éléments liés entre [!DNL Jira] et [!DNL Workfront].

>[!NOTE]
>
>* Après avoir configuré [!DNL Workfront for Jira] sur votre environnement [!DNL Jira], tous les utilisateurs et utilisatrices de [!DNL Jira] voient un panneau droit [!DNL Workfront] sur tous les éléments [!DNL Jira]. Le panneau contient des informations sur les éléments pouvant être liés à partir de [!DNL Workfront] ou spécifie qu’aucun élément [!DNL Workfront] n’est lié à des éléments [!DNL Jira].
>* Lors de l’utilisation de l’installation [!DNL Jira Server], seuls les problèmes associés aux projets identifiés comme déclencheurs de l’intégration Workfront affichent le panneau Workfront. Pour plus d’informations sur la configuration des déclencheurs pour le workflow [!DNL Workfront to Jira], voir [Configurer des déclencheurs pour la liaison automatique d’éléments entre  [!DNL Jira]  et  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Pour configurer [!DNL Workfront for Jira], procédez comme suit :

1. Connectez-vous à [!DNL Jira] en tant qu’administrateur ou administratrice [!DNL Jira].
1. Cliquez sur **[!UICONTROL Paramètres]** dans le menu principal [!DNL Jira].
1. Cliquez sur **[!UICONTROL Modules complémentaires]**, puis cliquez sur **[!UICONTROL Gérer les modules complémentaires]**.

1. Développez le module complémentaire **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Suivez les invites pour vous connecter à [!DNL Workfront].

   >[!NOTE]
   >
   >Une personne doit disposer d’un `apiKey` valide dans [!UICONTROL Workfront] pour établir une connexion réussie.

   Vous devez vous connecter à [!DNL Workfront] en tant qu’administrateur ou administratrice [!DNL Workfront] pour poursuivre la configuration.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] se connecte à [!DNL Jira] en utilisant OAuth 2.0, une norme utilisée par la plupart des intégrations web pour l’authentification et l’autorisation des utilisateurs et utilisatrices.
   >* Lorsque vous recevez une invitation à saisir le domaine de votre compte [!DNL Workfront], saisissez-le au format suivant : *domaineDeVotreEntreprise.my.workfront.com*. Le domaine de votre entreprise est généralement le nom de votre entreprise.
   >* L’authentification améliorée n’est pas disponible tant qu’un administrateur ou une administratrice de [!DNL Workfront] ne l’a pas activée pour cette intégration.

1. Dans Jira, sélectionnez l’option **[!UICONTROL Triggers]** pour configurer la création automatique d’éléments [!DNL Jira] au fur et à mesure que de nouveaux éléments [!DNL Workfront] sont créés.

   Pour plus d’informations sur la configuration des déclencheurs pour le workflow Workfront vers [!DNL Jira], voir [Configurer des déclencheurs pour la liaison automatique d’éléments entre  [!DNL Jira]  et  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Sélectionnez l’onglet **[!UICONTROL Configuration]** pour configurer la synchronisation des champs entre les éléments [!DNL Jira] et [!DNL Workfront] liés.

   Pour plus d’informations sur la configuration de la synchronisation des champs entre [!DNL Jira] et [!DNL Workfront], voir [Configurer la synchronisation des champs entre les éléments  [!DNL Jira]  et  [!DNL Workfront] ](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Après avoir défini les déclencheurs et la synchronisation des champs entre les deux applications, toute personne utilisant [!DNL Workfront] qui peut créer des tâches ou des problèmes peut potentiellement déclencher la création d’un élément dans [!DNL Jira]. La personne peut créer un élément si les critères de l’élément créé correspondent aux déclencheurs dans [!DNL Jira], même si la personne n’a pas de licence [!DNL Jira]. En outre, toute personne utilisant [!DNL Jira] peut immédiatement commencer à travailler sur l’élément [!DNL Jira] et ses mises à jour sont visibles dans [!DNL Workfront], sans nécessiter de licence [!DNL Workfront]. Toutes les mises à jour dans [!DNL Workfront] sont également visibles sur les éléments [!DNL Jira].

1. (Facultatif) Sélectionnez l’onglet **[!UICONTROL Journal d’activité]** pour passer en revue les erreurs qui se sont produites pendant l’intégration.

   Pour plus d’informations sur le [!UICONTROL Journal d’activité], voir [Afficher le Journal d’activité  [!DNL Jira] ](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurer des déclencheurs pour la liaison automatique d’éléments entre [!DNL Jira] et [!DNL Workfront]

En tant qu’administrateur ou administratrice système [!DNL Jira], vous pouvez définir des déclencheurs qui créent automatiquement des problèmes dans [!DNL Jira] lorsqu’un élément dans [!DNL Workfront] répond à certains critères.

>[!NOTE]
>
>L’intégration peut prendre jusqu’à 10 minutes pour créer de nouveaux problèmes dans [!DNL Jira].

Tenez compte de ce qui suit lors de la configuration du déclenchement de la création d’éléments [!DNL Jira] au fur et à mesure que des éléments [!DNL Workfront] sont créés :

* L’intégration est unidirectionnelle : vous ne pouvez que déclencher la création automatique dans [!DNL Jira] des éléments que vous créez dans [!DNL Workfront] . Vous ne pouvez pas déclencher la création automatique dans [!DNL Workfront] des éléments que vous créez dans [!DNL Jira].
* Le nombre de déclencheurs que vous pouvez avoir n’est pas limité.
* Si un élément créé dans [!DNL Workfront] correspond à plusieurs déclencheurs, un seul élément est créé dans [!DNL Jira]. L’élément est créé dans [!DNL Jira] selon le premier déclencheur (dans l’ordre dans lequel ils ont été définis dans [!DNL Jira]). Tous les autres déclencheurs sont ignorés.
* Un seul élément dans [!DNL Workfront] peut être lié à un élément dans Jira. Vous ne pouvez jamais lier un élément [!DNL Workfront] à plusieurs problèmes [!DNL Jira] ou un problème [!DNL Jira] à plusieurs éléments [!DNL Workfront].

Pour configurer des déclencheurs afin de créer automatiquement des éléments dans [!DNL Jira] :

1. Connectez vous à [!DNL Jira] en tant qu’administrateur ou administratrice système.
1. Cliquez sur **[!UICONTROL Paramètres]** dans le menu [!DNL Jira] principal.
1. Cliquez sur **[!UICONTROL Modules complémentaires]**, puis sur **[!UICONTROL Gérer les modules complémentaires]**.
1. Développez le module complémentaire **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur ou administratrice système.

   L’onglet **[!UICONTROL Déclencheurs]** est sélectionné par défaut dans Jira.

1. Cliquez sur **[!UICONTROL Ajouter un déclencheur]** pour ajouter un nouveau déclencheur.
1. Dans le champ **[!UICONTROL Équipe/utilisateur/utilisatrice/rôle Workfront]**, indiquez le nom d’une équipe, d’un utilisateur/utilisatrice ou d’une fonction [!DNL Workfront], puis cliquez pour le sélectionner lorsqu’il s’affiche dans la liste.

   >[!NOTE]
   >
   >Une même équipe, un même utilisateur ou une même utilisatrice ou un même rôle ne peut pas avoir plusieurs déclencheurs.

   Lorsqu’une personne crée une tâche ou un problème et l’affecte à l’une de ces entités, un problème est automatiquement créé dans [!DNL [!DNL Jira]].

1. Dans le champ de projet **[!UICONTROL [!DNL Jira]]**, commencez à saisir le nom d’un projet [!DNL Jira], puis cliquez pour le sélectionner lorsqu’il s’affiche dans la liste.

   Lorsque le problème [!DNL Jira] est créé, il est placé sur le projet que vous avez choisi ici.

1. Sélectionnez un **[!UICONTROL type de problème]** dans le menu déroulant.

   Cela indique le type de problème créé dans [!DNL Jira] lorsque les conditions de ce déclencheur sont remplies, en fonction de vos paramètres pour ce projet spécifique dans [!DNL Jira].

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Avec cette configuration, chaque fois qu’un utilisateur ou une utilisatrice [!DNL Workfront] crée un élément correspondant aux déclencheurs spécifiés, un nouveau problème est créé dans [!DNL Jira].

## Configurer la synchronisation des champs entre des éléments [!DNL Jira] et [!DNL Workfront]

En tant qu’administrateur ou administratrice [!DNL Jira], vous pouvez définir les champs à synchroniser automatiquement sur les éléments liés entre [!DNL Workfront] et Jira. Certains champs peuvent se synchroniser de l’élément [!DNL Workfront] vers l’élément [!DNL Jira] et d’autres se synchroniser de Jira vers Workfront.

Pour définir les champs à synchroniser automatiquement sur les éléments liés entre les deux applications :

1. Connectez-vous à [!DNL Jira] en tant qu’administrateur ou administratrice de Jira.
1. Cliquez sur **[!UICONTROL Paramètres]** dans le menu [!DNL Jira] principal.
1. Cliquez sur **[!UICONTROL Modules complémentaires]**, puis sur **[!UICONTROL Gérer les modules complémentaires]**.
1. Développez le module complémentaire **[!DNL Workfront]**.
1. Cliquez sur **[!UICONTROL Configurer]**.
1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur ou administratrice de Workfront.
1. Dans Jira, cliquez sur l’onglet **[!UICONTROL Configuration]**.
1. Dans la section **[!UICONTROL Synchroniser de Workfront vers Jira]**, sélectionnez les champs à mettre à jour dans [!DNL Jira] lorsqu’ils sont mis à jour dans Workfront.

   1. Sélectionnez l’une des fréquences de synchronisation des champs :

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>Les champs que vous spécifiez sont synchronisés entre les éléments Workfront et [!DNL Jira] liés lors de la création de l’élément dans Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>Les champs que vous spécifiez sont synchronisés entre les éléments Workfront et [!DNL Jira] liés lorsque les champs sont mis à jour dans Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>Les champs que vous spécifiez ne sont jamais synchronisés entre les éléments [!DNL Workfront] et [!DNL Jira] liés. Il n’y a aucune indication dans [!DNL Jira] que le champ a été mis à jour dans [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Sélectionnez l’une des options suivantes pour synchroniser les champs de [!DNL Workfront] vers [!DNL Jira] :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Le nom d’une tâche ou d’un problème dans [!DNL Workfront] devient le nom du problème auquel il est lié dans [!DNL Jira].</p><p>Remarque : lorsque de nouveaux éléments sont créés automatiquement dans [!DNL Jira], le nom [!DNL Workfront] est toujours mis à jour sur l’élément [!DNL Jira], que ce champ soit activé ou non ici. Lorsqu’un élément [!DNL Jira] est lié manuellement à un élément [!DNL Workfront], le nom de l’élément [!DNL Workfront] se met à jour uniquement dans [!DNL Jira] lorsque vous sélectionnez de <strong>Toujours</strong> synchroniser ce champ. Pour plus d’informations sur la liaison manuelle ou automatique d’éléments, voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Lier des éléments entre [!DNL Adobe Workfront] et [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>La description d’une tâche ou d’un problème dans [!DNL Workfront] devient la description du problème auquel il est lié dans [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documents</td>
         <td><p>Les documents joints à une tâche ou à un problème dans [!DNL Workfront] sont également joints au problème auquel il est lié dans Jira. Les nouvelles versions de document de [!DNL Workfront] sont ajoutées en tant que documents distincts à Jira et sont ajoutés avec <i>_v&lt;version number&gt;</i> pour indiquer la version numérotée dans Workfront. </p><p>Par exemple, si le nom d’un document dans [!DNL Workfront] est <strong>Main Ad</strong> (publicité principale), et que vous y ajoutez une nouvelle version dans [!DNL Workfront], la nouvelle version est transférée à [!DNL Jira] en tant que nouveau document portant le nom <strong>Main Ad_v2</strong>.</p><p>Important : <p>Tenez compte des points suivants lors de la synchronisation de documents :</p>
           <ul>
            <li><p>Les documents de plus de 5 Mo ne sont pas synchronisés. Si la synchronisation d’un document échoue parce que le document est trop volumineux, une erreur est consignée dans le journal d’activité. </p><p>Pour plus d’informations sur le journal d’activité, voir <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Afficher le journal d’activité Jira</a>.</p></li>
            <li><p>Les documents liés à des tâches et des problèmes depuis des serveurs externes ne sont pas transférés vers les éléments [!DNL Jira]. Seuls les documents chargés directement sur la tâche ou le problème dans [!DNL Workfront] sont transférés vers le problème lié dans [!DNL Jira].</p></li>
            <li><p>Pour créer une épreuve à partir d’un document, vous devez générer l’épreuve dans [!DNL Workfront]. </p><p>Pour plus d’informations sur la génération d’une épreuve, voir <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Créer une épreuve pour un document existant </a>dans <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Créer une épreuve pour un document</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Planned Completion Date]</td>
         <td><p>La [!UICONTROL Planned Completion Date] d’une tâche ou d’un problème dans [!DNL Workfront] devient la [!UICONTROL Due Date] du problème auquel il est lié dans [!DNL Jira].</p><p>Note : assurez-vous d’afficher la <strong>[!UICONTROL Due Date]</strong> sur les problèmes [!DNL Jira], pour que cette valeur se synchronise.</p></td>
        </tr>
       </tbody>
      </table>

1. Dans la section **[!UICONTROL Synchroniser depuis [!DNL Jira] vers[!DNL Workfront]]**, sélectionnez les champs à mettre à jour dans [!DNL Workfront] lorsqu’ils sont mis à jour dans [!DNL Jira].

   1. Sélectionnez l’une des fréquences de synchronisation des champs :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>Les champs que vous spécifiez sont toujours synchronisés entre les éléments [!DNL Workfront] et [!DNL Jira] lorsque les champs sont mis à jour dans [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>Les champs que vous spécifiez ne sont jamais synchronisés entre les éléments [!DNL Workfront] et [!DNL Jira]. Il n’y a aucune indication dans [!DNL Workfront] que le champ a été mis à jour dans [!DNL Jira].</p><p>Note : lorsque vous sélectionnez Jamais, les champs [!DNL Workfront] peuvent toujours être mis à jour manuellement à partir de [!DNL Jira] dans le panneau [!DNL Workfront] de gauche du problème [!DNL Jira]. Ces mises à jour n’apparaissent que sur les éléments [!DNL Workfront] dans [!DNL Jira] et [!DNL Workfront], et non sur les éléments [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

   1. Sélectionnez cette option pour synchroniser l’un des champs suivants de [!DNL Jira] vers [!DNL Workfront] :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>Le [!UICONTROL Status] d’un problème dans [!DNL Jira] devient le [!UICONTROL Status] de la tâche ou du problème auquel il est lié dans [!DNL Workfront].<br>Pour plus d’informations sur les statuts [!DNL Workfront], voir <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Créer ou modifier un statut</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>La [!UICONTROL Assignee] d’un problème dans [!DNL Jira] devient la [!UICONTROL Assignee] de la tâche ou du problème auquel il est lié dans [!DNL Workfront].</p><p>Important : lorsque vous affectez un élément dans [!DNL Jira] à une personne qui ne dispose pas de compte [!DNL Workfront], l’intégration crée un utilisateur actif ou une utilisatrice active dans [!DNL Workfront] uniquement lorsque l’option <strong>Créer automatiquement un utilisateur ou une utilisatrice dans [!DNL Workfront] si l’utilisateur ou l’utilisatrice [!DNL Jira] ne possède pas de compte [!DNL Workfront]</strong> est définie sur <strong>[!UICONTROL Always]</strong>. Cette personne ne dispose pas de licence [!DNL Workfront].Les utilisateurs et utilisatrices actifs peuvent être affectés à des éléments de travail dans [!DNL Workfront], mais ne peuvent pas être inclus dans les mises à jour. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Les pièces jointes d’un problème dans [!DNL Jira] sont également associées à l’objet (tâche ou problème) auquel il est lié dans [!DNL Workfront].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>Un commentaire sur un problème [!DNL Jira] est également publié sur l’élément [!DNL Workfront] lié dans la zone [!UICONTROL Updates]. À l’inverse, un commentaire publié dans la zone [!UICONTROL Updates] pour une tâche ou un problème [!DNL Workfront] se synchronise avec le flux des commentaires natifs de [!DNL Jira] pour le problème lié. </p><p>Ceci est défini sur <strong>[!UICONTROL Always]</strong> par défaut. Si vous sélectionnez <strong>[!UICONTROL Never]</strong> ici, vous pouvez toujours publier des commentaires manuellement sur un élément lié, dans [!DNL Workfront] ou dans [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. Dans la section **[!UICONTROL AUTRES]**, sélectionnez les champs supplémentaires à mettre à jour entre les éléments liés.

   1. Sélectionnez une option pour déterminer si les champs que vous réglez sur **[!UICONTROL Toujours]** ou **[!UICONTROL Jamais]** sont mis à jour dans [!DNL Jira] ou dans [!DNL Workfront] lorsqu’ils sont modifiés.

   1. Effectuez un choix dans les champs et mises à jour suivants :

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Custom Data in the right panel in [!DNL Jira]]</td>
         <td><p>Affiche les données personnalisées [!DNL Workfront] d’un élément dans le panneau droit de [!DNL Workfront].</p><p>Note : les sections Formulaire personnalisé s’affichent dans le panneau droit de [!DNL Workfront] avec le niveau d’accès de l’administration système [!DNL Workfront].</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Priority in the right panel in [!DNL Jira]]</td>
         <td>Affiche la priorité [!DNL Workfront] d’un élément dans le panneau droit de [!DNL Workfront].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Add an update in the [!DNL Workfront] Updates tab about Due Date changes in [!DNL Jira]]</td>
         <td>Ajoute un commentaire dans l’onglet [!UICONTROL Update] de l’élément [!DNL Workfront] lorsque la [!UICONTROL Due Date] change dans l’élément [!DNL Jira] lié.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatically create a user in [!DNL Workfront] if the [!DNL Jira] user does not have a [!DNL Workfront] account]</td>
         <td><p>Les scénarios suivants sont possibles :</p>
          <ul>
           <li>Lorsque vous sélectionnez <strong>[!UICONTROL Always]</strong>, vous activez l’intégration pour créer un utilisateur ou une utilisatrice Workfront à chaque fois qu’un utilisateur ou une utilisatrice [!DNL Jira] sans compte [!DNL Workfront] effectue les actions suivantes sur un problème [!DNL Jira] lié :
            <ul>
             <li>Affectation à un problème [!DNL Jira]</li>
             <li><p>Consignation de temps dans un problème [!DNL Jira]</p><p>Cette nouvelle personne ne dispose pas de licence [!DNL Workfront]. Le paramètre par défaut est Toujours.Le terme « [!UICONTROL Jira] » est ajouté au nom de la personne créée de cette façon dans [!DNL Workfront].</p></li>
            </ul></li>
           <li>Lorsque vous sélectionnez <strong>[!UICONTROL Never]</strong>, les événements suivants se produisent :
            <ul>
             <li>Vous ne pouvez pas voir les affectations [!DNL Jira] sur les éléments [!DNL Workfront]. Dans ce cas, seules les affectations effectuées dans [!DNL Workfront] s’affichent sur les éléments [!DNL Workfront].</li>
             <li>Les heures consignées sur un problème [!DNL Jira] lié par une personne ne disposant pas d’un compte [!DNL Workfront] ne sont pas automatiquement transférées vers l’élément [!DNL Workfront] lié. Vous pouvez toujours consigner les heures passées sur l’élément [!DNL Workfront] dans le panneau de droite du problème [!DNL Jira].</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Désormais, à chaque fois qu’une personne met à jour l’un des champs spécifiés dans cette configuration pour un élément dans [!DNL Jira] ou [!DNL Workfront], l’élément lié dans l’autre application est également mis à jour.

## Dépannage

### Les éléments ne peuvent pas être créés dans [!DNL Jira] en raison de champs déclencheurs marqués « [!UICONTROL Éléments introuvables] ».

#### Problème

Lorsqu’une erreur liée à l’application [!DNL Workfront for Jira] se produit, [!DNL Workfront] désactive les déclencheurs pour éviter d’autres complications. Lorsque ces déclencheurs sont désactivés, ils s’affichent sous la forme « [!UICONTROL Éléments introuvables] ».

#### Solution

Recherchez l’erreur qui a désactivé les déclencheurs. Vous trouverez l’erreur dans le [!UICONTROL Journal d’activité] [!DNL Workfront for Jira].

La cause la plus courante de ce comportement est l’erreur « [!UICONTROL Le champ « duedate » ne peut pas être défini. Il ne se trouve pas dans l’écran approprié ou il est inconnu.] »

Cette erreur signifie que vous tentez de synchroniser la « [!UICONTROL Date d’achèvement prévue] » de [!DNL Workfront] vers [!DNL Jira]. Pour ce faire, vous devez vous assurer que vos objets [!DNL Jira] ont un champ appelé « [!UICONTROL Date d’échéance] ». S’ils ne disposent pas de ce champ, [!DNL Workfront] ne peut pas synchroniser la date d’achèvement prévue à partir de [!DNL Workfront] et désactive vos déclencheurs.

Pour résoudre cette erreur, essayez l’une des méthodes suivantes :

* Demandez à votre équipe d’administration [!DNL Jira] de mettre à jour les objets [!DNL Jira] affectés afin de s’assurer qu’ils disposent d’un champ de date d’échéance.
* Désactivez la synchronisation de la date d’achèvement prévue de [!DNL Workfront] dans la page [!UICONTROL Configuration] de Workfront.
