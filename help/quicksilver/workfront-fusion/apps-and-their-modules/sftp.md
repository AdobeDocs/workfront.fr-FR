---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules SFTP
description: Le [!DNL Adobe Workfront Fusion SFTP] Les modules vous permettent de surveiller les modifications de fichier dans un dossier/sous-dossier sélectionné, de charger de nouveaux fichiers dans le dossier souhaité, de modifier ou de supprimer des fichiers existants qui se trouvent déjà dans un dossier ou de modifier les autorisations de fichier.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1931'
ht-degree: 0%

---

# Modules SFTP

Le [!DNL Adobe Workfront Fusion] SFLes modules TP vous permettent de surveiller les modifications de fichier dans un dossier/sous-dossier sélectionné, de charger de nouveaux fichiers dans le dossier souhaité, de modifier ou supprimer des fichiers existants qui se trouvent déjà dans un dossier ou de modifier les autorisations de fichier.

## Exigences d’accès

Vous devez disposer des accès suivants pour utiliser les fonctionnalités de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] ou version ultérieure</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Exigences de licence actuelles : Non [!DNL Workfront Fusion] conditions requises pour obtenir une licence.</p>
   <p>Ou</p>
   <p>Exigences de licence héritées : [!UICONTROL [!DNL Workfront Fusion] pour l’automatisation et l’intégration du travail] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>
   <p>Exigences actuelles du produit : Si vous disposez de [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront] Planifiez, votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article. [!DNL Workfront Fusion] est inclus dans l’[!UICONTROL Ultimate] [!DNL Workfront] planifiez.</p>
   <p>Ou</p>
   <p>Exigences de produit héritées : Votre entreprise doit acheter [!DNL Adobe Workfront Fusion] ainsi que [!DNL Adobe Workfront] pour utiliser la fonctionnalité décrite dans cet article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

Pour plus d’informations sur [!DNL Adobe Workfront Fusion] licences, voir [[!DNL Adobe Workfront Fusion] licences](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conditions préalables

Pour utiliser le protocole SFTP avec [!DNL Workfront Fusion], il est nécessaire d’avoir un compte SFTP (tel que [!DNL GoDaddy] hébergement web).

## Connexion de SFTP à [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

Pour connecter votre compte SFTP à [!DNL Workfront Fusion] vous devez saisir l’hôte cible et les informations d’identification SFTP (nom d’utilisateur et mot de passe ou nom d’utilisateur et clé) pour le module [!UICONTROL Création d’une connexion] boîte de dialogue.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nom de la connexion]</td> 
   <td> <p> Saisissez le nom de votre connexion SFTP.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
   <td> <p>Saisissez le nom d’hôte du serveur SFTP que vous souhaitez connecter.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>Saisissez le port du serveur SFTP. Par exemple, 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type d’authentification]</p> </td> 
   <td> <p>Sélectionnez la méthode d’autorisation à utiliser pour la connexion au serveur SFTP.</p> 
    <ul> 
     <li><strong>[!UICONTROL Nom d’utilisateur et mot de passe]</strong>: Saisissez vos informations d’identification.</li> 
     <li> <p><strong>[!UICONTROL Nom d’utilisateur et clé]</strong>: Saisissez votre nom d’utilisateur et votre clé/certificat privé.</p> <p>Téléchargez la clé privée pour utiliser l’autorisation côté client ou téléchargez votre certificat (fichier P12 ou PFX) si vous souhaitez utiliser TLS à l’aide de votre certificat auto-signé. Si vous utilisez l’autorisation de certificat côté client, vous pouvez saisir votre certificat d’autorité de certification ici.</p> <p>[!DNL Workfront Fusion] ne conserve ni ne stocke les données (fichiers, mots de passe) que vous fournissez ici. Le fichier et le mot de passe ne sont utilisés que pour extraire une clé/un certificat privé.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Après avoir saisi les informations de connexion, cliquez sur **[!UICONTROL Continuer]** pour établir une connexion.

## [!UICONTROL SFTP] modules et leurs champs

Lorsque vous configurez [!UICONTROL SFTP] modules, [!DNL Workfront Fusion] affiche les champs répertoriés ci-dessous. En plus de ces [!UICONTROL SFTP] peut s’afficher, selon des facteurs tels que votre niveau d’accès dans l’application ou le service. Un titre en gras dans un module indique un champ obligatoire.

Si le bouton de mappage situé au-dessus d’un champ ou d’une fonction s’affiche, vous pouvez l’utiliser pour définir des variables et des fonctions pour ce champ. Pour plus d’informations, voir [Mappage des informations d’un module à un autre dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Fichiers de contrôle dans un dossier]

Renvoie les fichiers avec des détails lorsqu’un fichier est créé ou modifié dans un dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Saisissez ou mappez le dossier à regarder. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Taille de la mémoire tampon [B]</td> 
   <td> <p> Saisissez la taille du tampon en octets. La valeur définit la taille des blocs transférés à partir du serveur. Certains serveurs peuvent entraîner des problèmes ou corrompre des fichiers lorsque la valeur est trop élevée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de fichiers renvoyés]</td> 
   <td> <p> Définissez le nombre maximal de fichiers qui [!DNL Workfront Fusion] fonctionnera pendant un cycle</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Surveiller les sous-dossiers dans un dossier]

Renvoie les dossiers contenant des détails lorsqu’un dossier est créé ou modifié dans un dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Saisissez ou mappez le dossier à regarder. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de fichiers renvoyés]</td> 
   <td> <p> Définissez le nombre maximal de dossiers qui [!DNL Workfront Fusion] revient pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

#### [!UICONTROL Liste du contenu d’un dossier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Afficher] </td> 
   <td> <p>Indiquez si vous souhaitez récupérer les fichiers, les dossiers ou les deux.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Saisissez ou mappez le dossier contenant les fichiers ou dossiers que vous souhaitez répertorier. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Saisissez ou mappez le terme recherché. Par exemple, si vous souhaitez rechercher des fichiers avec l’extension .txt, saisissez <code>.txt</code>.Vous pouvez également saisir ou mapper le nom du fichier que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trier Par]</td> 
   <td> <p> Choisissez si vous souhaitez trier les résultats par nom de fichier, taille, date de dernier accès ou date de dernière modification.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordre de tri] </td> 
   <td> <p>Indiquez si le résultat doit être renvoyé par ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Poursuivre l’exécution de l’itinéraire même si le module ne renvoie aucun résultat]</p> </td> 
   <td>Activez cette option pour vous assurer que ce module n’arrête pas le scénario s’il ne renvoie aucun résultat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de résultats renvoyés]</td> 
   <td> <p> Définissez le nombre maximal de résultats qui [!DNL Workfront Fusion] revient pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention de fichiers]

Ce module répertorie les fichiers d’un dossier spécifié.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Taille de la mémoire tampon [B]]</td> 
   <td> <p> Saisissez la taille du tampon en octets. La valeur définit la taille des blocs transférés à partir du serveur. Certains serveurs peuvent entraîner des problèmes ou corrompre des fichiers lorsque la valeur est trop élevée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Saisissez ou mappez le dossier contenant les fichiers ou dossiers que vous souhaitez répertorier. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Saisissez ou mappez le terme recherché. Par exemple, si vous souhaitez rechercher des fichiers avec l’extension .txt, saisissez <code>.txt</code>.Vous pouvez également saisir ou mapper le nom du fichier que vous souhaitez rechercher.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trier Par]</td> 
   <td> <p> Choisissez si vous souhaitez trier les résultats par nom, taille, date de dernier accès ou date de dernière modification du fichier.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordre de tri]</td> 
   <td> <p> Indiquez si le résultat doit être renvoyé par ordre croissant ou décroissant.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Poursuivre l’exécution de l’itinéraire même si le module ne renvoie aucun résultat]</p> </td> 
   <td>Activez cette option pour vous assurer que ce module n’arrête pas le scénario s’il ne renvoie aucun résultat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre maximal de résultats renvoyés]</td> 
   <td> <p> Définissez le nombre maximal de fichiers qui [!DNL Workfront Fusion] revient pendant un cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtention d’un fichier]

Ce module récupère les détails du fichier, y compris les données d’un fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Taille de la mémoire tampon [B]]</td> 
   <td> <p> Saisissez la taille du tampon en octets. La valeur définit la taille des blocs transférés à partir du serveur. Certains serveurs peuvent entraîner des problèmes ou corrompre des fichiers lorsque la valeur est trop élevée.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path] </td> 
   <td> <p>Saisissez le chemin d’accès au fichier. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Chargement d’un fichier]

Ce module permet de télécharger un fichier sur le serveur SFTP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Spécifiez un dossier existant comme emplacement de stockage du fichier. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fichier source]</td> 
   <td> <p> Mappez le fichier source d’un module précédent, tel que [!UICONTROL Dropbox] &gt; [!UICONTROL Obtenir un fichier]. Vous pouvez également saisir ou mapper le nom de fichier et les données de fichier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Définissez les autorisations souhaitées pour le fichier ou le dossier. Utilisez les paramètres chmod . Par exemple : <code>777 </code>ou <code>-rwxrwxrwx</code>.</p> <p>Pour plus d’informations sur les enfants, reportez-vous à la section <a href="https://ss64.com/bash/chmod.html">documentation chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Renommer un fichier]

Renomme un fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez renommer. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nouveau nom de fichier]</td> 
   <td> <p> Saisissez le nouveau nom du fichier, y compris son extension.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Déplacer un fichier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez déplacer. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nouveau dossier]</td> 
   <td> <p> Saisissez le chemin d’accès au nouvel emplacement du fichier. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un fichier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez supprimer. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mise à jour des autorisations de fichier]

Permet de modifier les autorisations du fichier.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Saisissez le chemin d’accès au fichier que vous souhaitez déplacer. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Définissez les autorisations de fichier de votre choix. Utilisez les paramètres chmod . Par exemple : <code>777 </code>ou <code>-rwxrwxrwx</code>.</p> <p>Doit correspondre au modèle <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Pour plus d’informations sur les enfants, reportez-vous à la section <a href="https://ss64.com/bash/chmod.html">documentation chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Créer un dossier]

Crée un dossier à l’emplacement spécifié.

>[!NOTE]
>
>Si le dossier existe déjà, le module renvoie une erreur. Pour continuer le flux sans interruption, joignez un itinéraire de gestionnaire d’erreur au module pour capturer l’erreur et utiliser la variable [!UICONTROL Reprendre] pour continuer le flux. Pour plus d’informations sur l’ajout d’un itinéraire de gestionnaire d’erreurs, voir [Gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Pour plus d’informations sur l’itinéraire du gestionnaire d’erreurs, voir [Directives de gestion des erreurs dans [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Spécifiez un dossier existant comme emplacement de stockage pour le nouveau dossier. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/file.txt</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder Name]</td> 
   <td> <p> Saisissez le nom du dossier.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Définissez les autorisations de dossier de votre choix. Utilisez les paramètres chmod . Par exemple : <code>777 </code>ou <code>-rwxrwxrwx</code>.</p> <p>Doit correspondre au modèle <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Pour plus d’informations sur les enfants, reportez-vous à la section <a href="https://ss64.com/bash/chmod.html">chmod Man Page</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suppression d’un dossier]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Pour obtenir des instructions sur la connexion de votre compte SFTP à [!DNL Workfront Fusion], voir <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connexion de SFTP à [!DNL Workfront Fusion]</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Spécifiez le chemin d’accès au dossier que vous souhaitez supprimer. Vous pouvez spécifier un chemin absolu, tel que <code>/home/user/</code>. Vous pouvez également spécifier un chemin relatif pointant vers un dossier spécifique de l’utilisateur connecté, tel que <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
