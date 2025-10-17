---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Installer un plan directeur
description: Vous pouvez installer un plan directeur dans votre environnement de production ou un environnement sandbox.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 74%

---

# Installer un plan directeur

<!-- Audited: 5/2025 -->

Vous pouvez installer un plan directeur dans votre environnement de production ou un environnement sandbox.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Administrateur ou administratrice Workfront</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Où installer un plan directeur ? {#where-should-i-install-a-blueprint}

Vous pouvez installer votre package dans l’un des environnements suivants :

<table style="table-layout:auto">
        <tr>
        <td><strong>Production</strong></td>
        <td>La production est votre environnement en ligne.</td>
    </tr>
    <tr>
        <td><strong>Aperçu de sandbox</strong></td>
        <td>L’aperçu du sandbox est un environnement de test qui sert de réplique de votre environnement en ligne et qui est actualisé chaque week-end par Adobe Workfront. Tous les packages de prise en charge ont accès à la prévisualisation sandbox. Pour plus d’informations, voir <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">l’environnement de prévisualisation sandbox [!DNL Adobe Workfront]</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 et 2</strong></td>
        <td>L’environnement de sandbox à actualisation personnalisée est un environnement de test distinct qui est actualisé manuellement par vos soins. L’obtention du sandbox à actualisation personnalisée entraîne des frais supplémentaires. Pour plus d’informations, voir <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">l’environement d’actualisation sandbox personnalisé [!DNL Adobe Workfront]</a>.</td>
    </tr>
</table>

>[!TIP]
>
>Nous vous recommandons d’installer d’abord le plan directeur dans un environnement Sandbox. Ainsi, vous pouvez tester le contenu du plan directeur et vous assurer qu’il convient à votre organisation sans apporter de modifications aux données actives.

>[!NOTE]
>
>Certains plans directeurs ne peuvent être installés que dans l’environnement de prévisualisation à des fins de test. Si vous accédez à du contenu de prévisualisation uniquement dans votre environnement de production, sandbox 1, ou sandbox 2, le bouton d’installation n’est pas actif et un message d’avertissement peut s’afficher.\
>En outre, la fonctionnalité de changement d’environnement est limitée lors de l’accès au contenu en prévisualisation uniquement, même lorsque vous vous trouvez dans l’environnement de Prévisualisation.

## Installer le plan directeur

{{step1-to-blueprints}}

1. Recherchez le plan directeur que vous souhaitez installer. Vous pouvez filtrer par cas d’utilisation, niveau de maturité, statut d’installation et type sur le côté droit de la page.
1. (Facultatif) Cliquez sur **[!UICONTROL Détails]** pour découvrir comment fonctionne le plan directeur.
1. Cliquez sur **[!UICONTROL Installer]**.
1. Choisissez d’effectuer l’installation sur votre environnement de production ou un environnement sandbox.\
   Pour plus d’informations, voir la section [Où installer un plan directeur ?](#where-should-i-install-a-blueprint) dans cet article.
1. Sur la page **Configurer**, vous pouvez choisir d’effectuer l’une des opérations suivantes :

   * Installez le plan directeur tel quel. Pour les types de plan directeur qui ne nécessitent aucune configuration, il s’agit de la seule option. Pour les types de plan directeur qui doivent être configurés, vous pouvez éventuellement choisir d’installer le plan directeur maintenant et de le configurer ultérieurement. Cliquez sur **[!UICONTROL Installer en l’état]**.
   * Configurez le plan directeur avant l’installation, pour les plans directeurs qui nécessitent une configuration. Effectuez vos sélections de configuration, puis cliquez sur **[!UICONTROL Installer le plan directeur]**.

     Pour plus d’informations, voir [Configurer un plan directeur](../../administration-and-setup/blueprints/configure-template-package.md).

   L’installation est terminée et un message affiche la liste des objets spécifiques (tels que des rôles, des équipes ou des groupes) qui ont été installés avec succès avec le plan directeur, ainsi que tous les objets dont l’installation a échoué.

Après l’installation du plan directeur, il se peut que des actions supplémentaires soient nécessaires pour compléter le déploiement. Pour plus d’informations, voir [Actions nécessaires après l’installation d’un plan directeur](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
