---
content-type: reference
navigation-topic: get-started-with-workfront
title: Langues prises en charge dans Adobe Workfront
description: Vous pouvez modifier la langue dans laquelle vous affichez Adobe Workfront et les e-mails provenant de Workfront en ajustant les préférences linguistiques de votre navigateur et vos paramètres régionaux d’e-mail par défaut dans Workfront.
feature: Get Started with Workfront
author: Becky
exl-id: 0b76175f-5fe2-49df-b605-68e6e66b4366
source-git-commit: 5304f25ecb198f45c024b71185747f47fa8307d4
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 65%

---

# Langues prises en charge dans Adobe Workfront

Vous pouvez modifier la langue d’affichage d’Adobe Workfront et des e-mails provenant de Workfront en ajustant les préférences linguistiques de votre navigateur (si votre organisation n’a pas été migrée vers Adobe Admin Console) ou vos préférences linguistiques de profil Adobe Experience Cloud (si sur Adobe Admin Console) et vos paramètres régionaux d’e-mail par défaut dans Workfront.

Pour modifier la langue d&#39;affichage de Workfront, consultez [Modifier la langue](#change-the-language) dans cet article.

La terminologie Workfront est mise à jour pour les langues prises en charge à chaque mise à jour de Workfront.

Workfront prend en charge les langues suivantes :

* Anglais (en-US)
* Français (fr-FR)
* Allemand (de-DE)
* Japonais (ja)
* Espagnol (es)
* Italien (it_IT)
* Portugais (pt-BR)
* Coréen (ko)
* Chinois - simplifié (zh-CN)
* Chinois - traditionnel (zh-TW)

La langue utilisée pour afficher Workfront dans votre navigateur est contrôlée par les paramètres de langue de votre navigateur si votre organisation ne se trouve pas sur le Adobe Admin Console, ou par la langue de profil de votre Adobe Experience Cloud si votre organisation se trouve sur le Adobe Admin Console. Dans les deux cas, veillez à sélectionner une langue répertoriée dans la liste des langues prises en charge.

Pour afficher les e-mails sortants dans l’une des langues prises en charge, modifiez vos paramètres régionaux d’e-mails utilisateur ou vos paramètres d’informations client dans Workfront.\
Pour modifier les paramètres d’informations client, vous devez être un administrateur ou une administratrice Workfront.\
Pour plus d’informations sur la modification des informations client et des paramètres régionaux des e-mails utilisateur, voir [Modifier les paramètres régionaux de Workfront et des e-mails utilisateur](#change-the-workfront-and-user-locales).

Vous pouvez demander à un tiers de traduire dans d’autres langues l’interface Workfront et les e-mails sortants de Workfront. Ces traductions ne sont pas prises en charge par Workfront et les langues autres que celles répertoriées ci-dessus ne sont pas prises en charge.

>[!NOTE]
>
>Certaines parties de l’interface peuvent encore ne pas être traduites dans les cas suivants :
>
>* Lorsque vous utilisez une langue non prise en charge, l’interface s’affiche en anglais.
>* Le menu Aide, ainsi que le contenu d’aide accessible à partir de ce menu, s’affiche en anglais.
>* Le texte que vous saisissez reste dans la langue d’origine saisie. Cela peut inclure, sans s’y limiter :
>
>   * Noms de projet
>   * Noms de tâche
>   * Noms de problème
>   * Noms de portfolio
>   * Noms de programme
>   * Noms d’approbation
>   * Descriptions
>   * Noms de formulaire personnalisé
>   * Noms de type d’heure
>   * Types de dépenses
>   * Jalons
>   * Onglets personnalisés
>   * Statuts
>   * Noms de rapport
>

## Incohérences de langue prises en charge lors de l’utilisation de la relecture

La visionneuse de relecture web de Workfront prend en charge la plupart des langues prises en charge dans Workfront.

Les langues suivantes ne sont pas prises en charge dans l’outil de relecture :

* Chinois - traditionnel (zh-TW)
* Coréen (ko-KR)

Votre entreprise doit acheter une licence de relecture afin d’accéder à la visionneuse de relecture web.

Pour plus d’informations sur la relecture, voir [Relecture](../review-and-approve-work/proofing/proofing.md).

Lorsque vous affichez Workfront dans une langue qui n’est pas prise en charge par l’outil de relecture, la visionneuse de relecture web s’affiche en anglais.

Si vous utilisez Workfront Proof (l’outil de relecture autonome) dans une langue qui n’est pas prise en charge dans Workfront, la visionneuse de relecture web dans Workfront s’affiche en anglais.\
Pour plus d’informations sur les langues prises en charge dans Workfront Proof, voir [Paramètres linguistiques dans Workfront Proof](../workfront-proof/wp-getstarted/system-information/language-settings.md).

## Langue prise en charge dans Adobe Workfront Fusion

Actuellement, Workfront Fusion ne prend en charge que l’anglais.

* Tout le contenu de Workfront Fusion, ainsi que tout contenu d’aide lié à Workfront Fusion, s’affiche en anglais.
* Workfront Fusion ne prend pas en charge l’utilisation de caractères de texte autres que l’anglais dans les champs saisis par l’utilisateur ou l’utilisatrice.

Votre entreprise doit acheter une licence Workfront Fusion pour pouvoir y accéder.\
Pour plus d’informations sur Workfront Fusion, voir [Vue d’ensemble d’Adobe Workfront Fusion](https://experienceleague.adobe.com/fr/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).

## Modifier la langue

Vous pouvez modifier la langue dans laquelle vous affichez Workfront et la langue des e-mails sortants en modifiant les paramètres suivants :

* Langue de votre navigateur (pour les utilisateurs qui ne se trouvent pas dans le Adobe Admin Console)
* Langue principale et secondaire de votre profil AEM (pour les utilisateurs et utilisatrices de l’Admin Console Adobe)
* Informations client et paramètres régionaux des e-mails utilisateur de votre compte Workfront.

Pour afficher toutes les traductions disponibles dans la langue de votre choix, les paramètres régionaux Workfront et les paramètres régionaux du navigateur doivent être définis sur la même langue.

Pour déterminer si votre organisation a été migrée vers Adobe Admin Console, examinez l’URL que vous utilisez pour afficher Workfront.

| URL | Adobe Experience | Contrôle de la langue |
|---|---|---|
| (Nom de l’entreprise).my.workfront.com | Non migré vers Adobe Admin Console | [Modifier la langue du navigateur](#change-the-browser-language) |
| experience.adobe.com | Migré vers Adobe Admin Console | [Modifier la langue du Adobe Experience Cloud](#change-the-adobe-experience-cloud-language) |

* [Modifier la langue du navigateur](#change-the-browser-language)
* [Modification de la langue du Adobe Experience Cloud](#change-the-adobe-experience-cloud-language)
* [Modifier les paramètres régionaux de Workfront et des e-mails utilisateur](#change-the-workfront-and-user-locales)

### Modifier la langue du navigateur {#change-the-browser-language}

Si votre organisation n’a pas été migrée vers Adobe Admin Console, lorsque vous modifiez la langue du navigateur, votre interface Workfront s’affiche dans cette langue.\
Pour plus d’informations sur les langues prises en charge par Workfront, voir [Langues prises en charge dans Adobe Workfront](#supported-languages).

La langue du navigateur doit être modifiée pour chaque personne.

Consultez le menu « Aide » de votre navigateur pour obtenir des informations spécifiques sur la modification de la langue de votre navigateur.

### Modification de la langue du Adobe Experience Cloud

Si votre organisation a été migrée vers Adobe Admin Console, la langue de profil de Adobe Experience Cloud détermine la langue affichée dans Workfront.

1. Cliquez sur l’image de votre profil à l’extrémité droite de la barre d’outils Adobe Experience Cloud, puis sur **Préférences**. La barre d’outils Adobe Experience Cloud se trouve directement au-dessus de la barre d’outils Workfront principale.

1. Sous **Profil** sous votre nom et votre adresse e-mail, cliquez sur le nom de la langue actuellement sélectionnée.

1. Sélectionnez vos langues préférées dans les listes déroulantes **Première langue** et **Seconde langue**. La première langue est votre choix de langue par défaut, tandis que la seconde langue s&#39;affiche uniquement si la première langue n&#39;est pas prise en charge par une application spécifique.

### Modifier les paramètres régionaux de Workfront et des e-mails utilisateur {#change-the-workfront-and-user-locales}

* [Modifier les paramètres régionaux des e-mails Workfront par défaut](#change-the-workfront-locale)
* [Modifier les paramètres régionaux des e-mails utilisateur](#change-the-user-locale)

### Modifier les paramètres régionaux des e-mails Workfront par défaut {#change-the-workfront-locale}

Lorsque vous modifiez les paramètres régionaux des e-mails Workfront par défaut, vous modifiez le format de langue, de date et de nombre utilisé dans les messages sortants pour toutes les personnes utilisant Workfront. Ces paramètres deviennent la valeur par défaut de chaque nouvelle personne que vous créez.

Pour modifier les paramètres régionaux des e-mails Workfront par défaut :

1. Connectez-vous à Workfront en tant qu’administrateur ou administratrice Workfront.
1. Cliquez sur l’icône **Menu principal** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Configuration** ![](assets/gear-icon-settings.png).

1. Cliquez sur **Système** > **Infos client**.

1. Dans la section **Informations de base**, cliquez sur la liste déroulante **Paramètres régionaux d’e-mail par défaut** pour sélectionner la langue dans laquelle les e-mails Workfront doivent s’afficher.

1. Cliquer sur **Enregistrer**.

### Modifier les paramètres régionaux des e-mails utilisateur {#change-the-user-locale}

Lorsque vous modifiez les paramètres régionaux des e-mails utilisateur, vous modifiez le format de langue, de date et de numéro utilisé dans les messages sortants. Ces paramètres remplacent les paramètres système sélectionnés dans la zone Infos client de la configuration.

>[!NOTE]
>
>Lorsque votre organisation se trouve sur l’expérience unifiée Adobe, les préférences linguistiques sont stockées dans votre profil Adobe et les paramètres régionaux des e-mails ne sont pas utilisés. Voir [Modifier la langue du Adobe Experience Cloud](#change-the-adobe-experience-cloud-language) dans cet article.

Pour modifier les paramètres régionaux des e-mails utilisateur :

1. Cliquez sur l’icône **Menu Principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur votre image de profil.

1. Cliquez sur le menu Plus ![](assets/more-icon.png), puis cliquez sur **Modifier**.

1. Dans la section **Préférences**, cliquez sur le menu déroulant **Paramètres régionaux d’e-mail** pour sélectionner la langue dans laquelle les e-mails Workfront doivent s’afficher.

1. Cliquez sur **Enregistrer les modifications**.
