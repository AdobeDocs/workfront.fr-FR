---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Questions fréquentes sur Adobe Unified Experience
description: Certaines fonctionnalités sont différentes entre [!DNL Workfront] et Adobe Experience Cloud, et vous pouvez avoir quelques questions car votre instance [!DNL Workfront] est migrée vers l’expérience unifiée.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 0cdd29a0fd58427197f1b9a4b4907089d3d86115
workflow-type: tm+mt
source-wordcount: '1302'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] - FAQ

[!DNL Adobe Unified Experience] pour [!DNL Workfront] vous permet de gérer toutes vos applications [!DNL Adobe] à un seul endroit avec une seule connexion. La zone de navigation [!DNL Adobe] est intégrée de manière transparente à [!DNL Workfront]. Certaines fonctionnalités sont différentes et vous pouvez poser certaines questions lorsque votre instance [!DNL Workfront] est migrée vers l’expérience unifiée.

Pour plus d&#39;informations sur la connexion à [!DNL Adobe Unified Experience], voir [[!DNL Adobe Unified Experience] pour [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparaison de l’expérience [!DNL Adobe Unified Experience] et [!DNL Workfront only]

Seuls les clients qui utilisent [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] peuvent accéder à [!DNL Adobe Unified Experience]. Les clients qui n’ont pas encore migré verront l’expérience [!DNL Workfront only], sans possibilité de basculer entre les applications [!DNL Adobe].

Ce tableau décrit certaines fonctionnalités qui diffèrent entre les deux expériences.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] seule expérience |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Le menu principal] se trouve à gauche ![Menu principal](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Le menu principal] se trouve à droite ![Menu principal](assets/main-menu-icon.png) |
| Une seule URL de connexion est disponible pour toutes les applications [!DNL Adobe Experience Cloud] | Connectez-vous à [!DNL Workfront] avec une URL [!DNL Workfront] personnalisée |
| Un &quot;sélecteur d’organisation&quot; vous permet de vous déplacer entre [!DNL Workfront] organisations et environnements. | Le &quot;sélecteur d’organisation&quot; n’est pas disponible |
| La navigation comprend une zone de navigation de niveau supérieur pour les produits [!DNL Adobe], les notifications [!DNL Adobe], l’aide et votre profil utilisateur, en plus de la barre de navigation [!DNL Workfront] | La navigation comprend uniquement la barre de navigation [!DNL Workfront] |
| L’aide est accessible à partir du [!UICONTROL menu principal] et de la zone de navigation supérieure. | L&#39;aide est accessible à partir de la barre de navigation [!UICONTROL Main Menu] et [!DNL Workfront] |
| La visionneuse de vérification s’ouvre dans un nouvel onglet. | La visionneuse de vérification s’ouvre dans Workfront |

{style="table-layout:auto"}

## Questions fréquentes

### Comment puis-je déterminer si j’utilise Adobe Unified Experience ou Adobe Workfront ?

Pour déterminer si votre organisation se trouve dans l’expérience unifiée Adobe, examinez l’URL que vous utilisez pour accéder à Workfront.

| URL | Adobe Experience |
|------------|------------|
| (Nom de l’entreprise).my.workfront.com | Expérience Workfront |
| experience.adobe.com | Adobe d’une expérience unifiée |

### Comment puis-je en savoir plus sur [!DNL Adobe Admin Console] ?

Pour plus d’informations sur [!DNL Admin Console], consultez ces articles :

* [Préparation de l’événement [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Différences d’administration basées sur une plateforme ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] overview](https://helpx.adobe.com/fr/enterprise/using/admin-console.html)

### Que dois-je faire en tant que client pour faciliter la migration ?

Les clients existants seront contactés pour planifier des migrations. Les collègues de l’équipe de migration vont guider les clients tout au long du processus, conseiller sur la configuration de [!DNL Admin Console] et fournir des liens vers la documentation nécessaire pour rendre le déplacement aussi simple et facile que possible.

* [[!DNL Adobe Workfront] Présentation de l’assistance](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] information](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] et  [!DNL Admin Console] FAQ](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### Comment gérez-vous [!DNL Adobe Admin Console] pour les entreprises qui ont déjà activé cette fonctionnalité pour les ID fédérés différemment de la configuration de l’authentification unique [!DNL Workfront] ?

[!DNL Adobe Admin Console] a la possibilité d’inclure [!DNL Workfront], en remplaçant SSO par IMS. L’ensemble des privilèges d’accès des utilisateurs se produit dans [!DNL Admin Console], et les utilisateurs voient l’écran de connexion [!DNL Adobe] pour accéder à [!DNL Experience Cloud] où ils voient [!DNL Workfront] comme une option (s’ils y ont accès).

### Comment cela affecte-t-il les clients qui disposent déjà du panneau d’administration d’AEM pour [!DNL Adobe Assets], mais que la connexion unique est configurée différemment de [!DNL Workfront?] ?

Une fois [!DNL Workfront] ajouté en tant qu’application [!DNL Admin Console], vous ne devriez rien faire d’autre pour [!DNL Workfront] pour tirer parti de la configuration SSO existante que vous avez pour [!DNL Adobe Assets].

### Comment cela affecte-t-il les configurations SSO ?

SSO est configuré dans [!DNL Admin Console] et hérité par l’application [!DNL Workfront].

### La connexion unique avec notre [!DNL Active Directory] interne sera-t-elle toujours une option avec IMS ?

IMS remplace l’authentification unique et les fonctions pratiquement identiques. Toutes les autorisations d’utilisateur sont accordées et configurées dans [!DNL Adobe Admin Console]. L’utilisateur voit l’écran de connexion [!DNL Adobe] dans lequel il peut choisir &quot;[!UICONTROL Compte personnel]&quot; ou &quot;[!UICONTROL Compte de société]&quot; pour se connecter (si vous avez [!DNL Active Directory], la plupart se connectent avec un compte de société).

### Pour ceux qui n’utilisent pas SSO, l’URL de connexion [!DNL Workfront] change-t-elle ?

L’URL de connexion change. Toutefois, l’ancienne URL redirige vers la nouvelle URL de connexion. Vous devez donc former à nouveau vos utilisateurs où aller.

### Les alias que nous avons configurés fonctionneront-ils toujours ou les liens [!DNL Workfront] changent-ils avec cette migration ?

[!DNL Workfront] redirections/alias sont disponibles pour accéder à la page d’accueil.

### Les redirections seront-elles désactivées à un moment donné ? Ou pourrons-nous toujours taper dans my.company.workfront.com ?

Vous pourrez toujours utiliser n’importe quelle URL personnalisée. Une fois que vous avez cliqué sur l’un de ces liens, vous accédez à [!DNL Workfront] et une URL différente s’affiche. Cependant, il est préférable [!DNL experience] de se connecter à experience.adobe.com et de mettre en signet des liens dans [!DNL Experience Cloud]. Moins de redirection équivaut à moins de temps/temps de chargement.

### Les liens directs vers les files d’attente de requête seront-ils rompus ?

Tous les liens directs doivent rediriger vers les nouveaux modèles d’URL. Cependant, si vous avez distribué des liens vers des personnes, vous devez envoyer une mise à jour afin d’exploiter le lien direct et d’éviter les retards d’accès à la page attendue.

### Allons-nous migrer vers [!DNL Experience Cloud] globalement ou pouvons-nous sélectionner certains utilisateurs (tous nos utilisateurs n&#39;utilisent même pas d&#39;autres produits Adobe) ?

Le compte client [!DNL Workfront] entier sera migré. Elle ne peut pas être effectuée utilisateur par utilisateur.

### Tous les utilisateurs de [!DNL Workfront] devront-ils se connecter via [!DNL Experience Cloud] ? Ou seulement les administrateurs ?

Oui, tous les utilisateurs se connecteront via [!DNL Experience Cloud]. La connexion IMS remplacera la connexion unique. C&#39;est une expérience très similaire, juste un écran de connexion différent.

### Les utilisateurs devront-ils lier leurs comptes [!DNL Adobe] à leurs comptes [!DNL Workfront] s&#39;ils disposent déjà des deux ?

Oui, il existe un processus pour cela. Des détails supplémentaires seront fournis lorsqu’il sera temps pour votre organisation de passer à IMS.

### Qu’advient-il des utilisateurs [!DNL Workfront] qui n’ont pas de compte [!DNL Adobe] ?

Les utilisateurs qui n&#39;ont pas reçu l&#39;accès dans [!DNL Adobe Admin Console] pour accéder à [!DNL Workfront] doivent créer un &quot;[!UICONTROL compte personnel]&quot; ou un compte [!DNL Adobe] ID pour pouvoir se connecter. Cette action envoie un courrier électronique à l’administrateur pour approuver ou rejeter sa demande. Elle permet en outre à l’administrateur de configurer le type d’accès dont dispose cet utilisateur. Lorsqu’ils se connectent, ils accèdent à experience.adobe.com, saisissent leur adresse électronique et choisissent [!UICONTROL Compte personnel]. A partir de là, ils pourront accéder à [!DNL Workfront].

### Que se passe-t-il si nous n&#39;avons pas d&#39;autres produits [!DNL Adobe] que [!DNL Workfront?] ?

Il est toujours recommandé que votre organisation migre vers le [!DNL Adobe Unified Experience]. Vous recevrez un ID [!DNL Adobe] avec les avantages répertoriés ci-dessus.

### Nous avons des utilisateurs externes inclus dans notre instance [!DNL Workfront]. Nous ne souhaitons pas qu’ils aient accès à d’autres produits inclus dans [!DNL Adobe]. Comment limiterions-nous leur accès dans la console ?

[!DNL Admin Console] donne aux administrateurs un grand contrôle sur ce à quoi les utilisateurs peuvent ou ne peuvent pas accéder. Chaque fois qu’un utilisateur externe souhaite y accéder, il doit créer un identifiant [!DNL Adobe], qui envoie un courrier électronique à l’administrateur. L’administrateur peut alors accepter ou refuser l’accès à un produit et définir ce à quoi il peut ou ne peut pas accéder pour les produits appartenant à cette organisation. Ensuite, l’administrateur système [!DNL Workfront] peut accéder à la zone [!UICONTROL Users] de [!DNL Workfront] pour obtenir des autorisations plus granulaires pour l’utilisateur externe.

### Les administrateurs de groupe sont utilisés pour créer des personnes dans [!DNL Workfront]. Avec le déplacement vers [!DNL Experience Cloud], les administrateurs de groupe pourront-ils toujours créer des personnes ?

Oui, la création de l’utilisateur est toujours possible via [!DNL Workfront]. Ces utilisateurs peuvent être ajoutés automatiquement à [!DNL Experience Cloud]. Vous pouvez également configurer vos administrateurs de groupe en tant que propriétaires de produits dans le [!DNL Admin Console] pour leur permettre d’affecter [!DNL Workfront] aux utilisateurs.

### Quelle est la date limite de basculement vers [!DNL Experience Cloud] ?

Il n’y a actuellement aucune date limite de déplacement vers [!DNL Adobe Experience Cloud]. Nous travaillons avec les clients pour leur permettre de choisir quand ils sont prêts à faire le déplacement.

### Notre équipe de support devra-t-elle faire quelque chose pour ce changement ?

Si l’équipe d’assistance est chargée de créer de nouveaux utilisateurs, elle devra se familiariser avec les interfaces [!DNL Admin Console] utilisées pour créer des utilisateurs et attribuer un droit à Workfront. Sinon, il n’y aura probablement aucun changement significatif pour votre équipe de support interne.

### Comment cela affecte-t-il les intégrations que nous avons via la fonction API ?

Le chemin d’accès à l’URL existant restera disponible pour le trafic de l’API. Vous ne devez rien faire pour mettre à jour les points de terminaison dans vos intégrations. Toutefois, la connexion directe par l’intermédiaire du nom d’utilisateur et du mot de passe ne sera pas prise en charge. Vous devez utiliser une clé API, à l’exception des connecteurs [!DNL Workfront Fusion].

### Qu’en est-il des utilisateurs de [!DNL Creative Cloud] ? Comment la migration les affecte-t-elle ? Y a-t-il des avantages pour eux ?

Il n’y a aucun impact pour les utilisateurs de [!DNL Creative Cloud] avec la migration vers [!DNL Adobe Unified Experience].

### Les connexions seront-elles modifiées pour les utilisateurs mobiles [!DNL Workfront] ?

[!DNL Workfront] les utilisateurs mobiles ne doivent pas être affectés par la migration vers [!DNL Adobe Unified Experience].
