---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Questions fréquentes sur Adobe Unified Experience
description: Certaines fonctionnalités diffèrent entre  [!DNL Workfront]  et Adobe Experience Cloud, et vous pouvez avoir des questions lorsque vous migrez votre instance  [!DNL Workfront]  vers l’expérience unifiée.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 4ce69180b8f419ff5634d0dba802f9fb57cd758b
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 90%

---

# Questions fréquentes sur [!DNL Adobe Unified Experience]

[!DNL Adobe Unified Experience] pour [!DNL Workfront] vous permet de gérer l’ensemble de vos applications [!DNL Adobe] depuis un même endroit avec une seule connexion. La zone de navigation [!DNL Adobe] est intégrée de manière transparente à [!DNL Workfront]. Certaines fonctionnalités sont différentes et vous pouvez vous poser des questions lorsque vous migrez votre instance [!DNL Workfront] vers l’expérience unifiée.

Pour plus d’informations sur la connexion à [!DNL Adobe Unified Experience], voir [[!DNL Adobe Unified Experience]  pour  [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparaison des expériences [!DNL Adobe Unified Experience] et [!DNL Workfront only]

Seuls les clientes et clients qui utilisent [!DNL Adobe Business Platform]/[!DNL Adobe Admin Console] peuvent accéder à [!DNL Adobe Unified Experience]. Les clientes et clients qui n’ont pas encore migré verront l’expérience [!DNL Workfront only] sans la possibilité de basculer entre les applications [!DNL Adobe].

Ce tableau décrit les fonctionnalités qui diffèrent entre les deux expériences.

| [!DNL Adobe Unified Experience] | Expérience [!DNL Workfront] uniquement |
| ---- | ----|
| Le menu principal [!UICONTROL [!DNL Workfront]] se trouve à gauche du ![Menu principal](assets/main-menu-icon-left-nav.png). | Le [!UICONTROL [!DNL Workfront]menu principal] se trouve à droite du ![Menu principal](assets/main-menu-icon.png). |
| Une seule URL de connexion est disponible pour toutes les applications [!DNL Adobe Experience Cloud]. | Connexion à [!DNL Workfront] avec une URL [!DNL Workfront] personnalisée |
| Un &quot;sélecteur d’organisation&quot; vous permet de passer d’une [!DNL Workfront] organisations et environnements | Le « sélecteur d’organisation » n’est pas disponible. |
| La navigation comprend une zone de navigation supérieure pour les produits [!DNL Adobe], les notifications [!DNL Adobe], l’aide et votre profil utilisateur, en plus de la barre de navigation [!DNL Workfront]. | La navigation comprend la barre de navigation [!DNL Workfront] uniquement. |
| L’aide est accessible à partir du [!UICONTROL menu principal] et de la zone de navigation supérieure. | L’aide est accessible à partir du [!UICONTROL menu principal] et de la barre de navigation [!DNL Workfront]. |
| Le lecteur de vérification s’ouvre dans un nouvel onglet | La visionneuse de relecture s’ouvre dans Workfront |
| L’URL utilisée pour accéder à Workfront est `experience.adobe.com` | L’URL utilisée pour accéder à Workfront est `(CompanyName).my.workfront.adobe.com` |
| Le format de date (MM/JJ/AAAA, par exemple) est basé sur les paramètres de langue de l’expérience unifiée. Si l’utilisateur n’a pas mis à jour ses paramètres de langue, les paramètres de `en-US` sont utilisés. | Le format des dates (MM/JJ/AAAA, par exemple) dépend des préférences du navigateur |

{style="table-layout:auto"}

## Questions fréquentes

### Comment déterminer si j’utilise Adobe Unified Experience ou Adobe Workfront ?

Pour déterminer si votre entreprise est sur Adobe Unified Experience, examinez l’URL que vous utilisez pour accéder à Workfront.

| URL | Adobe Experience |
|------------|------------|
| (Nom de l’entreprise).my.workfront.com | Expérience Workfront |
| experience.adobe.com | Adobe Unified Experience |

### Comment en savoir plus sur l’[!DNL Adobe Admin Console] ?

Pour plus d’informations sur l’[!DNL Admin Console], passez en revue ces articles :

* [Préparation pour  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Différences d’administration basées sur les plateformes ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* Vue d’ensemble d’[[!DNL Adobe Admin Console] &#x200B;](https://helpx.adobe.com/fr/enterprise/using/admin-console.html)

### En tant que client ou cliente, que dois-je faire pour faciliter la migration ?

Les clients et clientes existants seront contactés pour planifier les migrations. Les collègues de l’équipe d’assistance à la migration vont guider les clients et clientes tout au long du processus, les conseiller sur la configuration d’[!DNL Admin Console] et fournir des liens vers la documentation nécessaire pour que la migration soit aussi simple et facile que possible.

* Vue d’ensemble de l’assistance [[!DNL Adobe Workfront] &#x200B;](https://experienceleague.adobe.com/fr/docs/support-resources/adobe-support-tools-guide/workfront/overview)
* Questions fréquentes sur [[!DNL Adobe Business Platform]  et l’ [!DNL Admin Console] &#x200B;](https://experienceleague.adobe.com/fr/docs/support-resources/adobe-support-tools-guide/workfront/faq)

### Comment gérez-vous [!DNL Adobe Admin Console] pour les entreprises qui l’ont déjà activé pour les ID fédérés différemment de la configuration SSO [!DNL Workfront] ?

[!DNL Adobe Admin Console] a la possibilité d’inclure des [!DNL Workfront], en remplaçant l’authentification unique par le système Identity Management (IMS) d’Adobe. L’approvisionnement des utilisateurs et utilisatrices s’effectue dans [!DNL Admin Console]. Les utilisateurs et utilisatrices verront l’écran de connexion [!DNL Adobe] pour accéder à [!DNL Experience Cloud] où [!DNL Workfront] apparaît comme option (si l’accès leur est accordé).

### Comment cela affecte-t-il les clients et clientes qui disposent déjà du panneau d’administration AEM pour , mais dont SSO est configuré différemment de  ? [!DNL Adobe Assets]&#x200B;[!DNL Workfront?]

Une fois [!DNL Workfront] ajouté en tant qu’application [!DNL Admin Console], vous ne devriez pas avoir à faire quoi que ce soit d’autre pour [!DNL Workfront] afin d’utiliser la configuration SSO existante dont vous disposez pour [!DNL Adobe Assets].

### Comment cela affecte-t-il les configurations avec SSO ?

SSO est configuré dans [!DNL Admin Console] et hérité par l’application [!DNL Workfront].

### L’authentification unique avec notre [!DNL Active Directory] interne sera-t-elle toujours possible avec Adobe Identity Management System (IMS) ?

IMS remplace SSO et fonctionne pratiquement de la même manière. Toutes les autorisations sont accordées et configurées dans [!DNL Adobe Admin Console]. Les utilisateurs et utilisatrices verront l’écran de connexion [!DNL Adobe] et pourront choisir [!UICONTROL Compte personnel] ou [!UICONTROL Compte d’entreprise] pour se connecter (si vous avez [!DNL Active Directory], la plupart se connecteront avec un compte d’entreprise).

### Pour les personnes qui n’utilisent pas SSO, est-ce que l’URL de connexion [!DNL Workfront] change ?

L’URL de connexion change. Toutefois, l’ancienne URL redirige vers la nouvelle URL de connexion. Vous devez donc expliquer à vos utilisateurs et utilisatrices où aller.

### Les alias que nous avons configurés fonctionneront-ils toujours ou les liens [!DNL Workfront] changeront-ils avec cette migration ?

Les redirections/alias [!DNL Workfront] sont disponibles pour accéder à la page d’accueil.

### Les redirections seront-elles désactivées à un moment donné ? Ou pourrons-nous toujours saisir my.company.workfront.com ?

Vous pourrez toujours utiliser n’importe quelle URL personnalisée. Cliquer sur l’un de ces liens vous dirigera vers [!DNL Workfront] et affichera une autre URL. Cependant, c’est une meilleure [!DNL experience] de vous connecter à experience.adobe.com et de mettre en signet des liens à partir d’[!DNL Experience Cloud]. Moins de redirection signifie moins de délai ou de temps de chargement.

### Les liens directs vers les files d’attente des demandes seront-ils rompus ?

Tous les liens directs devraient rediriger vers les nouveaux modèles d’URL. Cependant, si vous avez partagé des liens avec d’autres personnes, vous devez envoyer une mise à jour pour utiliser le lien direct et éviter les retards d’accès à la page souhaitée.

### Allons-nous migrer globalement vers [!DNL Experience Cloud] ou pouvons-nous sélectionner certaines personnes (les autres produits Adobe ne sont pas utilisés par tous nos utilisateurs et utilisatrices) ?

L’ensemble du compte  du client ou de la cliente sera migré. [!DNL Workfront] Elle ne peut pas être effectuée au cas par cas pour chaque utilisateur ou utilisatrice.

### Est-ce que les [!DNL Workfront]utilisateurs et utilisatrices  doivent se connecter via [!DNL Experience Cloud] ? Ou seulement les administrateurs et les administratrices ?

Oui, tous les utilisateurs et toutes les utilisatrices se connecteront via [!DNL Experience Cloud]. La connexion à Adobe Identity Management System (IMS) remplacera SSO. L’expérience est très similaire, seul l’écran de connexion est différent.

### Les comptes [!DNL Adobe] des utilisateurs et des utilisatrices devront-ils être liés à leurs comptes [!DNL Workfront] si les deux leur appartiennent déjà ?

Oui, un processus est prévu pour cela. Vous recevrez des informations supplémentaires lorsque le moment sera venu pour votre organisation de migrer vers IMS.

### Que se passe-t-il pour les utilisateurs et les utilisatrices [!DNL Workfront] qui n’ont pas de compte [!DNL Adobe] ?

Les utilisateurs et les utilisatrices qui n’ont pas reçu d’autorisation d’accès dans  pour accéder à  doivent créer un « compte personnel » ou un identifiant de compte  pour pouvoir se connecter. [!DNL Adobe Admin Console]&#x200B;[!DNL Workfront]&#x200B;[!DNL Adobe] Cette action envoie un e-mail à l’administrateur ou à l’administratrice pour approuver ou rejeter sa requête. Elle permet en outre à l’administrateur ou à l’administratrice de configurer le type d’accès dont dispose cet utilisateur ou cette utilisatrice. Lorsque ces personnes se connectent, elles accèdent à experience.adobe.com, saisissent leur adresse e-mail et choisissent [!UICONTROL Compte personnel]. De là, elles peuvent accéder à [!DNL Workfront].

### Que faire si nous n’avons pas de produits  autres que  ? [!DNL Adobe]&#x200B;[!DNL Workfront?]

Il est toujours recommandé que votre entreprise effectue la migration vers . [!DNL Adobe Unified Experience] Vous recevrez un identifiant [!DNL Adobe] et disposerez des avantages répertoriés ci-dessus.

### Des utilisateurs et utilisatrices externes utilisent aussi notre instance . [!DNL Workfront] Nous ne souhaitons pas que l’accès à d’autres produits inclus dans  leur soit accordé. [!DNL Adobe] Comment pouvons-nous limiter leur accès dans la console ?

[!DNL Admin Console] offre aux administrateurs et aux administratrices un contrôle étendu sur les accès des utilisateurs et des utilisatrices. Lorsqu’un utilisateur ou une utilisatrice externe souhaite accéder au site, la création d’un identifiant [!DNL Adobe] s’accompagnant de l’envoi d’un e-mail à l’administrateur ou à l’administratrice doit être effectuée par leurs soins. L’administrateur ou l’administratrice peut alors accepter ou refuser l’accès à un produit et définir les autorisations d’accès pour tous les produits appartenant à cette organisation. L’administrateur ou l’administratrice système [!DNL Workfront] peut ensuite aller dans la zone [!UICONTROL Utilisateurs et utilisatrices] de [!DNL Workfront] pour accorder des autorisations plus granulaires à l’utilisateur ou à l’utilisatrice externe.

### Les administrateurs et les administratrices de groupes sont utilisés pour créer des personnes dans . [!DNL Workfront] Suite à la migration vers [!DNL Experience Cloud], la création de personnes pourra-t-elle toujours être effectuée par les administrateurs et les administratrices de groupes ?

Oui, la création d’un utilisateur ou d’une utilisatrice est toujours possible via . [!DNL Workfront] L’ajout de ces utilisateurs et de ces utilisatrices à [!DNL Experience Cloud] peut se faire automatiquement. Il est possible de configurer dans [!DNL Admin Console] les administrateurs et les administratrices de groupes en tant que propriétaires de produits pour leur permettre d’attribuer [!DNL Workfront] aux utilisateurs et aux utilisatrices.

### Quelle est la date limite pour migrer vers [!DNL Experience Cloud] ?

Aucune date limitre n’a été établie pour migrer vers [!DNL Adobe Experience Cloud]. Nous collaborons avec les clientes et les clients pour leur permettre de choisir le moment adéquat pour effectuer cette migration.

### Notre équipe d’assistance devra-t-elle faire quelque chose à cette occasion ?

Si l’équipe d’assistance est responsable de la création des nouvelles personnes, elle devra se familiariser avec les interfaces [!DNL Admin Console] utilisées pour les créer et leur affecter des droits dans Workfront. En dehors de cela, aucun changement significatif n’est à prévoir pour votre équipe d’assistance interne.

### Quel est l’impact sur les intégrations que nous avons réalisées par le biais de la fonction API ?

Le chemin d’accès à l’URL existant restera disponible pour le trafic de l’API. La mise à jour des points d’entrée dans vos intégrations ne devrait pas être nécessaire. Toutefois, la connexion directe par l’intermédiaire du nom d’utilisateur ou utilisatrice et du mot de passe ne sera pas prise en charge. Vous devez utiliser une clé API, à part pour les connecteurs [!DNL Workfront Fusion].

### Qu’en est-il des utilisateurs et utilisatrices de  ? [!DNL Creative Cloud] Comment la migration les affecte-t-elle ? Y a-t-il des avantages pour ces utilisateurs et utilisatrices ?

La migration vers [!DNL Adobe Unified Experience] n’a aucun impact sur les utilisateurs et utilisatrices de [!DNL Creative Cloud].

### Les connexions seront-elles modifiées pour les utilisateurs et utilisatrices [!DNL Workfront] mobiles ?

Les utilisateurs et utilisatrices [!DNL Workfront] mobiles ne devraient pas être affectés par la migration vers [!DNL Adobe Unified Experience].

### JumpSeat ne fonctionne pas avec le [!DNL Adobe Unified Experience]. Comment résoudre ce problème ?

JumpSeat fonctionne avec le [!DNL Adobe Unified Experience], mais nécessite une mise à jour de la configuration. À l’aide du panneau d’administration JumpSeat, modifiez l’URL de l’application de `workfront.com` en se terminant par `.workfront.adobe.com`
