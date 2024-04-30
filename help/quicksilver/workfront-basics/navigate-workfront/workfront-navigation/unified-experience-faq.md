---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe Unified Experience pour FAQ
description: Quelques fonctions différentes entre [!DNL Workfront] et Adobe Experience Cloud, et vous pouvez avoir quelques questions en tant que [!DNL Workfront] est migrée vers l’expérience unifiée.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '1289'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] FAQ

La variable [!DNL Adobe Unified Experience] pour [!DNL Workfront] vous permet de gérer l’ensemble des [!DNL Adobe] à un seul emplacement avec une seule connexion. La variable [!DNL Adobe] la zone de navigation est intégrée de manière transparente à [!DNL Workfront]. Certaines fonctionnalités sont différentes et vous pouvez poser quelques questions en tant que [!DNL Workfront] est migrée vers l’expérience unifiée.

Pour plus d’informations sur la connexion à la variable [!DNL Adobe Unified Experience], voir [[!DNL Adobe Unified Experience] pour [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparaison de [!DNL Adobe Unified Experience] et [!DNL Workfront only] expérience

Seuls les clients qui utilisent la variable [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] peut accéder au [!DNL Adobe Unified Experience]. Les clients qui n’ont pas encore migré verront le [!DNL Workfront only] sans la possibilité de basculer entre les [!DNL Adobe] applications.

Ce tableau décrit certaines fonctionnalités qui diffèrent entre les deux expériences.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] expérience unique |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Menu Principal] se trouve à gauche ![Menu Principal](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Menu Principal] est à droite ![Menu Principal](assets/main-menu-icon.png) |
| Une seule URL de connexion est disponible pour tous les [!DNL Adobe Experience Cloud] applications | Connexion à [!DNL Workfront] avec un [!DNL Workfront] URL |
| Un &quot;sélecteur d’organisation&quot; vous permet de passer d’une [!DNL Workfront] organisations et environnements | Le &quot;sélecteur d’organisation&quot; n’est pas disponible |
| La navigation comprend une zone de navigation de niveau supérieur pour [!DNL Adobe] produits, [!DNL Adobe] notifications, aide et votre profil utilisateur, en plus des [!DNL Workfront] barre de navigation | La navigation comprend les [!DNL Workfront] barre de navigation uniquement |
| L’aide est accessible à partir du [!UICONTROL Menu Principal] et la zone de navigation supérieure | L’aide est accessible à partir du [!UICONTROL Menu Principal] et [!DNL Workfront] barre de navigation |

{style="table-layout:auto"}

## Questions fréquentes

### Comment puis-je déterminer si j’utilise Adobe Unified Experience ou Adobe Workfront ?

Pour déterminer si votre organisation se trouve dans l’expérience unifiée Adobe, examinez l’URL que vous utilisez pour accéder à Workfront.

| URL | Expérience Adobe |
|------------|------------|
| (NomSociété).my.workfront.com | Expérience Workfront |
| experience.adobe.com | Adobe d’une expérience unifiée |

### Comment puis-je en savoir plus sur la variable [!DNL Adobe Admin Console]?

Pour plus d’informations sur la variable [!DNL Admin Console], passez en revue ces articles :

* [Préparation de la [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] aperçu](https://helpx.adobe.com/fr/enterprise/using/admin-console.html)

### Que dois-je faire en tant que client pour faciliter la migration ?

Les clients existants seront contactés pour planifier des migrations. Les collègues de l’équipe d’assistance à la migration vont guider les clients tout au long du processus, conseiller sur [!DNL Admin Console] et fournissez des liens vers la documentation nécessaire pour que le déplacement soit aussi simple et facile que possible.

* [[!DNL Adobe Workfront] Présentation de l’assistance](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] informations](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] et [!DNL Admin Console] FAQ](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### Comment gérez-vous ? [!DNL Adobe Admin Console] pour les entreprises qui ont déjà activé cette fonctionnalité pour les ID fédérés différemment de [!DNL Workfront] SSO est configuré ?

[!DNL Adobe Admin Console] dispose de la possibilité d’inclure [!DNL Workfront], en remplaçant SSO par IMS. L’ensemble de l’attribution des privilèges d’accès des utilisateurs s’effectue dans la variable [!DNL Admin Console], et les utilisateurs verront le [!DNL Adobe] écran de connexion auquel accéder [!DNL Experience Cloud] où ils verront [!DNL Workfront] comme option (s’ils y ont accès).

### Comment cela affecte-t-il les clients qui disposent déjà du panneau d’administration AEM pour [!DNL Adobe Assets] - mais l’authentification unique est configurée différemment de [!DNL Workfront?]

Une fois [!DNL Workfront] est ajouté en tant que [!DNL Admin Console] application, vous ne devriez avoir rien à faire d’autre pour [!DNL Workfront] pour tirer parti de la configuration SSO existante dont vous disposez pour [!DNL Adobe Assets].

### Comment cela affecte-t-il les configurations SSO ?

SSO est configuré dans la variable [!DNL Admin Console] et hérité par le [!DNL Workfront] application.

### La SSO est-elle interne à [!DNL Active Directory] sera-t-il toujours une option avec IMS ?

IMS remplace l’authentification unique et les fonctions pratiquement identiques. Toutes les autorisations d’utilisateur sont accordées et configurées dans [!DNL Adobe Admin Console], et l’utilisateur verra le [!DNL Adobe] Écran de connexion où ils peuvent choisir[!UICONTROL Compte personnel]&quot; ou &quot;[!UICONTROL Compte de société]&quot; pour se connecter (si vous avez [!DNL Active Directory], la plupart se connecteront avec un compte de société).

### Pour ceux qui n’utilisent pas SSO, la fonction [!DNL Workfront] changement d’URL de connexion ?

L’URL de connexion change. Toutefois, l’ancienne URL redirige vers la nouvelle URL de connexion. Vous devez donc former à nouveau vos utilisateurs où aller.

### Les alias que nous avons configurés fonctionneront-ils toujours, ou seront-ils [!DNL Workfront] les liens qui changent avec cette migration ?

[!DNL Workfront] les redirections/alias sont disponibles pour accéder à la page d’accueil.

### Les redirections seront-elles désactivées à un moment donné ? Ou pourrons-nous toujours taper dans my.company.workfront.com ?

Vous pourrez toujours utiliser n’importe quelle URL personnalisée. Une fois que vous avez cliqué sur l’un de ces liens, vous serez dirigé vers [!DNL Workfront] et afficher une autre URL. Cependant, c&#39;est une meilleure solution [!DNL experience] pour vous connecter à experience.adobe.com et mettre en signet des liens depuis l’intérieur de [!DNL Experience Cloud]. Moins de redirection équivaut à moins de temps/temps de chargement.

### Les liens directs vers les files d’attente de requête seront-ils rompus ?

Tous les liens directs doivent rediriger vers les nouveaux modèles d’URL. Cependant, si vous avez distribué des liens vers des personnes, vous devez envoyer une mise à jour afin d’exploiter le lien direct et d’éviter les retards d’accès à la page attendue.

### Allons-nous migrer vers [!DNL Experience Cloud] globalement ou pouvons-nous sélectionner certains utilisateurs (tous nos utilisateurs n’utilisent même pas d’autres produits Adobe) ?

L’ensemble [!DNL Workfront] Le compte client sera migré. Elle ne peut pas être effectuée utilisateur par utilisateur.

### Tout [!DNL Workfront] les utilisateurs doivent se connecter via [!DNL Experience Cloud]? Ou seulement les administrateurs ?

Oui, tous les utilisateurs se connecteront via [!DNL Experience Cloud]. La connexion IMS remplacera la connexion unique. C&#39;est une expérience très similaire, juste un écran de connexion différent.

### Les utilisateurs devront-ils lier leurs [!DNL Adobe] à leurs comptes [!DNL Workfront] s&#39;ils ont déjà les deux ?

Oui, il existe un processus pour cela. Des détails supplémentaires seront fournis lorsqu’il sera temps pour votre organisation de passer à IMS.

### Qu’advient-il de la variable [!DNL Workfront] les utilisateurs qui n’ont pas de [!DNL Adobe] compte ?

Utilisateurs n’ayant pas reçu l’accès à [!DNL Adobe Admin Console] pour entrer dans [!DNL Workfront] doit créer un &quot;[!UICONTROL compte personnel]&quot; ou [!DNL Adobe] ID pour pouvoir se connecter. Cette action envoie un courrier électronique à l’administrateur pour approuver ou rejeter sa demande. Elle permet en outre à l’administrateur de configurer le type d’accès dont dispose cet utilisateur. Lorsqu’ils se connectent, ils accèdent à experience.adobe.com, saisissent leur adresse électronique et choisissent [!UICONTROL Compte personnel]. De là, ils pourront accéder à [!DNL Workfront].

### Et si nous n&#39;en avons pas [!DNL Adobe] produits autres que [!DNL Workfront?]

Il est toujours recommandé que votre entreprise migre vers la variable [!DNL Adobe Unified Experience]. Vous recevrez une [!DNL Adobe] Identifiant ainsi que les avantages répertoriés ci-dessus.

### Nous avons des utilisateurs externes inclus dans notre [!DNL Workfront] instance. Nous ne voudrions pas qu’ils aient accès à d’autres produits inclus dans [!DNL Adobe]. Comment limiterions-nous leur accès dans la console ?

[!DNL Admin Console] permet aux administrateurs de contrôler largement ce à quoi les utilisateurs peuvent ou ne peuvent pas accéder. Lorsqu’un utilisateur externe souhaite y accéder, il doit créer une [!DNL Adobe] ID, qui envoie un courrier électronique à l’administrateur. L’administrateur peut alors accepter ou refuser l’accès à un produit et définir ce à quoi il peut ou ne peut pas accéder pour les produits appartenant à cette organisation. Ensuite, la variable [!DNL Workfront] L’administrateur système peut accéder à la variable [!UICONTROL Utilisateurs] area of [!DNL Workfront] pour obtenir des autorisations plus granulaires pour l’utilisateur externe.

### Les administrateurs de groupe sont utilisés pour créer des personnes dans [!DNL Workfront]. Avec le déplacement vers [!DNL Experience Cloud], les administrateurs de groupe pourront-ils toujours créer des personnes ?

Oui, la création d’un utilisateur est toujours possible via [!DNL Workfront]. Ces utilisateurs peuvent être ajoutés à [!DNL Experience Cloud] automatiquement. Vous pouvez également configurer vos administrateurs de groupe en tant que propriétaires de produits dans la variable [!DNL Admin Console] pour leur permettre d’affecter [!DNL Workfront] aux utilisateurs.

### Quelle est la date limite de basculement ? [!DNL Experience Cloud]?

Il n’y a actuellement pas de délai pour passer à [!DNL Adobe Experience Cloud]. Nous travaillons avec les clients pour leur permettre de choisir quand ils sont prêts à faire le déplacement.

### Notre équipe de support devra-t-elle faire quelque chose pour ce changement ?

Si l’équipe d’assistance est chargée de créer de nouveaux utilisateurs, elle doit se familiariser avec la variable [!DNL Admin Console] interfaces utilisées pour créer des utilisateurs et attribuer un droit à Workfront. Sinon, il n’y aura probablement aucun changement significatif pour votre équipe de support interne.

### Comment cela affecte-t-il les intégrations que nous avons via la fonction API ?

Le chemin d’accès à l’URL existant restera disponible pour le trafic de l’API. Vous ne devez rien faire pour mettre à jour les points de terminaison dans vos intégrations. Toutefois, la connexion directe par l’intermédiaire du nom d’utilisateur et du mot de passe ne sera pas prise en charge. Vous devez utiliser une clé API, à l’exception de [!DNL Workfront Fusion] connecteurs.

### Et à propos de [!DNL Creative Cloud] utilisateurs ? Comment la migration les affecte-t-elle ? Y a-t-il des avantages pour eux ?

Il n’y a aucun impact sur [!DNL Creative Cloud] utilisateurs avec la migration vers [!DNL Adobe Unified Experience].

### Les connexions seront-elles modifiées pour [!DNL Workfront] utilisateurs mobiles ?

[!DNL Workfront] Les utilisateurs mobiles ne doivent pas être affectés par la migration vers [!DNL Adobe Unified Experience].
