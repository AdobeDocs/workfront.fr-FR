---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Installation d’un plan directeur
description: Vous pouvez installer un plan directeur dans votre environnement de production ou un environnement Sandbox.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Installation d’un plan directeur

Vous pouvez installer un plan directeur dans votre environnement de production ou un environnement Sandbox.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] license</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Paramétrages du niveau d'accès</strong></td> 
   <td> <p>[!UICONTROL Administrateur système]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Où dois-je installer un plan directeur ? {#where-should-i-install-a-blueprint}

Vous pouvez installer votre package dans l’un des environnements suivants :

<table style="table-layout:auto">
        <tr>
        <td><strong>Production</strong></td>
        <td>La production est votre environnement en ligne.</td>
    </tr>
    <tr>
        <td><strong>Aperçu de Sandbox</strong></td>
        <td>L’aperçu sandbox est un environnement de test qui sert de réplique à votre environnement en ligne et qui est actualisé chaque week-end par Workfront. Tous les modules de prise en charge ont accès à l’aperçu Sandbox. Pour plus d’informations, voir <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Le [!DNL Adobe Workfront] Aperçu de l’environnement de test</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 et 2</strong></td>
        <td>L’environnement de test d’actualisation personnalisée est un environnement de test distinct que vous actualisez manuellement. L’obtention de l’environnement de test d’actualisation personnalisée entraîne des frais supplémentaires. Pour plus d’informations, voir <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">Le [!DNL Adobe Workfront] Environnement Sandbox d’actualisation personnalisée</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Nous vous recommandons d’installer d’abord le plan directeur dans un environnement de test. Ainsi, vous pouvez tester le contenu du plan directeur et vous assurer qu’il convient à votre organisation sans apporter de modifications aux données actives.

>[!NOTE]
>
>Certains plans directeurs ne peuvent être installés que dans l’environnement Aperçu à des fins de test. Si vous accédez au contenu Aperçu uniquement dans votre environnement de production, sandbox 1 ou sandbox 2, le bouton d’installation n’est pas principal et un message d’avertissement peut s’afficher.\
>En outre, la fonctionnalité de changement d’environnement est limitée lors de l’accès au contenu Aperçu uniquement, même lorsque vous vous trouvez dans l’environnement Aperçu .

## Installation du plan directeur

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe] Workfront, puis cliquez sur **[!UICONTROL Plans directeurs]**.
1. Recherchez le plan directeur que vous souhaitez installer. Vous pouvez filtrer par cas d’utilisation, niveau de maturité, état d’installation et saisir le texte sur le côté droit.
1. (Facultatif) Cliquez sur **[!UICONTROL Détails]** pour découvrir comment fonctionne le plan directeur.
1. Cliquez sur **[!UICONTROL Installer]**.
1. Choisissez d’effectuer l’installation sur votre environnement de production ou un environnement de test.\
   Pour plus d’informations, voir [Où dois-je installer un plan directeur ?](#where-should-i-install-a-blueprint) dans cet article.
1. Sur le [!UICONTROL Configurer] , vous pouvez choisir d’effectuer l’une des opérations suivantes :

   * Installez le plan directeur tel quel. Pour les types de plan directeur qui ne nécessitent aucune configuration, il s’agit de la seule option. Pour les types de plan directeur qui doivent être configurés, vous pouvez éventuellement choisir d’installer le plan directeur maintenant et de le configurer ultérieurement. Cliquez sur **[!UICONTROL Installer tel quel]**.
   * Configurez le plan directeur avant l’installation, pour les plans directeurs qui nécessitent une configuration. Effectuez vos sélections de configuration, puis cliquez sur **[!UICONTROL Installer le plan directeur]**.\

      Pour plus d’informations, voir [Configuration d’un plan directeur](../../administration-and-setup/blueprints/configure-template-package.md).
Une fois l’installation terminée, un message affiche la liste des objets spécifiques (tels que les rôles, les équipes ou les groupes) qui ont été correctement installés avec le plan directeur et les objets qui n’ont pas pu être installés.

Après l’installation du plan directeur, d’autres actions peuvent être nécessaires pour le déployer entièrement. Pour plus d’informations, voir [Actions à entreprendre après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
