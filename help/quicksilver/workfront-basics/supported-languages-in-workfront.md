---
content-type: reference
navigation-topic: get-started-with-workfront
title: Langues prises en charge dans Adobe Workfront
description: Vous pouvez modifier la langue dans laquelle vous affichez Adobe Workfront et les e-mails provenant de Workfront en ajustant les préférences linguistiques de votre navigateur et vos paramètres régionaux d’e-mail par défaut dans Workfront.
feature: Get Started with Workfront
author: Becky
exl-id: 0b76175f-5fe2-49df-b605-68e6e66b4366
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: eb5296348c27f806dd50b997970166ebae4c97f4
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 97%

---

# Langues prises en charge dans Adobe Workfront

Vous pouvez modifier la langue d’affichage d’Adobe Workfront et des e-mails provenant de Workfront en ajustant les préférences linguistiques de votre navigateur (si votre organisation n’a pas été migrée vers Adobe Admin Console) ou vos préférences linguistiques de profil Adobe Experience Cloud (si sur Adobe Admin Console) et vos paramètres régionaux d’e-mail par défaut dans Workfront.

Pour modifier la langue d’affichage de Workfront, consultez [Modifier la langue](#change-the-language) dans cet article.

La terminologie Workfront est mise à jour pour les langues prises en charge à chaque mise à jour de Workfront.

Workfront prend en charge les langues suivantes :

* Anglais (en-US)
* Français (fr-FR)
* Allemand (de-DE)
* Japonais (ja-JP)
* Espagnol (es-ES)
* Italien (it-IT)
* Portugais (pt-BR)
* Coréen (ko-KR)
* Chinois - simplifié (zh-CN)
* Chinois - traditionnel (zh-TW)

La langue utilisée pour afficher Workfront dans votre navigateur est contrôlée par les paramètres de langue de votre navigateur si votre organisation ne se trouve pas sur Adobe Admin Console, ou par la langue de profil de votre Adobe Experience Cloud si votre organisation se trouve sur Adobe Admin Console. Dans les deux cas, veillez à sélectionner une langue répertoriée dans la liste des langues prises en charge.

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

<!--* DELETE THIS SECTION MARCH 2026 The language on your browser (for users not on the Adobe Admin Console)-->
* Langue principale et secondaire de votre profil AEM (pour les utilisateurs et utilisatrices d’Adobe Admin Console)
* Informations client et paramètres régionaux des e-mails utilisateur de votre compte Workfront.

Pour afficher toutes les traductions disponibles dans la langue de votre choix, les paramètres régionaux Workfront et les paramètres régionaux du navigateur doivent être définis sur la même langue.

Pour déterminer si votre organisation a été migrée vers Adobe Admin Console, examinez l’URL que vous utilisez pour afficher Workfront.

| URL | Adobe Experience | Contrôle de la langue |
|---|---|---|
| (Nom de l’entreprise).my.workfront.com | Non migré vers Adobe Admin Console | [Modifier la langue du navigateur](#change-the-browser-language) |
| experience.adobe.com | Migré vers Adobe Admin Console | [Modifier la langue d’Adobe Experience Cloud](#change-the-adobe-experience-cloud-language) |

* [Modifier la langue du navigateur](#change-the-browser-language)
* [Modifier la langue d’Adobe Experience Cloud](#change-the-adobe-experience-cloud-language)
* [Modifier les paramètres régionaux de Workfront et des e-mails utilisateur](#change-the-workfront-and-user-locales)

<!--DELETE THIS SECTION MARCH 2026-->

<!--

### Change the browser language {#change-the-browser-language}

If your organization has not been migrated to the Adobe Admin Console, when you change the browser language, your Workfront interface displays in that language.   
For more information about what languages are supported by Workfront, see [Supported languages in Adobe Workfront](#supported-languages).

The browser language must be changed on an individual user basis.

See the "Help" menu for your browser for specific information about how to change the language of your browser.-->

### Modifier la langue d’Adobe Experience Cloud

Si votre organisation a été migrée vers Adobe Admin Console, la langue de profil d’Adobe Experience Cloud détermine la langue affichée dans Workfront.

1. Cliquez sur l’image de votre profil à l’extrémité droite de la barre d’outils d’Adobe Experience Cloud, puis sur **Préférences**. La barre d’outils d’Adobe Experience Cloud se trouve directement au-dessus de la barre d’outils Workfront principale.

1. Dans **Profil** sous votre nom et votre adresse e-mail, cliquez sur le nom de la langue actuellement sélectionnée.

1. Sélectionnez vos langues préférées dans les listes déroulantes **Première langue** et **Deuxième langue**. La première langue est votre choix de langue par défaut, tandis que la deuxième langue s’affiche uniquement si la première langue n’est pas prise en charge par une application spécifique.

### Modifier les paramètres régionaux de Workfront et des e-mails utilisateur {#change-the-workfront-and-user-locales}

* [Modifier les paramètres régionaux des e-mails Workfront par défaut](#change-the-workfront-locale)
* [Modifier les paramètres régionaux des e-mails utilisateur](#change-the-user-locale)

### Modifier les paramètres régionaux des e-mails Workfront par défaut {#change-the-workfront-locale}

Lorsque vous modifiez les paramètres régionaux des e-mails Workfront par défaut, vous modifiez le format de langue, de date et de nombre utilisé dans les messages sortants pour toutes les personnes utilisant Workfront. Ces paramètres deviennent la valeur par défaut de chaque nouvelle personne que vous créez.

Pour modifier les paramètres régionaux des e-mails Workfront par défaut :

1. Connectez-vous à Workfront en tant qu’administrateur ou administratrice Workfront.

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Infos client**.

1. Dans la section **Informations de base**, cliquez sur la liste déroulante **Paramètres régionaux d’e-mail par défaut** pour sélectionner la langue dans laquelle les e-mails Workfront doivent s’afficher.

1. Cliquer sur **Enregistrer**.

### Modifier les paramètres régionaux des e-mails utilisateur {#change-the-user-locale}

<!--


When changing your User Email Locale, you modify the language, date, and number format used in your outgoing messages. These settings override the system settings selected in the Customer Info area of Setup.-->

>[!NOTE]
>
>Les préférences linguistiques sont stockées dans votre profil Adobe et les paramètres régionaux de l’e-mail ne sont pas utilisés. Voir [Modifier la langue d’Adobe Experience Cloud](#change-the-adobe-experience-cloud-language) dans cet article.

<!--To change your User Email Locale:

{{step1-click-main-menu}}

1. Click your user profile picture.

1. Click the More menu ![](assets/more-icon.png), then click **Edit**.

1. In the **Preferences** section, click the **Email Locale** drop-down list to select the language that you want Workfront emails to display in.

1. Click **Save Changes**.-->
