---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Installer un plan directeur
description: Vous pouvez installer un plan directeur dans votre environnement de production ou un environnement Sandbox.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 6%

---

# Installer un plan directeur

Vous pouvez installer un plan directeur dans votre environnement de production ou un environnement Sandbox.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe de la licence [!DNL Workfront]</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurations du niveau d’accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Où installer un plan directeur ? {#where-should-i-install-a-blueprint}

Vous pouvez installer votre package dans l’un des environnements suivants :

<table style="table-layout:auto">
        <tr>
        <td><strong>Production</strong></td>
        <td>La production est votre environnement en ligne.</td>
    </tr>
    <tr>
        <td><strong>Aperçu de sandbox</strong></td>
        <td>L’aperçu sandbox est un environnement de test qui sert de réplique à votre environnement en ligne et qui est actualisé chaque week-end par Workfront. Tous les modules de prise en charge ont accès à l’aperçu Sandbox. Pour plus d’informations, voir <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">L’ [!DNL Adobe Workfront] environnement de test d’aperçu</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 et 2</strong></td>
        <td>L’environnement de test d’actualisation personnalisée est un environnement de test distinct que vous actualisez manuellement. L’obtention de l’environnement de test d’actualisation personnalisée entraîne des frais supplémentaires. Pour plus d’informations, voir <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">L’ [!DNL Adobe Workfront] environnement Sandbox d’actualisation personnalisée</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Nous vous recommandons d’installer d’abord le plan directeur dans un environnement de test. Ainsi, vous pouvez tester le contenu du plan directeur et vous assurer qu’il convient à votre organisation sans apporter de modifications aux données actives.

>[!NOTE]
>
>Certains plans directeurs ne peuvent être installés que dans l’environnement Aperçu à des fins de test. Si vous accédez au contenu Aperçu uniquement dans votre environnement de production, sandbox 1 ou sandbox 2, le bouton d’installation n’est pas actif et un message d’avertissement peut s’afficher.\
>En outre, la fonctionnalité de changement d’environnement est limitée lors de l’accès au contenu Aperçu uniquement, même lorsque vous vous trouvez dans l’environnement Aperçu .

## Installation du plan directeur

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Blueprints]**.
1. Recherchez le plan directeur que vous souhaitez installer. Vous pouvez filtrer par cas d’utilisation, niveau de maturité, état d’installation et saisir le texte sur le côté droit.
1. (Facultatif) Cliquez sur **[!UICONTROL Details]** pour découvrir le fonctionnement du plan directeur.
1. Cliquez sur **[!UICONTROL Installer]**.
1. Choisissez d’effectuer l’installation sur votre environnement de production ou un environnement de test.\
   Pour plus d’informations, voir [Où dois-je installer un plan directeur ?](#where-should-i-install-a-blueprint) de cet article.
1. Sur la page [!UICONTROL Configurer] , vous pouvez choisir d’effectuer l’une des opérations suivantes :

   * Installez le plan directeur tel quel. Pour les types de plan directeur qui ne nécessitent aucune configuration, il s’agit de la seule option. Pour les types de plan directeur qui doivent être configurés, vous pouvez éventuellement choisir d’installer le plan directeur maintenant et de le configurer ultérieurement. Cliquez sur **[!UICONTROL Installer tel quel]**.
   * Configurez le plan directeur avant l’installation, pour les plans directeurs qui nécessitent une configuration. Effectuez vos sélections de configuration et cliquez sur **[!UICONTROL Installer le plan directeur]**.\

     Pour plus d’informations, voir [Configuration d’un plan directeur](../../administration-and-setup/blueprints/configure-template-package.md).
Une fois l’installation terminée, un message affiche la liste des objets spécifiques (tels que les rôles, les équipes ou les groupes) qui ont été correctement installés avec le plan directeur et les objets qui n’ont pas pu être installés.

Après l’installation du plan directeur, il se peut que des actions supplémentaires soient nécessaires pour le déployer entièrement. Pour plus d’informations, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
